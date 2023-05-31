# Comparing `tmp/binarycpython-0.9.6.tar.gz` & `tmp/binarycpython-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binarycpython-0.9.6.tar", last modified: Sat Jan 21 15:27:47 2023, max compression
+gzip compressed data, was "binarycpython-1.0.0.tar", last modified: Wed May 31 10:47:02 2023, max compression
```

## Comparing `binarycpython-0.9.6.tar` & `binarycpython-1.0.0.tar`

### file list

```diff
@@ -1,91 +1,99 @@
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.694728 binarycpython-0.9.6/
--rw-rw-r--   0 david     (1002) david     (1002)     2112 2023-01-21 15:07:23.561799 binarycpython-0.9.6/Makefile
--rw-rw-r--   0 david     (1002) david     (1002)     9726 2023-01-21 15:27:47.694728 binarycpython-0.9.6/PKG-INFO
--rw-rw-r--   0 david     (1002) david     (1002)     7754 2023-01-21 15:27:28.346720 binarycpython-0.9.6/README.md
--rw-rw-r--   0 david     (1002) david     (1002)        6 2023-01-21 15:07:23.561799 binarycpython-0.9.6/VERSION
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.686728 binarycpython-0.9.6/binarycpython/
--rw-rw-r--   0 david     (1002) david     (1002)      198 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/__init__.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.686728 binarycpython-0.9.6/binarycpython/core/
--rw-rw-r--   0 david     (1002) david     (1002)       55 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/core/__init__.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.690728 binarycpython-0.9.6/binarycpython/tests/
--rw-rw-r--   0 david     (1002) david     (1002)        0 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/__init__.py
--rw-rw-r--   0 david     (1002) david     (1002)     1358 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/extra_tests.py
--rwxrwxr-x   0 david     (1002) david     (1002)     4950 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/main.py
--rwxrwxr-x   0 david     (1002) david     (1002)     5506 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/python_API_test.py
--rw-rw-r--   0 david     (1002) david     (1002)    15204 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_c_bindings.py
--rw-rw-r--   0 david     (1002) david     (1002)    10046 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_custom_logging.py
--rw-rw-r--   0 david     (1002) david     (1002)    19103 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_dicts.py
--rw-rw-r--   0 david     (1002) david     (1002)    13719 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_ensemble.py
--rw-rw-r--   0 david     (1002) david     (1002)    17062 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)    39372 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_grid.py
--rw-rw-r--   0 david     (1002) david     (1002)     3350 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_notebooks.py
--rw-rw-r--   0 david     (1002) david     (1002)     4844 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_plot_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)      215 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_run_system_wrapper.py
--rw-rw-r--   0 david     (1002) david     (1002)      108 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_stellar_types.py
--rw-rw-r--   0 david     (1002) david     (1002)     3380 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/test_useful_funcs.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.690728 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/
--rw-rw-r--   0 david     (1002) david     (1002)        0 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/__init__.py
--rw-rw-r--   0 david     (1002) david     (1002)    19088 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_HPC.py
--rw-rw-r--   0 david     (1002) david     (1002)      456 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_Moe_di_Stefano_2017.py
--rw-rw-r--   0 david     (1002) david     (1002)      209 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_analytics.py
--rw-rw-r--   0 david     (1002) david     (1002)      215 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_cache.py
--rw-rw-r--   0 david     (1002) david     (1002)     7304 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_condor.py
--rw-rw-r--   0 david     (1002) david     (1002)      535 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_dataIO.py
--rw-rw-r--   0 david     (1002) david     (1002)    35163 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_distribution_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)      319 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_grid_logging.py
--rw-rw-r--   0 david     (1002) david     (1002)     3324 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_grid_options_defaults.py
--rw-rw-r--   0 david     (1002) david     (1002)      489 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_gridcode.py
--rw-rw-r--   0 david     (1002) david     (1002)      182 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_metadata.py
--rw-rw-r--   0 david     (1002) david     (1002)      981 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_monte_carlo_sampling.py
--rw-rw-r--   0 david     (1002) david     (1002)     3976 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_sampling_variables.py
--rw-rw-r--   0 david     (1002) david     (1002)     7024 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_slurm.py
--rw-rw-r--   0 david     (1002) david     (1002)     1018 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_spacing_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)     6148 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_version_info.py
--rw-rw-r--   0 david     (1002) david     (1002)        0 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/tests/tmp_functions.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.690728 binarycpython-0.9.6/binarycpython/utils/
--rw-rw-r--   0 david     (1002) david     (1002)       44 2022-11-19 21:59:48.170284 binarycpython-0.9.6/binarycpython/utils/__init__.py
--rw-rw-r--   0 david     (1002) david     (1002)    19551 2023-01-21 15:07:23.561799 binarycpython-0.9.6/binarycpython/utils/custom_logging_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)    30209 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/dicts.py
--rw-rw-r--   0 david     (1002) david     (1002)    11784 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/ensemble.py
--rw-rw-r--   0 david     (1002) david     (1002)    38096 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/functions.py
--rw-rw-r--   0 david     (1002) david     (1002)   555286 2022-11-19 21:59:48.174284 binarycpython-0.9.6/binarycpython/utils/moe_di_stefano_2017_data.py
--rw-rw-r--   0 david     (1002) david     (1002)    17845 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/plot_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)    24044 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_class.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.694728 binarycpython-0.9.6/binarycpython/utils/population_extensions/
--rw-rw-r--   0 david     (1002) david     (1002)    24783 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/HPC.py
--rw-rw-r--   0 david     (1002) david     (1002)    52379 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/Moe_di_Stefano_2017.py
--rw-rw-r--   0 david     (1002) david     (1002)        0 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/__init__.py
--rw-rw-r--   0 david     (1002) david     (1002)     4288 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/analytics.py
--rw-rw-r--   0 david     (1002) david     (1002)    11832 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/argument_handling.py
--rw-rw-r--   0 david     (1002) david     (1002)    15727 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/cache.py
--rw-rw-r--   0 david     (1002) david     (1002)    22652 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/condor.py
--rw-rw-r--   0 david     (1002) david     (1002)     1405 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/custom_generator_sampling.py
--rw-rw-r--   0 david     (1002) david     (1002)    29231 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/dataIO.py
--rw-rw-r--   0 david     (1002) david     (1002)    94026 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/distribution_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)     4703 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/ensemble.py
--rw-rw-r--   0 david     (1002) david     (1002)    39915 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/evolution_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)     6169 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/failing_systems_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)    17319 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/grid_logging.py
--rw-rw-r--   0 david     (1002) david     (1002)    46254 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/grid_options_defaults.py
--rw-rw-r--   0 david     (1002) david     (1002)    36260 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/grid_sampling.py
--rw-rw-r--   0 david     (1002) david     (1002)     4813 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/metadata.py
--rw-rw-r--   0 david     (1002) david     (1002)    10743 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/miscellaneous_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)    42137 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/monte_carlo_sampling.py
--rw-rw-r--   0 david     (1002) david     (1002)     8533 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/return_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)    18334 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/sampling_variables.py
--rw-rw-r--   0 david     (1002) david     (1002)     2824 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/signal_handling.py
--rw-rw-r--   0 david     (1002) david     (1002)    17911 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/slurm.py
--rw-rw-r--   0 david     (1002) david     (1002)     4316 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/source_file_sampling.py
--rw-rw-r--   0 david     (1002) david     (1002)    26081 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/spacing_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)     2551 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/termination_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)    16095 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/population_extensions/version_info.py
--rw-rw-r--   0 david     (1002) david     (1002)     4153 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/run_system_wrapper.py
--rw-rw-r--   0 david     (1002) david     (1002)      981 2022-11-19 21:59:48.178284 binarycpython-0.9.6/binarycpython/utils/stellar_types.py
--rw-rw-r--   0 david     (1002) david     (1002)    10689 2023-01-21 15:07:23.565799 binarycpython-0.9.6/binarycpython/utils/useful_funcs.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.694728 binarycpython-0.9.6/include/
--rw-rw-r--   0 david     (1002) david     (1002)     3205 2023-01-21 15:07:23.809800 binarycpython-0.9.6/include/binary_c_python.h
--rw-rw-r--   0 david     (1002) david     (1002)      263 2023-01-21 15:07:23.813799 binarycpython-0.9.6/requirements.txt
--rw-rw-r--   0 david     (1002) david     (1002)       94 2023-01-21 15:07:23.813799 binarycpython-0.9.6/setup.cfg
--rw-rw-r--   0 david     (1002) david     (1002)     8952 2023-01-21 15:07:23.813799 binarycpython-0.9.6/setup.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-01-21 15:27:47.694728 binarycpython-0.9.6/src/
--rw-rw-r--   0 david     (1002) david     (1002)    51569 2023-01-21 15:07:23.813799 binarycpython-0.9.6/src/binary_c_python.c
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.315104 binarycpython-1.0.0/
+-rw-rw-r--   0 david     (1002) david     (1002)     2112 2023-04-19 10:19:13.418348 binarycpython-1.0.0/Makefile
+-rw-rw-r--   0 david     (1002) david     (1002)    10754 2023-05-31 10:47:02.315104 binarycpython-1.0.0/PKG-INFO
+-rw-rw-r--   0 david     (1002) david     (1002)     8596 2023-05-31 10:44:05.415183 binarycpython-1.0.0/README.md
+-rw-rw-r--   0 david     (1002) david     (1002)        6 2023-05-31 10:37:35.647715 binarycpython-1.0.0/VERSION
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.311104 binarycpython-1.0.0/binarycpython/
+-rw-rw-r--   0 david     (1002) david     (1002)      198 2023-04-19 10:19:13.422348 binarycpython-1.0.0/binarycpython/__init__.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.311104 binarycpython-1.0.0/binarycpython/core/
+-rw-rw-r--   0 david     (1002) david     (1002)       55 2023-04-19 10:19:13.422348 binarycpython-1.0.0/binarycpython/core/__init__.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.311104 binarycpython-1.0.0/binarycpython/tests/
+-rw-rw-r--   0 david     (1002) david     (1002)        0 2023-04-19 10:19:13.422348 binarycpython-1.0.0/binarycpython/tests/__init__.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1358 2023-04-19 10:19:13.422348 binarycpython-1.0.0/binarycpython/tests/extra_tests.py
+-rwxrwxr-x   0 david     (1002) david     (1002)     5258 2023-05-19 15:06:02.574478 binarycpython-1.0.0/binarycpython/tests/main.py
+-rwxrwxr-x   0 david     (1002) david     (1002)     5506 2023-04-19 10:19:13.422348 binarycpython-1.0.0/binarycpython/tests/python_API_test.py
+-rw-rw-r--   0 david     (1002) david     (1002)    15221 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/test_c_bindings.py
+-rw-rw-r--   0 david     (1002) david     (1002)    10063 2023-05-20 12:53:41.868293 binarycpython-1.0.0/binarycpython/tests/test_custom_logging.py
+-rw-rw-r--   0 david     (1002) david     (1002)    19120 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/test_dicts.py
+-rw-rw-r--   0 david     (1002) david     (1002)    13736 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/test_ensemble.py
+-rw-rw-r--   0 david     (1002) david     (1002)    21401 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/test_event_logging.py
+-rw-rw-r--   0 david     (1002) david     (1002)    17201 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/test_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)    39585 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/test_grid.py
+-rwxrwxr-x   0 david     (1002) david     (1002)     3500 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/test_notebooks.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4844 2023-05-09 08:52:21.113742 binarycpython-1.0.0/binarycpython/tests/test_plot_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)      215 2023-05-09 08:52:19.689717 binarycpython-1.0.0/binarycpython/tests/test_run_system_wrapper.py
+-rw-rw-r--   0 david     (1002) david     (1002)      108 2023-05-09 08:52:18.585698 binarycpython-1.0.0/binarycpython/tests/test_stellar_types.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3380 2023-05-18 16:29:47.396519 binarycpython-1.0.0/binarycpython/tests/test_useful_funcs.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.315104 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/
+-rw-rw-r--   0 david     (1002) david     (1002)        0 2023-04-19 10:19:13.426348 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/__init__.py
+-rw-rw-r--   0 david     (1002) david     (1002)    19616 2023-05-11 14:36:23.283031 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_HPC.py
+-rw-rw-r--   0 david     (1002) david     (1002)      352 2023-05-11 14:36:23.283031 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_Moe_di_Stefano_2017.py
+-rw-rw-r--   0 david     (1002) david     (1002)      209 2023-05-09 08:51:20.408631 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_analytics.py
+-rw-rw-r--   0 david     (1002) david     (1002)      215 2023-05-09 08:51:22.020662 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_cache.py
+-rw-rw-r--   0 david     (1002) david     (1002)     7472 2023-05-11 14:36:23.283031 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_condor.py
+-rw-rw-r--   0 david     (1002) david     (1002)      535 2023-05-09 08:51:27.316763 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_dataIO.py
+-rw-rw-r--   0 david     (1002) david     (1002)    35485 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_distribution_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)      319 2023-05-09 08:51:40.025001 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_grid_logging.py
+-rw-rw-r--   0 david     (1002) david     (1002)      406 2023-05-11 14:36:23.283031 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_gridcode.py
+-rw-rw-r--   0 david     (1002) david     (1002)      182 2023-05-09 08:51:53.589250 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_metadata.py
+-rw-rw-r--   0 david     (1002) david     (1002)    14664 2023-05-11 14:36:23.283031 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_monte_carlo_sampling.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3995 2023-05-11 14:36:23.283031 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_population_options_defaults.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4092 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_sampling_variables.py
+-rw-rw-r--   0 david     (1002) david     (1002)     7222 2023-05-11 14:36:23.283031 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_slurm.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4792 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_source_file_sampling.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1012 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_spacing_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     6936 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_version_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)        0 2023-04-19 10:19:13.434348 binarycpython-1.0.0/binarycpython/tests/tmp_functions.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.315104 binarycpython-1.0.0/binarycpython/utils/
+-rw-rw-r--   0 david     (1002) david     (1002)       44 2022-11-19 21:59:48.170284 binarycpython-1.0.0/binarycpython/utils/__init__.py
+-rw-rw-r--   0 david     (1002) david     (1002)    19551 2023-05-11 14:36:01.591043 binarycpython-1.0.0/binarycpython/utils/custom_logging_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)    30209 2023-05-11 14:36:01.591043 binarycpython-1.0.0/binarycpython/utils/dicts.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4418 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/utils/email_utils.py
+-rw-rw-r--   0 david     (1002) david     (1002)    11854 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/utils/ensemble.py
+-rw-rw-r--   0 david     (1002) david     (1002)    31031 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/utils/event_logging.py
+-rw-rw-r--   0 david     (1002) david     (1002)    40857 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/utils/functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1376 2023-05-19 15:06:02.786476 binarycpython-1.0.0/binarycpython/utils/logging_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)   555286 2023-05-19 16:14:47.675209 binarycpython-1.0.0/binarycpython/utils/moe_di_stefano_2017_data.py
+-rw-rw-r--   0 david     (1002) david     (1002)    17845 2023-04-19 10:19:13.438348 binarycpython-1.0.0/binarycpython/utils/plot_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)    29571 2023-05-28 12:12:54.663648 binarycpython-1.0.0/binarycpython/utils/population_class.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.315104 binarycpython-1.0.0/binarycpython/utils/population_extensions/
+-rw-rw-r--   0 david     (1002) david     (1002)    25255 2023-05-11 14:36:23.287031 binarycpython-1.0.0/binarycpython/utils/population_extensions/HPC.py
+-rw-rw-r--   0 david     (1002) david     (1002)    54079 2023-05-19 15:06:02.582478 binarycpython-1.0.0/binarycpython/utils/population_extensions/Moe_di_Stefano_2017.py
+-rw-rw-r--   0 david     (1002) david     (1002)        0 2023-04-19 10:19:13.442348 binarycpython-1.0.0/binarycpython/utils/population_extensions/__init__.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4002 2023-05-11 14:36:23.287031 binarycpython-1.0.0/binarycpython/utils/population_extensions/analytics.py
+-rw-rw-r--   0 david     (1002) david     (1002)    11874 2023-05-31 10:37:35.647715 binarycpython-1.0.0/binarycpython/utils/population_extensions/argument_handling.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16361 2023-05-11 14:36:23.291031 binarycpython-1.0.0/binarycpython/utils/population_extensions/cache.py
+-rw-rw-r--   0 david     (1002) david     (1002)    23198 2023-05-11 14:36:23.291031 binarycpython-1.0.0/binarycpython/utils/population_extensions/condor.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5317 2023-05-11 14:36:23.291031 binarycpython-1.0.0/binarycpython/utils/population_extensions/custom_binary_c_logging.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1431 2023-05-11 14:36:23.291031 binarycpython-1.0.0/binarycpython/utils/population_extensions/custom_generator_sampling.py
+-rw-rw-r--   0 david     (1002) david     (1002)    29094 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/dataIO.py
+-rw-rw-r--   0 david     (1002) david     (1002)    90381 2023-05-19 16:14:48.987236 binarycpython-1.0.0/binarycpython/utils/population_extensions/distribution_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1676 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/email_extension.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4101 2023-05-11 14:36:23.291031 binarycpython-1.0.0/binarycpython/utils/population_extensions/ensemble.py
+-rw-rw-r--   0 david     (1002) david     (1002)    40282 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/evolution_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5920 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/failing_systems_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     9891 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/grid_logging.py
+-rw-rw-r--   0 david     (1002) david     (1002)    40212 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/grid_sampling.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3083 2023-05-31 10:37:35.647715 binarycpython-1.0.0/binarycpython/utils/population_extensions/logging_functionality.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4871 2023-05-11 14:36:23.291031 binarycpython-1.0.0/binarycpython/utils/population_extensions/metadata.py
+-rw-rw-r--   0 david     (1002) david     (1002)    10597 2023-05-11 14:36:23.295031 binarycpython-1.0.0/binarycpython/utils/population_extensions/miscellaneous_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)    44430 2023-05-11 14:36:23.295031 binarycpython-1.0.0/binarycpython/utils/population_extensions/monte_carlo_sampling.py
+-rw-rw-r--   0 david     (1002) david     (1002)    63686 2023-05-31 10:37:35.651715 binarycpython-1.0.0/binarycpython/utils/population_extensions/population_options_defaults.py
+-rw-rw-r--   0 david     (1002) david     (1002)     8255 2023-05-11 14:36:23.295031 binarycpython-1.0.0/binarycpython/utils/population_extensions/return_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)    18438 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/sampling_variables.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2898 2023-05-11 14:36:23.295031 binarycpython-1.0.0/binarycpython/utils/population_extensions/signal_handling.py
+-rw-rw-r--   0 david     (1002) david     (1002)    18469 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/slurm.py
+-rw-rw-r--   0 david     (1002) david     (1002)     7829 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/source_file_sampling.py
+-rw-rw-r--   0 david     (1002) david     (1002)    26329 2023-05-31 10:37:35.651715 binarycpython-1.0.0/binarycpython/utils/population_extensions/spacing_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2666 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/termination_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)    21294 2023-05-19 15:06:02.586478 binarycpython-1.0.0/binarycpython/utils/population_extensions/version_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4153 2023-04-19 10:19:13.462348 binarycpython-1.0.0/binarycpython/utils/run_system_wrapper.py
+-rw-rw-r--   0 david     (1002) david     (1002)      981 2022-11-19 21:59:48.178284 binarycpython-1.0.0/binarycpython/utils/stellar_types.py
+-rw-rw-r--   0 david     (1002) david     (1002)    10689 2023-04-19 10:19:13.462348 binarycpython-1.0.0/binarycpython/utils/useful_funcs.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.315104 binarycpython-1.0.0/include/
+-rw-rw-r--   0 david     (1002) david     (1002)     3403 2023-05-11 14:36:23.503031 binarycpython-1.0.0/include/binary_c_python.h
+-rw-rw-r--   0 david     (1002) david     (1002)      274 2023-05-11 14:36:23.507031 binarycpython-1.0.0/requirements.txt
+-rw-rw-r--   0 david     (1002) david     (1002)       94 2023-04-19 10:19:13.730348 binarycpython-1.0.0/setup.cfg
+-rw-rw-r--   0 david     (1002) david     (1002)     9010 2023-05-19 15:06:02.702477 binarycpython-1.0.0/setup.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2023-05-31 10:47:02.315104 binarycpython-1.0.0/src/
+-rw-rw-r--   0 david     (1002) david     (1002)    53681 2023-05-11 14:36:23.507031 binarycpython-1.0.0/src/binary_c_python.c
```

### Comparing `binarycpython-0.9.6/Makefile` & `binarycpython-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/PKG-INFO` & `binarycpython-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 1.1
 Name: binarycpython
-Version: 0.9.6
-Summary: This is a python API for binary_c (versions 2.2.3) by David Hendriks, Rob Izzard and collaborators. Based on the initial set up by Jeff andrews.
-Home-page: https://gitlab.eps.surrey.ac.uk/ri0005/binary_c-python
+Version: 1.0.0
+Summary: This is a python API for binary_c (versions 2.2.4) by David Hendriks, Rob Izzard and collaborators. Based on the initial set up by Jeff andrews.
+Home-page: https://binary_c.gitlab.io/binary_c-python
 Author: David Hendriks
 Author-email: davidhendriks93@gmail.com
 License: gpl
 Description: # Python module for binary_c
-        ![docstring coverage](./badges/docstring_coverage.svg) ![test coverage](./badges/test_coverage.svg) ![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)
+        ![docstring coverage](./badges/docstring_coverage.svg) ![test coverage](./badges/test_coverage.svg)
         
-        We present our package [binary-c-python](https://binary_c.gitlab.io/binary_c-python/), a population synthesis code which is aimed to provide a convenient and easy-to-use interface to the [binary_c](https://binary_c.gitlab.io/binary_c/) framework, allowing the user to rapidly evolve single stellar systems and populations of star systems. Based on earlier Perl versions by Robert Izzard, updated and extended for Python 3 by David Hendriks, Robert Izzard. Credits to Jeff Andrews for early efforts on the python-c interface.
+        [![DOI](https://joss.theoj.org/papers/10.21105/joss.04642/status.svg)](https://doi.org/10.21105/joss.04642)
+        
+        We present our package [binary_c-python](https://binary_c.gitlab.io/binary_c-python/), a population synthesis code which is aimed to provide a convenient and easy-to-use interface to the [binary_c](https://binary_c.gitlab.io/binary_c/) framework, allowing the user to rapidly evolve single stellar systems and populations of star systems. Based on earlier Perl versions by [Robert Izzard](https://robizzard.gitlab.io/), updated and extended for Python 3 by [David Hendriks](https://davidhendriks.com/), Robert Izzard. Credits to Jeff Andrews for early efforts on the python-c interface.
         
         `binary_c-python` is developed for students and scientists in the field of stellar astrophysics, who want to study the evolution of individual or populations of single and binary star systems (see the [example use-case notebooks](https://binary_c.gitlab.io/binary_c-python/example_notebooks.html) in the [online documentation](https://binary_c.gitlab.io/binary_c-python)).
         
-        This is the release branch for `binary_c-python` version 0.9.6 and `binary_c` version 2.2.3.
+        This is the development branch for `binary_c-python` version [1.0.1](https://gitlab.com/binary_c/binary_c-python/-/tree/releases/1.0.1/2.2.4) and `binary_c` version [2.2.4](https://gitlab.com/binary_c/binary_c/-/tree/releases/2.2.4).
         
-        The latest stable release version for `binary_c-python` is [0.9.6](https://gitlab.com/binary_c/binary_c-python/-/tree/releases/0.9.6/2.2.3) for `binary_c` [2.2.3](https://gitlab.com/binary_c/binary_c/-/tree/releases/2.2.3)
+        The latest release branch is `binary_c-python` version [1.0.0](https://gitlab.com/binary_c/binary_c-python/-/tree/releases/1.0.0/2.2.4) and `binary_c` version [2.2.4](https://gitlab.com/binary_c/binary_c/-/tree/releases/2.2.4).
         
         ## Installation
         Below we provide the installation instructions for `binary_c-python`.
         
         ### Requirements
         To run this code you need to at least have installations of:
         
         - `Python` version 3.9 up to 3.12 (it's recommended to use [Pyenv](https://github.com/pyenv/pyenv) to manage your Python versions)
-        - `binary_c` version 2.2.3 (See [installation section](https://binary_c.gitlab.io/binary_c#magicparlabel-156))
+        - `binary_c` version 2.2.4 (See [installation section](https://binary_c.gitlab.io/binary_c#magicparlabel-156))
         
         The Python packages that are required for this code to run are listed in the `requirements.txt`, which automatically gets read out by `setup.py`.
         
+        To build the documentation the following additional software is required:
+        
+        - `pandoc` available on https://pandoc.org/ or via `sudo apt-get install pandoc`
+        
         ### Environment variables
         Before building `binary_c-python` please make sure to have defined the following environment variables:
         
         - `BINARY_C` should point to the root directory of your binary_c installation
         - `LD_LIBRARY_PATH` should include $BINARY_C/src and whatever directories are required to run binary_c (e.g. locations of libgsl, libmemoize, librinterpolate, etc.)
         - `LIBRARY_PATH` should include whatever directories are required to build binary_c (e.g. locations of libgsl, libmemoize, librinterpolate, etc.)
         - `GSL_DIR` should point to the root location where you installed GSL to. This root dir should contain `bin/`, `lib/` etc
@@ -83,44 +89,54 @@
         ## Development:
         If you want to contribute to the code, then it is recommended that you install the packages in `development_requirements.txt`:
         
         ```
         pip install -r development_requirements.txt
         ```
         
-        Please do not hesitate to contact us to discuss any developments.
+        Please do not hesitate to contact us to discuss any contribution. Please see `HOW_TO_CONTRIBUTE`.
         
         Some useful commands to generate documentation and coverage reports are stored in the `commands/` directory.
         
+        We use the following naming convention for development and release branches:
+        
+        ```
+        development/<binary_c-python version>/<binary_c version>
+        releases/<binary_c-python version>/<binary_c version>
+        ```
+        
         ### Generating documentation
         To build the documentation manually, run
         
         ```
         ./generate_docs.sh
         ```
         
-        from within the `commands/` directory.
+        from within the `commands/` directory. Note: this requires `pandoc` to be installed on your machine.
         
         ### Generating docstring and test coverage report
         To generate the unit test and docstring coverage report, run
         
         ```
         ./generate_reports.sh
         ```
         
         from within the `commands/` directory.
         
         ## JOSS paper
-        We've written a JOSS paper for `binary_c-python`, which is stored in https://gitlab.com/dhendriks/paper_joss_binarycpython. The paper is currently under review.
+        We've written a JOSS paper for `binary_c-python`, which is stored in [papers/joss/paper.pdf](https://gitlab.com/binary_c/binary_c-python/-/blob/master/papers/joss/paper.pdf).
+        
+        Paper review status:
+        [![status](https://joss.theoj.org/papers/7c43806e6d1f82c2945e12ae500f03b2/status.svg)](https://joss.theoj.org/papers/7c43806e6d1f82c2945e12ae500f03b2)
+        
         
         ## FAQ/Issues:
         If you encounter an issue with the code, or if you want to suggest extra features or changes in the code, please submit an issue at https://gitlab.com/binary_c/binary_c-python/-/issues/new.
         
         Here we provide a non-exhaustive list of some issues we encountered and solutions for these:
-        >>>>>>> releases/0.9.6/2.2.3
         
         Building issues with binary_c itself:
         - see the documentation of binary_c (in doc/).
         - If you have MESA installed, make sure that the `$MESASDK_ROOT/bin/mesasdk_init.sh` is not sourced. It comes with its own version of some programs, and those can interfere with installing.
         
         When Pip install fails:
         - Run the installation with `-v` and/or `--log <logfile>` to get some more info
@@ -130,17 +146,18 @@
         
         Other:
         - When running jupyter notebooks, make sure you are running the jupyter installation from the same virtual environment.
         - When the output of binary_c seems to be different than expected, you might need to rebuild this python package. Everytime binary_c is compiled, this package needs to be rebuilt too.
         
 Keywords: binary_c,astrophysics,stellar evolution,population synthesis
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `binarycpython-0.9.6/README.md` & `binarycpython-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # Python module for binary_c
-![docstring coverage](./badges/docstring_coverage.svg) ![test coverage](./badges/test_coverage.svg) ![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)
+![docstring coverage](./badges/docstring_coverage.svg) ![test coverage](./badges/test_coverage.svg)
 
-We present our package [binary-c-python](https://binary_c.gitlab.io/binary_c-python/), a population synthesis code which is aimed to provide a convenient and easy-to-use interface to the [binary_c](https://binary_c.gitlab.io/binary_c/) framework, allowing the user to rapidly evolve single stellar systems and populations of star systems. Based on earlier Perl versions by Robert Izzard, updated and extended for Python 3 by David Hendriks, Robert Izzard. Credits to Jeff Andrews for early efforts on the python-c interface.
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04642/status.svg)](https://doi.org/10.21105/joss.04642)
+
+We present our package [binary_c-python](https://binary_c.gitlab.io/binary_c-python/), a population synthesis code which is aimed to provide a convenient and easy-to-use interface to the [binary_c](https://binary_c.gitlab.io/binary_c/) framework, allowing the user to rapidly evolve single stellar systems and populations of star systems. Based on earlier Perl versions by [Robert Izzard](https://robizzard.gitlab.io/), updated and extended for Python 3 by [David Hendriks](https://davidhendriks.com/), Robert Izzard. Credits to Jeff Andrews for early efforts on the python-c interface.
 
 `binary_c-python` is developed for students and scientists in the field of stellar astrophysics, who want to study the evolution of individual or populations of single and binary star systems (see the [example use-case notebooks](https://binary_c.gitlab.io/binary_c-python/example_notebooks.html) in the [online documentation](https://binary_c.gitlab.io/binary_c-python)).
 
-This is the release branch for `binary_c-python` version 0.9.6 and `binary_c` version 2.2.3.
+This is the development branch for `binary_c-python` version [1.0.1](https://gitlab.com/binary_c/binary_c-python/-/tree/releases/1.0.1/2.2.4) and `binary_c` version [2.2.4](https://gitlab.com/binary_c/binary_c/-/tree/releases/2.2.4).
 
-The latest stable release version for `binary_c-python` is [0.9.6](https://gitlab.com/binary_c/binary_c-python/-/tree/releases/0.9.6/2.2.3) for `binary_c` [2.2.3](https://gitlab.com/binary_c/binary_c/-/tree/releases/2.2.3)
+The latest release branch is `binary_c-python` version [1.0.0](https://gitlab.com/binary_c/binary_c-python/-/tree/releases/1.0.0/2.2.4) and `binary_c` version [2.2.4](https://gitlab.com/binary_c/binary_c/-/tree/releases/2.2.4).
 
 ## Installation
 Below we provide the installation instructions for `binary_c-python`.
 
 ### Requirements
 To run this code you need to at least have installations of:
 
 - `Python` version 3.9 up to 3.12 (it's recommended to use [Pyenv](https://github.com/pyenv/pyenv) to manage your Python versions)
-- `binary_c` version 2.2.3 (See [installation section](https://binary_c.gitlab.io/binary_c#magicparlabel-156))
+- `binary_c` version 2.2.4 (See [installation section](https://binary_c.gitlab.io/binary_c#magicparlabel-156))
 
 The Python packages that are required for this code to run are listed in the `requirements.txt`, which automatically gets read out by `setup.py`.
 
+To build the documentation the following additional software is required:
+
+- `pandoc` available on https://pandoc.org/ or via `sudo apt-get install pandoc`
+
 ### Environment variables
 Before building `binary_c-python` please make sure to have defined the following environment variables:
 
 - `BINARY_C` should point to the root directory of your binary_c installation
 - `LD_LIBRARY_PATH` should include $BINARY_C/src and whatever directories are required to run binary_c (e.g. locations of libgsl, libmemoize, librinterpolate, etc.)
 - `LIBRARY_PATH` should include whatever directories are required to build binary_c (e.g. locations of libgsl, libmemoize, librinterpolate, etc.)
 - `GSL_DIR` should point to the root location where you installed GSL to. This root dir should contain `bin/`, `lib/` etc
@@ -75,44 +81,54 @@
 ## Development:
 If you want to contribute to the code, then it is recommended that you install the packages in `development_requirements.txt`:
 
 ```
 pip install -r development_requirements.txt
 ```
 
-Please do not hesitate to contact us to discuss any developments.
+Please do not hesitate to contact us to discuss any contribution. Please see `HOW_TO_CONTRIBUTE`.
 
 Some useful commands to generate documentation and coverage reports are stored in the `commands/` directory.
 
+We use the following naming convention for development and release branches:
+
+```
+development/<binary_c-python version>/<binary_c version>
+releases/<binary_c-python version>/<binary_c version>
+```
+
 ### Generating documentation
 To build the documentation manually, run
 
 ```
 ./generate_docs.sh
 ```
 
-from within the `commands/` directory.
+from within the `commands/` directory. Note: this requires `pandoc` to be installed on your machine.
 
 ### Generating docstring and test coverage report
 To generate the unit test and docstring coverage report, run
 
 ```
 ./generate_reports.sh
 ```
 
 from within the `commands/` directory.
 
 ## JOSS paper
-We've written a JOSS paper for `binary_c-python`, which is stored in https://gitlab.com/dhendriks/paper_joss_binarycpython. The paper is currently under review.
+We've written a JOSS paper for `binary_c-python`, which is stored in [papers/joss/paper.pdf](https://gitlab.com/binary_c/binary_c-python/-/blob/master/papers/joss/paper.pdf).
+
+Paper review status:
+[![status](https://joss.theoj.org/papers/7c43806e6d1f82c2945e12ae500f03b2/status.svg)](https://joss.theoj.org/papers/7c43806e6d1f82c2945e12ae500f03b2)
+
 
 ## FAQ/Issues:
 If you encounter an issue with the code, or if you want to suggest extra features or changes in the code, please submit an issue at https://gitlab.com/binary_c/binary_c-python/-/issues/new.
 
 Here we provide a non-exhaustive list of some issues we encountered and solutions for these:
->>>>>>> releases/0.9.6/2.2.3
 
 Building issues with binary_c itself:
 - see the documentation of binary_c (in doc/).
 - If you have MESA installed, make sure that the `$MESASDK_ROOT/bin/mesasdk_init.sh` is not sourced. It comes with its own version of some programs, and those can interfere with installing.
 
 When Pip install fails:
 - Run the installation with `-v` and/or `--log <logfile>` to get some more info
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/extra_tests.py` & `binarycpython-1.0.0/binarycpython/tests/extra_tests.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/tests/main.py` & `binarycpython-1.0.0/binarycpython/tests/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,19 @@
     test_BinarycEncoder,
     test_ensemble_file_type,
     test_extract_ensemble_json_from_string,
     test_handle_ensemble_string_to_json,
     test_load_ensemble,
     test_open_ensemble,
 )
+from binarycpython.tests.test_event_logging import (
+    test_event_file_processing,
+    test_event_parameter_descriptions,
+    test_event_types,
+)
 from binarycpython.tests.test_functions import (
     test_bin_data,
     test_create_arg_string,
     test_create_hdf5,
     test_example_parse_output,
     test_get_arg_keys,
     test_get_defaults,
@@ -65,19 +70,19 @@
     test_remove_file,
     test_temp_dir,
     test_verbose_print,
     test_write_binary_c_parameter_descriptions_to_rst_file,
 )
 from binarycpython.tests.test_grid import (
     test__cleanup_defaults,
-    test__dict_from_line_source_file,
     test__increment_count,
     test__increment_probtot,
     test__return_argline,
     test__setup,
+    test__source_file_sampling_system_dict_from_line_command_style,
     test_cmdline,
     test_evolve_single,
     test_export_all_info,
     test_grid_evolve,
     test_resultdict,
     test_return_all_info,
     test_return_binary_c_defaults,
@@ -125,19 +130,14 @@
     test_ktg93,
     test_number,
     test_powerlaw,
     test_raghavan2010_binary_fraction,
     test_sana12,
     test_three_part_power_law,
 )
-from binarycpython.tests.tests_population_extensions.test_grid_options_defaults import (
-    test_grid_options_description_checker,
-    test_grid_options_help,
-    test_write_grid_options_to_rst_file,
-)
 from binarycpython.tests.tests_population_extensions.test_HPC import (
     test_HPC_check_requirements,
     test_HPC_dir,
     test_HPC_dirs,
     test_HPC_get_status,
     test_HPC_id_filename,
     test_HPC_id_from_dir,
@@ -145,32 +145,38 @@
     test_HPC_job_task,
     test_HPC_job_type,
     test_HPC_jobID,
     test_HPC_jobID_tuple,
     test_HPC_njobs,
     test_HPC_set_status,
 )
-from binarycpython.tests.tests_population_extensions.test_sampling_variables import (
-    test_add_grid_variable,
+from binarycpython.tests.tests_population_extensions.test_population_options_defaults import (
+    test_population_options_description_checker,
+    test_population_options_validation,
+    test_write_population_options_to_rst_file,
+)
+from binarycpython.tests.tests_population_extensions.test_sampling_variables import (  # test_add_grid_variable,
     test_add_sampling_variable,
 )
 from binarycpython.tests.tests_population_extensions.test_slurm import (
     test_get_slurm_status,
     test_make_slurm_dirs,
     test_set_slurm_status,
     test_slurm_check_requirements,
     test_slurm_dirs,
     test_slurm_outfile,
     test_slurmID,
 )
+from binarycpython.tests.tests_population_extensions.test_source_file_sampling import (
+    test_source_file_sampling_column_type,
+    test_source_file_sampling_command_type,
+)
+from binarycpython.tests.tests_population_extensions.test_spacing_functions import (
+    test_const,
+)
 from binarycpython.tests.tests_population_extensions.test_version_info import (
     test_parse_binary_c_version_info,
     test_return_binary_c_version_info,
 )
 
-# from binarycpython.tests.test_spacing_functions import *
-# from binarycpython.tests.test_grid_options_defaults import *
-# from binarycpython.tests.test_hpc_functions import *
-
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/python_API_test.py` & `binarycpython-1.0.0/binarycpython/tests/python_API_test.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_c_bindings.py` & `binarycpython-1.0.0/binarycpython/tests/test_c_bindings.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 
 from binarycpython import _binary_c_bindings
 from binarycpython.utils.dicts import merge_dicts
 from binarycpython.utils.ensemble import extract_ensemble_json_from_string
 from binarycpython.utils.functions import Capturing, is_capsule, temp_dir
 
-TMP_DIR = temp_dir("tests", "test_c_bindings")
+TMP_DIR = temp_dir("tests", "test_c_bindings", clean_path=True)
 
 
 #### some useful functions
 def return_argstring(
     m1=15.0,
     m2=14.0,
     separation=0,
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_custom_logging.py` & `binarycpython-1.0.0/binarycpython/tests/test_custom_logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     binary_c_write_code,
     create_and_load_logging_function,
     from_binary_c_config,
     return_compilation_dict,
 )
 from binarycpython.utils.functions import Capturing, temp_dir
 
-TMP_DIR = temp_dir("tests", "test_custom_logging")
+TMP_DIR = temp_dir("tests", "test_custom_logging", clean_path=True)
 
 
 class test_autogen_C_logging_code(unittest.TestCase):
     """
     Unit test class for autogen_C_logging_code
     """
 
@@ -151,15 +151,15 @@
         output_1 = from_binary_c_config(BINARY_C_CONFIG, input_1)
         self.assertTrue(output_1.startswith("Usage"))
 
         input_2 = "version"
         output_2 = from_binary_c_config(BINARY_C_CONFIG, input_2)
         self.assertIn(
             output_2,
-            ["2.2.3"],
+            ["2.2.4"],
             msg="binary_c version doesnt match",
         )
 
 
 class test_return_compilation_dict(unittest.TestCase):
     """
     Unit test for return_compilation_dict
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_dicts.py` & `binarycpython-1.0.0/binarycpython/tests/test_dicts.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     recursive_change_key_to_string,
     set_opts,
     subtract_dicts,
     update_dicts,
 )
 from binarycpython.utils.functions import Capturing, temp_dir
 
-TMP_DIR = temp_dir("tests", "test_dicts")
+TMP_DIR = temp_dir("tests", "test_dicts", clean_path=True)
 
 
 class dummy:
     """
     Dummy class to be used in the merge_dicts
     """
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_ensemble.py` & `binarycpython-1.0.0/binarycpython/tests/test_ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     handle_ensemble_string_to_json,
     load_ensemble,
     open_ensemble,
 )
 from binarycpython.utils.functions import Capturing, temp_dir
 from binarycpython.utils.population_class import Population
 
-TMP_DIR = temp_dir("tests", "test_ensemble")
+TMP_DIR = temp_dir("tests", "test_ensemble", clean_path=True)
 TEST_VERBOSITY = 1
 
 
 class test_binaryc_json_serializer(unittest.TestCase):
     """
     Unittests for function binaryc_json_serializer
     """
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_functions.py` & `binarycpython-1.0.0/binarycpython/tests/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 TODO: Capturing
 TODO: call_binary_c_config
 """
 
 import json
 import os
 import tempfile
+import types
 import unittest
 
 import h5py
 
 from binarycpython.utils.custom_logging_functions import binary_c_log_code
 from binarycpython.utils.functions import (
     Capturing,
@@ -48,15 +49,15 @@
     remove_file,
     temp_dir,
     verbose_print,
     write_binary_c_parameter_descriptions_to_rst_file,
 )
 from binarycpython.utils.run_system_wrapper import run_system
 
-TMP_DIR = temp_dir("tests", "test_functions")
+TMP_DIR = temp_dir("tests", "test_functions", clean_path=True)
 
 
 class test_verbose_print(unittest.TestCase):
     """
     Unittests for verbose_print
     """
 
@@ -198,15 +199,15 @@
         """
         Test to check if the shape and contents of output_lines is correct
         """
 
         example_text = "hallo\ntest\n123"
         output_1 = output_lines(example_text)
 
-        self.assertTrue(isinstance(output_1, list))
+        self.assertTrue(isinstance(output_1, (list, types.GeneratorType)))
         self.assertIn("hallo", output_1)
         self.assertIn("test", output_1)
         self.assertIn("123", output_1)
 
 
 class test_example_parse_output(unittest.TestCase):
     """
@@ -599,8 +600,10 @@
 
         binned_value = bin_data(value, binwidth)
 
         self.assertEqual(binned_value, -0.5)
 
 
 if __name__ == "__main__":
-    unittest.main()
+    # unittest.main()
+    test_output_lines_obj = test_output_lines()
+    test_output_lines_obj._test_1()
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_grid.py` & `binarycpython-1.0.0/binarycpython/tests/test_grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,32 +15,36 @@
 TODO: _process_run_population_grid
 TODO: _cleanup
 TODO: _dry_run
 TODO: _dry_run_source_file
 TODO: _load_source_file
 TODO: was_killed
 TODO: _check_binary_c_error
-
-TODO: Before running the non-unit tests to cover functions like evolve, we need to run the unit tests
 """
 
 import gzip
 import json
 import os
 import shutil
 import sys
 import unittest
 
 import numpy as np
 
 from binarycpython.utils.dicts import merge_dicts
-from binarycpython.utils.functions import Capturing, bin_data, remove_file, temp_dir
+from binarycpython.utils.functions import (
+    Capturing,
+    bin_data,
+    output_lines,
+    remove_file,
+    temp_dir,
+)
 from binarycpython.utils.population_class import Population
 
-TMP_DIR = temp_dir("tests", "test_grid")
+TMP_DIR = temp_dir("tests", "test_grid", clean_path=True)
 shutil.rmtree(TMP_DIR)
 os.makedirs(TMP_DIR, exist_ok=True)
 
 TEST_VERBOSITY = 1
 
 
 def parse_function_test_grid_evolve_2_threads_with_custom_logging(
@@ -53,15 +57,15 @@
     # Get some information from the
     data_dir = self.custom_options["data_dir"]
 
     # make outputfilename
     output_filename = os.path.join(
         data_dir,
         "test_grid_evolve_2_threads_with_custom_logging_outputfile_population_{}_thread_{}.dat".format(
-            self.grid_options["_population_id"], self.process_ID
+            self.population_options["_population_id"], self.process_ID
         ),
     )
 
     # Check directory, make if necessary
     os.makedirs(data_dir, exist_ok=True)
 
     if not os.path.exists(output_filename):
@@ -75,36 +79,36 @@
 def parse_function_adding_results(self, output):  # pragma: no cover
     """
     Example parse function
     """
 
     parameters = ["time", "mass", "zams_mass", "probability", "stellar_type"]
 
-    self.grid_results["example"]["count"] += 1
+    self.population_results["example"]["count"] += 1
 
     # Go over the output.
-    for line in output.splitlines():
+    for line in output_lines(output):
         headerline = line.split()[0]
 
         # CHeck the header and act accordingly
         if headerline == "EXAMPLE_OUTPUT":
             values = line.split()[1:]
 
             # Bin the mass probability
-            self.grid_results["example"]["mass"][
+            self.population_results["example"]["mass"][
                 bin_data(float(values[2]), binwidth=0.5)
             ] += float(values[3])
 
             #
             if not len(parameters) == len(values):
                 print("Number of column names isnt equal to number of columns")
                 raise ValueError
 
     # record the probability of this line (Beware, this is meant to only be run once for each system. its a controls quantity)
-    self.grid_results["example"]["probability"] += float(values[3])
+    self.population_results["example"]["probability"] += float(values[3])
 
 
 class test__setup(unittest.TestCase):
     """
     Unittests for _setup function
     """
 
@@ -118,19 +122,18 @@
         """
         test_pop = Population(tmp_dir=TMP_DIR)
 
         self.assertTrue("orbital_period" in test_pop.defaults)
         self.assertTrue("metallicity" in test_pop.defaults)
         self.assertNotIn("help_all", test_pop.cleaned_up_defaults)
         self.assertEqual(test_pop.bse_options, {})
-        self.assertEqual(test_pop.custom_options, {"save_snapshot": False})
         self.assertEqual(test_pop.argline_dict, {})
         self.assertEqual(test_pop.persistent_data_memory_dict, {})
-        self.assertTrue(test_pop.grid_options["parse_function"] is None)
-        self.assertTrue(isinstance(test_pop.grid_options["_main_pid"], int))
+        self.assertTrue(test_pop.population_options["parse_function"] is None)
+        self.assertTrue(isinstance(test_pop.population_options["_main_pid"], int))
 
 
 class test_set(unittest.TestCase):
     """
     Unittests for _setup function
 
     TODO: split into 4 sub-tests
@@ -159,15 +162,15 @@
 
         # BSE options test special argument
         test_pop.set(ensemble_filter_SUPERNOVAE=1, ensemble_dt=1000)
         self.assertTrue(test_pop.bse_options["ensemble_filter_SUPERNOVAE"] == 1)
 
         # test grid options
         test_pop.set(num_cores=2)
-        self.assertTrue(test_pop.grid_options["num_cores"] == 2)
+        self.assertTrue(test_pop.population_options["num_cores"] == 2)
 
 
 class test_cmdline(unittest.TestCase):
     """
     Unittests for cmdline function
     TODO: this has to be fixed. See parse_cmdline function
     """
@@ -200,22 +203,20 @@
         test_pop.parse_cmdline()
 
         # metallicity
         self.assertTrue(isinstance(test_pop.bse_options["metallicity"], str))
         self.assertTrue(test_pop.bse_options["metallicity"] == "0.0002")
 
         # Number of cores
-        print(test_pop.grid_options["num_cores"])
-        print(type(test_pop.grid_options["num_cores"]))
         self.assertTrue(
-            isinstance(test_pop.grid_options["num_cores"], int)
-            or isinstance(test_pop.grid_options["num_cores"], dict)
-            or isinstance(test_pop.grid_options["num_cores"], str)
+            isinstance(test_pop.population_options["num_cores"], int)
+            or isinstance(test_pop.population_options["num_cores"], dict)
+            or isinstance(test_pop.population_options["num_cores"], str)
         )
-        self.assertTrue(test_pop.grid_options["num_cores"] == 2)
+        self.assertTrue(test_pop.population_options["num_cores"] == 2)
 
         # datadir
         self.assertTrue(isinstance(test_pop.custom_options["data_dir"], str))
         self.assertTrue(test_pop.custom_options["data_dir"] == "/tmp/binary_c_python")
 
         # put back the other args if they exist
         sys.argv = prev_sysargv.copy()
@@ -274,16 +275,16 @@
 
         population_settings = test_pop.return_population_settings()
 
         self.assertIn("bse_options", population_settings)
         self.assertTrue(population_settings["bse_options"]["metallicity"] == 0.02)
         self.assertTrue(population_settings["bse_options"]["M_1"] == 10)
 
-        self.assertIn("grid_options", population_settings)
-        self.assertTrue(population_settings["grid_options"]["num_cores"] == 2)
+        self.assertIn("population_options", population_settings)
+        self.assertTrue(population_settings["population_options"]["num_cores"] == 2)
 
         self.assertIn("custom_options", population_settings)
         self.assertTrue(population_settings["custom_options"]["data_dir"] == "/tmp")
 
 
 class test_return_binary_c_defaults(unittest.TestCase):
     """
@@ -438,15 +439,15 @@
     def _test__increment_probtot(self):
         """
         Unittests for the function _increment_probtot
         """
 
         test_pop = Population(tmp_dir=TMP_DIR)
         test_pop._increment_probtot(0.5)
-        self.assertEqual(test_pop.grid_options["_probtot"], 0.5)
+        self.assertEqual(test_pop.population_options["_probtot"], 0.5)
 
 
 class test__increment_count(unittest.TestCase):
     """
     Unittests for _increment_count function
     """
 
@@ -457,43 +458,47 @@
     def _test__increment_count(self):
         """
         Unittests for the function _increment_count
         """
 
         test_pop = Population(tmp_dir=TMP_DIR)
         test_pop._increment_count()
-        self.assertEqual(test_pop.grid_options["_count"], 1)
+        self.assertEqual(test_pop.population_options["_count"], 1)
 
 
-class test__dict_from_line_source_file(unittest.TestCase):
+class test__source_file_sampling_system_dict_from_line_command_style(unittest.TestCase):
     """
     Unittests for _dict_from_line_source_file function
     """
 
-    def test__dict_from_line_source_file(self):
+    def test__source_file_sampling_system_dict_from_line_command_style(self):
         with Capturing() as _:
-            self._test__dict_from_line_source_file()
+            self._test__source_file_sampling_system_dict_from_line_command_style()
 
-    def _test__dict_from_line_source_file(self):
+    def _test__source_file_sampling_system_dict_from_line_command_style(self):
         """
-        Unittests for the function _dict_from_line_source_file
+        Unittests for the function _source_file_sampling_system_dict_from_line_command_style
         """
 
         source_file = os.path.join(TMP_DIR, "example_source_file.txt")
 
         # write
         with open(source_file, "w") as f:
             f.write("binary_c M_1 10 metallicity 0.02\n")
 
         test_pop = Population(tmp_dir=TMP_DIR)
 
         # readout
         with open(source_file, "r") as f:
             for line in f.readlines():
-                argdict = test_pop._dict_from_line_source_file(line)
+                argdict = (
+                    test_pop._source_file_sampling_system_dict_from_line_command_style(
+                        line
+                    )
+                )
 
                 self.assertTrue(argdict["M_1"] == 10)
                 self.assertTrue(argdict["metallicity"] == 0.02)
 
 
 class test_evolve_single(unittest.TestCase):
     """
@@ -595,15 +600,15 @@
         stardata->model.max_evolution_time = stardata->model.time - stardata->model.dtm;
         """
 
         example_pop = Population(tmp_dir=TMP_DIR)
         example_pop.set(verbosity=0)
         example_pop.set(
             max_evolution_time=15000,  # bse_options
-            # grid_options
+            # population_options
             num_cores=3,
             tmp_dir=TMP_DIR,
             # Custom options
             data_dir=os.path.join(TMP_DIR, "test_resultdict"),  # custom_options
             C_logging_code=custom_logging_statement,
             parse_function=parse_function_adding_results,
         )
@@ -620,28 +625,28 @@
                 resolution["M_1"]
             ),
             precode="M_1=math.exp(lnm1)",
             probdist="self.three_part_powerlaw(M_1, 0.1, 0.5, 1.0, 150, -1.3, -2.3, -2.3)*M_1",
             dphasevol="dlnm1",
             parameter_name="M_1",
             condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
-            gridtype="left",
+            gridtype="centred",
         )
 
         ## Executing a population
         ## This uses the values generated by the sampling_variables
         analytics = example_pop.evolve()
 
         #
         grid_prob = analytics["total_probability"]
-        result_dict_prob = example_pop.grid_results["example"]["probability"]
+        result_dict_prob = example_pop.population_results["example"]["probability"]
 
         # amt systems
         grid_count = analytics["total_count"]
-        result_dict_count = example_pop.grid_results["example"]["count"]
+        result_dict_count = example_pop.population_results["example"]["count"]
 
         # Check if the total probability matches
         self.assertAlmostEqual(
             grid_prob,
             result_dict_prob,
             places=12,
             msg="Total probability from grid {} and from result dict {} are not equal".format(
@@ -656,28 +661,27 @@
             msg="Total count from grid {} and from result dict {} are not equal".format(
                 grid_count, result_dict_count
             ),
         )
 
         # Check if the structure is what we expect. Note: this depends on the probability calculation. if that changes we need to recalibrate this
         test_case_dict = {
-            2.25: 0.01895481306515,
-            3.75: 0.01081338190204,
-            5.75: 0.006168841009268,
-            9.25: 0.003519213484031,
-            13.75: 0.002007648361756,
-            21.25: 0.001145327489437,
-            33.25: 0.0006533888518775,
-            50.75: 0.0003727466560393,
-            78.25: 0.000212645301782,
-            120.75: 0.0001213103421247,
+            2.75: 0.02041431854182,
+            4.25: 0.01094189907528,
+            6.75: 0.005864763750417,
+            10.75: 0.003143462904527,
+            17.25: 0.001684869067647,
+            27.75: 0.0009030753221317,
+            45.25: 0.0004840406017911,
+            73.25: 0.0002594415974398,
+            118.25: 0.0001390584637591,
         }
 
         self.assertEqual(
-            test_case_dict, dict(example_pop.grid_results["example"]["mass"])
+            test_case_dict, dict(example_pop.population_results["example"]["mass"])
         )
 
 
 class test_grid_evolve(unittest.TestCase):
     """
     Unittests for function Population.evolve()
     """
@@ -710,19 +714,19 @@
             dphasevol="dlnm1",
             parameter_name="M_1",
             condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
         )
 
         analytics = test_pop_evolve_1_thread.evolve()
         self.assertLess(
-            np.abs(analytics["total_probability"] - 0.10820655287892997),
+            np.abs(analytics["total_probability"] - 0.10783066961989227),
             1e-10,
-            msg=analytics["total_probability"],
+            msg=analytics["total_probability"] - 0.10783066961989227,
         )
-        self.assertTrue(analytics["total_count"] == 10)
+        self.assertTrue(analytics["total_count"] == 9)
 
     def test_grid_evolve_2_threads(self):
         with Capturing() as _:
             self._test_grid_evolve_2_threads()
 
     def _test_grid_evolve_2_threads(self):
         """
@@ -747,20 +751,21 @@
             probdist="self.three_part_powerlaw(M_1, 0.1, 0.5, 1.0, 100, -1.3, -2.3, -2.3)*M_1",
             dphasevol="dlnm1",
             parameter_name="M_1",
             condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
         )
 
         analytics = test_pop.evolve()
+        print(analytics["total_probability"])
         self.assertLess(
-            np.abs(analytics["total_probability"] - 0.10820655287892997),
+            np.abs(analytics["total_probability"] - 0.10783066961989227),
             1e-10,
-            msg=analytics["total_probability"],
+            msg=np.abs(analytics["total_probability"] - 0.10783066961989227),
         )  #
-        self.assertTrue(analytics["total_count"] == 10)
+        self.assertTrue(analytics["total_count"] == 9)
 
     def test_grid_evolve_2_threads_with_custom_logging(self):
         with Capturing() as _:
             self._test_grid_evolve_2_threads_with_custom_logging()
 
     def _test_grid_evolve_2_threads_with_custom_logging(self):
         """
@@ -867,21 +872,21 @@
             dphasevol="dlnm1",
             parameter_name="M_1",
             condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
         )
 
         analytics = test_pop.evolve()
         self.assertLess(
-            np.abs(analytics["total_probability"] - 0.10820655287892997),
+            np.abs(analytics["total_probability"] - 0.10783066961989227),
             1e-10,
             msg=analytics["total_probability"],
         )  #
         self.assertEqual(analytics["failed_systems_error_codes"], [0])
-        self.assertTrue(analytics["total_count"] == 10)
-        self.assertTrue(analytics["failed_count"] == 10)
+        self.assertTrue(analytics["total_count"] == 9)
+        self.assertTrue(analytics["failed_count"] == 9)
         self.assertTrue(analytics["errors_found"] is True)
         self.assertTrue(analytics["errors_exceeded"] is True)
 
         # test to see if 1 thread does all the systems
 
         test_pop = Population(tmp_dir=TMP_DIR)
         test_pop.set(
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_notebooks.py` & `binarycpython-1.0.0/binarycpython/tests/test_notebooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,41 @@
+# /usr/bin/env python
 """
 Notebook tests
 """
 
 import os
 import unittest
 
 import nbformat
 from nbconvert.preprocessors import ExecutePreprocessor
 
 from binarycpython.utils.functions import temp_dir
 
-TMP_DIR = temp_dir("testing", "test_notebooks")
+TMP_DIR = temp_dir("testing", "test_notebooks", clean_path=True)
 NOTEBOOKS_DIR = os.path.abspath(
     os.path.join(os.path.abspath(__file__), "../../../examples")
 )
 
 # define notebooks
 notebooks = [
     "notebook_api_functionality.ipynb",
-    "notebook_population.ipynb",
-    "notebook_individual_systems.ipynb",
-    "notebook_custom_logging.ipynb",
-    "notebook_extra_features.ipynb",
-    "notebook_luminosity_function_single.ipynb",
-    "notebook_luminosity_function_binaries.ipynb",
     "notebook_BHBH.ipynb",
     "notebook_common_envelope_evolution.ipynb",
+    "notebook_custom_logging.ipynb",
     "notebook_ensembles.ipynb",
+    "notebook_event_based_logging.ipynb",
+    "notebook_extra_features.ipynb",
+    "notebook_HRD.ipynb",
+    "notebook_individual_systems.ipynb",
+    "notebook_luminosity_function_binaries.ipynb",
+    "notebook_luminosity_function_single.ipynb",
+    "notebook_population.ipynb",
     "notebook_solar_system.ipynb",
+    "notebook_source_file_sampling.ipynb",
 ]
 
 
 def run_notebook(notebook_path):
     """
     Function to run notebooks and get the errors
     """
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_plot_functions.py` & `binarycpython-1.0.0/binarycpython/tests/test_plot_functions.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/tests/test_useful_funcs.py` & `binarycpython-1.0.0/binarycpython/tests/test_useful_funcs.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_HPC.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_HPC.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_nJobs for condor
         """
 
         condor_pop = Population()
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_njobs"] = 10
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_njobs"] = 10
 
         result_condor = condor_pop.HPC_njobs()
 
         self.assertEqual(result_condor, 10)
 
     def test_slurm(self):
         with Capturing() as _:
@@ -60,16 +60,16 @@
 
     def _test_slurm(self):
         """
         Unit test for HPC_nJobs for slurm
         """
 
         slurm_pop = Population()
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_njobs"] = 11
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_njobs"] = 11
 
         result_slurm = slurm_pop.HPC_njobs()
 
         self.assertEqual(result_slurm, 11)
 
     def test_none(self):
         with Capturing() as _:
@@ -95,15 +95,15 @@
 
     def _test_HPC_job(self):
         """
         Test to see if its busy with a job
         """
 
         slurm_pop = Population()
-        slurm_pop.grid_options["slurm"] = 1
+        slurm_pop.population_options["slurm"] = 1
 
         self.assertTrue(slurm_pop.HPC_job())
 
 
 class test_HPC_job_type(unittest.TestCase):
     """
     Unittests for function HPC_job_type
@@ -115,30 +115,30 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_nJobs for condor
         """
 
         condor_pop = Population()
-        condor_pop.grid_options["condor"] = 1
+        condor_pop.population_options["condor"] = 1
         result_condor = condor_pop.HPC_job_type()
 
         self.assertEqual(result_condor, "condor")
 
     def test_slurm(self):
         with Capturing() as _:
             self._test_slurm()
 
     def _test_slurm(self):
         """
         Unit test for HPC_nJobs for slurm
         """
 
         slurm_pop = Population()
-        slurm_pop.grid_options["slurm"] = 1
+        slurm_pop.population_options["slurm"] = 1
         result_slurm = slurm_pop.HPC_job_type()
 
         self.assertEqual(result_slurm, "slurm")
 
     def test_none(self):
         with Capturing() as _:
             self._test_none()
@@ -164,17 +164,17 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_jobID for condor
         """
 
         condor_pop = Population()
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
 
         self.assertEqual(
             condor_pop.HPC_jobID(),
             "{ClusterID}.{Process}".format(ClusterID=2, Process=3),
         )
 
     def test_slurm(self):
@@ -183,17 +183,17 @@
 
     def _test_slurm(self):
         """
         Unit test for HPC_jobID for slurm
         """
 
         slurm_pop = Population()
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
 
         self.assertEqual(
             slurm_pop.HPC_jobID(),
             "{jobid}.{jobarrayindex}".format(jobid=4, jobarrayindex=5),
         )
 
     def test_none(self):
@@ -221,33 +221,33 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_jobID_tuple for condor
         """
 
         condor_pop = Population()
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
 
         self.assertEqual(condor_pop.HPC_jobID_tuple(), ("2", "3"))
 
     def test_slurm(self):
         with Capturing() as _:
             self._test_slurm()
 
     def _test_slurm(self):
         """
         Unit test for HPC_jobID for slurm
         """
 
         slurm_pop = Population()
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
 
         self.assertEqual(slurm_pop.HPC_jobID_tuple(), ("4", "5"))
 
     def test_none(self):
         with Capturing() as _:
             self._test_none()
 
@@ -271,28 +271,28 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_dirs for condor
         """
 
         condor_pop = Population()
-        condor_pop.grid_options["condor"] = 1
+        condor_pop.population_options["condor"] = 1
         self.assertEqual(condor_pop.HPC_dirs(), ["condor_dir"])
 
     def test_slurm(self):
         with Capturing() as _:
             self._test_slurm()
 
     def _test_slurm(self):
         """
         Unit test for HPC_jobID for slurm
         """
 
         slurm_pop = Population()
-        slurm_pop.grid_options["slurm"] = 1
+        slurm_pop.population_options["slurm"] = 1
         self.assertEqual(slurm_pop.HPC_dirs(), ["slurm_dir"])
 
     def test_none(self):
         with Capturing() as _:
             self._test_none()
 
     def _test_none(self):
@@ -315,28 +315,28 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_id_filename for condor
         """
 
         condor_pop = Population()
-        condor_pop.grid_options["condor"] = 1
+        condor_pop.population_options["condor"] = 1
         self.assertEqual(condor_pop.HPC_id_filename(), "ClusterID")
 
     def test_slurm(self):
         with Capturing() as _:
             self._test_slurm()
 
     def _test_slurm(self):
         """
         Unit test for HPC_id_filename for slurm
         """
 
         slurm_pop = Population()
-        slurm_pop.grid_options["slurm"] = 1
+        slurm_pop.population_options["slurm"] = 1
         self.assertEqual(slurm_pop.HPC_id_filename(), "jobid")
 
     def test_none(self):
         with Capturing() as _:
             self._test_none()
 
     def _test_none(self):
@@ -359,50 +359,50 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_check_requirements for condor
         """
 
         condor_pop = Population()
-        condor_pop.grid_options["condor"] = 1
+        condor_pop.population_options["condor"] = 1
         self.assertEqual(condor_pop.HPC_id_filename(), "ClusterID")
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
+        condor_pop.population_options["condor"] = 1
 
         # First the False test
         result_1 = condor_pop.HPC_check_requirements()
         self.assertFalse(result_1[0])
         self.assertTrue(len(result_1[1]) > 0)
 
         # First the True test
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor_dir"] = TMP_DIR
         result_2 = condor_pop.HPC_check_requirements()
         self.assertTrue(result_2[0])
         self.assertTrue(len(result_2[1]) == 0)
 
     def test_slurm(self):
         with Capturing() as _:
             self._test_slurm()
 
     def _test_slurm(self):
         """
         Unit test for HPC_check_requirements for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
+        slurm_pop.population_options["slurm"] = 1
 
         # First the False test
         result_1 = slurm_pop.HPC_check_requirements()
         self.assertFalse(result_1[0])
         self.assertTrue(len(result_1[1]) > 0)
 
         # First the True test
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
         result_2 = slurm_pop.HPC_check_requirements()
         self.assertTrue(result_2[0])
         self.assertTrue(len(result_2[1]) == 0)
 
     def test_none(self):
         with Capturing() as _:
             self._test_none()
@@ -429,49 +429,49 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_set_status for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         #
         os.makedirs(
             os.path.dirname(
                 condor_pop.condor_status_file(
-                    condor_dir=condor_pop.grid_options["condor_dir"]
+                    condor_dir=condor_pop.population_options["condor_dir"]
                 )
             ),
             exist_ok=True,
         )
         condor_pop.HPC_set_status("test_set_condor_status")
 
         # Check if ID file exists
         self.assertTrue(
             os.path.isfile(
-                os.path.join(condor_pop.grid_options["condor_dir"], "ClusterID")
+                os.path.join(condor_pop.population_options["condor_dir"], "ClusterID")
             )
         )
 
         # Check if status file exists
         self.assertTrue(
             os.path.isfile(
                 condor_pop.condor_status_file(
-                    condor_dir=condor_pop.grid_options["condor_dir"]
+                    condor_dir=condor_pop.population_options["condor_dir"]
                 )
             )
         )
 
         with open(
             condor_pop.condor_status_file(
-                condor_dir=condor_pop.grid_options["condor_dir"]
+                condor_dir=condor_pop.population_options["condor_dir"]
             ),
             "r",
         ) as f:
             content_file = f.read()
         self.assertTrue(content_file == "test_set_condor_status")
 
     def test_slurm(self):
@@ -480,46 +480,50 @@
 
     def _test_slurm(self):
         """
         Unit test for HPC_set_status for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
 
         #
         os.makedirs(
             os.path.dirname(
                 slurm_pop.slurm_status_file(
-                    slurm_dir=slurm_pop.grid_options["slurm_dir"]
+                    slurm_dir=slurm_pop.population_options["slurm_dir"]
                 )
             ),
             exist_ok=True,
         )
         slurm_pop.HPC_set_status("test_set_slurm_status")
 
         # Check if ID file exists
         self.assertTrue(
-            os.path.isfile(os.path.join(slurm_pop.grid_options["slurm_dir"], "jobid"))
+            os.path.isfile(
+                os.path.join(slurm_pop.population_options["slurm_dir"], "jobid")
+            )
         )
 
         # Check if status file exists
         self.assertTrue(
             os.path.isfile(
                 slurm_pop.slurm_status_file(
-                    slurm_dir=slurm_pop.grid_options["slurm_dir"]
+                    slurm_dir=slurm_pop.population_options["slurm_dir"]
                 )
             )
         )
 
         with open(
-            slurm_pop.slurm_status_file(slurm_dir=slurm_pop.grid_options["slurm_dir"]),
+            slurm_pop.slurm_status_file(
+                slurm_dir=slurm_pop.population_options["slurm_dir"]
+            ),
             "r",
         ) as f:
             content_file = f.read()
         self.assertTrue(content_file == "test_set_slurm_status")
 
 
 class test_HPC_get_status(unittest.TestCase):
@@ -533,24 +537,24 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_get_status for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         #
         os.makedirs(
             os.path.dirname(
                 condor_pop.condor_status_file(
-                    condor_dir=condor_pop.grid_options["condor_dir"]
+                    condor_dir=condor_pop.population_options["condor_dir"]
                 )
             ),
             exist_ok=True,
         )
         condor_pop.HPC_set_status("test_get_condor_status")
 
         #
@@ -563,24 +567,24 @@
 
     def _test_slurm(self):
         """
         Unit test for HPC_set_status for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
 
         #
         os.makedirs(
             os.path.dirname(
                 slurm_pop.slurm_status_file(
-                    slurm_dir=slurm_pop.grid_options["slurm_dir"]
+                    slurm_dir=slurm_pop.population_options["slurm_dir"]
                 )
             ),
             exist_ok=True,
         )
         slurm_pop.HPC_set_status("test_set_slurm_status")
 
         status = slurm_pop.HPC_get_status()
@@ -598,18 +602,18 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_job_task for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         #
         job_task = condor_pop.HPC_job_task()
         self.assertEqual(job_task, 1)
 
     def test_slurm(self):
         with Capturing() as _:
@@ -617,18 +621,18 @@
 
     def _test_slurm(self):
         """
         Unit test for HPC_set_status for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
 
         #
         job_task = slurm_pop.HPC_job_task()
         self.assertEqual(job_task, 1)
 
 
 class test_HPC_dir(unittest.TestCase):
@@ -642,36 +646,36 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_dir for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = os.path.join(TMP_DIR, "condor")
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = os.path.join(TMP_DIR, "condor")
 
         #
         self.assertEqual(condor_pop.HPC_dir(), os.path.join(TMP_DIR, "condor"))
 
     def test_slurm(self):
         with Capturing() as _:
             self._test_slurm()
 
     def _test_slurm(self):
         """
         Unit test for HPC_dir for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = os.path.join(TMP_DIR, "slurm")
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = os.path.join(TMP_DIR, "slurm")
 
         #
         self.assertEqual(slurm_pop.HPC_dir(), os.path.join(TMP_DIR, "slurm"))
 
     def test_none(self):
         with Capturing() as _:
             self._test_slurm()
@@ -698,18 +702,18 @@
 
     def _test_condor(self):
         """
         Unit test for HPC_id_from_dir for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         # id
         id_from_dir = condor_pop.HPC_id_from_dir(condor_pop.HPC_dir())
 
         self.assertEqual(id_from_dir.strip(), str(2))
 
     def test_slurm(self):
@@ -718,18 +722,18 @@
 
     def _test_slurm(self):
         """
         Unit test for HPC_id_from_dir for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = os.path.join(TMP_DIR)
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = os.path.join(TMP_DIR)
 
         # id
         id_from_dir = slurm_pop.HPC_id_from_dir(slurm_pop.HPC_dir())
 
         self.assertEqual(id_from_dir.strip(), str(4))
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_condor.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_condor.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
     def _test_condorID(self):
         """
         Unit test for condorID for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
 
         self.assertEqual(
             condor_pop.condorID(),
             "{ClusterID}.{Process}".format(ClusterID=2, Process=3),
         )
 
 
@@ -55,15 +55,15 @@
 
     def _test_condor_dirs(self):
         """
         Unit test for condor_dirs for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
+        condor_pop.population_options["condor"] = 1
         self.assertEqual(condor_pop.condor_dirs(), ["condor_dir"])
 
 
 class test_condor_check_requirements(unittest.TestCase):
     """
     Unittests for function condor_check_requirements
     """
@@ -74,23 +74,23 @@
 
     def _test_condor_check_requirements(self):
         """
         Unit test for condor_check_requirements for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
+        condor_pop.population_options["condor"] = 1
 
         # First the False test
         result_1 = condor_pop.condor_check_requirements()
         self.assertFalse(result_1[0])
         self.assertTrue(len(result_1[1]) > 0)
 
         # First the True test
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor_dir"] = TMP_DIR
         result_2 = condor_pop.condor_check_requirements()
         self.assertTrue(result_2[0])
         self.assertTrue(len(result_2[1]) == 0)
 
 
 class test_set_condor_status(unittest.TestCase):
     """
@@ -103,51 +103,51 @@
 
     def _test_set_condor_status(self):
         """
         Unit test for set_condor_status for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         id_filename = os.path.isfile(
-            os.path.join(condor_pop.grid_options["condor_dir"], "ClusterID")
+            os.path.join(condor_pop.population_options["condor_dir"], "ClusterID")
         )
         if os.path.isfile(id_filename):
             os.remove(id_filename)
 
         #
         os.makedirs(
             os.path.dirname(
                 condor_pop.condor_status_file(
-                    condor_dir=condor_pop.grid_options["condor_dir"]
+                    condor_dir=condor_pop.population_options["condor_dir"]
                 )
             ),
             exist_ok=True,
         )
         condor_pop.set_condor_status("test_set_condor_status")
 
         # Check if ID file exists
         self.assertTrue(os.path.exists(id_filename))
 
         # Check if status file exists
         self.assertTrue(
             os.path.isfile(
                 condor_pop.condor_status_file(
-                    condor_dir=condor_pop.grid_options["condor_dir"]
+                    condor_dir=condor_pop.population_options["condor_dir"]
                 )
             )
         )
 
         with open(
             condor_pop.condor_status_file(
-                condor_dir=condor_pop.grid_options["condor_dir"]
+                condor_dir=condor_pop.population_options["condor_dir"]
             ),
             "r",
         ) as f:
             content_file = f.read()
         self.assertTrue(content_file == "test_set_condor_status")
 
 
@@ -162,24 +162,24 @@
 
     def _test_get_condor_status(self):
         """
         Unit test for get_condor_status for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         #
         os.makedirs(
             os.path.dirname(
                 condor_pop.condor_status_file(
-                    condor_dir=condor_pop.grid_options["condor_dir"]
+                    condor_dir=condor_pop.population_options["condor_dir"]
                 )
             ),
             exist_ok=True,
         )
         condor_pop.set_condor_status("test_get_condor_status")
 
         #
@@ -198,26 +198,26 @@
 
     def _test_condor_outfile(self):
         """
         Unit test for condor_outfile for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         outfile = condor_pop.condor_outfile()
         condor_id = condor_pop.condorID()
         self.assertEqual(
             outfile,
             os.path.abspath(
                 os.path.join(
-                    condor_pop.grid_options["condor_dir"],
+                    condor_pop.population_options["condor_dir"],
                     "results",
                     "{}.gz".format(condor_id),
                 )
             ),
         )
 
 
@@ -232,18 +232,18 @@
 
     def _test_make_condor_dirs(self):
         """
         Unit test for make_condor_dirs for condor
         """
 
         condor_pop = Population(tmp_dir=TMP_DIR)
-        condor_pop.grid_options["condor"] = 1
-        condor_pop.grid_options["condor_ClusterID"] = 2
-        condor_pop.grid_options["condor_Process"] = 3
-        condor_pop.grid_options["condor_dir"] = TMP_DIR
+        condor_pop.population_options["condor"] = 1
+        condor_pop.population_options["condor_ClusterID"] = 2
+        condor_pop.population_options["condor_Process"] = 3
+        condor_pop.population_options["condor_dir"] = TMP_DIR
 
         shutil.rmtree(TMP_DIR)
         os.makedirs(TMP_DIR)
 
         #
         condor_pop.make_condor_dirs()
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_dataIO.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_dataIO.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_distribution_functions.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_distribution_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,38 +474,43 @@
     def _test_gaussian(self):
         """
         unittest for three_part_power_law
         """
 
         distribution_functions_pop = Population(tmp_dir=TMP_DIR)
 
-        perl_results = [
-            0.00218800520299544,
-            0.0121641269671571,
-            0.0657353455837751,
-            0.104951743573429,
-            0.16899534495487,
-            0.0134332780385336,
+        true_results = [
+            0.002198603353047357,
+            0.012223046956319811,
+            0.06605375115943717,
+            0.10546010357416327,
+            0.1698139161454027,
+            0.013498345478111231,
         ]
+
         python_results = []
         input_lists = []
 
         for logper in LOGPER_LIST:
             input_lists.append(logper)
             python_results.append(
                 distribution_functions_pop.gaussian(logper, 4.8, 2.3, -2.0, 12.0)
             )
 
         # GO over the results and check whether they are equal (within tolerance)
-        for i in range(len(python_results)):
-            msg = "Error: Value perl: {} Value python: {} for logper: {}".format(
-                perl_results[i], python_results[i], str(input_lists[i])
+        for python_result_i, python_result in enumerate(python_results):
+            msg = "Error: Value true: {} Value python: {} for logper: {}".format(
+                true_results[python_result_i],
+                python_result,
+                str(input_lists[python_result_i]),
             )
             self.assertLess(
-                np.abs(python_results[i] - perl_results[i]), TOLERANCE, msg=msg
+                np.abs(python_result - true_results[python_result_i]),
+                TOLERANCE,
+                msg=msg,
             )
 
         # Extra test:
         self.assertTrue(
             distribution_functions_pop.gaussian(15, 4.8, 2.3, -2.0, 12.0) == 0,
             msg="Probability should be 0 because the input period is out of bounds",
         )
@@ -602,70 +607,74 @@
     def _test_Izzard2012_period_distribution(self):
         """
         unittest for three_part_power_law
         """
 
         distribution_functions_pop = Population(tmp_dir=TMP_DIR)
 
-        perl_results = [
+        true_results = [
             0,
-            0.00941322840619318,
-            0.0575068231479569,
-            0.0963349886047932,
-            0.177058537292581,
-            0.0165713385659234,
+            0.009418106687495185,
+            0.05753662529956688,
+            0.09638491294035179,
+            0.17715029554114,
+            0.01657992644327932,
             0,
-            0.00941322840619318,
-            0.0575068231479569,
-            0.0963349886047932,
-            0.177058537292581,
-            0.0165713385659234,
+            0.009418106687495185,
+            0.05753662529956688,
+            0.09638491294035179,
+            0.17715029554114,
+            0.01657992644327932,
             0,
-            0.00941322840619318,
-            0.0575068231479569,
-            0.0963349886047932,
-            0.177058537292581,
-            0.0165713385659234,
+            0.009418106687495185,
+            0.05753662529956688,
+            0.09638491294035179,
+            0.17715029554114,
+            0.01657992644327932,
             0,
-            7.61631504133159e-09,
-            0.168028727846997,
-            0.130936282216512,
-            0.0559170865520968,
-            0.0100358604460285,
+            7.611759724531097e-09,
+            0.16792822989191364,
+            0.13085796924719031,
+            0.055883642551628955,
+            0.01002985799951086,
             0,
-            2.08432736869149e-21,
-            0.18713622563288,
-            0.143151383185002,
-            0.0676299576972089,
-            0.0192427864870784,
+            2.085068289582091e-21,
+            0.18720274739958628,
+            0.1432022695533882,
+            0.06765399828183155,
+            0.01924962676692883,
             0,
-            1.1130335685003e-24,
-            0.194272603987661,
-            0.14771508552257,
-            0.0713078479280884,
-            0.0221093965810181,
+            1.1134801674535124e-24,
+            0.19435055486356775,
+            0.1477743554353869,
+            0.07133645983265395,
+            0.02211826786185681,
         ]
         python_results = []
         input_lists = []
 
         for mass in MASS_LIST:
             for per in PER_LIST:
                 input_lists.append([mass, per])
 
                 python_results.append(
                     distribution_functions_pop.Izzard2012_period_distribution(per, mass)
                 )
 
         # GO over the results and check whether they are equal (within tolerance)
-        for i in range(len(python_results)):
-            msg = "Error: Value perl: {} Value python: {} for mass, per: {}".format(
-                perl_results[i], python_results[i], str(input_lists[i])
+        for python_results_i, python_result in enumerate(python_results):
+            msg = "Error: Value true: {} Value python: {} for mass, per: {}".format(
+                true_results[python_results_i],
+                python_result,
+                str(input_lists[python_results_i]),
             )
             self.assertLess(
-                np.abs(python_results[i] - perl_results[i]), TOLERANCE, msg=msg
+                np.abs(python_result - true_results[python_results_i]),
+                TOLERANCE,
+                msg=msg,
             )
 
 
 class test_flatsections(unittest.TestCase):
     """
     Class for unit test of flatsections
     """
@@ -1137,20 +1146,20 @@
 
         # Test without moecache
         global Moecache
         Moecache = {}
         _ = distribution_functions_pop._get_multiplicity_dict(system_dict)
 
         # test directly with values for Moe function
-        distribution_functions_pop.grid_options["Moe2017_options"]["M_1"] = system_dict[
+        distribution_functions_pop.population_options["Moe2017_options"][
             "M_1"
-        ]
+        ] = system_dict["M_1"]
         multiplicity_fractions_moe = (
             distribution_functions_pop.Moe_di_Stefano_2017_multiplicity_fractions(
-                distribution_functions_pop.grid_options["Moe2017_options"], 1
+                distribution_functions_pop.population_options["Moe2017_options"], 1
             )
         )
 
         multiplicity_dict_moe = distribution_functions_pop._get_multiplicity_dict(
             system_dict=system_dict
         )
         self.assertEqual(
@@ -1158,15 +1167,15 @@
             {
                 el + 1: multiplicity_fractions_moe[el]
                 for el in range(len(multiplicity_fractions_moe))
             },
         )
 
         # Test without setting Moe2017 options
-        distribution_functions_pop.grid_options["Moe2017_options"] = None
+        distribution_functions_pop.population_options["Moe2017_options"] = None
         self.assertRaises(
             ValueError, distribution_functions_pop._get_multiplicity_dict, {"M_1": 1}
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_sampling_variables.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_sampling_variables.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,63 +60,63 @@
             probdist="flatsections(q, [{'min': 0.1/M_1, 'max': 1.0, 'height': 1}])",
             dphasevol="dq",
             precode="M_2 = q * M_1",
             parameter_name="M_2",
             condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
         )
 
-        self.assertIn("q", test_pop.grid_options["_sampling_variables"])
-        self.assertIn("lnm1", test_pop.grid_options["_sampling_variables"])
-        self.assertEqual(len(test_pop.grid_options["_sampling_variables"]), 2)
-
-
-class test_add_grid_variable(unittest.TestCase):
-    """
-    Unittests for add_sampling_variable function
-    """
-
-    def test_add_grid_variable(self):
-        with Capturing() as _:
-            self._test_add_grid_variable()
-
-    def _test_add_grid_variable(self):
-        """
-        Unittests for the function add_grid_variable
-        """
-
-        test_pop = Population()
-
-        resolution = {"M_1": 10, "q": 10}
-
-        test_pop.add_grid_variable(
-            name="lnm1",
-            longname="Primary mass",
-            valuerange=[1, 100],
-            samplerfunc="const(math.log(1), math.log(100), {})".format(
-                resolution["M_1"]
-            ),
-            precode="M_1=math.exp(lnm1)",
-            probdist="three_part_powerlaw(M_1, 0.1, 0.5, 1.0, 100, -1.3, -2.3, -2.3)*M_1",
-            dphasevol="dlnm1",
-            parameter_name="M_1",
-            condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
-        )
-
-        test_pop.add_grid_variable(
-            name="q",
-            longname="Mass ratio",
-            valuerange=["0.1/M_1", 1],
-            samplerfunc="const(0.1/M_1, 1, {})".format(resolution["q"]),
-            probdist="flatsections(q, [{'min': 0.1/M_1, 'max': 1.0, 'height': 1}])",
-            dphasevol="dq",
-            precode="M_2 = q * M_1",
-            parameter_name="M_2",
-            condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
-        )
-
-        self.assertIn("q", test_pop.grid_options["_sampling_variables"])
-        self.assertIn("lnm1", test_pop.grid_options["_sampling_variables"])
-        self.assertEqual(len(test_pop.grid_options["_sampling_variables"]), 2)
+        self.assertIn("q", test_pop.population_options["_sampling_variables"])
+        self.assertIn("lnm1", test_pop.population_options["_sampling_variables"])
+        self.assertEqual(len(test_pop.population_options["_sampling_variables"]), 2)
+
+
+# class test_add_grid_variable(unittest.TestCase):
+#     """
+#     Unittests for add_sampling_variable function
+#     """
+
+#     def test_add_grid_variable(self):
+#         with Capturing() as _:
+#             self._test_add_grid_variable()
+
+#     def _test_add_grid_variable(self):
+#         """
+#         Unittests for the function add_grid_variable
+#         """
+
+#         test_pop = Population()
+
+#         resolution = {"M_1": 10, "q": 10}
+
+#         test_pop.add_grid_variable(
+#             name="lnm1",
+#             longname="Primary mass",
+#             valuerange=[1, 100],
+#             samplerfunc="const(math.log(1), math.log(100), {})".format(
+#                 resolution["M_1"]
+#             ),
+#             precode="M_1=math.exp(lnm1)",
+#             probdist="three_part_powerlaw(M_1, 0.1, 0.5, 1.0, 100, -1.3, -2.3, -2.3)*M_1",
+#             dphasevol="dlnm1",
+#             parameter_name="M_1",
+#             condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
+#         )
+
+#         test_pop.add_grid_variable(
+#             name="q",
+#             longname="Mass ratio",
+#             valuerange=["0.1/M_1", 1],
+#             samplerfunc="const(0.1/M_1, 1, {})".format(resolution["q"]),
+#             probdist="flatsections(q, [{'min': 0.1/M_1, 'max': 1.0, 'height': 1}])",
+#             dphasevol="dq",
+#             precode="M_2 = q * M_1",
+#             parameter_name="M_2",
+#             condition="",  # Impose a condition on this grid variable. Mostly for a check for yourself
+#         )
+
+#         self.assertIn("q", test_pop.population_options["_sampling_variables"])
+#         self.assertIn("lnm1", test_pop.population_options["_sampling_variables"])
+#         self.assertEqual(len(test_pop.population_options["_sampling_variables"]), 2)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_slurm.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_slurm.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
     def _test_slurmID(self):
         """
         Unit test for slurmID for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
 
         self.assertEqual(
             slurm_pop.HPC_jobID(),
             "{jobid}.{jobarrayindex}".format(jobid=4, jobarrayindex=5),
         )
 
 
@@ -55,15 +55,15 @@
 
     def _test_slurm_dirs(self):
         """
         Unit test for slurm_dirs for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
+        slurm_pop.population_options["slurm"] = 1
         self.assertEqual(slurm_pop.slurm_dirs(), ["slurm_dir"])
 
 
 class test_slurm_check_requirements(unittest.TestCase):
     """
     Unittests for function slurm_check_requirements
     """
@@ -74,23 +74,23 @@
 
     def _test_slurm_check_requirements(self):
         """
         Unit test for slurm_check_requirements for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
+        slurm_pop.population_options["slurm"] = 1
 
         # First the False test
         result_1 = slurm_pop.slurm_check_requirements()
         self.assertFalse(result_1[0])
         self.assertTrue(len(result_1[1]) > 0)
 
         # First the True test
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
         result_2 = slurm_pop.slurm_check_requirements()
         self.assertTrue(result_2[0])
         self.assertTrue(len(result_2[1]) == 0)
 
 
 class test_set_slurm_status(unittest.TestCase):
     """
@@ -103,50 +103,52 @@
 
     def _test_set_slurm_status(self):
         """
         Unit test for set_slurm_status for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
 
         id_filename = os.path.isfile(
-            os.path.join(slurm_pop.grid_options["slurm_dir"], "jobid")
+            os.path.join(slurm_pop.population_options["slurm_dir"], "jobid")
         )
         if os.path.isfile(id_filename):
             os.remove(id_filename)
 
         #
         os.makedirs(
             os.path.dirname(
                 slurm_pop.slurm_status_file(
-                    slurm_dir=slurm_pop.grid_options["slurm_dir"]
+                    slurm_dir=slurm_pop.population_options["slurm_dir"]
                 )
             ),
             exist_ok=True,
         )
         slurm_pop.set_slurm_status("test_set_slurm_status")
 
         # Check if ID file exists
         self.assertTrue(os.path.exists(id_filename))
 
         # Check if status file exists
         self.assertTrue(
             os.path.isfile(
                 slurm_pop.slurm_status_file(
-                    slurm_dir=slurm_pop.grid_options["slurm_dir"]
+                    slurm_dir=slurm_pop.population_options["slurm_dir"]
                 )
             )
         )
 
         with open(
-            slurm_pop.slurm_status_file(slurm_dir=slurm_pop.grid_options["slurm_dir"]),
+            slurm_pop.slurm_status_file(
+                slurm_dir=slurm_pop.population_options["slurm_dir"]
+            ),
             "r",
         ) as f:
             content_file = f.read()
         self.assertTrue(content_file == "test_set_slurm_status")
 
 
 class test_get_slurm_status(unittest.TestCase):
@@ -160,24 +162,24 @@
 
     def _test_get_slurm_status(self):
         """
         Unit test for get_slurm_status for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
 
         #
         os.makedirs(
             os.path.dirname(
                 slurm_pop.slurm_status_file(
-                    slurm_dir=slurm_pop.grid_options["slurm_dir"]
+                    slurm_dir=slurm_pop.population_options["slurm_dir"]
                 )
             ),
             exist_ok=True,
         )
         slurm_pop.set_slurm_status("test_set_slurm_status")
 
         status = slurm_pop.get_slurm_status()
@@ -195,26 +197,26 @@
 
     def _test_slurm_outfile(self):
         """
         Unit test for slurm_outfile for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
 
         outfile = slurm_pop.slurm_outfile()
         slurm_id = slurm_pop.slurmID()
         self.assertEqual(
             outfile,
             os.path.abspath(
                 os.path.join(
-                    slurm_pop.grid_options["slurm_dir"],
+                    slurm_pop.population_options["slurm_dir"],
                     "results",
                     "{}.gz".format(slurm_id),
                 )
             ),
         )
 
 
@@ -229,18 +231,18 @@
 
     def _test_make_slurm_dirs(self):
         """
         Unit test for slurm_outfile for slurm
         """
 
         slurm_pop = Population(tmp_dir=TMP_DIR)
-        slurm_pop.grid_options["slurm"] = 1
-        slurm_pop.grid_options["slurm_jobid"] = 4
-        slurm_pop.grid_options["slurm_jobarrayindex"] = 5
-        slurm_pop.grid_options["slurm_dir"] = TMP_DIR
+        slurm_pop.population_options["slurm"] = 1
+        slurm_pop.population_options["slurm_jobid"] = 4
+        slurm_pop.population_options["slurm_jobarrayindex"] = 5
+        slurm_pop.population_options["slurm_dir"] = TMP_DIR
 
         shutil.rmtree(TMP_DIR)
         os.makedirs(TMP_DIR)
 
         #
         slurm_pop.make_slurm_dirs()
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_spacing_functions.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_spacing_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,32 +19,34 @@
 from binarycpython.utils.functions import Capturing, temp_dir
 from binarycpython.utils.population_class import Population
 
 TMP_DIR = temp_dir("tests", "test_spacing_functions")
 
 shutil.rmtree(TMP_DIR)
 os.makedirs(TMP_DIR, exist_ok=True)
-distribution_functions_pop = Population()
 
 
-class test_spacing_functions(unittest.TestCase):
+class test_const(unittest.TestCase):
     """
     Unit test for spacing functions
     """
 
     def test_const(self):
         with Capturing() as _:
             self._test_const()
 
     def _test_const(self):
         """
         Unittest for function const
         """
 
+        distribution_functions_pop = Population()
+
         const_return = distribution_functions_pop.const_linear(1, 10, 10)
+
         self.assertTrue(
-            (const_return == np.linspace(1, 10, 10 + 1)).all(),
+            (const_return == np.linspace(1, 10, 10)).all(),
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `binarycpython-0.9.6/binarycpython/tests/tests_population_extensions/test_version_info.py` & `binarycpython-1.0.0/binarycpython/tests/tests_population_extensions/test_version_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,20 +40,24 @@
         self.assertTrue(isinstance(binary_c_version_info, dict))
         self.assertIn("isotopes", binary_c_version_info)
         self.assertIn("argpairs", binary_c_version_info)
         self.assertIn("ensembles", binary_c_version_info)
         self.assertIn("macros", binary_c_version_info)
         self.assertIn("dt_limits", binary_c_version_info)
         self.assertIn("nucleosynthesis_sources", binary_c_version_info)
+        self.assertIn("binary_c_error_codes", binary_c_version_info)
+        self.assertIn("deflists", binary_c_version_info)
         self.assertIn("miscellaneous", binary_c_version_info)
 
         self.assertIsNotNone(binary_c_version_info["argpairs"])
         self.assertIsNotNone(binary_c_version_info["ensembles"])
         self.assertIsNotNone(binary_c_version_info["macros"])
         self.assertIsNotNone(binary_c_version_info["dt_limits"])
+        self.assertIsNotNone(binary_c_version_info["binary_c_error_codes"])
+        self.assertIsNotNone(binary_c_version_info["deflists"])
         self.assertIsNotNone(binary_c_version_info["miscellaneous"])
 
         if binary_c_version_info["macros"]["NUCSYN"] == "on":
             self.assertIsNotNone(binary_c_version_info["isotopes"])
 
             if binary_c_version_info["macros"]["NUCSYN_ID_SOURCES"] == "on":
                 self.assertIsNotNone(binary_c_version_info["nucleosynthesis_sources"])
@@ -92,14 +96,16 @@
         self.assertIn("isotopes", version_info_parsed.keys())
         self.assertIn("argpairs", version_info_parsed.keys())
         self.assertIn("ensembles", version_info_parsed.keys())
         self.assertIn("macros", version_info_parsed.keys())
         self.assertIn("elements", version_info_parsed.keys())
         self.assertIn("dt_limits", version_info_parsed.keys())
         self.assertIn("nucleosynthesis_sources", version_info_parsed.keys())
+        self.assertIn("binary_c_error_codes", version_info_parsed.keys())
+        self.assertIn("deflists", version_info_parsed.keys())
         self.assertIn("miscellaneous", version_info_parsed.keys())
 
     def test_envvar(self):
         with Capturing() as _:
             self._test_envvar()
 
     def _test_envvar(self):
@@ -118,14 +124,16 @@
         self.assertIn("isotopes", version_info_parsed.keys())
         self.assertIn("argpairs", version_info_parsed.keys())
         self.assertIn("ensembles", version_info_parsed.keys())
         self.assertIn("macros", version_info_parsed.keys())
         self.assertIn("elements", version_info_parsed.keys())
         self.assertIn("dt_limits", version_info_parsed.keys())
         self.assertIn("nucleosynthesis_sources", version_info_parsed.keys())
+        self.assertIn("binary_c_error_codes", version_info_parsed.keys())
+        self.assertIn("deflists", version_info_parsed.keys())
         self.assertIn("miscellaneous", version_info_parsed.keys())
 
 
 class test_parse_binary_c_version_info(unittest.TestCase):
     """
     Unittests for function parse_binary_c_version_info
     """
@@ -148,20 +156,25 @@
         self.assertIn("isotopes", parsed_info.keys())
         self.assertIn("argpairs", parsed_info.keys())
         self.assertIn("ensembles", parsed_info.keys())
         self.assertIn("macros", parsed_info.keys())
         self.assertIn("elements", parsed_info.keys())
         self.assertIn("dt_limits", parsed_info.keys())
         self.assertIn("nucleosynthesis_sources", parsed_info.keys())
+        self.assertIn("binary_c_error_codes", parsed_info.keys())
+        self.assertIn("deflists", parsed_info.keys())
         self.assertIn("miscellaneous", parsed_info.keys())
 
+        #
         self.assertIsNotNone(parsed_info["argpairs"])
         self.assertIsNotNone(parsed_info["ensembles"])
         self.assertIsNotNone(parsed_info["macros"])
         self.assertIsNotNone(parsed_info["dt_limits"])
+        self.assertIsNotNone(parsed_info["binary_c_error_codes"])
+        self.assertIsNotNone(parsed_info["deflists"])
         self.assertIsNotNone(parsed_info["miscellaneous"])
 
         if parsed_info["macros"]["NUCSYN"] == "on":
             self.assertIsNotNone(parsed_info["isotopes"])
 
             if parsed_info["macros"]["NUCSYN_ID_SOURCES"] == "on":
                 self.assertIsNotNone(parsed_info["nucleosynthesis_sources"])
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/custom_logging_functions.py` & `binarycpython-1.0.0/binarycpython/utils/custom_logging_functions.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/utils/dicts.py` & `binarycpython-1.0.0/binarycpython/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/utils/ensemble.py` & `binarycpython-1.0.0/binarycpython/utils/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 from binarycpython.utils.dicts import (
     custom_sort_dict,
     keys_to_floats,
     recursive_change_key_to_float,
     recursive_change_key_to_string,
 )
-from binarycpython.utils.functions import verbose_print
+from binarycpython.utils.functions import output_lines
+from binarycpython.utils.logging_functions import verbose_print
 
 
 def new_grid_ensemble_results():
     """
     Function to return a new grid_ensemble_results dict: this should
     be pre-filled by sub-dicts to prevent later errors.
     """
@@ -47,15 +48,15 @@
         ]
     except KeyError:
         value = None
 
     if value is None:
         try:
             value = ensemble["metadata"]["settings"]["population_settings"][
-                "grid_options"
+                "population_options"
             ][parameter_name]
         except KeyError:
             value = None
 
     if value is None:
         try:
             value = ensemble["metadata"]["settings"]["population_settings"][
@@ -259,33 +260,33 @@
         # If there is no output just return an empty dict:
         if not binary_c_output:
             json_dict = {}
             return json_dict
 
         ensemble_jsons_strings = [
             line
-            for line in binary_c_output.splitlines()
+            for line in output_lines(binary_c_output)
             if line.startswith("ENSEMBLE_JSON")
         ]
 
         json_dict = handle_ensemble_string_to_json(
             ensemble_jsons_strings[0][len("ENSEMBLE_JSON ") :]
         )
 
         if len(ensemble_jsons_strings) > 1:
             verbose_print(
                 "Warning: There is more than one line starting with ENSEMBLE_JSON. Taking the first, but you should check this out.",
                 1,
-                0,
+                1,
             )
     except IndexError:
         verbose_print(
             "Error: Couldn't extract the ensemble information from the output string",
-            0,
-            0,
+            1,
+            1,
         )
 
     return json_dict
 
 
 def handle_ensemble_string_to_json(raw_output):
     """
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/functions.py` & `binarycpython-1.0.0/binarycpython/utils/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Module containing most of the utility functions for the binarycpython package
 
 Functions here are mostly functions used in other classes/functions, or
 useful functions for the user
-
-Tasks:
-    - TODO: change all prints to verbose_prints
 """
 
 import collections
+import copy
 import datetime
 import json
 import os
 import platform
 import resource
+import shutil
 import socket
 import subprocess
 import sys
 import tempfile
 import time
 import types
 from io import StringIO
@@ -27,20 +26,34 @@
 import humanize
 import numpy as np
 import psutil
 from colorama import Back, Fore, Style
 
 from binarycpython import _binary_c_bindings
 from binarycpython.utils.dicts import filter_dict_through_values
+from binarycpython.utils.logging_functions import verbose_print
 
 ########################################################
 # Unsorted
 ########################################################
 
 
+def get_numerical_value(string):
+    """
+    Function to turn a string to a numerical value
+    """
+
+    if "." in string:
+        numerical_value = float(string)
+    else:
+        numerical_value = int(string)
+
+    return numerical_value
+
+
 def calculate_total_mass_system(system_dict):
     """
     Function to calculate the total mass of the system
     """
 
     total_mass = (
         system_dict.get("M_1", 0)
@@ -428,36 +441,14 @@
 
 
 ########################################################
 # utility functions
 ########################################################
 
 
-def verbose_print(
-    message: str, verbosity: int, minimal_verbosity: int, newline: str = "\n"
-) -> None:
-    """
-    Function that decides whether to print a message based on the current verbosity
-    and its minimum verbosity. If verbosity is equal or higher than the minimum, then we print.
-
-    Args:
-        message: message to print.
-        verbosity: current verbosity level.
-        minimal_verbosity: threshold verbosity above which to print.
-        newline: newline character (or set of characters), defaults to ``\\n`` but ``\\x0d`` (carriage return) might be useful.
-    """
-
-    if verbosity >= minimal_verbosity:
-        if newline == "\n":
-            print(message)
-        else:
-            print(message, newline, sep="", end="")
-        sys.stdout.flush()
-
-
 def remove_file(file: str, verbosity: int = 0) -> None:
     """
     Function to remove files but with verbosity
 
     Args:
         file: full file path to the file that will be removed.
         verbosity: current verbosity level (Optional)
@@ -491,40 +482,44 @@
     """
     Function to get the username of the user that spawned the current process
     """
 
     return psutil.Process().username()
 
 
-def temp_dir(*child_dirs: str) -> str:
+def temp_dir(*child_dirs: str, clean_path=False) -> str:
     """
     Function to create directory within the TMP directory of the file system, starting with `/<TMP>/binary_c_python-<username>`
 
     Makes use of os.makedirs exist_ok which requires python 3.2+
 
     Args:
         *child_dirs: str input where each next input will be a child of the previous full_path. e.g. ``temp_dir('tests', 'grid')`` will become ``'/tmp/binary_c_python-<username>/tests/grid'``
-
+        *clean_path (optional): Boolean to make sure that the directory is cleaned if it exists
     Returns:
         the path of a sub directory called binary_c_python in the TMP of the file system
     """
 
     tmp_dir = tempfile.gettempdir()
     username = get_username()
-    path = os.path.join(tmp_dir, "binary_c_python-{}".format(username))
+    full_path = os.path.join(tmp_dir, "binary_c_python-{}".format(username))
 
     # loop over the other paths if there are any:
     if child_dirs:
         for extra_dir in child_dirs:
-            path = os.path.join(path, extra_dir)
+            full_path = os.path.join(full_path, extra_dir)
+
+    # Check if we need to clean the path
+    if clean_path and os.path.isdir(full_path):
+        shutil.rmtree(full_path)
 
     #
-    os.makedirs(path, exist_ok=True)
+    os.makedirs(full_path, exist_ok=True)
 
-    return path
+    return full_path
 
 
 def create_hdf5(data_dir: str, name: str) -> None:
     """
     Function to create an hdf5 file from the contents of a directory:
      - settings file is selected by checking on files ending on settings
      - data files are selected by checking on files ending with .dat
@@ -599,23 +594,27 @@
 ########################################################
 
 
 def output_lines(output: str) -> list:
     """
     Function that outputs the lines that were received from the binary_c run, but now as an iterator.
 
+    This function filters out lines that are empty.
+
     Args:
         output: raw binary_c output
 
     Returns:
         Iterator over the lines of the binary_c output
     """
 
     if output:
-        return output.splitlines()
+        for line in output.splitlines():
+            if line:
+                yield line
     return []
 
 
 def example_parse_output(output: str, selected_header: str) -> dict:
     """
     Function that parses output of binary_c. This version serves as an example and is quite
     detailed. Custom functions can be easier:
@@ -791,15 +790,18 @@
 
 ########################################################
 # Help functions
 ########################################################
 
 
 def get_help(
-    param_name: str = "", print_help: bool = True, fail_silently: bool = False
+    param_name: str = "",
+    print_help: bool = True,
+    fail_silently: bool = False,
+    store_memaddr=None,
 ) -> Union[dict, None]:
     """
     Function that returns the help info for a given parameter, by interfacing with binary_c
 
     Will check whether it is a valid parameter.
 
     Binary_c will output things in the following order:
@@ -829,15 +831,17 @@
             "Please set the param_name to any of the following:\n {}".format(
                 sorted(available_arg_keys)
             )
         )
         return None
 
     if param_name in available_arg_keys:
-        help_info = _binary_c_bindings.return_help(param_name)
+        help_info = _binary_c_bindings.return_help(
+            param_name, store_memaddr=store_memaddr
+        )
         cleaned = [el for el in help_info.split("\n") if not el == ""]
 
         # Get line numbers
         did_you_mean_nr = [
             i for i, el in enumerate(cleaned) if el.startswith("Did you mean")
         ]
         parameter_line_nr = [
@@ -899,27 +903,27 @@
                 param_name, list(available_arg_keys)
             )
         )
 
     return {}
 
 
-def get_help_all(print_help: bool = True) -> dict:
+def get_help_all(print_help: bool = True, store_memaddr=None) -> dict:
     """
     Function that reads out the output of the return_help_all API call to binary_c. This return_help_all binary_c returns all the information for the parameters, their descriptions and other properties. The output is categorised in sections.
 
     Args:
         print_help: (optional, default = True) prints all the parameters and their descriptions.
 
     Returns:
         returns a dictionary containing dictionaries per section. These dictionaries contain the parameters and descriptions etc for all the parameters in that section
     """
 
     # Call function
-    help_all = _binary_c_bindings.return_help_all()
+    help_all = _binary_c_bindings.return_help_all(store_memaddr=store_memaddr)
 
     # String manipulation
     split = help_all.split(
         "############################################################\n"
     )
     cleaned = [el for el in split if not el == "\n"]
 
@@ -1025,16 +1029,19 @@
         print_help: (optional, default = False) Whether to print the information
         fail_silently: (optional, default = True) Whether to fail silently or to print the errors
 
     Returns:
         dictionary containing all dictionaries per section, which then contain as much info as possible per parameter.
     """
 
+    # Setup store memaddr
+    store_memaddr = _binary_c_bindings.return_store_memaddr()
+
     # Get help_all information
-    help_all_dict = get_help_all(print_help=False)
+    help_all_dict = get_help_all(print_help=False, store_memaddr=store_memaddr)
 
     #
     help_all_super_dict = help_all_dict.copy()
 
     # Loop over all sections and stuff
     for section_name, section in help_all_dict.items():
         # Skipping the section i/o because that one shouldn't be available to python anyway
@@ -1043,14 +1050,15 @@
                 parameter = section["parameters"][parameter_name]
 
                 # Get detailed help info
                 detailed_help = get_help(
                     parameter_name,
                     print_help=False,
                     fail_silently=fail_silently,
+                    store_memaddr=store_memaddr,
                 )
 
                 if detailed_help:
                     # check whether the descriptions of help_all and detailed help are the same
                     if not fail_silently:
                         if not parameter["description"] == detailed_help["description"]:
                             print(json.dumps(parameter, indent=4, ensure_ascii=False))
@@ -1069,14 +1077,17 @@
                         parameter["macros"] = detailed_help["macros"]
 
                 section["parameters"][parameter_name] = parameter
 
     if print_help:
         print(json.dumps(help_all_super_dict, indent=4, ensure_ascii=False))
 
+    # Free store memaddr
+    _binary_c_bindings.free_store_memaddr(store_memaddr)
+
     return help_all_super_dict
 
 
 def make_build_text() -> str:
     """
     Function to make build text
 
@@ -1099,80 +1110,180 @@
 """.format(
         git_branch, git_revision, build_datetime
     )
 
     return info_string.strip()
 
 
+def binary_c_parameter_parse_description(parameter_dict: dict):
+    """
+    Function to parse the binary_c parameter dict
+    """
+
+    # Make a local copy
+    parameter_dict = copy.copy(parameter_dict)
+
+    ############
+    # Add description
+    description_string = "Description:\n   "
+
+    # Clean description text
+    description_text = (
+        parameter_dict["description"].strip().replace("|Rout/Rin-1|", "abs(Rout/Rin-1)")
+    )
+    description_text = description_text[0].capitalize() + description_text[1:]
+    if description_text[-1] != ".":
+        description_text = description_text + "."
+    description_string += description_text
+
+    ##############
+    # Add parameter value input type
+    if "parameter_value_input_type" in parameter_dict:
+        description_string += "\n\nParameter input type:\n   {}".format(
+            parameter_dict["parameter_value_input_type"]
+        )
+
+    ##############
+    # Add defaults
+    if "default" in parameter_dict:
+        description_string += "\n\nDefault value:\n   {}".format(
+            parameter_dict["default"]
+        )
+
+    ##############
+    # Add macros
+    if "macros" in parameter_dict:
+        description_string += "\n\nMacros:\n   {}".format(parameter_dict["macros"])
+
+    ##############
+    # Add extra
+    if "rest" in parameter_dict and not parameter_dict["rest"] == "(null)":
+        description_string += "\n\nExtra:\n   {}".format(parameter_dict["rest"])
+
+    ##############
+    # Check if there are newlines, and replace them by newlines with indent
+    description_string = description_string.replace("\n", "\n       ")
+
+    return description_string
+
+
+def build_binary_c_parameter_section_table(
+    section_name: str, section_dict: dict
+) -> str:
+    """
+    Function to build the binary_c parameter section table
+    """
+
+    #
+    indent = "   "
+
+    # Get parameter list and parse descriptions
+    parameter_list_with_descriptions = [
+        [
+            parameter,
+            binary_c_parameter_parse_description(
+                parameter_dict=section_dict[parameter]
+            ),
+        ]
+        for parameter in section_dict.keys()
+    ]
+
+    # Construct table
+    rst_table = """
+.. list-table:: {}
+{}:widths: 25, 75
+{}:header-rows: 1
+""".format(
+        section_name, indent, indent
+    )
+
+    #
+    rst_table += "\n"
+    rst_table += indent + "* - Option\n"
+    rst_table += indent + "  - Description\n"
+
+    for parameter_el in parameter_list_with_descriptions:
+        rst_table += indent + "* - {}\n".format(parameter_el[0])
+        rst_table += indent + "  - {}\n".format(parameter_el[1])
+
+    return rst_table
+
+
+def build_binary_c_parameter_section_text(section_name: str, section_dict: dict) -> str:
+    """
+    Function to write the binary_c parameter section text as an rst table
+    """
+
+    binary_c_parameter_section_text = ""
+
+    # Build header
+    binary_c_parameter_section_text_header = "Section: {}".format(section_name)
+    binary_c_parameter_section_text += binary_c_parameter_section_text_header + "\n"
+    binary_c_parameter_section_text += (
+        "-" * len("Section: {}".format(section_name)) + "\n\n"
+    )
+
+    # build table
+    binary_c_parameter_section_table_text = build_binary_c_parameter_section_table(
+        section_name=section_name, section_dict=section_dict
+    )
+    binary_c_parameter_section_text += binary_c_parameter_section_table_text
+
+    return binary_c_parameter_section_text
+
+
 def write_binary_c_parameter_descriptions_to_rst_file(output_file: str) -> None:
     """
     Function that calls the get_help_super() to get the help text/descriptions for all the
     parameters available in that build.
 
     Writes the results to a .rst file that can be included in the docs.
 
     Args:
         output_file: name of the output .rst file containing the ReStructuredText formatted output
             of all the binary_c parameters.
     """
 
-    # Get the whole arguments dictionary
-    arguments_dict = get_help_super()
-
-    build_info = make_build_text()
-
+    # Check input
     if not output_file.endswith(".rst"):
         raise ValueError(
             "Filename ({}) doesn't end with .rst, please provide a proper filename.".format(
                 output_file
             )
         )
 
+    # Get the whole arguments dictionary
+    arguments_dict = get_help_super()
+
+    # Make build-info text
+    build_info = make_build_text()
+
+    ##########
+    # Write to file
     with open(output_file, "w", encoding="utf-8") as f:
 
         print("Binary\\_c parameters", file=f)
         print("{}".format("=" * len("Binary\\_c parameters")), file=f)
         print(
             "The following chapter contains all the parameters that the current version of binary\\_c can handle, along with their descriptions and other properties.",
             file=f,
         )
         print("\n", file=f)
         print(build_info, file=f)
         print("\n", file=f)
 
-        for el in arguments_dict.keys():
-            print("Section: {}".format(el), file=f)
-            print("{}\n".format("-" * len("Section: {}".format(el))), file=f)
-
-            for arg in arguments_dict[el]["parameters"].keys():
-                argdict = arguments_dict[el]["parameters"][arg]
+        ##########
+        # Loop over sections and write arguments
+        for section_name in arguments_dict.keys():
+            binary_c_parameter_section_text = build_binary_c_parameter_section_text(
+                section_name=section_name,
+                section_dict=arguments_dict[section_name]["parameters"],
+            )
 
-                print("| **Parameter**: {}".format(argdict["param_name"]), file=f)
-                print(
-                    "| **Description**: {}".format(
-                        argdict["description"].replace(
-                            "|Rout/Rin-1|", "abs(Rout/Rin-1)"
-                        )
-                    ),
-                    file=f,
-                )
-                if "parameter_value_input_type" in argdict:
-                    print(
-                        "| **Parameter input type**: {}".format(
-                            argdict["parameter_value_input_type"]
-                        ),
-                        file=f,
-                    )
-                if "default" in argdict:
-                    print("| **Default value**: {}".format(argdict["default"]), file=f)
-                if "macros" in argdict:
-                    print("| **Macros**: {}".format(argdict["macros"]), file=f)
-                if not argdict["rest"] == "(null)":
-                    print("| **Extra**: {}".format(argdict["rest"]), file=f)
-                print("", file=f)
+            print(binary_c_parameter_section_text, file=f)
 
 
 ########################################################
 # log file functions
 ########################################################
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/moe_di_stefano_2017_data.py` & `binarycpython-1.0.0/binarycpython/utils/moe_di_stefano_2017_data.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/utils/plot_functions.py` & `binarycpython-1.0.0/binarycpython/utils/plot_functions.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_class.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/condor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,682 +1,565 @@
 """
-Module containing the Population grid class object.
+The class extension for the population object that contains the Condor functionality
 
-Here all the functionality of a Population object is defined.
-
-TODO: the save_snapshots and save_snapshot, are they actually distinct?
-
-Tasks:
-    - TODO: add functionality to 'on-init' set arguments
-    - TODO: type the private functions
-    - TODO: fix the correct object types for the default values of the bse_options
-    - TODO: think of a clean and nice way to unload and remove the custom_logging_info library from memory (and from disk)
-    - TODO: think of a nice way to remove the loaded grid_code/ generator from memory.
-    - TODO: Some of the methods that we have defined in the (mixin) class are designed to be used as a portal to information (return_binary_c_version_info for example.) The current design is that they are all instance methods, but that is not always necessary. We can decorate them with @staticmethod, or @classmethod to make it easier to use them (https://realpython.com/instance-class-and-static-methods-demystified/)
+TODO: there are many uses of $<variable name> in this file but this is not perl and we should replace them by actual format placeholders
 """
 
-import copy
-import json
-import multiprocessing
+# pylint: disable=E1101
+
 import os
+import pathlib
+import re
+import stat
+import subprocess
 import sys
 import time
-import uuid
-import warnings
 
-from colorama import init as colorama_init
+import datasize
+import lib_programname
+
+from binarycpython.utils.functions import command_string_from_list
+
 
-from binarycpython.utils.dicts import AutoVivificationDict
-from binarycpython.utils.ensemble import new_grid_ensemble_results
-from binarycpython.utils.functions import (
-    check_if_in_shell,
-    filter_arg_dict,
-    get_ANSI_colours,
-    get_defaults,
-    hostnames,
-    mem_use,
-)
-
-# Class extensions
-from binarycpython.utils.population_extensions.analytics import analytics
-from binarycpython.utils.population_extensions.argument_handling import (
-    argument_handling,
-)
-from binarycpython.utils.population_extensions.cache import cache
-from binarycpython.utils.population_extensions.custom_generator_sampling import (
-    custom_generator_sampling,
-)
-from binarycpython.utils.population_extensions.dataIO import dataIO
-from binarycpython.utils.population_extensions.distribution_functions import (
-    distribution_functions,
-)
-from binarycpython.utils.population_extensions.ensemble import ensemble
-from binarycpython.utils.population_extensions.evolution_functions import (
-    evolution_functions,
-)
-from binarycpython.utils.population_extensions.failing_systems_functions import (
-    failing_systems_functions,
-)
-from binarycpython.utils.population_extensions.grid_logging import grid_logging
-from binarycpython.utils.population_extensions.grid_options_defaults import (
-    grid_options_defaults,
-)
-from binarycpython.utils.population_extensions.grid_sampling import grid_sampling
-from binarycpython.utils.population_extensions.HPC import HPC
-from binarycpython.utils.population_extensions.metadata import metadata
-from binarycpython.utils.population_extensions.miscellaneous_functions import (
-    miscellaneous_functions,
-)
-from binarycpython.utils.population_extensions.Moe_di_Stefano_2017 import (
-    Moe_di_Stefano_2017,
-)
-from binarycpython.utils.population_extensions.monte_carlo_sampling import (
-    monte_carlo_sampling,
-)
-from binarycpython.utils.population_extensions.return_functions import return_functions
-from binarycpython.utils.population_extensions.sampling_variables import (
-    sampling_variables,
-)
-from binarycpython.utils.population_extensions.signal_handling import signal_handling
-from binarycpython.utils.population_extensions.source_file_sampling import (
-    source_file_sampling,
-)
-from binarycpython.utils.population_extensions.spacing_functions import (
-    spacing_functions,
-)
-from binarycpython.utils.population_extensions.termination_functions import (
-    termination_functions,
-)
-from binarycpython.utils.population_extensions.version_info import version_info
-
-# Initialise colorama
-colorama_init()
-
-
-class Population(
-    analytics,
-    cache,
-    dataIO,
-    distribution_functions,
-    grid_logging,
-    grid_options_defaults,
-    HPC,
-    metadata,
-    Moe_di_Stefano_2017,
-    spacing_functions,
-    version_info,
-    grid_sampling,
-    monte_carlo_sampling,
-    source_file_sampling,
-    custom_generator_sampling,
-    signal_handling,
-    return_functions,
-    ensemble,
-    argument_handling,
-    termination_functions,
-    miscellaneous_functions,
-    evolution_functions,
-    failing_systems_functions,
-    sampling_variables,
-):
+class condor:
     """
-    Population Object. Contains all the necessary functions to set up, run and process a
-    population of systems
+    Extension for the Population class containing the code for Condor grid runs
     """
 
     def __init__(self, **kwargs):
         """
-        Initialisation function of the population class
-
-        NOTE: (david): we could probably put some of these init statements in the mixin file that they belong to
+        Init function for the condor class
         """
 
-        # Initialise the mix-in classes
-        analytics.__init__(self)
-        cache.__init__(self)
-        dataIO.__init__(self)
-        distribution_functions.__init__(self)
-        grid_logging.__init__(self)
-        grid_options_defaults.__init__(self)
-        grid_sampling.__init__(self)
-        HPC.__init__(self)
-        metadata.__init__(self)
-        Moe_di_Stefano_2017.__init__(self)
-        spacing_functions.__init__(self)
-        version_info.__init__(self)
-        monte_carlo_sampling.__init__(self)
-        source_file_sampling.__init__(self)
-        signal_handling.__init__(self)
-        custom_generator_sampling.__init__(self)
-        argument_handling.__init__(self)
-        return_functions.__init__(self)
-        ensemble.__init__(self)
-        termination_functions.__init__(self)
-        miscellaneous_functions.__init__(self)
-        evolution_functions.__init__(self)
-        failing_systems_functions.__init__(self)
-        sampling_variables.__init__(self)
-
-        # caches
-        self.caches = {}
-        self.cached_function_cache = {}
-        self.original_function_cache = {}
-        self.hostnameslist = hostnames()
-
-        # TODO: put in parameter handling or something
-        # Different sections of options
-        # get binary_c defaults and create a cleaned up dict
-        # Setting stuff will check against the defaults to see if the input is correct.
-        self.defaults = get_defaults()
-        self.cleaned_up_defaults = self._cleanup_defaults()
-        self.available_keys = list(self.defaults.keys())
-        self.special_params = [
-            el for el in list(self.defaults.keys()) if el.endswith("%d")
-        ]
-        self.preloaded_population = None
-        self.signal_count = {}
-
-        # make the input dictionary
-        self.bse_options = {}  # bse_options is just empty.
-
-        # Grid options
-        self.grid_options = copy.deepcopy(self.get_grid_options_defaults_dict())
-
-        # Custom options
-        # TODO: is this really necessary here? The custom options should be empty on start i think
-        self.custom_options = {
-            "save_snapshot": False,
-        }
-
-        # grid code generation
-        self.indent_depth = 0
-        self.indent_string = "    "
-        self.code_string = ""
-
-        # cached value of minimum stellar mass
-        self._minimum_stellar_mass = None
-
-        # logging levels
-        self._LOGGER_VERBOSITY_LEVEL = 1
-        self._CUSTOM_LOGGING_VERBOSITY_LEVEL = 2
-
-        # Set the options that are passed at creation of the object
-        self.set(**kwargs)
-
-        # Load Moe and di Stefano options
-        self.grid_options["Moe2017_options"] = copy.deepcopy(
-            self.get_Moe_di_Stefano_2017_default_options()
-        )
-
-        # Write MOE2017 options to a file. NOTE: (david) not sure why i put this here anymore
-        os.makedirs(
-            os.path.join(self.grid_options["tmp_dir"], "moe_distefano"), exist_ok=True
-        )
-        with self.open(
-            os.path.join(
-                os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
-                "moeopts.dat",
-            ),
-            "w",
-        ) as f:
-            json.dump(
-                self.grid_options["Moe2017_options"], f, indent=4, ensure_ascii=False
-            )
-
-        # Argline dict
-        self.argline_dict = {}
-
-        # Set some memory dicts
-        self.persistent_data_memory_dict = {}
-
-        # shared memory used for logging
-        self.shared_memory = {}
-
-        # variable to test if we're running in a shell
-        self.in_shell = check_if_in_shell()
-
-        # ANSI colours: use them if in a shell
-        self.ANSI_colours = get_ANSI_colours()
-        if self.in_shell is False:
-            for c in self.ANSI_colours:
-                self.ANSI_colours[c] = ""
-
-        # Set global (OS) process id
-        self.grid_options["_main_pid"] = os.getpid()
-
-        # local process ID
-        self.process_ID = 0
-
-        # Create location to store results. Users should write to this dictionary.
-        # The AutoVivificationDict allows for Perl-like addition of possibly
-        # non-existant subdicts.
-        self.grid_results = AutoVivificationDict()
-
-        # Create grid ensemble data location
-        self.grid_ensemble_results = new_grid_ensemble_results()
-
-        # add metadata
-        self.add_system_metadata()
-
-        # set up function cache.
-        # NOTE: (david) I added this here to be able to test the distributions functions without actually running anything.
-        self.setup_function_cache()
+        return
 
-    def jobID(self):
+    def condorID(self, ClusterID=None, Process=None):
         """
-        Function to return the job ID number of this process as a string.
-
-        Normal processes return their process ID (PID)
-        HPC processes return whatever HPC_jobID() gives.
+        Function to return a Condor job ID as a string, [ClusterID].[Process]. The ClusterID and Process passed in are used if given, otherwise we default to the condor_ClusterID and condor_Process in population_options.
         """
-        if self.HPC_job():
-            jobID = self.HPC_jobID()
-            if not jobID:
-                # fallback: use process ID but with "HPC" prepended
-                # (this should never happen!)
-                jobID = "HPC{}".format(self.process_ID)
-        else:
-            jobID = "{}".format(self.process_ID)
-        return jobID
+        if ClusterID is None:
+            ClusterID = self.population_options["condor_ClusterID"]
+        if Process is None:
+            Process = self.population_options["condor_Process"]
+        return "{ClusterID}.{Process}".format(ClusterID=ClusterID, Process=Process)
 
-    ###################################################
-    # Evolution functions
-    ###################################################
-
-    def _pre_run_setup(self) -> None:
+    def condorpath(self, path, condor_dir=None):
         """
-        Function to clean up some stuff in the grid before a run (like results, ensemble results etc)
+        Function to return the full condor directory path.
         """
 
-        # empty results
-        self.grid_results = AutoVivificationDict()
-        self.grid_ensemble_results = new_grid_ensemble_results()
-
-        # set number of processes/cores we want to use
-        self._set_nprocesses()
+        if condor_dir is None:
+            condor_dir = self.population_options["condor_dir"]
+        return os.path.abspath(os.path.join(condor_dir, path))
 
-        # Reset the process ID (should not have a value initially, but can't hurt if it does)
-        self.process_ID = 0
-
-        # Reset population ID:
-        self.grid_options["_population_id"] = uuid.uuid4().hex
-
-        # save number of stored log stats
-        self.shared_memory["n_saved_log_stats"] = multiprocessing.Value("i", 0)
-
-        # set previous logging time
-        _t = time.time()
-        self.shared_memory["prev_log_time"] = multiprocessing.Array(
-            "d", [_t] * self.grid_options["n_logging_stats"]
-        )
-
-        # set previous logging system number to 0
-        self.shared_memory["prev_log_system_number"] = multiprocessing.Array(
-            "i", [0] * self.grid_options["n_logging_stats"]
+    def condor_status_file(self, ClusterID=None, Process=None, condor_dir=None):
+        """
+        Return the condor status file corresponding to the ClusterID and Process, which default to population_options condor_ClusterID and condor_Process, respectively.
+        """
+        return os.path.join(
+            self.condorpath("status", condor_dir=condor_dir),
+            self.condorID(ClusterID, Process),
         )
 
-        # arrays to store memory and max memory use per-thread
-        mem = 1.0 * mem_use()
-        for x in ["", "max_"]:
-            self.shared_memory[x + "memory_use_per_thread"] = multiprocessing.Array(
-                "d", [mem] * self.grid_options["num_processes"]
-            )
-
-        ############################################################
-        # set and check default directory locations
-        ############################################################
-
-        # check tmp_dir exists
-        if self.grid_options["tmp_dir"] is None or not os.path.isdir(
-            self.grid_options["tmp_dir"]
+    def condor_check_requirements(self):
+        """
+        Function to check whether the condor parameters in population_options have been set appropriately.
+        """
+        if self.population_options["condor"] > 0 and (
+            self.population_options["condor_dir"] is None
+            or not os.path.isdir(self.population_options["condor_dir"])
         ):
-            print(
-                "grid_options['tmp_dir'] is not set or it is not a directory : this should point to a temporary directory location, preferably local to your CPUs"
+            return (
+                False,
+                "You have set condor={condor} but not set condor_dir ({condor_dir}) correctly. Please set it and try again.".format(
+                    condor=self.population_options["condor"],
+                    condor_dir=self.population_options["condor_dir"],
+                ),
             )
-            self.exit(code=1)
-
-        # check any HPC requirements are met
-        if self.HPC_job() and not self.HPC_check_requirements()[0]:
-            print(self.HPC_check_requirements()[1])
-            self.exit(code=1)
-
-        # default status_dir and cache_dir to be in tmp_dir
-        #
-        # NOTE: binary_c-python uses its own status_dir, which is not
-        #       the same dir as HPC jobs use (so tmp_dir can be local
-        #       to an HPC job, while the HPC status dir is common to
-        #       all jobs)
-        for x in ["status", "cache"]:
-            if self.grid_options[x + "_dir"] is None:
-                self.grid_options[x + "_dir"] = os.path.join(
-                    self.grid_options["tmp_dir"], x
-                )
-
-        # make list of directories we want to use
-        dirs = ["tmp_dir", "status_dir", "cache_dir"] + self.HPC_dirs()
-
-        for dir in dirs:
-            # try to make directories if they don't exist
-            path = self.grid_options[dir]
-            if path is not None:
-                os.makedirs(path, exist_ok=True)
-
-            # check directories exist and can be written to
-            if path is not None and self.dir_ok(path) is False:
-                print(
-                    "Directory {dir} currently set to {path} cannot be written to. Please check that this directory is correct and you have write access.".format(
-                        dir=dir, path=path
-                    )
-                )
-                self.exit(code=1)
-
-        # Make sure the subdirs of the tmp dir exist
-        subdirs = [
-            "failed_systems",
-            "process_summary",
-            "runtime_systems",
-            "snapshots",
-        ]
-        for subdir in subdirs:
-            path = os.path.join(self.grid_options["tmp_dir"], subdir)
-            os.makedirs(path, exist_ok=True)
-            if self.dir_ok(path) is False:
-                print(
-                    "Sub-Directory {subdir} (in tmp_dir) currently set to {path} cannot be written to. Please check that this directory is correct and you have write access.".format(
-                        subdir=subdir, path=path
-                    )
-                )
-                self.exit(code=1)
-
-        # make sure the arg logging directory exists if we need it
-        if self.grid_options["log_args"]:
-            path = os.path.join(self.grid_options["log_args_dir"])
-            os.makedirs(path, exist_ok=True)
-            if self.dir_ok(path) is False:
-                print(
-                    "Failed to make directory at {path} for output of system arguments. Please check that this directory is correct and you have write access.".format(
-                        path=path
-                    )
-                )
-                self.exit(code=1)
-
-        # restore from existing HPC files
-        self.HPC_restore()
-
-        # set up function cache
-        self.setup_function_cache()
+        return (True, "")
 
-        return
-
-    def clean(self) -> None:
+    def condor_dirs(self):
         """
-        Clean the contents of the population object so it can be reused.
-
-        Calling _pre_run_setup()
-
-        TODO: decide to deprecate this function
+        Directories associated specifically with this condor job.
         """
 
-        self._pre_run_setup()
+        return ["condor_dir"]
 
-    def evolve(self) -> None:
+    def set_condor_status(self, string, condor_dir=None):
         """
-        Entry point function of the whole object. From here, based on the settings,
-        we set up a grid and (probably) evolve the population.
+        Set the condor status corresponing to the self object, which should have condor_ClusterID and condor_Process set.
 
-        There are no direct arguments to this function, the grid_options
-        contain all the relevant settings.
-
-        Returns:
-               a dictionary containing the analytics of the run.
+        Args:
+            string : the status string to be set
+            dir : the directory in which the status directory is held. If not set, this defaults to the HPC directory (e.g. slurm_dir or condor_dir).
         """
+        # save condor ClusterID to file
 
-        # Just to make sure we don't have stuff from a previous run hanging around
-        self._pre_run_setup()
-
-        if self.HPC_job():
-            # run HPC grid: if this returns True, then exit immediately
-            self.grid_options["symlink_latest_gridcode"] = False
-            if self.HPC_grid():
-                self.exit(code=0)
-
-        if self.grid_options["evolution_type"] == "join":
-            # join previously calculated data and return immediately
-            self.HPC_join_previous()
-            return
-
-        # Execute population evolution subroutines
-        result = self._evolve_population_wrapper()
+        if condor_dir is None:
+            condor_dir = self.population_options["condor_dir"]
 
-        if result is False:
-            print("Error detected in _evolve_population() : stopping here")
-
-            sys.exit()
-
-        # make analytics information
-        analytics_dict = self.make_analytics_dict()
-
-        if self.HPC_job():
-            self.HPC_dump_status("HPC grid after analytics")
+        idfile = os.path.join(condor_dir, "ClusterID")
+        if not os.path.exists(idfile):
+            with self.open(idfile, "w", encoding="utf-8") as fClusterID:
+                fClusterID.write(
+                    "{ClusterID}\n".format(
+                        ClusterID=self.population_options["condor_ClusterID"]
+                    )
+                )
+                fClusterID.close()
+                self.NFS_flush_hack(idfile)
 
-        if self.custom_options["save_snapshot"]:
-            # we must save a snapshot, not the population object
-            # ... also save the new starting point: this has to take into
-            # account where we originally started, and that the modulo may
-            # not be == 1.
-            self.grid_options["start_at"] = (
-                self.grid_options["start_at"]
-                + self.grid_options["_count"] * self.grid_options["modulo"]
+        # save condor status
+        file = self.condor_status_file(condor_dir=condor_dir)
+        if file:
+            with self.open(file, "w", encoding="utf-8") as f:
+                f.write(string)
+                f.close()
+                self.NFS_flush_hack(file)
+
+    def get_condor_status(self, ClusterID=None, Process=None, condor_dir=None):
+        """
+        Get and return the condor status corresponing to the self object, or ClusterID.Process if they are passed in. If no status is found, returns an empty string..
+        """
+        if ClusterID is None:
+            ClusterID = self.population_options["condor_ClusterID"]
+        if Process is None:
+            Process = self.population_options["condor_Process"]
+        if ClusterID is None or Process is None:
+            return None
+
+        try:
+            path = pathlib.Path(
+                self.condor_status_file(
+                    condor_dir=condor_dir, ClusterID=ClusterID, Process=Process
+                )
             )
-            # then save the snapshot
-            self.save_snapshot()
-            exitcode = 1 if self.was_killed() else 0
-            self.exit(code=exitcode)
-
-        # Save object to a pickle file
-        elif self.grid_options["save_population_object"]:
-            self.save_population_object()
-
-        # if we're running an HPC grid, exit here
-        # unless we're joining
-        if self.HPC_job() and self.grid_options["evolution_type"] != "join":
-            self.exit()
+            if path:
+                s = path.read_text().strip()
+                return s
+            return ""
 
-        ##
-        # Clean up code: remove files, unset values, unload interpolators etc. This is placed in the general evolve function,
-        # because that makes for easier control
-        self._cleanup()
+        # NOTE: What is the actual exception that can occur here?
+        # TODO: We should specify that exception
+        except:
+            return ""
 
-        return analytics_dict
-
-    ############################################################
-    def _setup(self):
+    def condor_outfile(self, condor_dir=None):
         """
-        Function to set up the necessary stuff for the population evolution.
-
-        The idea is to do all the stuff that is necessary for a population to run.
-        Since we have different methods of running a population, this setup function
-        will do different things depending on different settings
-
-        Returns:
-        True if we want to continue.
-        False if we should return to the original calling script.
+        return a standard filename for the condor chunk files
         """
+        file = "{id}.gz".format(id=self.condorID())
+        if condor_dir is None:
+            condor_dir = self.population_options["condor_dir"]
+        return os.path.abspath(os.path.join(condor_dir, "results", file))
 
-        # Check for restore
-        if self.grid_options["restore_from_snapshot_file"]:
-            self.load_snapshot(self.grid_options["restore_from_snapshot_file"])
-
-        # Check for parse function
-        if not self.grid_options["parse_function"]:
-            print("Warning: No parse function set. Make sure you intended to do this.")
-
-        # #######################
-        # ### Custom logging code:
-        self._set_custom_logging()
-
-        # Unset some value
-        self.grid_options["_probtot"] = 0
-
-        ## check the settings and set all the warnings.
-        if self.bse_options.get("ensemble", None):
-            self._ensemble_setup()
-
-        ##################
-        # Call setup function for specific evolution type
-
-        # grid type
-        if self.grid_options["evolution_type"] == "grid":
-            self._grid_sampling_setup()
-
-        # user-provided custom generator
-        if self.grid_options["evolution_type"] == "custom_generator":
-            self._custom_generator_sampling_setup()
-
-        # Source file
-        elif self.grid_options["evolution_type"] == "source_file":
-            self._source_file_sampling_setup()
-
-        # Monte-carlo
-        elif self.grid_options["evolution_type"] == "monte_carlo":
-            warnings.warn(
-                "Currently the Monte-Carlo implementation is not well-tested and should not be used for anything other than developing reasons."
-            )
-            self._monte_carlo_sampling_setup()
-
-        #######################
-        # Reset values and prepare the grid function
-        self.grid_options[
-            "_probtot"
-        ] = 0  # To make sure that the values are reset. TODO: fix this in a cleaner way
-
-        return True
-
-    def _cleanup(self):
+    def make_condor_dirs(self, condor_dir=None):
         """
-        Function that handles all the cleaning up after the grid has been generated and/or run
-
-        - reset values to 0
-        - remove grid file
-        - unload grid function/module
-        - remove dry grid file
-        - unload dry grid function/module
+        Function to make the condor directories
         """
 
-        # Reset values
-        for x in [
-            "_count",
-            "_probtot",
-            "_failed_count",
-            "_failed_prob",
-            "_total_mass_run",
-            "_total_probability_weighted_mass_run",
-        ]:
-            self.grid_options[x] = 0
-        for x in ["_errors_found", "_errors_exceeded"]:
-            self.grid_options[x] = False
-        self.grid_options["_system_generator"] = None
-        self.grid_options["_failed_systems_error_codes"] = []
-        self.grid_options["_queue_done"] = False
-        self.grid_options["stop_queue"] = False
-        self.grid_options["_job_crashed"] = False
-
-        ############
-        # Calls to each specific evolution type cleanup functions
-
-        # grid type
-        if self.grid_options["evolution_type"] == "grid":
-            self._grid_sampling_cleanup()
+        # make the condor directories
+        if condor_dir is None:
+            condor_dir = self.population_options["condor_dir"]
+        if not condor_dir:
+            self.vb_error(
+                "You must set self.population_options['condor_dir'] (or pass condor_dir=whatever to make_condor_dirs()) to a directory which we can use to set up binary_c-python's Condor files. This should be unique to your set of grids."
+            )
+            os.exit()
 
-        # user-provided custom generator
-        if self.grid_options["evolution_type"] == "custom_generator":
-            self._custom_generator_sampling_cleanup()
+        # make a list of directories, these contain the various condor
+        # output, status files, etc.
+        dirs = []
+        for d in ["stdout", "stderr", "log", "results", "status", "snapshots"]:
+            dirs.append(self.condorpath(d, condor_dir=condor_dir))
+
+        # make the directories: we do not allow these to already exist
+        # as the condor directory should be a fresh location for each set of jobs
+        for d in dirs:
+            try:
+                pathlib.Path(self.condorpath(d, condor_dir=condor_dir)).mkdir(
+                    exist_ok=False, parents=True
+                )
+            # TODO: specify the actual exception
+            # TODO: is this try-except necessary? Especially having the code fail here, instead of earlier, if the directories exist already. Otherwise we can also just do exist_ok=True?
+            except:
+                self.vb_error(
+                    "Tried to make the directory {d} but it already exists. When you launch a set of binary_c jobs on Condor, you need to set your condor_dir to be a fresh directory with no contents.".format(
+                        d=d
+                    )
+                )
+                self.exit(code=1)
 
-        # Source file
-        elif self.grid_options["evolution_type"] == "source_file":
-            self._source_file_sampling_cleanup()
+        # check that they have been made and exist: we need this
+        # because on network mounts (NFS) there's often a delay between the mkdir
+        # above and the actual directory being made. This shouldn't be too long...
+        fail = True
+        count = 0
+        count_warn = 10
+        while fail is True:
+            fail = False
+            count += 1
+            if count > count_warn:
+                self.vb_warning(
+                    "Warning: Have been waiting about {} seconds for Condor directories to be made, there seems to be significant delay...".format(
+                        count
+                    )
+                )
+            for d in dirs:
+                if os.path.isdir(d) is False:
+                    fail = True
+                    time.sleep(1)
+                    break
+
+    def condor_grid(self):  # pragma: no cover
+        """
+        function to be called when running grids when population_options['condor']>=1
+
+        if population_options['condor']==1, we set up the condor script and launch the jobs, then return True to exit.
+        if population_options['condor']==2, we run the stars, which means we return False to continue.
+        if population_options['condor']==3, we are being called from the jobs to run the grids, return False to continue.
+
+        TODO: split this function into some parts
+        TODO: Comment this function better
+        """
+
+        if self.population_options["condor"] == 3:
+            # joining : set the evolution type to "join"
+            #
+            # return False to continue
+            self.population_options["evolution_type"] = "join"
+            return False
+
+        if self.population_options["condor"] == 2:
+            # run a grid of stars only, leaving the results
+            # in the appropriate outfile
+            #
+            # return False to actually run the stars
+            self.population_options["evolution_type"] = "grid"
+            return False
+
+        if self.population_options["condor"] == 1:
+            # if condor=1,  we should have no evolution type, we
+            # set up the Condor scripts and get them evolving
+            # in a Condor queue
+            self.population_options["evolution_type"] = None
+
+            # make dirs
+            self.make_condor_dirs()
+
+            # check we're not using too much RAM
+            if datasize.DataSize(
+                self.population_options["condor_memory"]
+            ) > datasize.DataSize(self.population_options["condor_warn_max_memory"]):
+                self.vb_error(
+                    "WARNING: you want to use {} MB of RAM : this is unlikely to be correct. If you believe it is, set condor_warn_max_memory to something very large (it is currently {} MB)\n".format(
+                        self.population_options["condor_memory"],
+                        self.population_options["condor_warn_max_memory"],
+                    )
+                )
+                self.exit(code=1)
 
-        # Monte-carlo
-        elif self.grid_options["evolution_type"] == "monte_carlo":
-            self._monte_carlo_sampling_cleanup()
+            # get job id (might be passed in)
+            ClusterID = (
+                self.population_options["condor_ClusterID"]
+                if self.population_options["condor_ClusterID"] != ""
+                else "$ClusterID"
+            )
 
-    def _dry_run(self):
-        """
-        Function to dry run the grid and know how many stars it will run
+            # # get job array index
+            # Process = (
+            #     self.population_options["condor_Process"]
+            #     if self.population_options["condor_Process"] != ""
+            #     else "$Process"
+            # )
+
+            if self.population_options["condor_njobs"] == 0:
+                self.vb_error(
+                    "binary_c-python Condor : You must set grid_option condor_njobs to be non-zero"
+                )
+                self.exit(code=1)
 
-        Requires the grid to be built as a dry run grid
+            # find the path to the Python script that we are running
+            pyscriptpath = str(lib_programname.get_path_executed_script())
 
-        NOTE: (david): this is a rather general function, and I'm not sure if we want to have a general dry-run function?
-        """
+            # set the condor initial dir to be our current working directory
+            if not self.population_options["condor_initial_dir"]:
+                self.population_options["condor_initial_dir"] = os.getcwd()
+
+            # build the grid command
+            grid_command = (
+                [
+                    str(self.population_options["condor_env"]),
+                    sys.executable,
+                    pyscriptpath,
+                ]
+                + sys.argv[1:]
+                + [
+                    "start_at=$Process",  # Process is 0,1,2... which is what we want
+                    "modulo=" + str(self.population_options["condor_njobs"]),
+                    "condor_njobs=" + str(self.population_options["condor_njobs"]),
+                    "condor_dir=" + self.population_options["condor_dir"],
+                    "verbosity=" + str(self.population_options["verbosity"]),
+                    "num_cores=" + str(self.population_options["_num_processes"]),
+                ]
+            )
 
-        self.verbose_print(
-            "Doing a dry run of the grid.", self.grid_options["verbosity"], 1
-        )
-        system_generator = self.grid_options["_system_generator"]
-        total_starcount = system_generator(self)
-        self.grid_options["_total_starcount"] = total_starcount
+            grid_command = command_string_from_list(grid_command)
 
-    ###################################################
-    # Unordered functions
-    #
-    # Functions that aren't ordered yet
-    ###################################################
+            # make condor script paths
+            submit_script_path = self.condorpath("condor_submit_script")
+            job_script_path = self.condorpath("condor_job_script")
+
+            # open the files
+            try:
+                submit_script = self.open(submit_script_path, "w", encoding="utf-8")
+            except IOError:
+                self.vb_error(
+                    "Could not open Condor script at {path} for writing: please check you have set {condor_dir} correctly (it is currently {condor_dir} and can write to this directory.".format(
+                        path=submit_script_path,
+                        condor_dir=self.population_options["condor_dir"],
+                    )
+                )
+            try:
+                job_script = self.open(job_script_path, "w", encoding="utf-8")
+            except IOError:
+                self.vb_error(
+                    "Could not open Condor script at {path} for writing: please check you have set {condor_dir} correctly (it is currently {condor_dir} and can write to this directory.".format(
+                        path=job_script_path,
+                        condor_dir=self.population_options["condor_dir"],
+                    )
+                )
 
-    def _cleanup_defaults(self):
-        """
-        Function to clean up the default values:
+            ############################################################
+            # The condor job script calls your binary_c-pthyon script
+            ############################################################
+            condor_job_script = """#!{bash}
+echo "Condor Job Args: $@"
+
+# first two arguments are ClusterID and Process
+export ClusterID="$1"
+export Process="$2"
+shift 2
+
+echo "Job ClusterID $ClusterID Process $Process"
+
+# Set binary_c startup conditions
+export BINARY_C_PYTHON_ORIGINAL_CMD_LINE={cmdline}
+export BINARY_C_PYTHON_ORIGINAL_WD=`{pwd}`
+export BINARY_C_PYTHON_ORIGINAL_SUBMISSION_TIME=`{date}`
+
+# set status to \"running\"
+echo \"running\" > "{condor_dir}/status/$ClusterID.$ProcessID"
+
+# make list of files which is checked for joining
+# echo "{condor_dir}/results/$ClusterID.$Process.gz" >> "{condor_dir}/results/$ClusterID.all"
+
+# run grid of stars and, if this returns 0, set status to finished
+{grid_command} "condor=2" "evolution_type=grid" "condor_ClusterID=$ClusterID" "condor_Process=$Process" "save_population_object={condor_dir}/results/$ClusterID.$Process.gz" && echo -n \"finished\" > "{condor_dir}/status/$ClusterID.$ProcessID" && echo """.format(
+                bash=self.population_options["condor_bash"],
+                date=self.population_options["condor_date"],
+                pwd=self.population_options["condor_pwd"],
+                cmdline=repr(self.population_options["command_line"]),
+                grid_command=grid_command,
+                condor_dir=self.population_options["condor_dir"],
+            )
 
-        from a dictionary, removes the entries that have the following values:
-        - "NULL"
-        - ""
-        - "Function"
+            if not self.population_options["condor_postpone_join"]:
+                joinfile = "{condor_dir}/results/{ClusterID}.all".format(
+                    condor_dir=self.population_options["condor_dir"],
+                    ClusterID=ClusterID,
+                )
+                condor_job_script += """&& echo \"Checking if we can join...\" && echo && {grid_command} "condor=3" "evolution_type=join" "joinlist={joinfile}" "condor_ClusterID=$ClusterID" "condor_Process=$Process"
+                """.format(
+                    # bash=self.population_options["condor_bash"],
+                    grid_command=grid_command,
+                    joinfile=joinfile,
+                )
 
-        Uses the function from utils.functions
+                ############################################################
+                # The Condor submit script is sent to condor_submit
+                # In here we know $(Cluster) and $(Process) which identify
+                # each job
+                ############################################################
+                extra_settings = ""
+                if self.population_options["condor_extra_settings"]:
+                    for key in self.population_options["condor_extra_settings"]:
+                        extra_settings += "{key} = {value}\n".format(
+                            key=key,
+                            value=self.population_options["condor_extra_settings"][key],
+                        )
+
+                jobid = "$(Cluster).$(Process)"
+                condor_submit_script = """
+executable = {usr_bin_env}
+arguments = {bash} {job_script_path} $(Cluster) $(Process)
+universe = {universe}
+getenv = {getenv}
+initial_dir = {initial_dir}
+output = {outfile}
+error = {errfile}
+log = {logfile}
+stream_output = {stream_output}
+stream_error = {stream_error}
+request_memory = {request_memory}
+request_cpus = {request_cpus}
+should_transfer_files = {should_transfer_files}
+when_to_transfer_output = {when_to_transfer_output}
+requirements = {requirements}
+JobBatchName = {batchname}
+kill_sig = {kill_sig}
+{extra_settings}
+queue {njobs}
+            """.format(
+                    usr_bin_env=self.population_options["condor_env"],
+                    bash=self.population_options["condor_bash"],
+                    job_script_path=job_script_path,
+                    universe=self.population_options["condor_universe"],
+                    getenv=self.population_options["condor_getenv"],
+                    initial_dir=self.population_options["condor_initial_dir"],
+                    outfile=os.path.abspath(
+                        os.path.join(
+                            self.population_options["condor_dir"], "stdout", jobid
+                        )
+                    ),
+                    errfile=os.path.abspath(
+                        os.path.join(
+                            self.population_options["condor_dir"], "stderr", jobid
+                        )
+                    ),
+                    logfile=os.path.abspath(
+                        os.path.join(
+                            self.population_options["condor_dir"], "log", jobid
+                        )
+                    ),
+                    stream_output=self.population_options["condor_stream_output"],
+                    stream_error=self.population_options["condor_stream_error"],
+                    request_memory=self.population_options["condor_memory"],
+                    request_cpus=self.population_options["_num_processes"],
+                    should_transfer_files=self.population_options[
+                        "condor_should_transfer_files"
+                    ],
+                    when_to_transfer_output=self.population_options[
+                        "condor_when_to_transfer_output"
+                    ],
+                    requirements=self.population_options["condor_requirements"],
+                    batchname=self.population_options["condor_batchname"],
+                    kill_sig=self.population_options["condor_kill_sig"],
+                    extra_settings=extra_settings,
+                    njobs=self.population_options["condor_njobs"],
+                )
 
-        TODO: Rethink this functionality. seems a bit double, could also be just outside of the class
-        """
+            # write the scripts, close them and make them executable by
+            # all (so the condor user can pick it up)
+            for file, contents in [
+                (submit_script, condor_submit_script),
+                (job_script, condor_job_script),
+            ]:
+                path = file.name
+                file.writelines(contents)
+                file.close()
+                os.chmod(
+                    path,
+                    stat.S_IREAD
+                    | stat.S_IWRITE
+                    | stat.S_IEXEC
+                    | stat.S_IRGRP
+                    | stat.S_IXGRP
+                    | stat.S_IROTH
+                    | stat.S_IXOTH,
+                )
 
-        binary_c_defaults = self.return_binary_c_defaults().copy()
-        cleaned_dict = filter_arg_dict(binary_c_defaults)
+            if not self.population_options["condor_postpone_submit"]:
+                # call sbatch to launch the condor jobs
+                cmd = [self.population_options["condor_submit"], submit_script_path]
+                with subprocess.Popen(
+                    cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+                ) as pipes:
+                    std_out, std_err = pipes.communicate()
+
+                if pipes.returncode != 0:
+                    # an error happened!
+                    err_msg = "{red}{err}\nReturn Code: {code}{reset}".format(
+                        err=std_err.strip(),
+                        code=pipes.returncode,
+                        red=self.ANSI_colours["red"],
+                        reset=self.ANSI_colours["reset"],
+                    )
+                    raise Exception(err_msg)
 
-        return cleaned_dict
+                if len(std_err) > 0:
+                    self.vb_info(
+                        "{red}{err}{reset}".format(
+                            red=self.ANSI_colours["red"],
+                            reset=self.ANSI_colours["reset"],
+                            err=std_err.strip().decode("utf-8"),
+                        )
+                    )
 
-    def _increment_probtot(self, prob):
-        """
-        Function to add to the total probability. For now not used
-        """
+                self.vb_info(
+                    "{yellow}{out}{reset}".format(
+                        yellow=self.ANSI_colours["yellow"],
+                        reset=self.ANSI_colours["reset"],
+                        out=std_out.strip().decode("utf-8"),
+                    )
+                )
+            else:
+                # just say we would have (use this for testing)
+                self.vb_info(
+                    "Condor script is at {path} but has not been launched".format(
+                        path=submit_script_path
+                    )
+                )
 
-        self.grid_options["_probtot"] += prob
+        # some messages to the user, then return
+        if self.population_options["condor_postpone_submit"] == 1:
+            self.vb_info(
+                "Condor script written, to {path}, but launching the jobs with sbatch was postponed.".format(
+                    path=submit_script_path
+                )
+            )
+        else:
+            self.vb_info("Condor jobs launched.")
+            self.vb_info("All done in condor_grid().")
 
-    def _increment_count(self):
-        """
-        Function to add to the total number of stars. For now not used
-        """
-        self.grid_options["_count"] += 1
+        # return True so we exit immediately
+        return True
 
-    #####
-    #
-    def _get_generator(self):
+    def condor_queue_stats(self):  # pragma: no cover
         """
-        Function to get the generator. Handles the choice of evolution method
+        Return condor queue statistics for this job
         """
 
-        ###
-        # Get generator for different evolution methods
+        _id = self.population_options["condor_ClusterID"]
+        if not _id:
+            return None
 
-        # grid type
-        if self.grid_options["evolution_type"] == "grid":
-            generator = self._grid_sampling_get_generator()
+        cmd = "{} {} 2>&1".format(
+            "/usr/bin/condor_q", _id  # self.population_options["condor_q"],
+        )
+        self.vb_debug("Q cmd", cmd)
 
-        # user-provided custom generator
-        if self.grid_options["evolution_type"] == "custom_generator":
-            generator = self._custom_generator_sampling_get_generator()
+        with subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE) as subp:
+            result = subp.stdout.read()
+        self.vb_debug("Q result ", result)
 
-        # Source file
-        elif self.grid_options["evolution_type"] == "source_file":
-            generator = self._source_file_sampling_get_generator()
+        if not result:
+            return None
 
-        # Monte-carlo
-        elif self.grid_options["evolution_type"] == "monte_carlo":
-            generator = self._monte_carlo_sampling_get_generator()
+        d = {}
+        for x in [
+            "jobs",
+            "completed",
+            "removed",
+            "idle",
+            "running",
+            "held",
+            "suspended",
+        ]:
+            self.vb_debug("Q x ", x)
+            m = re.search("(\d+)\s+{}".format(x), result)  # noqa: W605
+            self.vb_debug("Q m ", m)
+            if m:
+                d[x] = m.group(0)
 
-        return generator
+        self.vb_debug("Q d ", d)
+        return d
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/HPC.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/HPC.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         slurm.__init__(self)
 
     def HPC_njobs(self):
         """
         Function to return the number of jobs this HPC jobs will use, as an int.
         """
 
-        if self.grid_options["slurm"] > 0:
-            n = self.grid_options["slurm_njobs"]
-        elif self.grid_options["condor"] > 0:
-            n = self.grid_options["condor_njobs"]
+        if self.population_options["slurm"] > 0:
+            n = self.population_options["slurm_njobs"]
+        elif self.population_options["condor"] > 0:
+            n = self.population_options["condor_njobs"]
         else:
             n = None
         return int(n)
 
     def HPC_make_joiningfile(
         self,
         hpc_jobid=None,
@@ -95,222 +95,220 @@
                 )
             ]
         string = "".join(lines)
 
         # check the joiningfile doesn't exist
         if not overwrite and os.path.isfile(file):
             # file already exists
-            print(
+            self.vb_info(
                 "Cannot make joiningfile at {file} because it already exists, instead I am waiting for it to be unlocked.".format(
                     file=file
                 )
             )
             self.wait_for_unlock(file)
             joinfiles = self.HPC_load_joinfiles_list(joinlist=file)
-            print(
+            self.vb_info(
                 "Unlocked and got {} should be {}".format(
                     len(joinfiles), self.HPC_njobs()
                 )
             )
             # perhaps exit here? (e.g. for debugging)
             if error_on_overwrite:
                 self.exit(code=1)
             x = False
         else:
             # open the file, but locked so we have first unique access
             (f, lock) = self.locked_open_for_write(file)
 
             # write to it if we are first to obtain unique access
             if lock and f:
-                print("Making joiningfile list range (0,{}) at {}".format(n, file))
+                self.vb_info(
+                    "Making joiningfile list range (0,{}) at {}".format(n, file)
+                )
                 f.write(string)
                 f.flush()
                 os.fsync(f.fileno())
                 x = True
                 self.locked_close(f, lock)
                 os.sync()
                 self.NFS_flush_hack(file)
 
-                print(
+                self.vb_info(
                     "Checking joiningfile {} length (size = {})".format(
                         file, os.path.getsize(file)
                     )
                 )
                 joinfiles = self.HPC_load_joinfiles_list(joinlist=file)
-                print("Got {} should be {}".format(len(joinfiles), self.HPC_njobs()))
+                self.vb_info(
+                    "Got {} should be {}".format(len(joinfiles), self.HPC_njobs())
+                )
 
             else:
                 x = False
-                print("Joiningfile failed to get lock: waiting for it to be unlocked")
+                self.vb_info(
+                    "Joiningfile failed to get lock: waiting for it to be unlocked"
+                )
                 self.wait_for_unlock(file)
         return x
 
     def HPC_joinlist(self, joinlist=None):
         """
         Function to return the default HPC joinlist file.
         """
 
         if joinlist is None:
-            joinlist = self.grid_options["joinlist"]
+            joinlist = self.population_options["joinlist"]
         return joinlist
 
     def HPC_load_joinfiles_list(self, joinlist=None):
         """
         Function to load in the list of files we should join, and return it.
 
-        If grid_options['HPC_rebuild_joinlist'] is True, we rebuild it.
+        If population_options['HPC_rebuild_joinlist'] is True, we rebuild it.
         """
 
         prefix = os.path.join(self.HPC_dir(), "results")
 
-        if self.grid_options["HPC_rebuild_joinlist"] == 1:
+        if self.population_options["HPC_rebuild_joinlist"] == 1:
             # we should rebuild the joinlist from the
             # files we find at the prefix directory
-            print("Rebuild joinlist from existing files")
+            self.vb_info("Rebuild joinlist from existing files")
             joinlist = glob.glob(str(prefix) + "/*.gz")
             return joinlist
 
         joinlist = self.HPC_joinlist(joinlist=joinlist)
         try:
             self.wait_for_unlock(joinlist)
             f = self.open(joinlist, "r", encoding="utf-8")
             joinlist = f.read().splitlines()
             f.close()
 
-            if False:
-                print(
-                    "HPC_load_joinfiles_list read joinlist {joinlist} -> gave file joinlist of length {len_joinlist} with contents {joinlist}".format(
-                        joinlist=joinlist, len_joinlist=len(joinlist)
-                    )
+            self.vb_info(
+                "HPC_load_joinfiles_list read joinlist {joinlist} -> gave file joinlist of length {len_joinlist} with contents {joinlist}".format(
+                    joinlist=joinlist, len_joinlist=len(joinlist)
                 )
+            )
         except Exception as e:
-            print(
+            self.vb_info(
                 "Failed to open joinlist at {joinlist} : {e}".format(
                     joinlist=joinlist, e=e
                 )
             )
             self.exit(code=1)
 
         return joinlist
 
     def HPC_join_from_files(self, newobj, joinfiles):
         """
         Merge the results from the list joinfiles into newobj.
         """
         for file in joinfiles:
-            print("Join data in", file)
+            self.vb_info("Join data in", file)
             self.merge_populations_from_file(newobj, file)
         return newobj
 
     def HPC_can_join(self, joinfiles, joiningfile, vb=False):
         """
         Check the joinfiles to make sure they all exist
         and their .saved equivalents also exist
         """
 
-        print("HPC check if we can join at {}".format(now()))
+        self.vb_info("HPC check if we can join at {}".format(now()))
 
-        if self.grid_options["HPC_force_join"] == 0 and os.path.exists(joiningfile):
-            if vb:
-                print(
-                    "cannot join : joiningfile exists at {} (check 1)".format(
-                        joiningfile
-                    )
-                )
+        if self.population_options["HPC_force_join"] == 0 and os.path.exists(
+            joiningfile
+        ):
+            self.vb_warning(
+                "cannot join : joiningfile exists at {} (check 1)".format(joiningfile)
+            )
             return False
         else:
-            if vb:
-                print("joiningfile (at {}) does not exist".format(joiningfile))
+            self.vb_warning("joiningfile (at {}) does not exist".format(joiningfile))
 
         for file in joinfiles:
-            if vb:
-                print("check for {}".format(file))
-
+            self.vb_info("check for {}".format(file))
             if os.path.exists(file) is False:
-                if vb:
-                    print('cannot join : file "{}" does not exist'.format(file))
+                self.vb_warning('cannot join : file "{}" does not exist'.format(file))
                 return False
 
             savedfile = file + ".saved"
-            if vb:
-                print("check for {}".format(savedfile))
 
+            self.vb_info("check for {}".format(savedfile))
             if os.path.exists(savedfile) is False:
-                if vb:
-                    print(
-                        'cannot join : savedfile "{}" does not exist'.format(savedfile)
-                    )
+                self.vb_warning(
+                    'cannot join : savedfile "{}" does not exist'.format(savedfile)
+                )
                 return False
 
             # found both files
-            if vb:
-                print("found {} and {}".format(file, savedfile))
+            self.vb_info("found {} and {}".format(file, savedfile))
 
         # check for joiningfile again
-        if self.grid_options["HPC_force_join"] == 1:
-            print("Forcing join because HPC_force_join is set")
+        if self.population_options["HPC_force_join"] == 1:
+            self.vb_info("Forcing join because HPC_force_join is set")
             x = True
         elif os.path.exists(joiningfile):
-            if vb:
-                print(
-                    "cannot join: joiningfile exists at {} (check 2)".format(
-                        joiningfile
-                    )
-                )
+            self.vb_warning(
+                "cannot join: joiningfile exists at {} (check 2)".format(joiningfile)
+            )
             x = False
         elif vb:
-            print("joiningfile at {} does not exist : can join".format(joiningfile))
+            self.vb_warning(
+                "joiningfile at {} does not exist : can join".format(joiningfile)
+            )
             x = True
 
-        if vb:
-            print("returning {} from HPC_can_join()".format(x))
+        self.vb_info("returning {} from HPC_can_join()".format(x))
 
         return x
 
     def HPC_job(self):
         """
         Function to return True if we're running an HPC (Slurm or Condor) job, False otherwise.
         """
 
-        return bool(self.grid_options["slurm"] > 0 or self.grid_options["condor"] > 0)
+        return bool(
+            self.population_options["slurm"] > 0
+            or self.population_options["condor"] > 0
+        )
 
     def HPC_job_task(self):
         """
         Function to return the HPC task number, which is 1 when setting
         up and running the scripts, 2 when joining data.
         """
-        if self.grid_options["slurm"] > 0:
-            x = self.grid_options["slurm"]
-        elif self.grid_options["condor"] > 0:
-            x = self.grid_options["condor"]
+        if self.population_options["slurm"] > 0:
+            x = self.population_options["slurm"]
+        elif self.population_options["condor"] > 0:
+            x = self.population_options["condor"]
         else:
             x = 0
         return x
 
     def HPC_job_type(self):
         """
         Function to return a string telling us the type of an HPC job, i.e.
         "slurm", "condor" or "None".
         """
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             hpc_type = "slurm"
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             hpc_type = "condor"
         else:
             hpc_type = "None"
         return hpc_type
 
     def HPC_jobID(self):
         """
         Function to return an HPC (Slurm or Condor) job id in the form of a string, x.y. Returns None if not an HPC job.
         """
 
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             hpc_jobid = self.slurmID()
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             hpc_jobid = self.condorID()
         else:
             # not an HPC job
             hpc_jobid = None
 
         return hpc_jobid
 
@@ -335,51 +333,51 @@
         """
         Set the appropriate HPC job (Condor or Slurm) status file to whatever is given in string.
 
         Arguments:
                  string : the new contents of the status file
         """
 
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             self.set_slurm_status(string)
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             self.set_condor_status(string)
         else:
             pass
 
     def HPC_get_status(self, job_id=None, job_index=None, hpc_dir=None):
         """
         Get and return the appropriate HPC job (Condor or Slurm) status string for this job (or, if given, the job at id.index)
 
         Args:
             hpc_dir : optional HPC run directory. If not set, the default (e.g. slurm_dir or condor_dir)
                   is used.
             job_id,job_index : the id and index of the job to be queried
         """
 
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             status = self.get_slurm_status(
                 jobid=job_id, jobarrayindex=job_index, slurm_dir=hpc_dir
             )
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             status = self.get_condor_status(
                 ClusterID=job_id, Process=job_index, condor_dir=hpc_dir
             )
         else:
             status = None
 
         return status
 
     def HPC_dirs(self):
         """
         Function to return a list of directories required for this HPC job.
         """
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             dirs = self.slurm_dirs()
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             dirs = self.condor_dirs()
         else:
             dirs = []
         return dirs
 
     def HPC_grid(self, makejoiningfile=True):  # pragma: no cover
         """
@@ -397,46 +395,46 @@
 
         # give some current status about the HPC run
         self.HPC_dump_status("HPC grid before")
 
         if makejoiningfile and self.HPC_job_task() == 2 and jobid is not None:
             self.HPC_make_joiningfile()
 
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             x = self.slurm_grid()
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             x = self.condor_grid()
         else:
             x = None  # should not happen
 
         # give some current status about the HPC run
         self.HPC_dump_status("HPC grid after")
 
         return x
 
     def HPC_check_requirements(self):
         """
         Function to check HPC option requirements have been met. Returns a tuple: (True,"") if all is ok, (False,<warning string>) otherwise.
         """
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             t = self.slurm_check_requirements()
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             t = self.condor_check_requirements()
         else:
             t = (True, "")
         return t
 
     def HPC_id_filename(self):
         """
         HPC jobs have a filename in their directory which specifies the job id. This function returns the contents of that file as a string, or None on failure.
         """
 
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             filename = "jobid"
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             filename = "ClusterID"
         else:
             filename = None
         return filename
 
     def HPC_id_from_dir(self, hpc_dir):
         """
@@ -446,161 +444,165 @@
         filename = self.HPC_id_filename()
         if not filename:
             return None
 
         file = os.path.join(hpc_dir, filename)
         f = self.open(file, "r", encoding="utf-8")
         if not f:
-            print(
+            self.vb_error(
                 "Error: could not open {file} to read the HPC jobid of the directory {hpc_dir}".format(
                     file=file, hpc_dir=hpc_dir
                 )
             )
             self.exit(code=1)
 
         oldjobid = f.read().strip()
         if not oldjobid:
-            print("Error: could not find jobid in {hpc_dir}".format(hpc_dir=hpc_dir))
+            self.vb_error(
+                "Error: could not find jobid in {hpc_dir}".format(hpc_dir=hpc_dir)
+            )
             self.exit(code=1)
         else:
             f.close()
             return oldjobid
 
     def HPC_restore(self):
         """
-        Set grid_options['restore_from_snapshot_file'] so that we restore data from existing
-        an HPC run if self.grid_options[hpc_job_type+'_restart_dir'], where hpc_job_type is "slurm" or "condor",
-        is provided, otherwise do nothing. This only works if grid_options[hpc_job_type] == self.HPC_job_task() == 2, which is
+        Set population_options['restore_from_snapshot_file'] so that we restore data from existing
+        an HPC run if self.population_options[hpc_job_type+'_restart_dir'], where hpc_job_type is "slurm" or "condor",
+        is provided, otherwise do nothing. This only works if population_options[hpc_job_type] == self.HPC_job_task() == 2, which is
         the run-grid stage of the process.
         """
 
         hpc_job_type = self.HPC_job_type()
         if hpc_job_type is None:
             return
 
         key = hpc_job_type + "_restart_dir"
-        if key not in self.grid_options:
+        if key not in self.population_options:
             return
 
         # get restart directory
-        hpc_dir = self.grid_options[hpc_job_type + "_restart_dir"]
+        hpc_dir = self.population_options[hpc_job_type + "_restart_dir"]
         if hpc_dir is None:
             return
 
         # get HPC job index
         index = self.HPC_jobID_tuple()[1]
         if index is None:
             return
 
-        if self.HPC_job_task() == 2:  # (same as) self.grid_options[hpc_job_type] == 2:
+        if (
+            self.HPC_job_task() == 2
+        ):  # (same as) self.population_options[hpc_job_type] == 2:
             old_id = self.HPC_id_from_dir(hpc_dir)
-            print(
+            self.vb_info(
                 "Restart from hpc_dir {hpc_dir} which was has (old) ID {old_id}, we are job index {index}".format(
                     hpc_dir=hpc_dir, old_id=old_id, index=index
                 )
             )
 
             # check status: if "finished", we don't have to do anything
             status = self.HPC_get_status(hpc_dir=hpc_dir)
 
             if status == "finished":
-                print("Status is finished, cannot and do not need to restart.")
+                self.vb_info("Status is finished, cannot and do not need to restart.")
                 self.exit(code=0)
 
             file = os.path.join(
                 dir, "snapshots", "{id}.{index}.gz".format(id=old_id, index=index)
             )
 
             if os.path.exists(file):
                 # have data from which we can restore, set it in
                 # the appropriate grid option
-                print("Restore this run from snapshot {file}".format(file=file))
-                self.grid_options["restore_from_snapshot_file"] = file
+                self.vb_info("Restore this run from snapshot {file}".format(file=file))
+                self.population_options["restore_from_snapshot_file"] = file
             else:
                 # no snapshot: so no need to restore, just exit
-                print(
+                self.vb_info(
                     "Expected snapshot at {file} but none was found".format(file=file)
                 )
                 self.exit(code=0)
         return
 
     def HPC_join_previous(self):
         """
         Function to join previously generated datasets.
         """
         # check that our job has finished
         status = self.HPC_get_status()
-        print("Job status", status)
+        self.vb_info("Job status", status)
 
-        if self.grid_options["HPC_force_join"] == 0 and status != "finished":
+        if self.population_options["HPC_force_join"] == 0 and status != "finished":
             # job did not finish : save a snapshot
-            print(
+            self.vb_info(
                 "This job did not finish (status is {status}) : cannot join".format(
                     status=status
                 )
             )
         else:
             # our job has finished
             HPC_status = self.HPC_status()
 
             # HPC_queue_stats = self.HPC_queue_stats()
 
             if HPC_status["status"]["finished"] != HPC_status["njobs"]:
-                print(
+                self.vb_info(
                     "HPC_status reports {} finished jobs out of {}. We cannot join because not all the jobs are finished. Exiting.".format(
                         HPC_status["status"]["finished"], HPC_status["njobs"]
                     )
                 )
                 self.exit(1)
 
             joinfiles = self.HPC_load_joinfiles_list()
             joiningfile = self.HPC_path("joining")
-            print(
+            self.vb_info(
                 "Joinfile list n={n} (should be {m})".format(
                     n=len(joinfiles), m=self.HPC_njobs()
                 )
             )
-            print("Joingingfile path : ", joiningfile)
+            self.vb_info("Joingingfile path : ", joiningfile)
 
             if len(joinfiles) != self.HPC_njobs():
-                print("Number of joinfiles != njobs : this is wrong, exiting.")
+                self.vb_error("Number of joinfiles != njobs : this is wrong, exiting.")
                 self.exit(1)
 
             if self.HPC_can_join(joinfiles, joiningfile, vb=True):
                 # join object files
-                print("We can join")
+                self.vb_info("We can join")
                 try:
                     # touch joiningfile
-                    if self.grid_options["HPC_force_join"] == 0:
-                        print("Making joiningfile at {}".format(joiningfile))
+                    if self.population_options["HPC_force_join"] == 0:
+                        self.vb_info("Making joiningfile at {}".format(joiningfile))
                         self.HPC_touch(joiningfile)
                     try:
-                        print("Calling HPC_join_from_files()")
+                        self.vb_info("Calling HPC_join_from_files()")
                         self.HPC_join_from_files(self, joinfiles)
                     except Exception as e:
-                        print("Join gave exception", e)
+                        self.vb_info("Join gave exception", e)
                         # disable analytics calculations : use the
                         # values we just loaded
-                    self.grid_options["do_analytics"] = False
+                    self.population_options["do_analytics"] = False
                     return
                 except Exception as e:
-                    print("pass {}", e)
+                    self.vb_info("pass {}", e)
                     pass
             else:
-                print("cannot join : other tasks are not yet finished\n")
-                print("Finished this job : exiting")
+                self.vb_info("cannot join : other tasks are not yet finished\n")
+                self.vb_info("Finished this job : exiting")
         self.exit(code=1)
 
     def HPC_path(self, path):
         """
         Function to file the filename of this HPC job's file at path.
         """
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             p = self.slurmpath(path)
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             p = self.condorpath(path)
         else:
             p = None
         return p
 
     def HPC_snapshot_filename(self):
         """
@@ -612,18 +614,18 @@
             file = None
         return file
 
     def HPC_dir(self):
         """
         Function to return an HPC job's directory.
         """
-        if self.grid_options["slurm"] > 0:
-            d = self.grid_options["slurm_dir"]
-        elif self.grid_options["condor"] > 0:
-            d = self.grid_options["condor_dir"]
+        if self.population_options["slurm"] > 0:
+            d = self.population_options["slurm_dir"]
+        elif self.population_options["condor"] > 0:
+            d = self.population_options["condor_dir"]
         else:
             d = None
         return d
 
     def HPC_touch(self, filename, string=None):
         """
         Function to touch the file at filename, put into it the job number
@@ -675,15 +677,14 @@
             # default types
             for x in ["running", "starting", "finishing", "finished", "killed"]:
                 d["status"][x] = 0
                 d["joblist"][x] = []
 
             for i in self.HPC_job_id_range():
                 s = self.HPC_get_status(job_id=_id, job_index=i)
-                # print("HPC get job",_id,':',i," status=",s)
                 if s is None:
                     s = "unknown"
                 if s not in d["status"]:
                     d["status"][s] = 1
                 else:
                     d["status"][s] += 1
                 if s not in d["joblist"]:
@@ -699,37 +700,37 @@
         """
 
         if not string:
             string = ""
 
         d = self.HPC_status()
 
-        print("############################################################")
-        print("HPC job status " + string)
-        print(json.dumps(d, indent=4))
-        print("############################################################")
+        self.vb_info("############################################################")
+        self.vb_info("HPC job status " + string)
+        self.vb_info(json.dumps(d, indent=4))
+        self.vb_info("############################################################")
 
     def HPC_queue_stats(self):  # pragma: no cover
         """
         Function that returns the queue stats for the HPC grid
         """
 
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             x = self.slurm_queue_stats()
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             x = self.condor_queue_stats()
         else:
             x = None
 
         return x
 
     def HPC_job_id_range(self):
         n = self.HPC_njobs()
-        if self.grid_options["slurm"] > 0:
+        if self.population_options["slurm"] > 0:
             return range(1, n + 1)
-        elif self.grid_options["condor"] > 0:
+        elif self.population_options["condor"] > 0:
             return range(0, n)
         else:
-            print(
+            self.vb_error(
                 "Called HPC_job_id_range when not running an HPC grid : you cannot do this."
             )
             raise
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/Moe_di_Stefano_2017.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/Moe_di_Stefano_2017.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,116 +13,251 @@
 import json
 import os
 
 import py_rinterpolate
 
 from binarycpython.utils import moe_di_stefano_2017_data
 from binarycpython.utils.dicts import normalize_dict, update_dicts
-from binarycpython.utils.functions import verbose_print
 from binarycpython.utils.population_extensions.distribution_functions import (
     LOG_LN_CONVERTER,
     Moecache,
 )
-from binarycpython.utils.population_extensions.grid_options_defaults import (
-    _MOE2017_VERBOSITY_LEVEL,
-)
 
 
 class Moe_di_Stefano_2017:
     """
     Extension to the population grid object that contains functionality to handle handle the Moe & distefano distributions
     """
 
     def __init__(self, **kwargs):
         """
         Init function for the Moe_di_Stefano_2017 class
         """
 
-        return
+        self.moe_distefano_options_defaults_dict = {
+            "JSON": {
+                "value": None,
+                "description": "Parameter that stores the interpolation data",
+            },
+            "resolutions": {
+                "value": {
+                    "M": [
+                        20,  # M1
+                        20,  # M2 (i.e. q)
+                        0,  # M3 currently unused
+                        0,  # M4 currently unused
+                    ],
+                    "logP": [
+                        20,  # P2 (binary period)
+                        0,  # P3 (triple period) currently unused
+                        0,  # P4 (quadruple period) currently unused
+                    ],
+                    "ecc": [
+                        10,  # e (binary eccentricity)
+                        0,  # e2 (triple eccentricity) currently unused
+                        0,  # e3 (quadruple eccentricity) currently unused
+                    ],
+                },
+                "description": "Dictionary that stores the resolutions for each of the variables that are used to sample the systems. The structure is as follows: resolutions = {'M': [M1 res, M2 res, ..], 'logP': [logP1 res, logP2 res, ...], 'ecc': [ecc1 res, ecc2 res, ...]}",
+            },
+            "samplerfuncs": {
+                "value": {
+                    "M": [None, None, None, None],
+                    "logP": [None, None, None],
+                    "ecc": [None, None, None],
+                },
+                "description": "sampler functions to each of the parameters. NEEDS UPDATING",
+            },
+            "IMF_distribution": {
+                "value": "kroupa2001",
+                "description": "IMF choice for the M&S sampling. Currently only supporting 'kroupa2001': Kroupa 2001 IMF and 'chabrier2003': Chabrier 2003 IMF.",
+            },
+            "ranges": {
+                "value": {
+                    # stellar masses (Msun)
+                    "M": [
+                        self.minimum_stellar_mass()
+                        * 1.05,  # 0.08 is a tad bit above the minimum mass. Don't sample at 0.07, otherwise the first row of q values will have a phasevol of 0. Anything higher is fine.
+                        80.0,  # (rather arbitrary) upper mass cutoff
+                    ],
+                    "q": [
+                        None,  # artificial qmin : set to None to use default
+                        None,  # artificial qmax : set to None to use default
+                    ],
+                    "logP": [0.0, 8.0],  # 0 = log10(1 day)  # 8 = log10(10^8 days)
+                    "ecc": [0.0, 0.99],
+                },
+                "description": "Ranges for the parameters that are sampled through the M&S distributions. Input is as follows: resolutions = {'M': [M1 lower bound, M2 upper bound], 'q': [q lower bound, q upper bound]}",
+            },
+            "Mmin": {
+                "value": self.minimum_stellar_mass(),
+                "description": "Minimum stellar mass that is regarded a star",
+            },
+            "multiplicity_model": {
+                "value": "Poisson",
+                "description": """
+multiplicity model (as a function of log10M1)
+
+You can use 'Poisson' which uses the system multiplicity
+given by Moe and maps this to single/binary/triple/quad
+fractions.
+
+Alternatively, 'data' takes the fractions directly
+from the data, but then triples and quadruples are
+combined (and there are NO quadruples).
+""",
+            },
+            "multiplicity_modulator": {
+                "value": [
+                    1,  # single
+                    1,  # binary
+                    0,  # triple
+                    0,  # quadruple
+                ],
+                "description": """
+[single, binary, triple, quadruple]
+
+e.g. [1,0,0,0] for single stars only
+     [0,1,0,0] for binary stars only
+
+defaults to [1,1,0,0] i.e. singles and binaries
+""",
+            },
+            "normalize_multiplicities": {
+                "value": "merge",
+                "description": """
+'norm': normalise so the whole population is 1.0
+        after implementing the appropriate fractions
+        S/(S+B+T+Q), B/(S+B+T+Q), T/(S+B+T+Q), Q/(S+B+T+Q)
+        given a mix of multiplicities, you can either (noting that
+        here (S,B,T,Q) = appropriate modulator * model(S,B,T,Q) )
+        note: if you only set one multiplicity_modulator
+        to 1, and all the others to 0, then normalising
+        will mean that you effectively have the same number
+        of stars as single, binary, triple or quad (whichever
+        is non-zero) i.e. the multiplicity fraction is ignored.
+        This is probably not useful except for
+        testing purposes or comparing to old grids.
+
+'raw'   : stick to what is predicted, i.e.
+          S/(S+B+T+Q), B/(S+B+T+Q), T/(S+B+T+Q), Q/(S+B+T+Q)
+          without normalisation
+          (in which case the total probability < 1.0 unless
+          all you use single, binary, triple and quadruple)
+
+'merge' : e.g. if you only have single and binary,
+          add the triples and quadruples to the binaries, so
+          binaries represent all multiple systems
+          ...
+          *** this is canonical binary population synthesis ***
+
+          It only takes the maximum multiplicity into account,
+          i.e. it doesn't multiply the resulting array by the multiplicity modulator again.
+          This prevents the resulting array to always be 1 if only 1 multiplicity modulator element is nonzero
+
+          Note: if multiplicity_modulator == [1,1,1,1]. this option does nothing (equivalent to 'raw').
+""",
+            },
+            "q_low_extrapolation_method": {
+                "value": "flat",
+                "description": """
+q extrapolation (below 0.15) method
+    none
+    flat
+    linear2
+    plaw2
+    nolowq
+""",
+            },
+            "q_high_extrapolation_method": {
+                "value": "flat",
+                "description": "Same as q_low_extrapolation_method",
+            },
+        }
 
     def set_moe_di_stefano_settings(self, options=None):
         """
         Function to set user input configurations for the Moe & di Stefano methods
 
         If nothing is passed then we just use the default options
         """
 
         if not options:
             options = {}
 
         # Take the option dictionary that was given and override.
-        options = update_dicts(self.grid_options["Moe2017_options"], options)
-        self.grid_options["Moe2017_options"] = copy.deepcopy(options)
+        options = update_dicts(self.population_options["Moe2017_options"], options)
+        self.population_options["Moe2017_options"] = copy.deepcopy(options)
 
         # Write options to a file
         os.makedirs(
-            os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
+            os.path.join(self.population_options["tmp_dir"], "moe_distefano"),
             exist_ok=True,
         )
         with open(
             os.path.join(
-                os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
+                os.path.join(self.population_options["tmp_dir"], "moe_distefano"),
                 "moeopts.dat",
             ),
             "w",
             encoding="utf-8",
         ) as f:
             f.write(
                 json.dumps(
-                    self.grid_options["Moe2017_options"], indent=4, ensure_ascii=False
+                    self.population_options["Moe2017_options"],
+                    indent=4,
+                    ensure_ascii=False,
                 )
             )
             f.close()
 
     def _load_moe_di_stefano_data(self):
         """
         Function to load the moe & di stefano data
         """
 
         # Only if the grid is loaded and Moecache contains information
-        if not self.grid_options["_loaded_Moe2017_data"]:  # and not Moecache:
+        if not self.population_options["_loaded_Moe2017_data"]:  # and not Moecache:
 
-            if self.grid_options["_Moe2017_JSON_data"]:
+            if self.population_options["_Moe2017_JSON_data"]:
                 # Use the existing (perhaps modified) JSON data
-                json_data = self.grid_options["_Moe2017_JSON_data"]
+                json_data = self.population_options["_Moe2017_JSON_data"]
 
             else:
                 # Load the JSON data from a file
                 json_data = self.get_moe_di_stefano_dataset(
-                    self.grid_options["Moe2017_options"],
-                    verbosity=self.grid_options["verbosity"],
+                    self.population_options["Moe2017_options"],
+                    verbosity=self.population_options["verbosity"],
                 )
 
             # entry of log10M1 is a list containing 1 dict.
             # We can take the dict out of the list
             if isinstance(json_data["log10M1"], list):
                 json_data["log10M1"] = json_data["log10M1"][0]
 
             # save this data in case we want to modify it later
-            self.grid_options["_Moe2017_JSON_data"] = json_data
+            self.population_options["_Moe2017_JSON_data"] = json_data
 
             # Get all the masses
             logmasses = sorted(json_data["log10M1"].keys())
             if not logmasses:
                 msg = "The table does not contain masses."
-                verbose_print(
+                self.vb_debug(
                     "\tMoe_di_Stefano_2017: {}".format(msg),
-                    self.grid_options["verbosity"],
-                    0,
                 )
                 raise ValueError(msg)
 
             # Write to file
             os.makedirs(
-                os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
+                os.path.join(self.population_options["tmp_dir"], "moe_distefano"),
                 exist_ok=True,
             )
             with open(
                 os.path.join(
-                    os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
+                    os.path.join(self.population_options["tmp_dir"], "moe_distefano"),
                     "moe.log",
                 ),
                 "w",
                 encoding="utf-8",
             ) as logfile:
                 logfile.write("log₁₀Masses(M☉) {}\n".format(logmasses))
 
@@ -137,47 +272,45 @@
                 if logperiods != current_logperiods:
                     msg = (
                         "Period values are not consistent throughout the dataset logperiods = "
                         + " ".join(str(x) for x in logperiods)
                         + "\nCurrent periods = "
                         + " ".join(str(x) for x in current_logperiods)
                     )
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe_di_Stefano_2017: {}".format(msg),
-                        self.grid_options["verbosity"],
-                        0,
                     )
                     raise ValueError(msg)
 
                 ############################################################
                 # log10period binwidth : of course this assumes a fixed
                 # binwidth, so we check for this too.
                 for i in range(len(current_logperiods) - 1):
                     if not dlog10P == (
                         float(current_logperiods[i + 1]) - float(current_logperiods[i])
                     ):
                         msg = "Period spacing is not consistent throughout the dataset"
-                        verbose_print(
+                        self.vb_debug(
                             "\tMoe_di_Stefano_2017: {}".format(msg),
-                            self.grid_options["verbosity"],
-                            0,
                         )
                         raise ValueError(msg)
 
             # save the logperiods list in the cache:
             # this is used in the renormalization integration
             Moecache["logperiods"] = logperiods
 
             # Write to file
             os.makedirs(
-                os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
+                os.path.join(self.population_options["tmp_dir"], "moe_distefano"),
                 exist_ok=True,
             )
             with open(
-                os.path.join(self.grid_options["tmp_dir"], "moe_distefano", "moe.log"),
+                os.path.join(
+                    self.population_options["tmp_dir"], "moe_distefano", "moe.log"
+                ),
                 "a",
                 encoding="utf-8",
             ) as logfile:
                 logfile.write("log₁₀Periods(days) {}\n".format(logperiods))
 
             # Fill the global dict
             for logmass in logmasses:
@@ -327,495 +460,604 @@
                         float(logmass),
                         float(logperiods[-1]) + 0.5 * dlog10P + epslog10P,
                         0.0,
                         0.0,
                     ]
                 )
 
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017: Length period_distributions table: {}".format(
                     len(Moecache["period_distributions"])
                 ),
-                self.grid_options["verbosity"],
-                _MOE2017_VERBOSITY_LEVEL,
             )
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017: Length multiplicity table: {}".format(
                     len(Moecache["multiplicity_table"])
                 ),
-                self.grid_options["verbosity"],
-                _MOE2017_VERBOSITY_LEVEL,
             )
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017: Length q table: {}".format(
                     len(Moecache["q_distributions"])
                 ),
-                self.grid_options["verbosity"],
-                _MOE2017_VERBOSITY_LEVEL,
             )
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017: Length ecc table: {}".format(
                     len(Moecache["ecc_distributions"])
                 ),
-                self.grid_options["verbosity"],
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
             # Write to log file
             os.makedirs(
-                os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
+                os.path.join(self.population_options["tmp_dir"], "moe_distefano"),
                 exist_ok=True,
             )
             with open(
                 os.path.join(
-                    os.path.join(self.grid_options["tmp_dir"], "moe_distefano"),
+                    os.path.join(self.population_options["tmp_dir"], "moe_distefano"),
                     "moecache.json",
                 ),
                 "w",
                 encoding="utf-8",
             ) as cache_filehandle:
                 cache_filehandle.write(
                     json.dumps(Moecache, indent=4, ensure_ascii=False)
                 )
 
             # Signal that the data has been loaded
-            self.grid_options["_loaded_Moe2017_data"] = True
+            self.population_options["_loaded_Moe2017_data"] = True
 
     def _set_moe_di_stefano_distributions(self):
         """
         Function to set the Moe & di Stefano distribution
         """
 
-        ############################################################
-        # first, the multiplicity, this is 1,2,3,4, ...
-        # for singles, binaries, triples, quadruples, ...
+        ##############
+        # Handle multiplicity loop if we are doing grid sampling
+        if not self.population_options["evolution_type"] == "monte_carlo":
+
+            ############################################################
+            # first, the multiplicity, this is 1,2,3,4, ...
+            # for singles, binaries, triples, quadruples, ...
 
-        max_multiplicity = self.get_max_multiplicity(
-            self.grid_options["Moe2017_options"]["multiplicity_modulator"]
-        )
-        verbose_print(
-            "\tMoe_di_Stefano_2017: Max multiplicity = {}".format(max_multiplicity),
-            self.grid_options["verbosity"],
-            _MOE2017_VERBOSITY_LEVEL,
-        )
-        ######
-        # Setting up the grid variables
+            max_multiplicity = self.get_max_multiplicity(
+                self.population_options["Moe2017_options"]["multiplicity_modulator"]
+            )
+            self.vb_debug(
+                "\tMoe_di_Stefano_2017: Max multiplicity = {}".format(max_multiplicity),
+            )
 
-        # Multiplicity
-        self.add_sampling_variable(
-            name="multiplicity",
-            parameter_name="multiplicity",
-            longname="multiplicity",
-            valuerange=[1, max_multiplicity],
-            samplerfunc="self.const_int(1, {n}, {n})".format(n=max_multiplicity),
-            precode='self.grid_options["multiplicity"] = multiplicity; self.bse_options["multiplicity"] = multiplicity; options={}'.format(
-                self.grid_options["Moe2017_options"]
-            ),
-            condition="({}[int(multiplicity)-1] > 0)".format(
-                str(self.grid_options["Moe2017_options"]["multiplicity_modulator"])
-            ),
-            gridtype="discrete",
-            probdist=1,
-        )
+            # Multiplicity
+            self.add_sampling_variable(
+                name="multiplicity",
+                parameter_name="multiplicity",
+                longname="multiplicity",
+                valuerange=[1, max_multiplicity],
+                samplerfunc="self.const_int(1, {n}, {n})".format(n=max_multiplicity),
+                precode='self.population_options["multiplicity"] = multiplicity; self.bse_options["multiplicity"] = multiplicity; options={}'.format(
+                    self.population_options["Moe2017_options"]
+                ),
+                condition="({}[int(multiplicity)-1] > 0)".format(
+                    str(
+                        self.population_options["Moe2017_options"][
+                            "multiplicity_modulator"
+                        ]
+                    )
+                ),
+                gridtype="discrete",
+                probdist=1,
+            )
+
+        ####################################
+        # Set up the sampling variables
 
-        ############################################################
-        # always require M1, for all systems
-        #
-        # log-spaced m1 with given resolution
+        ################
+        # Primary mass: M_1
         self.add_sampling_variable(
             name="lnM_1",
             parameter_name="M_1",
             longname="Primary mass",
-            samplerfunc=self.grid_options["Moe2017_options"]["samplerfuncs"]["M"][0]
+            samplerfunc=self.population_options["Moe2017_options"]["samplerfuncs"]["M"][
+                0
+            ]
             or "self.const_linear(np.log({}), np.log({}), {})".format(
-                self.grid_options["Moe2017_options"]["ranges"]["M"][0],
-                self.grid_options["Moe2017_options"]["ranges"]["M"][1],
-                self.grid_options["Moe2017_options"]["resolutions"]["M"][0],
+                self.population_options["Moe2017_options"]["ranges"]["M"][0],
+                self.population_options["Moe2017_options"]["ranges"]["M"][1],
+                self.population_options["Moe2017_options"]["resolutions"]["M"][0],
             ),
             valuerange=[
                 "np.log({})".format(
-                    self.grid_options["Moe2017_options"]["ranges"]["M"][0]
+                    self.population_options["Moe2017_options"]["ranges"]["M"][0]
                 ),
                 "np.log({})".format(
-                    self.grid_options["Moe2017_options"]["ranges"]["M"][1]
+                    self.population_options["Moe2017_options"]["ranges"]["M"][1]
                 ),
             ],
             gridtype="centred",
             dphasevol="dlnM_1",
             precode='M_1 = np.exp(lnM_1); options["M_1"]=M_1',
-            probdist="self.Moe_di_Stefano_2017_pdf({{{}, {}, {}}}, verbosity=self.grid_options['verbosity'])['total_probdens'] if multiplicity == 1 else 1".format(
-                str(dict(self.grid_options["Moe2017_options"]))[1:-1],
+            probdist="self.Moe_di_Stefano_2017_pdf({{{}, {}, {}}}, verbosity=self.population_options['verbosity'])['total_probdens'] if multiplicity == 1 else 1".format(
+                str(dict(self.population_options["Moe2017_options"]))[1:-1],
                 "'multiplicity': multiplicity",
                 "'M_1': M_1",
             ),
+            ###########
+            # Monte-Carlo sampling related
+            # To indicate that this is a branchpoint and we want to execute this when the multiplicity==1
+            branchpoint=1,
+            branchcode="multiplicity == 1",
         )
 
-        # Go to higher multiplicities
+        ################
+        # Handle binaries
         if max_multiplicity >= 2:
-            # binaries: period
+
+            ################
+            # Orbital period inner binary: orbital_period
             self.add_sampling_variable(
                 name="log10per",
                 parameter_name="orbital_period",
                 longname="log10(Orbital_Period)",
                 probdist=1.0,
-                condition='(self.grid_options["multiplicity"] >= 2)',
-                branchpoint=1
-                if max_multiplicity > 1
-                else 0,  # Signal here to put a branchpoint if we have a max multiplicity higher than 1.
+                condition='(self.population_options["multiplicity"] >= 2)',
                 gridtype="centred",
                 dphasevol="({} * dlog10per)".format(LOG_LN_CONVERTER),
                 valuerange=[
-                    self.grid_options["Moe2017_options"]["ranges"]["logP"][0],
-                    self.grid_options["Moe2017_options"]["ranges"]["logP"][1],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][0],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][1],
                 ],
-                samplerfunc=self.grid_options["Moe2017_options"]["samplerfuncs"][
+                samplerfunc=self.population_options["Moe2017_options"]["samplerfuncs"][
                     "logP"
                 ][0]
                 or "self.const_linear({}, {}, {})".format(
-                    self.grid_options["Moe2017_options"]["ranges"]["logP"][0],
-                    self.grid_options["Moe2017_options"]["ranges"]["logP"][1],
-                    self.grid_options["Moe2017_options"]["resolutions"]["logP"][0],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][0],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][1],
+                    self.population_options["Moe2017_options"]["resolutions"]["logP"][
+                        0
+                    ],
                 ),
                 precode="""orbital_period = 10.0**log10per
 qmin={}/M_1
 qmax=maximum_mass_ratio_for_RLOF(M_1, orbital_period)
 """.format(
-                    self.grid_options["Moe2017_options"]["Mmin"]
+                    self.population_options["Moe2017_options"]["Mmin"]
                 ),
             )  # TODO: change the maximum_mass_ratio_for_RLOF
 
-            # binaries: mass ratio
+            ################
+            # Mass ratio inner binary: q / M_2
             self.add_sampling_variable(
                 name="q",
                 parameter_name="M_2",
                 longname="Mass ratio",
                 valuerange=[
-                    self.grid_options["Moe2017_options"]["ranges"]["q"][0]
-                    if self.grid_options["Moe2017_options"]
+                    self.population_options["Moe2017_options"]["ranges"]["q"][0]
+                    if self.population_options["Moe2017_options"]
                     .get("ranges", {})
                     .get("q", None)
                     else "options['Mmin']/M_1",
-                    self.grid_options["Moe2017_options"]["ranges"]["q"][1]
-                    if self.grid_options["Moe2017_options"]
+                    self.population_options["Moe2017_options"]["ranges"]["q"][1]
+                    if self.population_options["Moe2017_options"]
                     .get("ranges", {})
                     .get("q", None)
                     else "qmax",
                 ],
                 probdist=1,
                 gridtype="centred",
                 dphasevol="dq",
                 precode="""
 M_2 = q * M_1
 sep = calc_sep_from_period(M_1, M_2, orbital_period)
     """,
-                samplerfunc=self.grid_options["Moe2017_options"]["samplerfuncs"]["M"][1]
+                samplerfunc=self.population_options["Moe2017_options"]["samplerfuncs"][
+                    "M"
+                ][1]
                 or "self.const_linear({}, {}, {})".format(
-                    self.grid_options["Moe2017_options"]["ranges"]["q"][0]
-                    if self.grid_options["Moe2017_options"]
+                    self.population_options["Moe2017_options"]["ranges"]["q"][0]
+                    if self.population_options["Moe2017_options"]
                     .get("ranges", {})
                     .get("q", [None, None])[0]
-                    else "{}/M_1".format(self.grid_options["Moe2017_options"]["Mmin"]),
-                    self.grid_options["Moe2017_options"]["ranges"]["q"][1]
-                    if self.grid_options["Moe2017_options"]
+                    else "{}/M_1".format(
+                        self.population_options["Moe2017_options"]["Mmin"]
+                    ),
+                    self.population_options["Moe2017_options"]["ranges"]["q"][1]
+                    if self.population_options["Moe2017_options"]
                     .get("ranges", {})
                     .get("q", [None, None])[1]
                     else "qmax",
-                    self.grid_options["Moe2017_options"]["resolutions"]["M"][1],
+                    self.population_options["Moe2017_options"]["resolutions"]["M"][1],
                 ),
+                ###########
+                # Monte-Carlo sampling related
+                # To indicate that this is a branchpoint and we want to execute this when the multiplicity==2
+                branchpoint=1
+                if (
+                    self.population_options["evolution_type"] == "evolution_type"
+                    and self.population_options["Moe2017_options"]["resolutions"][
+                        "ecc"
+                    ][0]
+                    == 0
+                )
+                else 0,
+                branchcode="multiplicity == 2"
+                if (
+                    self.population_options["evolution_type"] == "evolution_type"
+                    and self.population_options["Moe2017_options"]["resolutions"][
+                        "ecc"
+                    ][0]
+                    == 0
+                )
+                else None,
             )
 
-            # (optional) binaries: eccentricity
-            if self.grid_options["Moe2017_options"]["resolutions"]["ecc"][0] > 0:
+            ################
+            # (optional) eccentricity inner binary: ecc
+            if self.population_options["Moe2017_options"]["resolutions"]["ecc"][0] > 0:
                 self.add_sampling_variable(
                     name="ecc",
                     parameter_name="eccentricity",
                     longname="Eccentricity",
                     probdist=1,
                     gridtype="centred",
                     dphasevol="decc",
                     precode="eccentricity=ecc",
                     valuerange=[
-                        self.grid_options["Moe2017_options"]["ranges"]["ecc"][
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][
                             0
                         ],  # Just fail if not defined.
-                        self.grid_options["Moe2017_options"]["ranges"]["ecc"][1],
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][1],
                     ],
-                    samplerfunc=self.grid_options["Moe2017_options"]["samplerfuncs"][
-                        "ecc"
-                    ][0]
+                    samplerfunc=self.population_options["Moe2017_options"][
+                        "samplerfuncs"
+                    ]["ecc"][0]
                     or "self.const_linear({}, {}, {})".format(
-                        self.grid_options["Moe2017_options"]["ranges"]["ecc"][
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][
                             0
                         ],  # Just fail if not defined.
-                        self.grid_options["Moe2017_options"]["ranges"]["ecc"][1],
-                        self.grid_options["Moe2017_options"]["resolutions"]["ecc"][0],
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][1],
+                        self.population_options["Moe2017_options"]["resolutions"][
+                            "ecc"
+                        ][0],
                     ),
+                    ###########
+                    # Monte-Carlo sampling related
+                    # To indicate that this is a branchpoint and we want to execute this when the multiplicity==2
+                    branchpoint=1
+                    if (self.population_options["evolution_type"] == "evolution_type")
+                    else 0,
+                    branchcode="multiplicity == 2"
+                    if (self.population_options["evolution_type"] == "evolution_type")
+                    else None,
                 )
 
-            # Now for triples and quadruples
-            if max_multiplicity >= 3:
-                # Triple: period
-                self.add_sampling_variable(
-                    name="log10per2",
-                    parameter_name="orbital_period_triple",
-                    longname="log10(Orbital_Period2)",
-                    probdist=1.0,
-                    condition='(self.grid_options["multiplicity"] >= 3)',
-                    branchpoint=2
-                    if max_multiplicity > 2
-                    else 0,  # Signal here to put a branchpoint if we have a max multiplicity higher than 1.
-                    gridtype="centred",
-                    dphasevol="({} * dlog10per2)".format(LOG_LN_CONVERTER),
-                    valuerange=[
-                        self.grid_options["Moe2017_options"]["ranges"]["logP"][0],
-                        self.grid_options["Moe2017_options"]["ranges"]["logP"][1],
+        ################
+        # Handle triple systems
+        if max_multiplicity >= 3:
+            ################
+            # Orbital period hierarchical triple system: orbital_period_triple
+            self.add_sampling_variable(
+                name="log10per2",
+                parameter_name="orbital_period_triple",
+                longname="log10(Orbital_Period2)",
+                probdist=1.0,
+                condition='(self.population_options["multiplicity"] >= 3)',
+                gridtype="centred",
+                dphasevol="({} * dlog10per2)".format(LOG_LN_CONVERTER),
+                valuerange=[
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][0],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][1],
+                ],
+                samplerfunc=self.population_options["Moe2017_options"]["samplerfuncs"][
+                    "logP"
+                ][1]
+                or "self.const_linear({}, {}, {})".format(
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][0],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][1],
+                    self.population_options["Moe2017_options"]["resolutions"]["logP"][
+                        1
                     ],
-                    samplerfunc=self.grid_options["Moe2017_options"]["samplerfuncs"][
-                        "logP"
-                    ][1]
-                    or "self.const_linear({}, {}, {})".format(
-                        self.grid_options["Moe2017_options"]["ranges"]["logP"][0],
-                        self.grid_options["Moe2017_options"]["ranges"]["logP"][1],
-                        self.grid_options["Moe2017_options"]["resolutions"]["logP"][1],
-                    ),
-                    precode="""orbital_period_triple = 10.0**log10per2
+                ),
+                precode="""orbital_period_triple = 10.0**log10per2
 q2min={}/(M_1+M_2)
 q2max=maximum_mass_ratio_for_RLOF(M_1+M_2, orbital_period_triple)
-    """.format(
-                        self.grid_options["Moe2017_options"]["Mmin"]
-                    ),
-                )
+""".format(
+                    self.population_options["Moe2017_options"]["Mmin"]
+                ),
+            )
 
-                # Triples: mass ratio
-                # Note, the mass ratio is M_outer/M_inner
-                self.add_sampling_variable(
-                    name="q2",
-                    parameter_name="M_3",
-                    longname="Mass ratio outer/inner",
-                    valuerange=[
-                        self.grid_options["Moe2017_options"]["ranges"]["q"][0]
-                        if self.grid_options["Moe2017_options"]
-                        .get("ranges", {})
-                        .get("q", None)
-                        else "options['Mmin']/(M_1+M_2)",
-                        self.grid_options["Moe2017_options"]["ranges"]["q"][1]
-                        if self.grid_options["Moe2017_options"]
-                        .get("ranges", {})
-                        .get("q", None)
-                        else "q2max",
-                    ],
-                    probdist=1,
-                    gridtype="centred",
-                    dphasevol="dq2",
-                    precode="""
+            ################
+            # mass ratio hierarchical triple system: q2 & M_3
+            # NOTE: the mass ratio is M_outer/M_inner
+            self.add_sampling_variable(
+                name="q2",
+                parameter_name="M_3",
+                longname="Mass ratio outer/inner",
+                valuerange=[
+                    self.population_options["Moe2017_options"]["ranges"]["q"][0]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "options['Mmin']/(M_1+M_2)",
+                    self.population_options["Moe2017_options"]["ranges"]["q"][1]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "q2max",
+                ],
+                probdist=1,
+                gridtype="centred",
+                dphasevol="dq2",
+                precode="""
 M_3 = q2 * (M_1 + M_2)
 sep2 = calc_sep_from_period((M_1+M_2), M_3, orbital_period_triple)
 eccentricity2=0
 """,
-                    samplerfunc=self.grid_options["Moe2017_options"]["samplerfuncs"][
-                        "M"
-                    ][2]
+                samplerfunc=self.population_options["Moe2017_options"]["samplerfuncs"][
+                    "M"
+                ][2]
+                or "self.const_linear({}, {}, {})".format(
+                    self.population_options["Moe2017_options"]["ranges"]["q"][0]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "options['Mmin']/(M_1+M_2)",
+                    self.population_options["Moe2017_options"]["ranges"]["q"][1]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "q2max",
+                    self.population_options["Moe2017_options"]["resolutions"]["M"][2],
+                ),
+                ###########
+                # Monte-Carlo sampling related
+                # To indicate that this is a branchpoint and we want to execute this when the multiplicity==3
+                branchpoint=1
+                if (
+                    self.population_options["evolution_type"] == "evolution_type"
+                    and self.population_options["Moe2017_options"]["resolutions"][
+                        "ecc"
+                    ][1]
+                    == 0
+                )
+                else 0,
+                branchcode="multiplicity == 3"
+                if (
+                    self.population_options["evolution_type"] == "evolution_type"
+                    and self.population_options["Moe2017_options"]["resolutions"][
+                        "ecc"
+                    ][1]
+                    == 0
+                )
+                else None,
+            )
+
+            ################
+            # (optional) eccentricity hierarchical triple system: eccentricity_triple
+            if self.population_options["Moe2017_options"]["resolutions"]["ecc"][1] > 0:
+                self.add_sampling_variable(
+                    name="ecc2",
+                    parameter_name="eccentricity2",
+                    longname="Eccentricity of the triple",
+                    probdist=1,
+                    gridtype="centred",
+                    dphasevol="decc2",
+                    precode="eccentricity_triple=ecc2",
+                    valuerange=[
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][
+                            0
+                        ],  # Just fail if not defined.
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][1],
+                    ],
+                    samplerfunc=self.population_options["Moe2017_options"][
+                        "samplerfuncs"
+                    ]["ecc"][1]
                     or "self.const_linear({}, {}, {})".format(
-                        self.grid_options["Moe2017_options"]["ranges"]["q"][0]
-                        if self.grid_options["Moe2017_options"]
-                        .get("ranges", {})
-                        .get("q", None)
-                        else "options['Mmin']/(M_1+M_2)",
-                        self.grid_options["Moe2017_options"]["ranges"]["q"][1]
-                        if self.grid_options["Moe2017_options"]
-                        .get("ranges", {})
-                        .get("q", None)
-                        else "q2max",
-                        self.grid_options["Moe2017_options"]["resolutions"]["M"][2],
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][
+                            0
+                        ],  # Just fail if not defined.
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][1],
+                        self.population_options["Moe2017_options"]["resolutions"][
+                            "ecc"
+                        ][1],
                     ),
+                    ###########
+                    # Monte-Carlo sampling related
+                    # To indicate that this is a branchpoint and we want to execute this when the multiplicity==3
+                    branchpoint=1
+                    if (self.population_options["evolution_type"] == "evolution_type")
+                    else 0,
+                    branchcode="multiplicity == 3"
+                    if (self.population_options["evolution_type"] == "evolution_type")
+                    else None,
                 )
 
-                # (optional) triples: eccentricity
-                if self.grid_options["Moe2017_options"]["resolutions"]["ecc"][1] > 0:
-                    self.add_sampling_variable(
-                        name="ecc2",
-                        parameter_name="eccentricity2",
-                        longname="Eccentricity of the triple",
-                        probdist=1,
-                        gridtype="centred",
-                        dphasevol="decc2",
-                        precode="eccentricity2=ecc2",
-                        valuerange=[
-                            self.grid_options["Moe2017_options"]["ranges"]["ecc"][
-                                0
-                            ],  # Just fail if not defined.
-                            self.grid_options["Moe2017_options"]["ranges"]["ecc"][1],
-                        ],
-                        samplerfunc=self.grid_options["Moe2017_options"][
-                            "samplerfuncs"
-                        ]["ecc"][1]
-                        or "self.const_linear({}, {}, {})".format(
-                            self.grid_options["Moe2017_options"]["ranges"]["ecc"][
-                                0
-                            ],  # Just fail if not defined.
-                            self.grid_options["Moe2017_options"]["ranges"]["ecc"][1],
-                            self.grid_options["Moe2017_options"]["resolutions"]["ecc"][
-                                1
-                            ],
-                        ),
-                    )
+        ################
+        # Handle quadruple systems
+        if max_multiplicity == 4:
 
-                if max_multiplicity == 4:
-                    # Quadruple: period
-                    self.add_sampling_variable(
-                        name="log10per3",
-                        parameter_name="orbital_period_quadruple",
-                        longname="log10(Orbital_Period3)",
-                        probdist=1.0,
-                        condition='(self.grid_options["multiplicity"] >= 4)',
-                        branchpoint=3
-                        if max_multiplicity > 3
-                        else 0,  # Signal here to put a branchpoint if we have a max multiplicity higher than 1.
-                        gridtype="centred",
-                        dphasevol="({} * dlog10per3)".format(LOG_LN_CONVERTER),
-                        valuerange=[
-                            self.grid_options["Moe2017_options"]["ranges"]["logP"][0],
-                            self.grid_options["Moe2017_options"]["ranges"]["logP"][1],
-                        ],
-                        samplerfunc=self.grid_options["Moe2017_options"][
-                            "samplerfuncs"
-                        ]["logP"][2]
-                        or "self.const_linear({}, {}, {})".format(
-                            self.grid_options["Moe2017_options"]["ranges"]["logP"][0],
-                            self.grid_options["Moe2017_options"]["ranges"]["logP"][1],
-                            self.grid_options["Moe2017_options"]["resolutions"]["logP"][
-                                2
-                            ],
-                        ),
-                        precode="""orbital_period_quadruple = 10.0**log10per3
+            ################
+            # Orbital period hierarchical quadruple system: orbital_period_quadruple
+            self.add_sampling_variable(
+                name="log10per3",
+                parameter_name="orbital_period_quadruple",
+                longname="log10(Orbital_Period3)",
+                probdist=1.0,
+                condition='(self.population_options["multiplicity"] >= 4)',
+                branchpoint=3
+                if max_multiplicity > 3
+                else 0,  # Signal here to put a branchpoint if we have a max multiplicity higher than 1.
+                gridtype="centred",
+                dphasevol="({} * dlog10per3)".format(LOG_LN_CONVERTER),
+                valuerange=[
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][0],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][1],
+                ],
+                samplerfunc=self.population_options["Moe2017_options"]["samplerfuncs"][
+                    "logP"
+                ][2]
+                or "self.const_linear({}, {}, {})".format(
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][0],
+                    self.population_options["Moe2017_options"]["ranges"]["logP"][1],
+                    self.population_options["Moe2017_options"]["resolutions"]["logP"][
+                        2
+                    ],
+                ),
+                precode="""orbital_period_quadruple = 10.0**log10per3
 q3min={}/(M_3)
 q3max=maximum_mass_ratio_for_RLOF(M_3, orbital_period_quadruple)
-    """.format(
-                            self.grid_options["Moe2017_options"]["Mmin"]
-                        ),
-                    )
+""".format(
+                    self.population_options["Moe2017_options"]["Mmin"]
+                ),
+            )
 
-                    # Quadruple: mass ratio : M_outer / M_inner
-                    self.add_sampling_variable(
-                        name="q3",
-                        parameter_name="M_4",
-                        longname="Mass ratio outer low/outer high",
-                        valuerange=[
-                            self.grid_options["Moe2017_options"]["ranges"]["q"][0]
-                            if self.grid_options["Moe2017_options"]
-                            .get("ranges", {})
-                            .get("q", None)
-                            else "options['Mmin']/(M_3)",
-                            self.grid_options["Moe2017_options"]["ranges"]["q"][1]
-                            if self.grid_options["Moe2017_options"]
-                            .get("ranges", {})
-                            .get("q", None)
-                            else "q3max",
-                        ],
-                        probdist=1,
-                        gridtype="centred",
-                        dphasevol="dq3",
-                        precode="""
+            ################
+            # mass ratio hierarchical triple system: q3 & M_4
+            # NOTE: the mass ratio is M_outer/M_inner
+            self.add_sampling_variable(
+                name="q3",
+                parameter_name="M_4",
+                longname="Mass ratio outer low/outer high",
+                valuerange=[
+                    self.population_options["Moe2017_options"]["ranges"]["q"][0]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "options['Mmin']/(M_3)",
+                    self.population_options["Moe2017_options"]["ranges"]["q"][1]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "q3max",
+                ],
+                probdist=1,
+                gridtype="centred",
+                dphasevol="dq3",
+                precode="""
 M_4 = q3 * M_3
 sep3 = calc_sep_from_period((M_3), M_4, orbital_period_quadruple)
 eccentricity3=0
 """,
-                        samplerfunc=self.grid_options["Moe2017_options"][
-                            "samplerfuncs"
-                        ]["M"][3]
-                        or "self.const_linear({}, {}, {})".format(
-                            self.grid_options["Moe2017_options"]["ranges"]["q"][0]
-                            if self.grid_options["Moe2017_options"]
-                            .get("ranges", {})
-                            .get("q", None)
-                            else "options['Mmin']/(M_3)",
-                            self.grid_options["Moe2017_options"]["ranges"]["q"][1]
-                            if self.grid_options["Moe2017_options"]
-                            .get("ranges", {})
-                            .get("q", None)
-                            else "q3max",
-                            self.grid_options["Moe2017_options"]["resolutions"]["M"][2],
-                        ),
-                    )
+                samplerfunc=self.population_options["Moe2017_options"]["samplerfuncs"][
+                    "M"
+                ][3]
+                or "self.const_linear({}, {}, {})".format(
+                    self.population_options["Moe2017_options"]["ranges"]["q"][0]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "options['Mmin']/(M_3)",
+                    self.population_options["Moe2017_options"]["ranges"]["q"][1]
+                    if self.population_options["Moe2017_options"]
+                    .get("ranges", {})
+                    .get("q", None)
+                    else "q3max",
+                    self.population_options["Moe2017_options"]["resolutions"]["M"][2],
+                ),
+                ###########
+                # Monte-Carlo sampling related
+                # To indicate that this is a branchpoint and we want to execute this when the multiplicity==4
+                branchpoint=1
+                if (
+                    self.population_options["evolution_type"] == "evolution_type"
+                    and self.population_options["Moe2017_options"]["resolutions"][
+                        "ecc"
+                    ][2]
+                    == 0
+                )
+                else 0,
+                branchcode="multiplicity == 4"
+                if (
+                    self.population_options["evolution_type"] == "evolution_type"
+                    and self.population_options["Moe2017_options"]["resolutions"][
+                        "ecc"
+                    ][2]
+                    == 0
+                )
+                else None,
+            )
 
-                    # (optional) triples: eccentricity
-                    if (
-                        self.grid_options["Moe2017_options"]["resolutions"]["ecc"][2]
-                        > 0
-                    ):
-                        self.add_sampling_variable(
-                            name="ecc3",
-                            parameter_name="eccentricity3",
-                            longname="Eccentricity of the triple+quadruple/outer binary",
-                            probdist=1,
-                            gridtype="centred",
-                            dphasevol="decc3",
-                            precode="eccentricity3=ecc3",
-                            valuerange=[
-                                self.grid_options["Moe2017_options"]["ranges"]["ecc"][
-                                    0
-                                ],  # Just fail if not defined.
-                                self.grid_options["Moe2017_options"]["ranges"]["ecc"][
-                                    1
-                                ],
-                            ],
-                            samplerfunc=self.grid_options["Moe2017_options"][
-                                "samplerfuncs"
-                            ]["ecc"][2]
-                            or "self.const_linear({}, {}, {})".format(
-                                self.grid_options["Moe2017_options"]["ranges"]["ecc"][
-                                    0
-                                ],  # Just fail if not defined.
-                                self.grid_options["Moe2017_options"]["ranges"]["ecc"][
-                                    1
-                                ],
-                                self.grid_options["Moe2017_options"]["resolutions"][
-                                    "ecc"
-                                ][2],
-                            ),
-                        )
+            ################
+            # (optional) eccentricity hierarchical quadruple system: eccentricity_quadruple
+            if self.population_options["Moe2017_options"]["resolutions"]["ecc"][2] > 0:
+                self.add_sampling_variable(
+                    name="ecc3",
+                    parameter_name="eccentricity3",
+                    longname="Eccentricity of the triple+quadruple/outer binary",
+                    probdist=1,
+                    gridtype="centred",
+                    dphasevol="decc3",
+                    precode="eccentricity3=ecc3",
+                    valuerange=[
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][
+                            0
+                        ],  # Just fail if not defined.
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][1],
+                    ],
+                    samplerfunc=self.population_options["Moe2017_options"][
+                        "samplerfuncs"
+                    ]["ecc"][2]
+                    or "self.const_linear({}, {}, {})".format(
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][
+                            0
+                        ],  # Just fail if not defined.
+                        self.population_options["Moe2017_options"]["ranges"]["ecc"][1],
+                        self.population_options["Moe2017_options"]["resolutions"][
+                            "ecc"
+                        ][2],
+                    ),
+                    ###########
+                    # Monte-Carlo sampling related
+                    # To indicate that this is a branchpoint and we want to execute this when the multiplicity==4
+                    branchpoint=1
+                    if (self.population_options["evolution_type"] == "evolution_type")
+                    else 0,
+                    branchcode="multiplicity == 4"
+                    if (self.population_options["evolution_type"] == "evolution_type")
+                    else None,
+                )
+
+        ###################
+        # Wrap up
 
         # Now we are at the last part.
         # Here we should combine all the information that we calculate and update the options
         # dictionary. This will then be passed to the Moe_di_Stefano_2017_pdf to calculate
         # the real probability. The trick we use is to strip the options_dict as a string
         # and add some keys to it:
 
+        # TODO: we need to add this to each 'final' sampling variable at each metallicity. The stochastic nature of monte-carlo sampling makes that we have changing multipliticies
         updated_options = "{{{}, {}, {}, {}, {}, {}, {}, {}, {}, {}, {}, {}}}".format(
-            str(dict(self.grid_options["Moe2017_options"]))[1:-1],
+            str(dict(self.population_options["Moe2017_options"]))[1:-1],
             '"multiplicity": multiplicity',
             '"M_1": M_1',
             '"M_2": M_2',
             '"M_3": M_3',
             '"M_4": M_4',
             '"P": orbital_period',
             '"P2": orbital_period_triple',
             '"P3": orbital_period_quadruple',
             '"ecc": eccentricity',
-            '"ecc2": eccentricity2',
-            '"ecc3": eccentricity3',
+            '"ecc2": eccentricity_triple',
+            '"ecc3": eccentricity_quadruple',
         )
 
-        probdist_addition = "self.Moe_di_Stefano_2017_pdf({}, verbosity=self.grid_options['verbosity'])['total_probdens']".format(
+        probdist_addition = "self.Moe_di_Stefano_2017_pdf({}, verbosity=self.population_options['verbosity'])['total_probdens']".format(
             updated_options
         )
 
         # and finally the probability calculator
-        self.grid_options["_sampling_variables"][self._last_sampling_variable()][
+        self.population_options["_sampling_variables"][self._last_sampling_variable()][
             "probdist"
         ] = probdist_addition
 
-        verbose_print(
+        self.vb_debug(
             "\tMoe_di_Stefano_2017: Added final call to the pdf function",
-            self.grid_options["verbosity"],
-            _MOE2017_VERBOSITY_LEVEL,
         )
 
         # Signal that the MOE2017 grid has been set
-        self.grid_options["_set_Moe2017_grid"] = True
+        self.population_options["_set_Moe2017_grid"] = True
 
     ################################################################################################
     def Moe_di_Stefano_2017(self, options=None):
         """
         Function to handle setting the user input settings,
         set up the data and load that into interpolators and
         then set the distribution functions
@@ -837,15 +1079,15 @@
         options = update_dicts(default_options, options)
 
         # clean cache?
         if options["clean all"] or options["clean cache"]:
             Moecache.clear()
 
         if options["clean all"] or options["clean load flag"]:
-            self.grid_options["_loaded_Moe2017_data"] = False
+            self.population_options["_loaded_Moe2017_data"] = False
 
         # Set the user input
         if options["apply settings"]:
             self.set_moe_di_stefano_settings(options=options)
 
         # Load the data
         if options["load data"]:
@@ -875,125 +1117,127 @@
 
     def _calculate_multiplicity_fraction(self, system_dict):
         """
         Function to calculate multiplicity fraction
 
         Makes use of the self.bse_options['multiplicity'] value. If its not set, it will raise an error
 
-        grid_options['multiplicity_fraction_function'] will be checked for the choice
+        population_options['multiplicity_fraction_function'] will be checked for the choice
 
         TODO: add option to put a manual binary fraction in here (solve via negative numbers being the functions)
         """
 
         # Just return 1 if no option has been chosen
-        if self.grid_options["multiplicity_fraction_function"] in [0, "None"]:
-            verbose_print(
+        if self.population_options["multiplicity_fraction_function"] in [0, "None"]:
+            self.vb_debug(
                 "_calculate_multiplicity_fraction: Chosen not to use any multiplicity fraction.",
-                self.grid_options["verbosity"],
-                3,
             )
 
             return 1
 
         # Raise an error if the multiplicity is not set
         if not system_dict.get("multiplicity", None):
             msg = "Multiplicity value has not been set. When using a specific multiplicity fraction function please set the multiplicity"
             raise ValueError(msg)
 
         # Go over the chosen options
-        if self.grid_options["multiplicity_fraction_function"] in [1, "Arenou2010"]:
+        if self.population_options["multiplicity_fraction_function"] in [
+            1,
+            "Arenou2010",
+        ]:
             # Arenou 2010 will be used
-            verbose_print(
+            self.vb_debug(
                 "_calculate_multiplicity_fraction: Using Arenou 2010 to calculate multiplicity fractions",
-                self.grid_options["verbosity"],
-                3,
             )
 
             binary_fraction = self.Arenou2010_binary_fraction(system_dict["M_1"])
             multiplicity_fraction_dict = {
                 1: 1 - binary_fraction,
                 2: binary_fraction,
                 3: 0,
                 4: 0,
             }
 
-        elif self.grid_options["multiplicity_fraction_function"] in [2, "Raghavan2010"]:
+        elif self.population_options["multiplicity_fraction_function"] in [
+            2,
+            "Raghavan2010",
+        ]:
             # Raghavan 2010 will be used
-            verbose_print(
+            self.vb_debug(
                 "_calculate_multiplicity_fraction: Using Raghavan (2010) to calculate multiplicity fractions",
-                self.grid_options["verbosity"],
-                3,
             )
 
             binary_fraction = self.raghavan2010_binary_fraction(system_dict["M_1"])
             multiplicity_fraction_dict = {
                 1: 1 - binary_fraction,
                 2: binary_fraction,
                 3: 0,
                 4: 0,
             }
 
-        elif self.grid_options["multiplicity_fraction_function"] in [3, "Moe2017"]:
+        elif self.population_options["multiplicity_fraction_function"] in [
+            3,
+            "Moe2017",
+        ]:
             # We need to check several things now here:
 
             # First, are the options for the MOE2017 grid set? On start it is filled with the default settings
-            if not self.grid_options["Moe2017_options"]:
+            if not self.population_options["Moe2017_options"]:
                 msg = "The MOE2017 options do not seem to be set properly. The value is {}".format(
-                    self.grid_options["Moe2017_options"]
+                    self.population_options["Moe2017_options"]
                 )
                 raise ValueError(msg)
 
             # Second: is the Moecache filled.
             if not Moecache:
-                verbose_print(
+                self.vb_debug(
                     "_calculate_multiplicity_fraction: Moecache is empty. It needs to be filled with the data for the interpolators. Loading the data now",
-                    self.grid_options["verbosity"],
-                    3,
                 )
 
                 # Load the data
                 self._load_moe_di_stefano_data()
 
             # record the prev value
-            prev_M1_value_ms = self.grid_options["Moe2017_options"].get("M_1", None)
+            prev_M1_value_ms = self.population_options["Moe2017_options"].get(
+                "M_1", None
+            )
 
             # Set value of M1 of the current system
-            self.grid_options["Moe2017_options"]["M_1"] = system_dict["M_1"]
+            self.population_options["Moe2017_options"]["M_1"] = system_dict["M_1"]
 
             # Calculate the multiplicity fraction
             multiplicity_fraction_list = (
                 self.Moe_di_Stefano_2017_multiplicity_fractions(
-                    self.grid_options["Moe2017_options"], self.grid_options["verbosity"]
+                    self.population_options["Moe2017_options"],
+                    self.population_options["verbosity"],
                 )
             )
 
             # Turn into dict
             multiplicity_fraction_dict = {
                 el + 1: multiplicity_fraction_list[el]
                 for el in range(len(multiplicity_fraction_list))
             }
 
             # Set the prev value back
-            self.grid_options["Moe2017_options"]["M_1"] = prev_M1_value_ms
+            self.population_options["Moe2017_options"]["M_1"] = prev_M1_value_ms
 
         # we don't know what to do next
         else:
             msg = "Chosen value for the multiplicity fraction function is not known."
             raise ValueError(msg)
 
         # To make sure we normalize the dictionary
         multiplicity_fraction_dict = normalize_dict(multiplicity_fraction_dict)
 
-        verbose_print(
+        self.vb_debug(
             "Multiplicity: {} multiplicity_fraction: {}".format(
                 system_dict["multiplicity"],
                 multiplicity_fraction_dict[system_dict["multiplicity"]],
             ),
-            self.grid_options["verbosity"],
-            3,
         )
 
         return multiplicity_fraction_dict[system_dict["multiplicity"]]
 
     def get_moe_di_stefano_dataset(self, options, verbosity=0):
         """
             Function to get the default Moe and di Stefano dataset or accept a user input.
@@ -1006,222 +1250,37 @@
         if "JSON" in options:
             # use the JSON data passed in
             json_data = options["JSON"]
 
         elif "file" in options:
             # use the file passed in, if provided
             if not os.path.isfile(options["file"]):
-                verbose_print(
+                self.vb_error(
                     "The provided 'file' Moe and de Stefano JSON file does not seem to exist at {}".format(
                         options["file"]
                     ),
-                    verbosity,
-                    1,
                 )
 
                 raise ValueError
             if not options["file"].endswith(".json"):
-                verbose_print(
+                self.vb_error(
                     "Provided filename is not a json file",
-                    verbosity,
-                    1,
                 )
+                raise ValueError
 
             else:
                 # Read input data and Clean up the data if there are white spaces around the keys
                 with open(options["file"], "r", encoding="utf-8") as data_filehandle:
                     datafile_data = data_filehandle.read()
                     datafile_data = datafile_data.replace('" ', '"')
                     datafile_data = datafile_data.replace(' "', '"')
                     datafile_data = datafile_data.replace(' "', '"')
                     json_data = json.loads(datafile_data)
 
         if not json_data:
             # no JSON data or filename given, use the default 2017 dataset
-            verbose_print(
+            self.vb_info(
                 "Using the default Moe and de Stefano 2017 datafile",
-                verbosity,
-                1,
             )
             json_data = copy.deepcopy(moe_di_stefano_2017_data.moe_di_stefano_2017_data)
 
         return json_data
-
-    def get_Moe_di_Stefano_2017_default_options(self):
-        """
-        Function that returns the default options for the Moe & diStefano grid options
-        """
-
-        return {
-            # place holder for the JSON data to be used if a file
-            # isn't specified
-            "JSON": None,
-            # resolution data
-            "resolutions": {
-                "M": [
-                    20,  # M1
-                    20,  # M2 (i.e. q)
-                    0,  # M3 currently unused
-                    0,  # M4 currently unused
-                ],
-                "logP": [
-                    20,  # P2 (binary period)
-                    0,  # P3 (triple period) currently unused
-                    0,  # P4 (quadruple period) currently unused
-                ],
-                "ecc": [
-                    10,  # e (binary eccentricity)
-                    0,  # e2 (triple eccentricity) currently unused
-                    0,  # e3 (quadruple eccentricity) currently unused
-                ],
-            },
-            "samplerfuncs": {
-                "M": [None, None, None, None],
-                "logP": [None, None, None],
-                "ecc": [None, None, None],
-            },
-            "ranges": {
-                # stellar masses (Msun)
-                "M": [
-                    self.minimum_stellar_mass()
-                    * 1.05,  # 0.08 is a tad bit above the minimum mass. Don't sample at 0.07, otherwise the first row of q values will have a phasevol of 0. Anything higher is fine.
-                    80.0,  # (rather arbitrary) upper mass cutoff
-                ],
-                "q": [
-                    None,  # artificial qmin : set to None to use default
-                    None,  # artificial qmax : set to None to use default
-                ],
-                "logP": [0.0, 8.0],  # 0 = log10(1 day)  # 8 = log10(10^8 days)
-                "ecc": [0.0, 0.99],
-            },
-            # minimum stellar mass
-            "Mmin": self.minimum_stellar_mass(),  # We take the value that binary_c has set as the default
-            # multiplicity model (as a function of log10M1)
-            #
-            # You can use 'Poisson' which uses the system multiplicity
-            # given by Moe and maps this to single/binary/triple/quad
-            # fractions.
-            #
-            # Alternatively, 'data' takes the fractions directly
-            # from the data, but then triples and quadruples are
-            # combined (and there are NO quadruples).
-            "multiplicity_model": "Poisson",
-            # multiplicity modulator:
-            # [single, binary, triple, quadruple]
-            #
-            # e.g. [1,0,0,0] for single stars only
-            #      [0,1,0,0] for binary stars only
-            #
-            # defaults to [1,1,0,0] i.e. all types
-            #
-            "multiplicity_modulator": [
-                1,  # single
-                1,  # binary
-                0,  # triple
-                0,  # quadruple
-            ],
-            # given a mix of multiplicities, you can either (noting that
-            # here (S,B,T,Q) = appropriate modulator * model(S,B,T,Q) )
-            #
-            # 'norm'  : normalise so the whole population is 1.0
-            #           after implementing the appropriate fractions
-            #           S/(S+B+T+Q), B/(S+B+T+Q), T/(S+B+T+Q), Q/(S+B+T+Q)
-            #
-            # 'raw'   : stick to what is predicted, i.e.
-            #           S/(S+B+T+Q), B/(S+B+T+Q), T/(S+B+T+Q), Q/(S+B+T+Q)
-            #           without normalisation
-            #           (in which case the total probability < 1.0 unless
-            #            all you use single, binary, triple and quadruple)
-            #
-            # 'merge' : e.g. if you only have single and binary,
-            #           add the triples and quadruples to the binaries, so
-            #           binaries represent all multiple systems
-            #           ...
-            #           *** this is canonical binary population synthesis ***
-            #
-            #           Note: if multiplicity_modulator == [1,1,1,1] this
-            #                 option does nothing (equivalent to 'raw').
-            #
-            #
-            # note: if you only set one multiplicity_modulator
-            # to 1, and all the others to 0, then normalising
-            # will mean that you effectively have the same number
-            # of stars as single, binary, triple or quad (whichever
-            # is non-zero) i.e. the multiplicity fraction is ignored.
-            # This is probably not useful except for
-            # testing purposes or comparing to old grids.
-            "normalize_multiplicities": "merge",
-            # q extrapolation (below 0.15 and above 0.9) method. We can choose from ['flat', 'linear', 'plaw2', 'nolowq']
-            "q_low_extrapolation_method": "linear",
-            "q_high_extrapolation_method": "linear",
-        }
-
-    def get_Moe_di_Stefano_2017_default_options_description(self):
-        """
-        Function to return the descriptions for all the Moe & diStefano grid options
-        """
-
-        return {
-            "resolutions": "",
-            "ranges": "",
-            "Mmin": "Minimum stellar mass",
-            "multiplicity_model": """
-        multiplicity model (as a function of log10M1)
-
-        You can use 'Poisson' which uses the system multiplicity
-        given by Moe and maps this to single/binary/triple/quad
-        fractions.
-
-        Alternatively, 'data' takes the fractions directly
-        from the data, but then triples and quadruples are
-        combined (and there are NO quadruples).
-        """,
-            "multiplicity_modulator": """
-        [single, binary, triple, quadruple]
-
-        e.g. [1,0,0,0] for single stars only
-             [0,1,0,0] for binary stars only
-
-        defaults to [1,1,0,0] i.e. singles and binaries
-        """,
-            "normalize_multiplicities": """
-        'norm': normalise so the whole population is 1.0
-                after implementing the appropriate fractions
-                S/(S+B+T+Q), B/(S+B+T+Q), T/(S+B+T+Q), Q/(S+B+T+Q)
-                given a mix of multiplicities, you can either (noting that
-                here (S,B,T,Q) = appropriate modulator * model(S,B,T,Q) )
-                note: if you only set one multiplicity_modulator
-                to 1, and all the others to 0, then normalising
-                will mean that you effectively have the same number
-                of stars as single, binary, triple or quad (whichever
-                is non-zero) i.e. the multiplicity fraction is ignored.
-                This is probably not useful except for
-                testing purposes or comparing to old grids.
-
-        'raw'   : stick to what is predicted, i.e.
-                  S/(S+B+T+Q), B/(S+B+T+Q), T/(S+B+T+Q), Q/(S+B+T+Q)
-                  without normalisation
-                  (in which case the total probability < 1.0 unless
-                  all you use single, binary, triple and quadruple)
-
-        'merge' : e.g. if you only have single and binary,
-                  add the triples and quadruples to the binaries, so
-                  binaries represent all multiple systems
-                  ...
-                  *** this is canonical binary population synthesis ***
-
-                  It only takes the maximum multiplicity into account,
-                  i.e. it doesn't multiply the resulting array by the multiplicity modulator again.
-                  This prevents the resulting array to always be 1 if only 1 multiplicity modulator element is nonzero
-
-                  Note: if multiplicity_modulator == [1,1,1,1]. this option does nothing (equivalent to 'raw').
-        """,
-            "q_low_extrapolation_method": """
-        q extrapolation (below 0.15) method
-            none
-            flat
-            linear2
-            plaw2
-            nolowq
-        """,
-            "q_high_extrapolation_method": "Same as q_low_extrapolation_method",
-        }
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/analytics.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/analytics.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,96 +24,87 @@
     #######################
 
     def make_analytics_dict(self):
         """
         Function to create the analytics dictionary
         """
 
-        print("Do analytics")
+        self.vb_info("Do analytics")
 
         analytics_dict = {}
 
-        if self.grid_options["do_analytics"]:
+        if self.population_options["do_analytics"]:
             # Put all interesting stuff in a variable and output that afterwards, as analytics of the run.
             analytics_dict = {
-                "population_id": self.grid_options["_population_id"],
-                "evolution_type": self.grid_options["evolution_type"],
-                "failed_count": self.grid_options["_failed_count"],
-                "failed_prob": self.grid_options["_failed_prob"],
-                "failed_systems_error_codes": self.grid_options[
+                "population_id": self.population_options["_population_id"],
+                "evolution_type": self.population_options["evolution_type"],
+                "failed_count": self.population_options["_failed_count"],
+                "failed_prob": self.population_options["_failed_prob"],
+                "failed_systems_error_codes": self.population_options[
                     "_failed_systems_error_codes"
                 ].copy(),
-                "errors_exceeded": self.grid_options["_errors_exceeded"],
-                "errors_found": self.grid_options["_errors_found"],
-                "total_probability": self.grid_options["_probtot"],
-                "total_count": self.grid_options["_count"],
-                "start_timestamp": self.grid_options["_start_time_evolution"],
-                "end_timestamp": self.grid_options["_end_time_evolution"],
+                "errors_exceeded": self.population_options["_errors_exceeded"],
+                "errors_found": self.population_options["_errors_found"],
+                "total_probability": self.population_options["_probtot"],
+                "total_count": self.population_options["_count"],
+                "start_timestamp": self.population_options["_start_time_evolution"],
+                "end_timestamp": self.population_options["_end_time_evolution"],
                 "time_elapsed": self.time_elapsed(),
-                "total_mass_run": self.grid_options["_total_mass_run"],
-                "total_probability_weighted_mass_run": self.grid_options[
+                "total_mass_run": self.population_options["_total_mass_run"],
+                "total_probability_weighted_mass_run": self.population_options[
                     "_total_probability_weighted_mass_run"
                 ],
-                "zero_prob_stars_skipped": self.grid_options[
+                "zero_prob_stars_skipped": self.population_options[
                     "_zero_prob_stars_skipped"
                 ],
             }
 
         if "metadata" in self.grid_ensemble_results:
             # Add analytics dict to the metadata too:
             self.grid_ensemble_results["metadata"].update(analytics_dict)
-            print("Added analytics to metadata")
+            self.vb_info("Added analytics to metadata")
             self.add_system_metadata()
         else:
             # use existing analytics dict
             analytics_dict = self.grid_ensemble_results.get("metadata", {})
 
         return analytics_dict
 
     def set_time(self, when):
         """
         Function to set the timestamp at when, where when is 'start' or 'end'.
 
         If when == end, we also calculate the time elapsed.
         """
-        self.grid_options["_" + when + "_time_evolution"] = time.time()
+        self.population_options["_" + when + "_time_evolution"] = time.time()
         if when == "end":
-            self.grid_options["_time_elapsed"] = self.time_elapsed(force=True)
+            self.population_options["_time_elapsed"] = self.time_elapsed(force=True)
 
     def time_elapsed(self, force=False):
         """
         Function to return how long a population object has been running.
 
         We return the cached value if it's available, and calculate
         the time elapsed if otherwise or if force is True
         """
         for x in ["_start_time_evolution", "_end_time_evolution"]:
-            if not self.grid_options[x]:
-                self.grid_options[x] = time.time()
-                # print("{} missing : {}".format(x, self.grid_options[x]))
-
-        if force or "_time_elapsed" not in self.grid_options:
-            self.grid_options["_time_elapsed"] = (
-                self.grid_options["_end_time_evolution"]
-                - self.grid_options["_start_time_evolution"]
+            if not self.population_options[x]:
+                self.population_options[x] = time.time()
+
+        if force or "_time_elapsed" not in self.population_options:
+            self.population_options["_time_elapsed"] = (
+                self.population_options["_end_time_evolution"]
+                - self.population_options["_start_time_evolution"]
             )
-            # print(
-            #     "set time elapsed = {} - {} = {}".format(
-            #         self.grid_options["_end_time_evolution"],
-            #         self.grid_options["_start_time_evolution"],
-            #         self.grid_options["_time_elapsed"],
-            #     )
-            # )
 
-        return self.grid_options["_time_elapsed"]
+        return self.population_options["_time_elapsed"]
 
     def CPU_time(self):
         """
         Function to return how much CPU time we've used
         """
-        dt = self.grid_options["_time_elapsed"]
 
-        ncpus = self.grid_options.get("num_processes", 1)
+        dt = self.population_options["_time_elapsed"]
 
-        # print("CPU time : dt={} n={} -> {}".format(dt, ncpus, dt * ncpus))
+        ncpus = self.population_options.get("_num_processes", 1)
 
         return dt * ncpus
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/argument_handling.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/argument_handling.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 """
 Main script to provide the argument handling class extensions
 """
 
 # pylint: disable=E1101
+
+import logging
+import os
 import sys
+from logging import config
 
 import str2bool
 
+from binarycpython.utils.logging_functions import verbosity_level_dict
+
 
 class argument_handling:
     """
     Extension for the Population class containing the code for source-file sampling functions
-
-    ###################################################
-    # Argument functions
-    ###################################################
-
-    # General flow of generating the arguments for the binary_c call:
-    # - user provides parameter and value via set (or manually but that is risky)
-    # - The parameter names of these input get compared to the parameter names in the self.defaults;
-    #    with this, we know that its a valid parameter to give to binary_c.
-    # - For a single system, the bse_options will be written as a arg line
-    # - For a population the bse_options will get copied to a temp_bse_options dict and updated with
-    #   all the parameters generated by the grid
-
-    # I will not create the argument line by fully writing all the defaults and overriding user
-    # input, that seems not necessary because by using the get_defaults() function we already
-    # know for sure which parameter names are valid for the binary_c version
-    # And because binary_c uses internal defaults, its not necessary to explicitly pass them.
-    # I do however suggest everyone to export the binary_c defaults to a file, so that you know
-    # exactly which values were the defaults.
     """
 
     def __init__(self, **kwargs):
         """
         Init function for the spacing_functions class
         """
 
@@ -43,116 +30,157 @@
         """
         Function to set the values of the population. This is the preferred method to set values
         of functions, as it provides checks on the input.
 
         the bse_options will get populated with all the those that have a key that is present
         in the self.defaults
 
-        the grid_options will get updated with all the those that have a key that is present
-        in the self.grid_options
+        the population_options will get updated with all the those that have a key that is present
+        in the self.population_options
 
         If neither of above is met; the key and the value get stored in a custom_options dict.
 
         Args:
-            via kwargs all the arguments are either set to binary_c parameters, grid_options or custom_options (see above)
+            via kwargs all the arguments are either set to binary_c parameters, population_options or custom_options (see above)
         """
 
+        ###############
         # Go over all the input
         for key, value in kwargs.items():
             # match to hostname if appropriate
             value = self._match_arg_to_host(arg={key: value})
 
+            ###############
+            # Filter out keys for the population_options
+            if key in self.population_options.keys():
+                self.vb_warning(
+                    "adding: {}={} to population_options".format(key, value),
+                )
+
+                # validate values
+                self._validate_population_options(key, value)
+
+                # Set values
+                self.population_options[key] = value
+
+                ###########
+                # Handle some actions for specific key setting
+
+                # Update config for loggers
+                if key == "log_config_file":
+                    if value is not None:
+                        # check if file exists
+                        if os.path.isfile(value):
+                            config.fileConfig(value)
+                            self.logger = logging
+                        else:
+                            raise ValueError(f"File {value} does not exist.")
+
+                    # Unset the loggers
+                    if value is None:
+                        self.logger = None
+
+                # Update verbosity
+                if key == "verbosity":
+                    if self.logger is not None:
+                        self.logger.setLevel(verbosity_level_dict[value])
+                        for handler in self.logger.handlers:
+                            handler.setLevel(verbosity_level_dict[value])
+
+                # Update logfile for logging
+                if key == "log_file":
+                    if self.logger is not None:
+                        for handler in self.logger.handlers:
+                            if isinstance(handler, logging.FileHandler):
+                                handler.close()
+                                handler.baseFilename = os.path.abspath(value)
+
+            ###############
             # Filter out keys for the bse_options
-            if key in self.defaults:
-                self.verbose_print(
+            elif key in self.defaults:
+                self.vb_warning(
                     "adding: {}={} to BSE_options".format(key, value),
-                    self.grid_options["verbosity"],
-                    2,
                 )
                 self.bse_options[key] = value
 
+            ###############
             # Extra check to check if the key fits one of parameter names that end with %d
             elif self._check_key_is_special_param(key):
-                self.verbose_print(
+                self.vb_warning(
                     "adding: {}={} to BSE_options by catching the %d".format(
                         key, value
                     ),
-                    self.grid_options["verbosity"],
-                    1,
                 )
                 self.bse_options[key] = value
 
-            # Filter out keys for the grid_options
-            elif key in self.grid_options.keys():
-                self.verbose_print(
-                    "adding: {}={} to grid_options".format(key, value),
-                    self.grid_options["verbosity"],
-                    1,
-                )
-                self.grid_options[key] = value
-
+            ###############
             # The of the keys go into a custom_options dict
             else:
-                self.verbose_print(
+                self.vb_warning(
                     "<<<< Warning: Key does not match previously known parameter: \
                     adding: {}={} to custom_options >>>>".format(
                         key, value
                     ),
-                    self.grid_options["verbosity"],
-                    0,  # NOTE: setting this to be 0 prevents mistakes being overlooked.
                 )
                 self.custom_options[key] = value
 
+    def _validate_population_options(self, key, value):
+        """
+        Function to handle validation of the arguments passed to the population options
+        """
+
+        # validate
+        self.validation_schema({key: value})
+
     def parse_cmdline(self) -> None:
         """
         Function to handle settings values via the command line in the form x=y, w=z, etc.
 
         Best to be called after all the .set(..) lines, and just before the .evolve() is called
 
-        If you input any known parameter (i.e. contained in grid_options, defaults/bse_options
+        If you input any known parameter (i.e. contained in population_options, defaults/bse_options
         or custom_options), this function will attempt to convert the input from string
         (because everything is string) to the type of the value that option had before.
 
         The values of the bse_options are initially all strings, but after user input they
         can change to ints.
 
         The value of any new parameter (which will go to custom_options) will be a string.
         """
 
         # get the cmd-line args in the form x=y
         cmdline_args = sys.argv[1:]
 
         if cmdline_args:
-            self.verbose_print(
+            self.vb_info(
                 "Found cmdline args. Parsing them now",
-                self.grid_options["verbosity"],
-                1,
             )
 
             # Grab the input and split them up, while accepting only non-empty entries
             # cmdline_args = args
-            self.grid_options["_commandline_input"] = cmdline_args
+            self.population_options["_commandline_input"] = cmdline_args
 
             # expand args by hostname
             cmdline_args = self.expand_args_by_hostname(cmdline_args)
 
             # Make dict and fill it
             cmdline_dict = {}
             for cmdline_arg in cmdline_args:
                 split = cmdline_arg.split("=")
 
+                # Check if its actually a key-value pair separated by "="
                 if len(split) == 2:
                     parameter = split[0]
                     value = split[1]
 
                     old_value_found = False
 
                     # Find an old value
-                    if parameter in self.grid_options:
-                        old_value = self.grid_options[parameter]
+                    if parameter in self.population_options:
+                        old_value = self.population_options[parameter]
                         old_value_found = True
 
                     elif parameter in self.custom_options:
                         old_value = self.custom_options[parameter]
                         old_value_found = True
 
                     elif parameter in self.bse_options:
@@ -164,31 +192,29 @@
                         old_value = self.defaults[parameter]
                         old_value_found = True
 
                     # (attempt to) convert type
                     if old_value_found:
                         if old_value is not None:
                             try:
-                                self.verbose_print(
+                                self.vb_debug(
                                     "Converting type of {} from {} to {}".format(
                                         parameter, type(value), type(old_value)
                                     ),
-                                    self.grid_options["verbosity"],
-                                    3,
                                 )
                                 try:
                                     if isinstance(old_value, bool):
                                         value = str2bool.str2bool(value)
                                     else:
                                         value = type(old_value)(value)
-                                    self.verbose_print(
-                                        "Success!", self.grid_options["verbosity"], 2
+                                    self.vb_debug(
+                                        "Success!",
                                     )
                                 except Exception as e:
-                                    print(
+                                    self.vb_error(
                                         "Failed to convert {param} value with type {type}: old_value is '{old}', new value is '{new}', {e}".format(
                                             param=parameter,
                                             old=old_value,
                                             type=type(old_value),
                                             new=split[1],
                                             e=e,
                                         )
@@ -199,41 +225,36 @@
 
                                 # might be able to eval the parameter, e.g.
                                 # an expression like "2-1" can eval to "1"
                                 # which would be valid
                                 try:
                                     evaled = eval(value)
                                     value = type(old_value)(evaled)
-                                    self.verbose_print(
+                                    self.vb_debug(
                                         "Success! (evaled)",
-                                        self.grid_options["verbosity"],
-                                        2,
                                     )
 
                                 except ValueError:
-                                    self.verbose_print(
+                                    self.vb_warning(
                                         "Tried to convert the given parameter {}/value {} to its correct type {} (from old value {}). But that wasn't possible.".format(
                                             parameter, value, type(old_value), old_value
                                         ),
-                                        self.grid_options["verbosity"],
-                                        0,
                                     )
+
                     # Add to dict
-                    self.verbose_print(
+                    self.vb_info(
                         "setting {} = {} ".format(parameter, value),
-                        self.grid_options["verbosity"],
-                        3,
                     )
                     cmdline_dict[parameter] = value
 
                 else:
-                    print(
-                        "Error: I do not know how to process",
-                        cmdline_arg,
-                        " : cmdline args should be in the format x=y, yours appears not to be.",
+                    self.vb_error(
+                        "Error: I do not know how to process {}: cmdline args should be in the format x=y, yours appears not to be.".format(
+                            cmdline_arg
+                        ),
                     )
                     self.exit(1)
 
             # unpack the dictionary into the setting function that handles where the values are set
             self.set(**cmdline_dict)
 
     def _return_argline(self, parameter_dict=None):
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/cache.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 File containing the class extension for the population object that contains cache functionality
 
 Module containing (e.g. LRU) cache functionality for binary_c-python.
 
 We use cachetools when possible because this allows us to set up the
-cache of the appropriate size for the task in the grid_options dict.
+cache of the appropriate size for the task in the population_options dict.
 Please see the LRU_* options in there.
 """
 
 # pylint: disable=E1101
 
 import contextlib
 import getpass
@@ -27,17 +27,30 @@
     def __init__(self, **kwargs):
         """
         Init function for the spacing_functions class
         """
 
         return
 
+    # def default_cache_dir(self):
+    #     """
+    #     Return a default cache directory path, or None if we cannot find one.
+    #     """
+    #     error_string = "__*ERR*__"  # string that cannot be a path
+    #     for path in [
+    #         os.path.join(os.environ.get("HOME", error_string), ".cache", "binary_c"),
+    #         os.path.join(os.environ.get("TMP", error_string), "cache"),
+    #     ]:
+    #         if error_string not in path and os.path.isdir(path):
+    #             return path
+    #     return None
+
     def default_cache_dir(self):
         """
-        Return a default cache directory path for binary_c-python, or None if we cannot find one. This is used in grid_options_defaults.py
+        Return a default cache directory path for binary_c-python, or None if we cannot find one. This is used in population_options_defaults.py
         """
 
         error_string = "__*ERR*__"  # string that cannot be a path
         for path in [
             os.path.join(os.environ.get("HOME", error_string), ".cache"),
             os.path.join(os.environ.get("TMP", error_string), "cache"),
             os.path.join("var", "tmp", getpass.getuser(), "cache"),
@@ -88,62 +101,63 @@
 
             return
 
     def setup_function_cache(self, vb=False, cachetype=None):
         """
         Function to wrap binary_c-python's functions in function cache.
 
-        The functions listed in self.grid_options['function_cache_functions'] are
-        given caches of size self.grid_options['function_cache_size'][func]
+        The functions listed in self.population_options['function_cache_functions'] are
+        given caches of size self.population_options['function_cache_size'][func]
 
         Args: None
         """
 
         # add our custom NullCache to the cachetools selection
         setattr(cachetools, "NullCache", self.NullCache)
 
-        if not self.grid_options["function_cache"]:
+        if not self.population_options["function_cache"]:
             # no function cache: set all to NullCache
             # TODO: This cachetype(Nullcache) is wrong.
-            for func in self.grid_options["function_cache_functions"].keys():
+            for func in self.population_options["function_cache_functions"].keys():
                 self.function_cache[func] = cachetype(self.NullCache)
 
-        for func in self.grid_options["function_cache_functions"].keys():
-            (maxsize, cachetype, testargs) = self.grid_options[
+        for func in self.population_options["function_cache_functions"].keys():
+            (maxsize, cachetype, testargs) = self.population_options[
                 "function_cache_functions"
             ].get(func)
 
             # which cache should we use?
             if cachetype:
                 # use type passed in, if given
                 usecachetype = cachetype
-            elif not self.grid_options["function_cache"]:
+            elif not self.population_options["function_cache"]:
                 # function cache is disabled, use NoCache
                 usecachetype = "NoCache"
             else:
                 if cachetype is None:
                     # use the default type
-                    usecachetype = self.grid_options["function_cache_default_type"]
+                    usecachetype = self.population_options[
+                        "function_cache_default_type"
+                    ]
                 else:
                     # use type passed in
                     usecachetype = cachetype
 
-            if vb:
-                print(
-                    "Setup cache for func {func} : maxsize={maxsize}, cachetype={cachetype}, testargs={testargs}-> use {usecachetype}".format(
-                        func=func,
-                        maxsize=maxsize,
-                        cachetype=cachetype,
-                        testargs=testargs,
-                        usecachetype=usecachetype,
-                    )
+            self.vb_info(
+                "Setup cache for func {func} : maxsize={maxsize}, cachetype={cachetype}, testargs={testargs}-> use {usecachetype}".format(
+                    func=func,
+                    maxsize=maxsize,
+                    cachetype=cachetype,
+                    testargs=testargs,
+                    usecachetype=usecachetype,
                 )
+            )
 
             if usecachetype == "TTLCache":
-                extra_cacheargs = [self.grid_options["function_cache_TTL"]]
+                extra_cacheargs = [self.population_options["function_cache_TTL"]]
             else:
                 extra_cacheargs = []
 
             # detect if the function is already wrapped
             x = func.split(".")
             modulename = "binarycpython.utils.population_extensions." + x[0]
             module = importlib.import_module(modulename)  # noqa: F841
@@ -180,22 +194,21 @@
             # (it's never actually set)
             if usecachetype == "NoCache":
                 cachetools_func = getattr(cachetools, "NullCache")
             else:
                 cachetools_func = getattr(cachetools, usecachetype)
 
             if maxsize == 0:
-                maxsize = self.grid_options["function_cache_default_maxsize"]
+                maxsize = self.population_options["function_cache_default_maxsize"]
 
-            if vb:
-                print(
-                    "Make function cache for func {func}, maxsize {maxsize}".format(
-                        func=func, maxsize=maxsize
-                    )
+            self.vb_info(
+                "Make function cache for func {func}, maxsize {maxsize}".format(
+                    func=func, maxsize=maxsize
                 )
+            )
 
             # set up cache function args
             if maxsize is None:
                 args = [2]
             else:
                 args = [maxsize]
             args += extra_cacheargs
@@ -218,33 +231,33 @@
 
         Args:
             dt (default 5) in seconds the length of each test. Long is more accurate, but takes longer.
         """
 
         # loop lists
         cachetypes = ("NoCache", "NullCache", "FIFOCache", "LRUCache", "TTLCache")
-        functions = self.grid_options["function_cache_functions"].keys()
+        functions = self.population_options["function_cache_functions"].keys()
         maxsizes = (0, 1, 2, 4, 8, 16, 32, 64, 128, 256)
 
-        self.grid_options["function_cache"] = True
+        self.population_options["function_cache"] = True
         for n, func in enumerate(functions):
-            print("Cache speed test of function {func}".format(func=func))
-            print("{:18s}".format(""), end="")
+            self.vb_debug("Cache speed test of function {func}".format(func=func))
+            self.vb_debug("{:18s}".format(""), end="")
             for x, maxsize in enumerate(maxsizes):
-                print("{:>9s}".format(str(maxsize)), end="")
-            print("")
+                self.vb_debug("{:>9s}".format(str(maxsize)), end="")
+            self.vb_debug("")
 
             best = 0
             best_type = None
             best_maxsize = None
             for y, type in enumerate(cachetypes):
-                print("{:18s}".format(type), end="")
-                self.grid_options["function_cache_default_type"] = type
+                self.vb_debug("{:18s}".format(type), end="")
+                self.population_options["function_cache_default_type"] = type
                 self.setup_function_cache()
-                (maxsize, cachetype, testargs) = self.grid_options[
+                (maxsize, cachetype, testargs) = self.population_options[
                     "function_cache_functions"
                 ].get(func)
 
                 # TODO: Make this part better: needs to be able to handle any depth
                 x = func.split(".")
                 modulename = (  # noqa: F841
                     "binarycpython.utils.population_extensions." + x[0]
@@ -276,29 +289,28 @@
                             count = 0
                             try:
                                 while time.time() < tfin:
                                     _method(self, *args, **kwargs)
                                     count += 1
                             # TODO: specify the exception
                             except Exception as e:
-                                print("Cache call failed:", e)
+                                self.vb_error("Cache call failed:", e)
                                 self.exit(1)
 
                         if count < 99999:
-                            print("{:9d}".format(count), end="")
+                            self.vb_debug("{:9d}".format(count), end="")
                         else:
-                            print("{:9.2e}".format(float(count)), end="")
+                            self.vb_debug("{:9.2e}".format(float(count)), end="")
 
                         if count > best:
                             best = count
                             best_type = type
                             best_maxsize = maxsize
-                    print("")
 
-            print(
+            self.vb_info(
                 "Best cache type {type} with maxsize {maxsize}\n".format(
                     type=best_type, maxsize=best_maxsize
                 )
             )
 
     """
 Cache speed test of function distribution_functions.powerlaw_constant
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/custom_generator_sampling.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/custom_generator_sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,23 +25,23 @@
         """
 
     def _custom_generator_sampling_get_generator(self):
         """
         Function to get the generator for the _custom_generator_sampling sampling method. Called by _get_generator and used in the actual evolution loop.
         """
 
-        generator = self.grid_options["custom_generator"]
+        generator = self.population_options["custom_generator"]
 
         return generator
 
     def _custom_generator_sampling_setup(self):
         """
         Function to prepare the class for sampling via a custom generator
         """
 
-        if not isinstance(self.grid_options["custom_generator"], Iterable):
-            print(
+        if not isinstance(self.population_options["custom_generator"], Iterable):
+            self.vb_error(
                 "Error. provided no or wrong custom value for the system generator (custom_generator: {})".format(
-                    self.grid_options["custom_generator"]
+                    self.population_options["custom_generator"]
                 )
             )
             raise ValueError
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/dataIO.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/dataIO.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import compress_pickle
 import flufl.lock
 import msgpack
 
 from binarycpython.utils.dicts import merge_dicts
 from binarycpython.utils.ensemble import ensemble_file_type
-from binarycpython.utils.functions import now, verbose_print
+from binarycpython.utils.functions import now
 
 
 class dataIO:
     """
     Class extension for the population object that contains data input-output (IO) functions
     """
 
@@ -46,19 +46,19 @@
         self,
         population_object=None,
         filename=None,
         confirmation=True,
         compression="gzip",
     ):
         """
-        Save pickled Population object to file at filename or, if filename is None, whatever is set at self.grid_options['save_population_object']
+        Save pickled Population object to file at filename or, if filename is None, whatever is set at self.population_options['save_population_object']
 
         Args:
             population_object : the object to be saved to the file. If population_object is None, use self.
-            filename : the name of the file to be saved. If not set, use self.grid_options['save_population_object']
+            filename : the name of the file to be saved. If not set, use self.population_options['save_population_object']
             confirmation : if True, a file "filename.saved" is touched just after the dump, so we know it is finished. TODO: fix this
             compression (optional, default = "gzip"): TODO: fix this
 
         Compression is performed according to the filename, as stated in the
         compress_pickle documentation at
         https://lucianopaz.github.io/compress_pickle/html/
 
@@ -69,39 +69,39 @@
 
         if population_object is None:
             # default to using self
             population_object = self
 
         if filename is None:
             # get filename from self
-            filename = self.grid_options["save_population_object"]
+            filename = self.population_options["save_population_object"]
 
         if filename:
-            print(
+            self.vb_info(
                 "Save population {id}, probtot {probtot} to pickle in {filename}".format(
-                    id=self.grid_options["_population_id"],
-                    probtot=population_object.grid_options["_probtot"],
+                    id=self.population_options["_population_id"],
+                    probtot=population_object.population_options["_probtot"],
                     filename=filename,
                 )
             )
 
             # Some parts of the population_object cannot be pickled:
             # remove them, and restore them after pickling
 
             # remove shared memory
             shared_memory = population_object.shared_memory
             population_object.shared_memory = None
 
             # delete system generator
-            system_generator = population_object.grid_options["_system_generator"]
-            population_object.grid_options["_system_generator"] = None
+            system_generator = population_object.population_options["_system_generator"]
+            population_object.population_options["_system_generator"] = None
 
             # delete _store_memaddr
-            _store_memaddr = population_object.grid_options["_store_memaddr"]
-            population_object.grid_options["_store_memaddr"] = None
+            _store_memaddr = population_object.population_options["_store_memaddr"]
+            population_object.population_options["_store_memaddr"] = None
 
             # delete persistent_data_memory_dict
             persistent_data_memory_dict = population_object.persistent_data_memory_dict
             population_object.persistent_data_memory_dict = None
 
             # add metadata if it doesn't exist
             if "metadata" not in population_object.grid_ensemble_results:
@@ -117,27 +117,27 @@
 
             # add max memory use
             try:
                 self.grid_ensemble_results["metadata"][
                     "max_memory_use"
                 ] = copy.deepcopy(sum(shared_memory["max_memory_use_per_thread"]))
             except Exception as e:
-                print("save_population_object : Error: ", e)
+                self.vb_error("save_population_object : Error: ", e)
                 raise Exception(e) from e
 
             # dump pickle file
             compress_pickle.dump(population_object, filename, pickler_method="dill")
 
             # restore data
             population_object.shared_memory = shared_memory
-            population_object.grid_options["_system_generator"] = system_generator
+            population_object.population_options["_system_generator"] = system_generator
             del population_object.grid_ensemble_results["metadata"][
                 "save_population_time"
             ]
-            population_object.grid_options["store_memaddr"] = _store_memaddr
+            population_object.population_options["store_memaddr"] = _store_memaddr
             population_object.persistent_data_memory_dict = persistent_data_memory_dict
 
             self.NFS_flush_hack(filename)
 
             # touch 'saved' file
             saved = filename + ".saved"
             self.HPC_touch(saved)
@@ -151,15 +151,17 @@
         if filename is None:
             obj = None
         else:
             try:
                 obj = compress_pickle.load(filename, pickler_method="dill")
             except Exception as e:
                 obj = None
-                print("Loading of the compressed object went wrong: {}".format(e))
+                self.vb_error(
+                    "Loading of the compressed object went wrong: {}".format(e)
+                )
         return obj
 
     def merge_populations(self, refpop, newpop):
         """
         merge newpop's results data into refpop's results data
 
         Args:
@@ -170,15 +172,17 @@
             nothing
 
         Note:
             The file should be saved using save_population_object()
         """
 
         # combine data
-        refpop.grid_results = merge_dicts(refpop.grid_results, newpop.grid_results)
+        refpop.population_results = merge_dicts(
+            refpop.population_results, newpop.population_results
+        )
 
         # special cases
         maxmem = 0
         if "max_memory_use" in refpop.grid_ensemble_results.get(
             "metadata", {}
         ) and "max_memory_use" in newpop.grid_ensemble_results.get("metadata", {}):
             maxmem = max(
@@ -209,21 +213,21 @@
                 refpop.grid_ensemble_results, newpop.grid_ensemble_results
             )
 
             # set special cases
             refpop.grid_ensemble_results["metadata"]["max_memory_use"] = maxmem
 
         except Exception as e:
-            print("Error merging grid_ensemble_results:", e)
+            self.vb_error("Error merging grid_ensemble_results:", e)
             raise Exception(e) from e
 
         for key in ["_probtot"]:
-            refpop.grid_options[key] += newpop.grid_options[key]
+            refpop.population_options[key] += newpop.population_options[key]
 
-        refpop.grid_options["_killed"] |= newpop.grid_options["_killed"]
+        refpop.population_options["_killed"] |= newpop.population_options["_killed"]
 
     def merge_populations_from_file(self, refpop, filename):
         """
          Wrapper for merge_populations so it can be done directly
          from a file.
 
         Args:
@@ -232,89 +236,89 @@
 
         Note:
             The file should be saved using save_population_object()
         """
 
         mtime = time.localtime(os.path.getmtime(filename))
         modtime = time.strftime("%a, %d %b %Y %H:%M:%S", mtime)
-        print(
+        self.vb_debug(
             "Load data from {filename} : size {size}, modtime {modtime}".format(
                 filename=filename,
                 size=os.path.getsize(filename),
                 modtime=modtime,
             )
         )
 
         newpop = self.load_population_object(filename)
 
-        if "total_count" in newpop.grid_options:
-            n = newpop.grid_options["total_count"]
-        elif "_count" in newpop.grid_options:
-            n = newpop.grid_options["_count"]
+        if "total_count" in newpop.population_options:
+            n = newpop.population_options["total_count"]
+        elif "_count" in newpop.population_options:
+            n = newpop.population_options["_count"]
         elif (
             "metadata" in newpop.grid_ensemble_results
             and "_count" in newpop.grid_ensemble_results["metadata"]
         ):
             n = newpop.grid_ensemble_results["metadata"]["_count"]
         else:
             n = -1
 
-        print("Loaded data from {n} stars".format(n=n))
+        self.vb_info("Loaded data from {n} stars".format(n=n))
 
         # merge with refpop
         self.merge_populations(refpop, newpop)
 
     def snapshot_filename(self):
         """
         Automatically choose the snapshot filename.
         """
         if self.HPC_job():
             return self.HPC_snapshot_filename()
 
-        file = os.path.join(self.grid_options["tmp_dir"], "snapshot.gz")
+        file = os.path.join(self.population_options["tmp_dir"], "snapshot.gz")
         return file
 
     def load_snapshot(self, file):
         """
         Load a snapshot from file and set it in the preloaded_population placeholder.
         """
         newpop = self.load_population_object(file)
 
         # unset the _killed flag, in case it was set
-        newpop.grid_options["_killed"] = False
+        newpop.population_options["_killed"] = False
 
         # set in preloaded_population for later  merge
         self.preloaded_population = newpop
 
         # set the start position for new stars
-        self.grid_options["start_at"] = newpop.grid_options["start_at"]
+        self.population_options["start_at"] = newpop.population_options["start_at"]
 
-        print(
+        self.vb_info(
             "Loaded from snapshot at {file} : {nstars} stars, start at star {nstart}".format(
                 file=file,
-                nstars=0,  # self.grid_options[''],
-                nstart=self.grid_options["start_at"],
+                nstars=0,  # self.population_options[''],
+                nstart=self.population_options["start_at"],
             )
         )
         return
 
     def save_snapshot(self, file=None):
         """
         Save the population object to a snapshot file, automatically choosing the filename if none is given.
         """
         if file is None:
             file = self.snapshot_filename()
 
-        if "_count" in self.grid_options:
-            n = self.grid_options["_count"]
+        if "_count" in self.population_options:
+            n = self.population_options["_count"]
         else:
             n = "?"
 
-        print("Saving snapshot containing {} stars to {}".format(n, file))
-        self.save_population_object(object=self, filename=file)
+        self.vb_info("Saving snapshot containing {} stars to {}".format(n, file))
+        self.save_population_object(population_object=self, filename=file)
 
     def write_ensemble(
         self,
         output_file,
         data=None,
         sort_keys=True,
         indent=4,
@@ -355,15 +359,15 @@
         file_type = ensemble_file_type(output_file)
 
         # default to using grid_ensemble_results if no data is given
         if data is None:
             data = self.grid_ensemble_results
 
         if not file_type:
-            print(
+            self.vb_error(
                 "Unable to determine file type from ensemble filename {} : it should be .json or .msgpack.".format(
                     output_file
                 )
             )
             self.exit(code=1)
         else:
             if file_type == "JSON":
@@ -383,15 +387,15 @@
                 )  # TODO: i think something is going wrong here. not sure but doing msgpack and .gz e.g gives an error about str input rather than bytes. i think this is because the self.open does not take into account that the msgpack stream requires different properties.
 
                 # msgpack output
                 msgpack.dump(data, f)
 
             f.close()
 
-        print(
+        self.vb_info(
             "Thread {thread}: Wrote ensemble results to file: {colour}{file}{reset} (file type {file_type})".format(
                 thread=self.process_ID,
                 file=output_file,
                 colour=self.ANSI_colours["green"],
                 reset=self.ANSI_colours["reset"],
                 file_type=file_type,
             )
@@ -421,47 +425,45 @@
             include_defaults: (optional, default = None) whether to include the defaults of binary_c in the lines that are written. Beware that this will result in very long lines, and it might be better to just export the binary_c defaults and keep them in a separate file.
 
         Returns:
             filename: filename that was used to write the calls to
         """
 
         # Check if there is no compiled grid yet. If not, lets try to build it first.
-        if not self.grid_options["_system_generator"]:
+        if not self.population_options["_system_generator"]:
 
             ## check the settings:
             if self.bse_options.get("ensemble", None):
                 if self.bse_options["ensemble"] == 1:
                     if not self.bse_options.get("ensemble_defer", 0) == 1:
-                        verbose_print(
+                        self.vb_error(
                             "Error, if you want to run an ensemble in a population, the output needs to be deferred",
-                            self.grid_options["verbosity"],
-                            0,
                         )
                         raise ValueError
 
             # Put in check
-            if len(self.grid_options["_sampling_variables"]) == 0:
-                print("Error: you haven't defined any grid variables! Aborting")
+            if len(self.population_options["_sampling_variables"]) == 0:
+                self.vb_error("Error: you haven't defined any grid variables! Aborting")
                 raise ValueError
 
             #
             self._generate_grid_code(dry_run=False)
 
             #
             self._load_grid_function()
 
         # then if the _system_generator is present, we go through it
-        if self.grid_options["_system_generator"]:
+        if self.population_options["_system_generator"]:
             # Check if there is an output dir configured
             if self.custom_options.get("data_dir", None):
                 binary_c_calls_output_dir = self.custom_options["data_dir"]
                 # otherwise check if there's one passed to the function
             else:
                 if not output_dir:
-                    print(
+                    self.vb_error(
                         "Error. No data_dir configured and you gave no output_dir. Aborting"
                     )
                     raise ValueError
                 binary_c_calls_output_dir = output_dir
 
             # check if there's a filename passed to the function
             if output_filename:
@@ -469,52 +471,54 @@
                 # otherwise use default value
             else:
                 binary_c_calls_filename = "binary_c_calls.txt"
 
             binary_c_calls_full_filename = os.path.join(
                 binary_c_calls_output_dir, binary_c_calls_filename
             )
-            print("Writing binary_c calls to {}".format(binary_c_calls_full_filename))
+            self.vb_info(
+                "Writing binary_c calls to {}".format(binary_c_calls_full_filename)
+            )
 
             # Write to file
             with self.open(
                 binary_c_calls_full_filename, "w", encoding=encoding
             ) as file:
                 # Get defaults and clean them, then overwrite them with the set values.
                 if include_defaults:
                     # TODO: make sure that the defaults here are cleaned up properly
                     cleaned_up_defaults = self.cleaned_up_defaults
                     full_system_dict = cleaned_up_defaults.copy()
                     full_system_dict.update(self.bse_options.copy())
                 else:
                     full_system_dict = self.bse_options.copy()
 
-                for system in self.grid_options["_system_generator"](self):
+                for system in self.population_options["_system_generator"](self):
                     # update values with current system values
                     full_system_dict.update(system)
 
                     binary_cmdline_string = self._return_argline(full_system_dict)
                     file.write(binary_cmdline_string + "\n")
         else:
-            print("Error. No grid function found!")
+            self.vb_error("Error. No grid function found!")
             raise ValueError
 
         return binary_c_calls_full_filename
 
     def set_status(self, string, format_statment="process_{}.txt", ID=None):
         """
         Function to set the status string in its appropriate file
         """
 
         if ID is None:
             ID = self.process_ID
 
-        if self.grid_options["status_dir"]:
+        if self.population_options["status_dir"]:
             path = os.path.join(
-                self.grid_options["status_dir"],
+                self.population_options["status_dir"],
                 format_statment.format(ID),
             )
             with self.open(path, "w", encoding="utf-8") as f:
                 f.write(string)
                 f.close()
                 self.NFS_flush_hack(path)
 
@@ -583,97 +587,84 @@
 
         Returns:
             (file_object, lock_object) tuple.
             If the file was not opened, returns (None,None).
         """
 
         if exists_ok is False and os.path.isfile(filename):
-            if vb:
-                print("File at {} already exists: cannot write to it".format(filename))
+            self.vb_warning(
+                "File at {} already exists: cannot write to it".format(filename)
+            )
             return (None, None)
 
         # set the lockfile path: this should be the same
         # for all processes, so it's just the original file
         # plus the lock_suffix
         lockfilename = filename + lock_suffix
-        if vb:
-            print("lockfile={}".format(lockfilename))
+        self.vb_info("lockfile={}".format(lockfilename))
 
         while True:
             # if the file exists, just return
             if os.path.isfile(lockfilename):
-                if vb:
-                    print(
-                        "lockfile at {} already exists (corresponding to file at {})".format(
-                            lockfilename, filename
-                        )
+                self.vb_warning(
+                    "lockfile at {} already exists (corresponding to file at {})".format(
+                        lockfilename, filename
                     )
+                )
                 return (None, None)
 
             # make the lock object by opening the lockfile
             lock = flufl.lock.Lock(lockfilename, default_timeout=lock_timeout)
-            if vb:
-                print("post-lock: {}".format(lock))
+            self.vb_info("post-lock: {}".format(lock))
 
             if lock:
                 # we have the lockfile, so set the lifetime and try to lock it
                 lock.lifetime = datetime.timedelta(seconds=lock_lifetime)
                 try:
-                    if vb:
-                        print("try to lock {}".format(lock))
+                    self.vb_info("try to lock {}".format(lock))
                     lock.lock()
-                    if vb:
-                        if lock.is_locked:
-                            print("locked {}".format(lock))
-                        else:
-                            print("failed to lock {}".format(lock))
+                    if lock.is_locked:
+                        self.vb_info("locked {}".format(lock))
+                    else:
+                        self.vb_info("failed to lock {}".format(lock))
                 except:
                     pass
 
                 # if we acquired the lock, try to open the file
                 if lock.is_locked:
-                    if vb:
-                        print(
-                            "{} is locked by {} to {}".format(
-                                filename, lock, lockfilename
-                            )
-                        )
+                    self.vb_info(
+                        "{} is locked by {} to {}".format(filename, lock, lockfilename)
+                    )
 
                     if exists_ok is False and os.path.isfile(filename):
-                        if vb:
-                            print(
-                                "File at {} already exists (2): cannot write to it, unlocking and returning (None,None)".format(
-                                    filename
-                                )
+                        self.vb_warning(
+                            "File at {} already exists (2): cannot write to it, unlocking and returning (None,None)".format(
+                                filename
                             )
+                        )
                         lock.unlock()
                         return (None, None)
 
                     # All is apparently ok: file is locked
                     try:
-                        if vb:
-                            print("Try to open file at {}".format(filename))
+                        self.vb_info("Try to open file at {}".format(filename))
                         f = self.open(filename, mode="w", encoding=encoding, **kwargs)
-                        if vb:
-                            print("Return locked file {}, {}".format(f, lock))
+                        self.vb_info("Return locked file {}, {}".format(f, lock))
                         return (f, lock)
 
                     # error on open should be fatal
                     except Exception as e:
-                        print("Error in locked_open_for_write() : {}".format(e))
+                        self.vb_error("Error in locked_open_for_write() : {}".format(e))
                         if fatal_open_errors:
-                            if vb:
-                                print("fatal exit on open")
+                            self.vb_error("fatal exit on open")
                             self.exit(1)
                         else:
-                            if vb:
-                                print("unlock {}".format(lock))
+                            self.vb_info("unlock {}".format(lock))
                             lock.unlock()
-                            if vb:
-                                print("unlocked {} return None,None".format(lock))
+                            self.vb_info("unlocked {} return None,None".format(lock))
                             return (None, None)
 
             # failed to lock this time, keep trying
             # (we shouldn't lock up the CPU because the timeout is non-zero)
             continue
 
     def NFS_flush_hack(self, filename):
@@ -719,40 +710,37 @@
         """
         Wrapper for open() with automatic compression based on the file extension.
         """
 
         if compression is None:
             compression = self.compression_type(file)
 
-        if vb:
-            print(
-                'open() file at "{file}" with mode = {mode}, compression {compression}, compresslevel {compresslevel}'.format(
-                    file=file,
-                    compression=compression,
-                    compresslevel=compresslevel,
-                    mode=mode,
-                )
+        self.vb_info(
+            'open() file at "{file}" with mode = {mode}, compression {compression}, compresslevel {compresslevel}'.format(
+                file=file,
+                compression=compression,
+                compresslevel=compresslevel,
+                mode=mode,
             )
+        )
 
         if compression:
             if compresslevel is None:
                 compresslevel = 9
             if "b" not in mode:
                 # if we don't specify binary-mode, the gzip module
                 # defaults to binary, which isn't compatible with JSON,
                 # so default to text if not specified otherwise
                 mode += "t"
-                if vb:
-                    print("open() adding text mode")
+                self.vb_debug("open() adding text mode")
             else:
                 encoding = None
                 errors = None
                 newline = None
-                if vb:
-                    print("open() setting encoding=errors=newline=None")
+                self.vb_debug("open() setting encoding=errors=newline=None")
             if compression == "bzip2":
                 file_object = bz2.open(
                     file,
                     mode=mode,
                     compresslevel=compresslevel,
                     encoding=encoding,
                     errors=errors,
@@ -775,16 +763,15 @@
                 encoding=encoding,
                 errors=errors,
                 newline=newline,
                 closefd=closefd,
                 opener=opener,
             )
 
-        if vb:
-            print("open() return file_object =", file_object)
+        self.vb_debug("open() return file_object = {}".format(file_object))
         return file_object
 
     def NFSpath(self, path):
         """
         Test path to see if it's on an NFS mount.
 
         Args:
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/distribution_functions.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/distribution_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 from typing import Union
 
 import cachetools
 import numpy as np
 import py_rinterpolate
 
 from binarycpython.utils.dicts import normalize_dict, prepare_dict
-from binarycpython.utils.functions import verbose_print
-from binarycpython.utils.population_extensions.grid_options_defaults import (
+from binarycpython.utils.population_extensions.population_options_defaults import (
     _MOE2017_VERBOSITY_INTERPOLATOR_LEVEL,
     _MOE2017_VERBOSITY_LEVEL,
 )
 from binarycpython.utils.useful_funcs import calc_period_from_sep, calc_sep_from_period
 
 # Global dictinary to store values in
 Moecache = {}
@@ -125,19 +124,14 @@
             k: power law slope
 
         Returns:
             constant to normalise the given power law between the min_val and max_val range
         """
 
         k1 = k + 1.0
-        # print(
-        #     "Powerlaw consts from {} to {}, k={} where k1={}".format(
-        #         min_val, max_val, k, k1
-        #     )
-        # )
 
         powerlaw_const = k1 / (max_val**k1 - min_val**k1)
         return powerlaw_const
 
     @cachetools.cachedmethod(
         lambda self: self.caches[
             "population_extensions._distribution_functions.powerlaw_constant"
@@ -160,19 +154,14 @@
             k: power law slope
 
         Returns:
             constant to normalise the given power law between the min_val and max_val range
         """
 
         k1 = k + 1.0
-        # print(
-        #     "Powerlaw consts from {} to {}, k={} where k1={}".format(
-        #         min_val, max_val, k, k1
-        #     )
-        # )
 
         powerlaw_const = k1 / (max_val**k1 - min_val**k1)
         return powerlaw_const
 
     def powerlaw(
         self,
         min_val: Union[int, float],
@@ -195,15 +184,15 @@
 
         # Handle faulty value
         if k == -1:
             msg = "wrong value for k"
             raise ValueError(msg)
 
         if (x < min_val) or (x > max_val):
-            print("input value is out of bounds!")
+            self.vb_debug("input value is out of bounds!")
             return 0
 
         powerlaw_const = self.powerlaw_constant(min_val, max_val, k)
 
         # power law
         prob = powerlaw_const * (x**k)
         return prob
@@ -586,110 +575,114 @@
     def _get_multiplicity_dict(self, system_dict):
         """
         Function to get the multiplicity dict according to a prescription choice
         TODO: combine with the M&S multiplicity function: this function can be used to get the multiplicity dict, and then that function wraps this one.
         """
 
         # Just return 1 if no option has been chosen
-        if self.grid_options["multiplicity_fraction_function"] in [0, "None"]:
+        if self.population_options["multiplicity_fraction_function"] in [0, "None"]:
 
             # Raise an error if the multiplicity is not set
             if not system_dict.get("multiplicity", None):
                 msg = "Multiplicity value has not been set. When not using a specific multiplicity fraction function please set the multiplicity"
                 raise ValueError(msg)
 
-            verbose_print(
+            self.vb_debug(
                 "_calculate_multiplicity_fraction: Chosen not to use any multiplicity fraction.",
-                self.grid_options["verbosity"],
-                3,
             )
 
             multiplicity_fraction_dict = {
                 1: 0,
                 2: 0,
                 3: 0,
                 4: 0,
             }
             multiplicity_fraction_dict[system_dict["multiplicity"]] = 1
 
         # Go over the chosen options
-        elif self.grid_options["multiplicity_fraction_function"] in [1, "Arenou2010"]:
+        elif self.population_options["multiplicity_fraction_function"] in [
+            1,
+            "Arenou2010",
+        ]:
             # Arenou 2010 will be used
-            verbose_print(
+            self.vb_debug(
                 "_calculate_multiplicity_fraction: Using Arenou 2010 to calculate multiplicity fractions",
-                self.grid_options["verbosity"],
-                3,
             )
 
             binary_fraction = self.Arenou2010_binary_fraction(system_dict["M_1"])
             multiplicity_fraction_dict = {
                 1: 1 - binary_fraction,
                 2: binary_fraction,
                 3: 0,
                 4: 0,
             }
 
-        elif self.grid_options["multiplicity_fraction_function"] in [2, "Raghavan2010"]:
+        elif self.population_options["multiplicity_fraction_function"] in [
+            2,
+            "Raghavan2010",
+        ]:
             # Raghavan 2010 will be used
-            verbose_print(
+            self.vb_debug(
                 "_calculate_multiplicity_fraction: Using Raghavan (2010) to calculate multiplicity fractions",
-                self.grid_options["verbosity"],
-                3,
             )
 
             binary_fraction = self.raghavan2010_binary_fraction(system_dict["M_1"])
             multiplicity_fraction_dict = {
                 1: 1 - binary_fraction,
                 2: binary_fraction,
                 3: 0,
                 4: 0,
             }
 
-        elif self.grid_options["multiplicity_fraction_function"] in [3, "Moe2017"]:
+        elif self.population_options["multiplicity_fraction_function"] in [
+            3,
+            "Moe2017",
+        ]:
             # We need to check several things now here:
 
             # First, are the options for the MOE2017 grid set? On start it is filled with the default settings
-            if not self.grid_options["Moe2017_options"]:
+            if not self.population_options["Moe2017_options"]:
                 msg = "The MOE2017 options do not seem to be set properly. The value is {}".format(
-                    self.grid_options["Moe2017_options"]
+                    self.population_options["Moe2017_options"]
                 )
                 raise ValueError(msg)
 
             # Second: is the Moecache filled.
             if not Moecache:
-                verbose_print(
+                self.vb_debug(
                     "_calculate_multiplicity_fraction: Moecache is empty. It needs to be filled with the data for the interpolators. Loading the data now",
-                    self.grid_options["verbosity"],
-                    3,
                 )
 
                 # Load the data
                 self._load_moe_di_stefano_data()
 
             # record the prev value
-            prev_M1_value_ms = self.grid_options["Moe2017_options"].get("M_1", None)
+            prev_M1_value_ms = self.population_options["Moe2017_options"].get(
+                "M_1", None
+            )
 
             # Set value of M1 of the current system
-            self.grid_options["Moe2017_options"]["M_1"] = system_dict["M_1"]
+            self.population_options["Moe2017_options"]["M_1"] = system_dict["M_1"]
 
             # Calculate the multiplicity fraction
             multiplicity_fraction_list = (
                 self.Moe_di_Stefano_2017_multiplicity_fractions(
-                    self.grid_options["Moe2017_options"], self.grid_options["verbosity"]
+                    self.population_options["Moe2017_options"],
+                    self.population_options["verbosity"],
                 )
             )
 
             # Turn into dict
             multiplicity_fraction_dict = {
                 el + 1: multiplicity_fraction_list[el]
                 for el in range(len(multiplicity_fraction_list))
             }
 
             # Set the prev value back
-            self.grid_options["Moe2017_options"]["M_1"] = prev_M1_value_ms
+            self.population_options["Moe2017_options"]["M_1"] = prev_M1_value_ms
 
         # we don't know what to do next
         else:
             msg = "Chosen value for the multiplicity fraction function is not known."
             raise ValueError(msg)
 
         # To make sure we normalize the dictionary
@@ -709,38 +702,32 @@
             The multiplicity fractions of the quadruples are folded onto that of the triples
         """
 
         if max_multiplicity not in range(1, 5):
             msg = "\tMoe and di Stefano 2017: merge_multiplicities: max_multiplicity has to be between 1 and 4. It is {} now".format(
                 max_multiplicity
             )
-            verbose_print(
+            self.vb_debug(
                 msg,
-                verbosity,
-                0,
             )
             raise ValueError(msg)
 
         # Fold multiplicities:
-        verbose_print(
+        self.vb_debug(
             "\tMoe and di Stefano 2017: merge_multiplicities: Merging multiplicities with initial array {} and max multiplicity {}".format(
                 result_array, max_multiplicity
             ),
-            verbosity,
-            _MOE2017_VERBOSITY_LEVEL,
         )
         for i in range(max_multiplicity, len(result_array))[::-1]:
             result_array[i - 1] += result_array[i]
             result_array[i] = 0
-        verbose_print(
+        self.vb_debug(
             "\tMoe and di Stefano 2017: merge_multiplicities: Merging multiplicities to new array {}".format(
                 result_array
             ),
-            verbosity,
-            _MOE2017_VERBOSITY_LEVEL,
         )
 
         return result_array
 
     def Arenou2010_binary_fraction(self, m: Union[int, float]) -> Union[int, float]:
         """
         Arenou 2010 function for the binary fraction as f(M1)
@@ -806,18 +793,16 @@
         )  # Modulator array
 
         # Check for length
         if len(multiplicity_modulator_array) != 4:
             msg = "Multiplicity modulator has to have 4 elements. Now it is {}, len: {}".format(
                 multiplicity_modulator_array, len(multiplicity_modulator_array)
             )
-            verbose_print(
+            self.vb_error(
                 msg,
-                verbosity,
-                0,
             )
             raise ValueError(msg)
 
         # Set up some arrays
         full_fractions_array = np.zeros(4)  # Meant to contain the real fractions
         weighted_fractions_array = np.zeros(
             4
@@ -847,20 +832,18 @@
             # Fill the multiplicity array
             for n in range(4):
                 full_fractions_array[n] = self.poisson(multiplicity, n, 3)
 
             # Normalize it so it fills to one when taking all the multiplicities:
             full_fractions_array = full_fractions_array / np.sum(full_fractions_array)
 
-            verbose_print(
+            self.vb_info(
                 "\tMoe and di Stefano 2017: Moe_di_Stefano_2017_multiplicity_fractions: using model {}: full_fractions_array: {}".format(
                     "Poisson", full_fractions_array
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
         elif options["multiplicity_model"] == "data":
             # use the fractions calculated from Moe's data directly
             #
             # note that in this case, there are no quadruples: these
             # are combined with triples
@@ -869,75 +852,65 @@
             for n in range(3):
                 full_fractions_array[n] = Moecache[
                     "rinterpolator_multiplicity"
                 ].interpolate([np.log10(options["M_1"])])[n + 1]
 
             # Set last value
             full_fractions_array[3] = 0.0  # no quadruples
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: Moe_di_Stefano_2017_multiplicity_fractions: using model {}: full_fractions_array: {}".format(
                     "data", full_fractions_array
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
         # Normalisation:
         if options["normalize_multiplicities"] == "raw":
             # Don't multiply by the multiplicity_array, but do give a fractions array
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: Moe_di_Stefano_2017_multiplicity_fractions: Not normalising (using raw results): results: {}".format(
                     full_fractions_array
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
             result = full_fractions_array
 
         elif options["normalize_multiplicities"] == "norm":
             # Multiply the full_multiplicity_fraction array by the multiplicity_multiplier_array, creating a weighted fractions array
             weighted_fractions_array = (
                 full_fractions_array * multiplicity_modulator_array
             )
 
             # Normalise this so it is in total 1:
             result = weighted_fractions_array / np.sum(weighted_fractions_array)
 
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: Moe_di_Stefano_2017_multiplicity_fractions: Normalising with {}. result: {}".format(
                     "norm", result
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
         elif options["normalize_multiplicities"] == "merge":
             # We first take the full multiplicity array
             # (i.e. not multiplied by multiplier) and do the merging
             result = self.merge_multiplicities(
                 full_fractions_array, max_multiplicity, verbosity=verbosity
             )
 
             # Then normalise to be sure
             result = result / np.sum(result)
 
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: Moe_di_Stefano_2017_multiplicity_fractions: Normalising with {}, max_multiplicity={} result={}".format(
                     "merge", max_multiplicity, result
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
-        verbose_print(
+        self.vb_debug(
             "\tMoe and di Stefano 2017: Moe_di_Stefano_2017_multiplicity_fractions: {}".format(
                 str(result)
             ),
-            verbosity,
-            _MOE2017_VERBOSITY_LEVEL,
         )
 
         # return array reference
         return result
 
     ########################################################################
     # Period distributions
@@ -1258,61 +1231,53 @@
                 Moecache["rinterpolator_q_metadata"].get(p, None)
             ):
                 if (Moecache["rinterpolator_q_metadata"][m] == options[m]) and (
                     Moecache["rinterpolator_q_metadata"][p] == options[p]
                 ):
                     incache = True
 
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe and di Stefano 2017: build_q_table: Found cached values for m={} p={}".format(
                             options[m], options[p]
                         ),
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
                 else:
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe and di Stefano 2017: build_q_table: Cached values for different m={} p={}. Freeing current table and making new table".format(
                             options[m], options[p]
                         ),
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
 
         #
         if not incache:
             # trim and/or expand the table to the range qmin to qmax.
 
             # qmin is set by the minimum stellar mass
             qmin = options["Mmin"] / options["M_1"]
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: build_q_table qmin: {}".format(
                     qmin,
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
             # qmax = maximum_mass_ratio_for_RLOF(options[m], options[p])
             # TODO: change this to the above
             qmax = 1
 
             # qdata contains the table that we modify: we get
             # the original data by interpolating Moe's table
             qdata = {}
             can_renormalize = 1
 
             qeps = 1e-8  # small number but such that qeps+1 != 1
             if qeps + 1 == 1.0:
-                verbose_print(
+                self.vb_debug(
                     "\tMoe and di Stefano 2017: build_q_table: qeps (= {}) +1 == 1. Make qeps larger".format(
                         qeps,
                     ),
-                    verbosity,
-                    _MOE2017_VERBOSITY_LEVEL,
                 )
 
             if qmin >= qmax:
                 # there may be NO binaries in this part of the parameter space:
                 # in which case, set up a table with lots of zero in it
 
                 qdata = {0: 0, 1: 0}
@@ -1414,105 +1379,89 @@
                             [0, 1] if pre == "low" else [len(qs) - 1, len(qs) - 2]
                         )  # Based on whether we do the high or low end we need to use two different indices
                         method = options.get(
                             "q_{}_extrapolation_method".format(pre), None
                         )
                         qlimit = qmin if pre == "low" else qmax
 
-                        verbose_print(
+                        self.vb_debug(
                             "\tMoe and di Stefano 2017: build_q_table: Extrapolating: Q: {} method: {}, indices: {} End index: {}".format(
                                 pre, method, indices, end_index
                             ),
-                            verbosity,
-                            _MOE2017_VERBOSITY_LEVEL,
                         )
 
                         # truncate the distribution
                         qdata[max(0.0, min(1.0, qlimit + sign * qeps))] = 0
 
                         if method is None:
                             # no extrapolation : just interpolate between 0.10 and 0.95
-                            verbose_print(
+                            self.vb_debug(
                                 "\tMoe and di Stefano 2017: build_q_table: using no extrapolations",
-                                verbosity,
-                                _MOE2017_VERBOSITY_LEVEL,
                             )
                             continue
                         if method == "flat":
                             # use the end value and extrapolate it
                             # with zero slope
                             qdata[qlimit] = qdata[qs[end_index]]
-                            verbose_print(
+                            self.vb_debug(
                                 "\tMoe and di Stefano 2017: build_q_table: using constant extrapolation",
-                                verbosity,
-                                _MOE2017_VERBOSITY_LEVEL,
                             )
                         elif method == "linear":
                             qdata[qlimit] = self.linear_extrapolation_q(
                                 qs=qs,
                                 indices=indices,
                                 qlimit=qlimit,
                                 qdata=qdata,
                                 end_index=end_index,
                                 verbosity=verbosity,
                             )
 
-                            verbose_print(
+                            self.vb_debug(
                                 "\tMoe and di Stefano 2017: build_q_table: using linear extrapolation",
-                                verbosity,
-                                _MOE2017_VERBOSITY_LEVEL,
                             )
                             if pre == "low":
                                 below_qlimit = qlimit - qeps
                                 if below_qlimit > 0:
                                     qdata[below_qlimit] = 0
                                 qdata[0] = 0
-                                verbose_print(
+                                self.vb_debug(
                                     "\tMoe and di Stefano 2017: build_q_table: using linear extrapolation and setting the points below the lower q bound ({}) to 0 ".format(
                                         qlimit
                                     ),
-                                    verbosity,
-                                    _MOE2017_VERBOSITY_LEVEL,
                                 )
 
                         elif method == "plaw2":
                             qdata[qlimit] = self.powerlaw_extrapolation_q(
                                 qs=qs,
                                 indices=indices,
                                 qdata=qdata,
                                 verbosity=verbosity,
                             )
 
-                            verbose_print(
+                            self.vb_debug(
                                 "\tMoe and di Stefano 2017: build_q_table: using powerlaw extrapolation",
-                                verbosity,
-                                _MOE2017_VERBOSITY_LEVEL,
                             )
                         elif method == "nolowq":
                             newq = 0.05
                             qdata[newq] = 0
-                            verbose_print(
+                            self.vb_debug(
                                 "\tMoe and di Stefano 2017: build_q_table: setting lowq to 0",
-                                verbosity,
-                                _MOE2017_VERBOSITY_LEVEL,
                             )
                         elif method == "poly":
                             # TODO: consider implementing the poly method (see Perl version)
                             raise ValueError(
                                 "Moe and di Stefano 2017: build_q_table: Method 'poly' not implemented"
                             )
 
                         else:
                             msg = "\tMoe and di Stefano 2017: build_q_table: Error no other methods available. The chosen method ({}) does not exist!".format(
                                 method
                             )
-                            verbose_print(
+                            self.vb_debug(
                                 msg,
-                                verbosity,
-                                _MOE2017_VERBOSITY_LEVEL,
                             )
                             raise ValueError(msg)
 
             # regenerate qs in new table. This is now the updated list of qs where we have some extrapolated numbers
             tmp_table = []
             for q in sorted(qdata.keys()):
                 tmp_table.append([q, qdata[q]])
@@ -1520,60 +1469,65 @@
             # Make an interpolation table to contain our modified data
             q_interpolator = py_rinterpolate.Rinterpolate(
                 table=tmp_table,
                 nparams=1,
                 ndata=1,  # Contains the table of data  # q  #
                 verbosity=verbosity - (_MOE2017_VERBOSITY_INTERPOLATOR_LEVEL - 1),
             )
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: build_q_table: Created a new Q table",
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
             if can_renormalize:
-                verbose_print(
+                self.vb_debug(
                     "\tMoe and di Stefano 2017: build_q_table: Renormalising table",
-                    verbosity,
-                    _MOE2017_VERBOSITY_LEVEL,
                 )
 
                 # now we integrate and renormalise (if the table is not all zero)
                 integration_constant_q = self.get_integration_constant_q(
                     q_interpolator, tmp_table, qdata, verbosity=verbosity
                 )
 
+                self.vb_debug(
+                    "\tMoe and di Stefano 2017: build_q_table: using integration_constant_q: {}".format(
+                        integration_constant_q
+                    ),
+                )
+
                 if integration_constant_q > 0:
                     # normalise to 1.0 by dividing the data by 1.0/$I
                     q_interpolator.multiply_table_column(
                         1, 1.0 / integration_constant_q
                     )
 
                     # test this
                     new_integration_constant_q = self.get_integration_constant_q(
                         q_interpolator, tmp_table, qdata, verbosity=verbosity
                     )
 
+                    self.vb_debug(
+                        "\tMoe and di Stefano 2017: build_q_table: using new_integration_constant_q: {}".format(
+                            new_integration_constant_q
+                        ),
+                    )
+
                     # fail if error in integral > 1e-6 (should be ~ machine precision)
                     if abs(1.0 - new_integration_constant_q) > 1e-6:
-                        verbose_print(
+                        self.vb_debug(
                             "\tMoe and di Stefano 2017: build_q_table: Error: > 1e-6 in q probability integral: {}".format(
                                 integration_constant_q
                             ),
-                            verbosity,
-                            _MOE2017_VERBOSITY_LEVEL,
                         )
+
             # set this new table in the cache
             Moecache["rinterpolator_q_given_{}_log10{}".format(m, p)] = q_interpolator
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: build_q_table: stored q_interpolater as {}".format(
                     "rinterpolator_q_given_{}_log10{}".format(m, p)
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
             # Store the values for which this table was set up in the dict
             if not Moecache.get("rinterpolator_q_metadata", None):
                 Moecache["rinterpolator_q_metadata"] = {}
             Moecache["rinterpolator_q_metadata"][m] = options[m]
             Moecache["rinterpolator_q_metadata"][p] = options[p]
@@ -1606,32 +1560,30 @@
         Function to do the linear extrapolation for q.
         """
 
         # linear extrapolation
         dq = qs[indices[1]] - qs[indices[0]]
 
         if dq == 0:
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: build_q_table: linear dq=0",
                 verbosity,
                 _MOE2017_VERBOSITY_LEVEL,
             )
             # No change
             return qs[end_index]
 
         slope = (qdata[qs[indices[1]]] - qdata[qs[indices[0]]]) / dq
 
         intercept = qdata[qs[indices[0]]] - slope * qs[indices[0]]
         qdata[qlimit] = max(0.0, slope * qlimit + intercept)
-        verbose_print(
+        self.vb_debug(
             "\tMoe and di Stefano 2017: build_q_table: linear Slope: {} intercept: {} dn/dq({}) = {}".format(
                 slope, intercept, qlimit, qdata[qlimit]
             ),
-            verbosity,
-            _MOE2017_VERBOSITY_LEVEL,
         )
 
         return max(0.0, slope * qlimit + intercept)
 
     def get_integration_constant_q(self, q_interpolator, tmp_table, qdata, verbosity=0):
         """
         Function to integrate the q interpolator and return the integration constant
@@ -1645,22 +1597,21 @@
         for q in np.arange(0, 1 + 2e-6, dq):
             x = q_interpolator.interpolate([q])
 
             if len(x) == 0:
                 msg = "\tMoe and di Stefano 2017: get_integration_constant_q: Q interpolator table interpolation failed.\n\t\ttmp_table = {}\n\t\tq_data = {}".format(
                     str(tmp_table), str(qdata)
                 )
-                verbose_print(
+                self.vb_debug(
                     msg,
-                    verbosity,
-                    _MOE2017_VERBOSITY_LEVEL,
                 )
                 raise ValueError(msg)
 
             integration_constant_q += x[0] * dq
+
         return integration_constant_q
 
     def fill_data(self, sample_values, data_dict):
         """
         Function that returns the normalised array of values for given logmass and logperiod
         used for the e and q values
 
@@ -1728,44 +1679,40 @@
                     ]
                 )[0]
 
                 integation_constant_e += dp_decc * decc
 
             # Set the integral value in the dict
             Moecache[integrals_string][mass_period_string] = integation_constant_e
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: calc_ecc_integral: min_ecc: {} max ecc: {} integrals_string: {} interpolator_name: {} mass_string: {} period_string: {} mass: {} period: {} I: {}".format(
                     min_ecc,
                     max_ecc,
                     integrals_string,
                     interpolator_name,
                     mass_string,
                     period_string,
                     options[mass_string],
                     options[period_string],
                     integation_constant_e,
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
         else:
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: calc_ecc_integral: Found cached value for min_ecc: {} max ecc: {} integrals_string: {} interpolator_name: {} mass_string: {} period_string: {} mass: {} period: {} I: {}".format(
                     min_ecc,
                     max_ecc,
                     integrals_string,
                     interpolator_name,
                     mass_string,
                     period_string,
                     options[mass_string],
                     options[period_string],
                     Moecache[integrals_string][mass_period_string],
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
     def calc_P_integral(
         self,
         options,
         min_logP,
         max_logP,
@@ -1797,38 +1744,34 @@
                     [np.log10(options[mass_string]), logP]
                 )[0]
 
                 integation_constant_P += dp_dlogP * dlogP
 
             # Set the integral value in the dict
             Moecache[integrals_string][options[mass_string]] = integation_constant_P
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: calc_P_integral: min_logP: {} integrals_string: {} interpolator_name: {} mass_string: {} mass: {} I: {}".format(
                     min_logP,
                     integrals_string,
                     interpolator_name,
                     mass_string,
                     options[mass_string],
                     integation_constant_P,
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
         else:
-            verbose_print(
+            self.vb_debug(
                 "\tMoe and di Stefano 2017: calc_P_integral: Found cached value for min_logP: {} integrals_string: {} interpolator_name: {} mass_string: {} mass: {} I: {}".format(
                     min_logP,
                     integrals_string,
                     interpolator_name,
                     mass_string,
                     options[mass_string],
                     Moecache[integrals_string][options[mass_string]],
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
 
     def calc_total_probdens(self, prob_dict):
         """
         Function to calculate the total probability density
         """
 
@@ -1849,88 +1792,96 @@
         P, P2, P3 => periods (days) [number: none=binary, 2=triple, 3=quadruple]
         ecc, ecc2, ecc3 => eccentricities [numbering as for P above]
 
         mmin => minimum allowed stellar mass (default 0.07)
         mmax => maximum allowed stellar mass (default 80.0)
         """
 
-        verbose_print(
+        self.vb_debug(
             "\tMoe_di_Stefano_2017_pdf with options:\n\t\t{}".format(
                 json.dumps(options, ensure_ascii=False)
             ),
-            verbosity,
-            _MOE2017_VERBOSITY_LEVEL,
         )
 
         prob_dict = (
             {}
         )  # Dictionary containing all the pdf values for the different parameters
 
         # Get the multiplicity from the options, and if its not there, calculate it based on the
         # TODO: the function below makes no sense. We NEED to pass the multiplicity in the
         if not options.get("multiplicity", None):
             msg = "\tMoe_di_Stefano_2017_pdf: Did not find a multiplicity value in the options dictionary"
-            verbose_print(
+            self.vb_debug(
                 msg,
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
             raise ValueError(msg)
 
         multiplicity = options["multiplicity"]
 
         # Immediately return 0 if the multiplicity modulator is 0
         if options["multiplicity_modulator"][int(multiplicity) - 1] == 0:
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017_pdf: returning 0 because of the multiplicity modulator being 0",
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
             return 0
 
         ############################################################
         # multiplicity fraction
         # Calculate the probability, or rather, fraction, of stars that belong to this mass
 
         multiplicity_probability = self.Moe_di_Stefano_2017_multiplicity_fractions(
             options, verbosity
         )[int(multiplicity) - 1]
         prob_dict["multiplicity"] = multiplicity_probability
-        verbose_print(
+        self.vb_debug(
             "\tMoe_di_Stefano_2017_pdf: Appended multiplicity (mass1 = {}) probability ({}) to the prob dict ({})".format(
                 options["M_1"], prob_dict["multiplicity"], prob_dict
             ),
-            verbosity,
-            _MOE2017_VERBOSITY_LEVEL,
         )
 
-        ############################################################
-        # always require an IMF for the primary star
+        #################
+        # Calculate the M1_probability
+        #   we use an IMF distribution function to calculate this probability
         #
         # NB multiply by M1 to convert dN/dM to dN/dlnM
         # (dlnM = dM/M, so 1/dlnM = M/dM)
 
-        # TODO: Create an n-part-powerlaw method that can have breakpoints and slopes. I'm using a three-part power law now.
-        # TODO: is this actually the correct way? putting the M1 in there? Do we sample in log space?
-        M1_probability = self.Kroupa2001(options["M_1"]) * options["M_1"]
+        # Store M_1 value temporarily
+        options["M_1_temp"] = options["M_1"]
+
+        # Handle choice for IMF
+        if options["IMF_distribution"] == "kroupa2001":
+            M1_probability = (
+                self.Kroupa2001(
+                    options["M_1"], newopts={"mmax": options["ranges"]["M"][-1] + 1e-4}
+                )
+                * options["M_1"]
+            )
+        elif options["IMF_distribution"] == "chabrier2003":
+            M1_probability = self.imf_chabrier2003(options["M_1"]) * options["M_1"]
+        else:
+            raise ValueError(
+                "IMF_distribution choice ({}) for Moe & diStefano 2017 distributions not supported.".format(
+                    options["IMF_distribution"]
+                )
+            )
+
+        # Set and return if zero
         prob_dict["M_1"] = M1_probability
-        verbose_print(
+        self.vb_debug(
             "\tMoe_di_Stefano_2017_pdf: Appended Mass (m={}) probability ({}) to the prob dict ({})".format(
                 options["M_1"], prob_dict["M_1"], prob_dict
             ),
-            verbosity,
-            _MOE2017_VERBOSITY_LEVEL,
         )
         # if M1_probability == 0: # If the probability is 0 then we don't have to calculate more
         #     calc_total_probdens(prob_dict)
         #     return prob_dict
 
-        """
-        From here we go through the multiplicities.
-        """
+        #################
+        # From here we go through the multiplicities.
         if multiplicity >= 2:
             # If the multiplicity is higher than 1, we will need to construct the following tables:
             # - period distribution table
             # - q distribution table
             # - eccentricity distribution table
 
             # Set up the interpolator for the periods
@@ -1939,20 +1890,18 @@
                     table=Moecache[
                         "period_distributions"
                     ],  # Contains the table of data
                     nparams=2,  # log10M, log10P
                     ndata=2,  # binary, triple
                     verbosity=verbosity - (_MOE2017_VERBOSITY_INTERPOLATOR_LEVEL - 1),
                 )
-                verbose_print(
+                self.vb_debug(
                     "\tMoe_di_Stefano_2017_pdf: Created new period interpolator: {}".format(
                         Moecache["rinterpolator_log10P"]
                     ),
-                    verbosity,
-                    _MOE2017_VERBOSITY_LEVEL,
                 )
 
             # Make a table storing Moe's data for q distributions
             if (
                 options.get("M_2", None)
                 or options.get("M_3", None)
                 or options.get("M_4", None)
@@ -1961,20 +1910,18 @@
                     Moecache["rinterpolator_q"] = py_rinterpolate.Rinterpolate(
                         table=Moecache["q_distributions"],  # Contains the table of data
                         nparams=3,  # log10M, log10P, q
                         ndata=1,  #
                         verbosity=verbosity
                         - (_MOE2017_VERBOSITY_INTERPOLATOR_LEVEL - 1),
                     )
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe_di_Stefano_2017_pdf: Created new q interpolator: {}".format(
                             Moecache["rinterpolator_q"]
                         ),
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
 
             # Make a table storing Moe's data for q distributions, but only if the ecc is actually sampled
             if "ecc" in options:
                 if not options["ecc"] is None:
                     if not Moecache.get("rinterpolator_e", None):
                         Moecache["rinterpolator_e"] = py_rinterpolate.Rinterpolate(
@@ -1982,20 +1929,18 @@
                                 "ecc_distributions"
                             ],  # Contains the table of data
                             nparams=3,  # log10M, log10P, e
                             ndata=1,  #
                             verbosity=verbosity
                             - (_MOE2017_VERBOSITY_INTERPOLATOR_LEVEL - 1),
                         )
-                        verbose_print(
+                        self.vb_debug(
                             "\tMoe_di_Stefano_2017_pdf: Created new e interpolator: {}".format(
                                 Moecache["rinterpolator_e"]
                             ),
-                            verbosity,
-                            _MOE2017_VERBOSITY_LEVEL,
                         )
 
             ###############
             # Calculation for period of the binary
 
             if options.get("M_2", None):
                 # Separation of the inner binary
@@ -2025,20 +1970,18 @@
 
             # Set probabilty for P1
             p_val = Moecache["rinterpolator_log10P"].interpolate(
                 [np.log10(options["M_1"]), np.log10(options["P"])]
             )[0]
             p_val = p_val / Moecache["P_integrals"][options["M_1"]]
             prob_dict["P"] = p_val
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017_pdf: Appended period (m={}, P={}) probability ({}) to the prob list ({})".format(
                     options["M_1"], options["P"], prob_dict["P"], prob_dict
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
             # if prob_dict['P'] == 0: # If the probability is 0 then we don't have to calculate more
             #     calc_total_probdens(prob_dict)
             #     return prob_dict
 
             ############################################################
             # mass ratio (0 < q = M2/M1 < qmax)
@@ -2051,41 +1994,37 @@
                 primary_mass = options["M_1"]
                 secondary_mass = options["M_2"]
                 m_label = "M_1"
                 p_label = "P"
 
                 # Construct the q table
                 self.build_q_table(options, m_label, p_label, verbosity=verbosity)
-                verbose_print(
+                self.vb_debug(
                     "\tMoe_di_Stefano_2017_pdf: Created q_table ({}) for m={} p={}".format(
                         Moecache[
                             "rinterpolator_q_given_{}_log10{}".format(m_label, p_label)
                         ],
                         options[m_label],
                         options[p_label],
                     ),
-                    verbosity,
-                    _MOE2017_VERBOSITY_LEVEL,
                 )
 
                 # Add probability for the mass ratio
                 q_prob = Moecache[
                     "rinterpolator_q_given_{}_log10{}".format(m_label, p_label)
                 ].interpolate([secondary_mass / primary_mass])[0]
                 prob_dict["q"] = q_prob
-                verbose_print(
+                self.vb_debug(
                     "\tMoe_di_Stefano_2017_pdf: appended mass ratio (M={} P={} q={}) probability ({}) to the prob list ({}) ".format(
                         options["M_1"],
                         options["P"],
                         options["M_2"] / options["M_1"],
                         prob_dict["q"],
                         prob_dict,
                     ),
-                    verbosity,
-                    _MOE2017_VERBOSITY_LEVEL,
                 )
                 # if prob_dict['q'] == 0: # If the probability is 0 then we don't have to calculate more
                 #     calc_total_probdens(prob_dict)
                 #     return prob_dict
 
             ############################################################
             # Eccentricity
@@ -2111,24 +2050,22 @@
                             np.log10(options["M_1"]),
                             np.log10(options["P"]),
                             options["ecc"],
                         ]
                     )[0]
                     ecc_val = ecc_val / Moecache["ecc_integrals"][mass_period_string]
                     prob_dict["ecc"] = ecc_val
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe_di_Stefano_2017_pdf: Appended eccentricity (m={}, P={}, ecc={}) probability ({}) to the prob list ({})".format(
                             options["M_1"],
                             options["P"],
                             options["ecc"],
                             prob_dict["ecc"],
                             prob_dict,
                         ),
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
                     # if prob_dict['ecc'] == 0: # If the probability is 0 then we don't have to calculate more
                     #     calc_total_probdens(prob_dict)
                     #     return prob_dict
 
             # Calculations for when multiplicity is bigger than 3
             # BEWARE: binary_c does not evolve these systems actually and the code below should be revised for when binary_c actually evolves triples.
@@ -2154,20 +2091,18 @@
                 # max_logP2 = 10.0
                 # min_logP = Moecache['logperiods'][0]
                 max_logP2 = float(Moecache["logperiods"][-1])
 
                 if options["P2"] < min_P2:
                     # period is too short : system is not hierarchical
                     prob_dict["P2"] = 0
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe_di_Stefano_2017_pdf: period2 is too short: {} < {}, system is not hierarchical. Added 0 to probability list".format(
                             options["P1"], min_P2
                         ),
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
                     # if prob_dict['P2'] == 0: # If the probability is 0 then we don't have to calculate more
                     #     calc_total_probdens(prob_dict)
                     #     return prob_dict
 
                 else:
                     # period is long enough that the system is hierarchical
@@ -2190,24 +2125,22 @@
 
                     # Add the probability
                     p_val = Moecache["rinterpolator_log10P"].interpolate(
                         [np.log10(options["M_1+M_2"]), np.log10(options["P2"])]
                     )[0]
                     p_val = p_val / Moecache["P2_integrals"][options["M_1+M_2"]]
                     prob_dict["P2"] = p_val
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe_di_Stefano_2017_pdf: Appended period2 (m1={} m2={}, P2={}) probability ({}) to the prob list ({})".format(
                             options["M_1"],
                             options["M_2"],
                             options["P2"],
                             prob_dict["P2"],
                             prob_dict,
                         ),
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
                     # if prob_dict['P2'] == 0: # If the probability is 0 then we don't have to calculate more
                     #     calc_total_probdens(prob_dict)
                     #     return prob_dict
 
                     ############################################################
                     # mass ratio 2 = q2 = M3 / (M1+M2)
@@ -2219,36 +2152,32 @@
                     primary_mass = options["M_1+M_2"]
                     secondary_mass = options["M_3"]
                     m_label = "M_1+M_2"
                     p_label = "P2"
 
                     # Build q table
                     self.build_q_table(options, m_label, p_label, verbosity=verbosity)
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe_di_Stefano_2017_pdf: Called build_q_table",
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
 
                     # Add the probability
                     q2_val = Moecache[
                         "rinterpolator_q_given_{}_log10{}".format(m_label, p_label)
                     ].interpolate([secondary_mass / primary_mass])[0]
                     prob_dict["q2"] = q2_val
-                    verbose_print(
+                    self.vb_debug(
                         "\tMoe_di_Stefano_2017_pdf: appended mass ratio (M_1+M_2={} M_3={} P={} q={}) probability ({}) to the prob list ({}) ".format(
                             options["M_1+M_2"],
                             options["M_3"],
                             options["P"],
                             secondary_mass / primary_mass,
                             prob_dict["q2"],
                             prob_dict,
                         ),
-                        verbosity,
-                        _MOE2017_VERBOSITY_LEVEL,
                     )
                     # if prob_dict['q2'] == 0: # If the probability is 0 then we don't have to calculate more
                     #     calc_total_probdens(prob_dict)
                     #     return prob_dict
 
                     # TODO: Implement ecc2 calculation
                     if multiplicity == 4:
@@ -2282,24 +2211,22 @@
 
                         # Set probability
                         p_val = Moecache["rinterpolator_log10P"].interpolate(
                             [np.log10(options["M_1+M_2"]), np.log10(options["P2"])]
                         )[0]
                         p_val = p_val / Moecache["P2_integrals"][options["M_1+M_2"]]
                         prob_dict["P3"] = p_val
-                        verbose_print(
+                        self.vb_debug(
                             "\tMoe_di_Stefano_2017_pdf: Appended period2 (M=4) (M_1={} M_2={}, P2={}) probability ({}) to the prob list ({})".format(
                                 options["M_1"],
                                 options["M_2"],
                                 options["P2"],
                                 prob_dict["P3"],
                                 prob_dict,
                             ),
-                            verbosity,
-                            _MOE2017_VERBOSITY_LEVEL,
                         )
                         # if prob_dict['P3'] == 0: # If the probability is 0 then we don't have to calculate more
                         #     calc_total_probdens(prob_dict)
                         #     return prob_dict
 
                         ############################################################
                         # mass ratio 2
@@ -2314,107 +2241,95 @@
                         m_label = "M_1+M_2"
                         p_label = "P2"
 
                         # Calculate new q table
                         self.build_q_table(
                             options, m_label, p_label, verbosity=verbosity
                         )
-                        verbose_print(
+                        self.vb_debug(
                             "\tMoe_di_Stefano_2017_pdf: Created q_table ",
-                            verbosity,
-                            _MOE2017_VERBOSITY_LEVEL,
                         )
 
                         # Add the probability
                         q3_prob = Moecache[
                             "rinterpolator_q_given_{}_log10{}".format(m_label, p_label)
                         ].interpolate([secondary_mass / primary_mass])[0]
                         prob_dict["q3"] = q3_prob
-                        verbose_print(
+                        self.vb_debug(
                             "\tMoe_di_Stefano_2017_pdf: appended mass ratio (M_1+M_2={} M_3={} P={} q={}) probability ({}) to the prob list ({}) ".format(
                                 options["M_1+M_2"],
                                 options["M_3"],
                                 options["P"],
                                 secondary_mass / primary_mass,
                                 prob_dict["q3"],
                                 prob_dict,
                             ),
-                            verbosity,
-                            _MOE2017_VERBOSITY_LEVEL,
                         )
                         # if prob_dict['q3'] == 0: # If the probability is 0 then we don't have to calculate more
                         #     calc_total_probdens(prob_dict)
                         #     return prob_dict
 
                         # TODO: ecc 3
 
         # check for input of multiplicity
         elif multiplicity not in range(1, 5):
             msg = "\tMoe_di_Stefano_2017_pdf: Unknown multiplicity {}".format(
                 multiplicity
             )
-            verbose_print(
+            self.vb_debug(
                 msg,
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
             raise ValueError(msg)
 
         # Calculate total probdens:
         prob_dict = self.calc_total_probdens(prob_dict)
 
         # Some info
         if multiplicity == 1:
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017_pdf: M_1={} q=N/A log10P=N/A ({}): {} -> {}\n".format(
                     options["M_1"],
                     len(prob_dict),
                     str(prob_dict),
                     prob_dict["total_probdens"],
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
         elif multiplicity == 2:
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017_pdf: M_1={} q={} log10P={} ecc={} ({}): {} -> {}\n".format(
                     options["M_1"],
                     options["M_2"] / options["M_1"]
                     if options.get("M_2", None)
                     else "N/A",
                     np.log10(options["P"]),
                     options["ecc"] if options.get("ecc", None) else "N/A",
                     len(prob_dict),
                     str(prob_dict),
                     prob_dict["total_probdens"],
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
         elif multiplicity == 3:
-            verbose_print(
+            self.vb_debug(
                 "\tMoe_di_Stefano_2017_pdf: M_1={} q={} log10P={} ecc={} M_3={} log10P2={} ecc2={} ({}): {} -> {}".format(
                     options["M_1"],
                     options["M_2"] / options["M_1"]
                     if options.get("M_2", None)
                     else "N/A",
                     np.log10(options["P"]),
                     options["ecc"] if options.get("ecc", None) else "N/A",
                     options["M_3"],
                     np.log10(options["P2"]),
                     options["ecc2"] if options.get("ecc2", None) else "N/A",
                     len(prob_dict),
                     str(prob_dict),
                     prob_dict["total_probdens"],
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
         elif multiplicity == 4:
-            verbose_print(
+            self.vb_debug(
                 "Moe_di_Stefano_2017_pdf: M_1={} q={} log10P={} ecc={} M_3={} log10P2={} ecc2={} M_4={} log10P3={} ecc3={} ({}) : {} -> {}".format(
                     options["M_1"],
                     options["M_2"] / options["M_1"]
                     if options.get("M_2", None)
                     else "N/A",
                     np.log10(options["P"]),
                     options["ecc"] if options.get("ecc", None) else "N/A",
@@ -2424,11 +2339,13 @@
                     options["M_4"],
                     np.log10(options["P3"]),
                     options["ecc3"] if options.get("ecc3", None) else "N/A",
                     len(prob_dict),
                     str(prob_dict),
                     prob_dict["total_probdens"],
                 ),
-                verbosity,
-                _MOE2017_VERBOSITY_LEVEL,
             )
+
+        # restore temp M-1 value
+        options["M_1"] = options["M_1_temp"]
+
         return prob_dict
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/evolution_functions.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/evolution_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import json
 import multiprocessing
 
 # pylint: disable=E1101
 import os
 import queue
 import signal
-import sys
 import time
 from collections import OrderedDict
 from typing import Any
 
 import setproctitle
 
 from binarycpython import _binary_c_bindings
@@ -62,103 +61,92 @@
         if self._setup() is False:
             return
 
         ############################################################
         # Evolve systems
         self.set_time("start")
         if (
-            self.grid_options["evolution_type"]
-            in self.grid_options["_evolution_type_options"]
+            self.population_options["evolution_type"]
+            in self.population_options["_evolution_type_options"]
         ):
-            if self.grid_options["evolution_type"] in [
-                "grid",
-                "custom_generator",
-                "monte_carlo",
-            ]:
-                if self._evolve_population_core() is False:
-                    return False
+            if self._evolve_population_core() is False:
+                return False
         else:
-            print(
-                "Warning. you chose a wrong option for the grid evolution types.\
+            msg = "Warning. you chose a wrong option ({}) for the grid evolution types.\
                 Please choose from the following: {}.".format(
-                    self.grid_options["_evolution_type_options"]
-                )
+                self.population_options["evolution_type"],
+                self.population_options["_evolution_type_options"],
             )
-            raise ValueError()
+            self.vb_warning(msg)
+            raise ValueError(msg)
         self.set_time("end")
 
         ############################################################
         # Log and print some information
         string1 = "Population-{} finished!\nThe total probability is {:g}.".format(
-            self.grid_options["_population_id"], self.grid_options["_probtot"]
+            self.population_options["_population_id"],
+            self.population_options["_probtot"],
         )
         string2 = "It took a total of {dtsecs} to run {starcount} systems on {ncores} cores\n = {CPUtime} of CPU time.\nMaximum memory use {memuse:.3f} MB".format(
-            dtsecs=timedelta(self.grid_options["_time_elapsed"]),
-            starcount=self.grid_options[
+            dtsecs=timedelta(self.population_options["_time_elapsed"]),
+            starcount=self.population_options[
                 "_count"
             ],  # not _total_count! we may have ended the run early...
-            ncores=self.grid_options["num_processes"],
+            ncores=self.population_options["_num_processes"],
             CPUtime=timedelta(self.CPU_time()),
             memuse=sum(self.shared_memory["max_memory_use_per_thread"]),
         )
 
         ############################################################
         # add warning about a grid that was killed
         ############################################################
         if self.was_killed():
             string2 += "\n>>> Grid was killed <<<"
             self.set_status("killed")
 
-        self.verbose_print(
-            self._boxed(string1, string2), self.grid_options["verbosity"], 0
-        )
+        self.vb_critical("\n" + self._boxed(string1, string2))
 
         ############################################################
         # handle errors
         ############################################################
-        if self.grid_options["_errors_found"]:
+        if self.population_options["_errors_found"]:
             # Some information afterwards
-            self.verbose_print(
-                self._boxed(
+            self.vb_critical(
+                "\n"
+                + self._boxed(
                     "During the run {} failed systems were found\nwith a total probability of {:g}\nwith the following unique error codes: {} ".format(
-                        self.grid_options["_failed_count"],
-                        self.grid_options["_failed_prob"],
-                        self.grid_options["_failed_systems_error_codes"],
+                        self.population_options["_failed_count"],
+                        self.population_options["_failed_prob"],
+                        self.population_options["_failed_systems_error_codes"],
                     )
                 ),
-                self.grid_options["verbosity"],
-                0,
             )
             # Some information on where we logged the systems
             if (
-                self.grid_options["log_failed_systems"]
-                and self.grid_options["log_failed_systems_dir"] is not None
+                self.population_options["log_failed_systems"]
+                and self.population_options["log_failed_systems_dir"] is not None
             ):
 
-                self.verbose_print(
-                    "The full failed arglines have been written to {self.grid_options['log_failed_systems_dir']}/process_{self.jobID()}.txt",
-                    self.grid_options["verbosity"],
-                    0,
+                self.vb_critical(
+                    "The full failed arglines have been written to {self.population_options['log_failed_systems_dir']}/process_{self.jobID()}.txt",
                 )
         else:
-            self.verbose_print(
+            self.vb_critical(
                 "No failed systems were found in this run.",
-                self.grid_options["verbosity"],
-                0,
             )
 
         return True
 
     def _evolve_population_core(self):
         """
         Function that handles running the population using multiprocessing.
 
         First we set up the multiprocessing manager and the job and result queue.
 
-        Then we spawn <self.grid_options["num_processes"]> number of process instances,
+        Then we spawn <self.population_options["_num_processes"]> number of process instances,
         and signal them to start.
 
         While the processes are waiting for their instructions, we start the queue filler,
         which goes over the grid code and puts all the tasks in a queue until its full.
 
         The processes take these jobs, evolve the and store results.
 
@@ -175,35 +163,39 @@
         # Set process name
         setproctitle.setproctitle("binarycpython parent process")
 
         # if max_queue_size is zero, calculate automatically
         # to be double the number of processes - you don't want to
         # make the queue too large because when it's killed you
         # want to end quickly
-        if self.grid_options["max_queue_size"] == 0:
-            self.grid_options["max_queue_size"] = 2 * self.grid_options["num_processes"]
+        if self.population_options["max_queue_size"] == 0:
+            self.population_options["max_queue_size"] = (
+                2 * self.population_options["_num_processes"]
+            )
 
         ############
         # Set up the manager object and queues
         manager = multiprocessing.Manager()
-        job_queue = manager.Queue(maxsize=self.grid_options["max_queue_size"])
-        result_queue = manager.Queue(maxsize=self.grid_options["max_queue_size"])
-        final_result_queue = manager.Queue(maxsize=self.grid_options["num_processes"])
+        job_queue = manager.Queue(maxsize=self.population_options["max_queue_size"])
+        result_queue = manager.Queue(maxsize=self.population_options["max_queue_size"])
+        final_result_queue = manager.Queue(
+            maxsize=self.population_options["_num_processes"]
+        )
 
         ############
         # data to be sent to signal handlers
         signal_data = {
             "where": "_evolve_population_core",
             "queue": job_queue,
         }
 
         ############
         # Create process instances to run the stars
         processes = []
-        for ID in range(self.grid_options["num_processes"]):
+        for ID in range(self.population_options["_num_processes"]):
             processes.append(
                 multiprocessing.Process(
                     target=self._process_queue,
                     args=(job_queue, result_queue, final_result_queue, ID),
                 )
             )
 
@@ -220,54 +212,54 @@
             signal.SIGTERM, functools.partial(self._parent_signal_handler, signal_data)
         )
         signal.signal(
             signal.SIGINT, functools.partial(self._parent_signal_handler, signal_data)
         )
 
         # Set up the system_queue in the parent process
-        self.grid_options["_job_crashed"] = False
+        self.population_options["_job_crashed"] = False
         self._system_queue_handler(
             job_queue,
             result_queue,
             processes,
-            num_processes=self.grid_options["num_processes"],
+            num_processes=self.population_options["_num_processes"],
         )
 
         ############
         # Handle killing of processes or join and clean up
-        if self.grid_options["_job_crashed"] is True:
+        if self.population_options["_job_crashed"] is True:
             # job crashed while in system_queue_filler : kill children
             # and return False
-            print(
+            self.vb_critical(
                 "A child process crashed or was killed : I will not join incomplete data"
             )
             self._kill_child_processes(processes)
             return False
 
         else:
             # Join the processes after the queue filler has finished
-            print("Do join of subprocesses ...")
+            self.vb_info("Do join of subprocesses ...")
 
-            while self.grid_options["_job_crashed"] is False and processes:
+            while self.population_options["_job_crashed"] is False and processes:
                 if self._all_children_running(processes) is False:
                     # job crashed: stop children and return False
-                    self.grid_options["_job_crashed"] = True
+                    self.population_options["_job_crashed"] = True
                 else:
                     # join first process: it should finish work soon
                     p = processes.pop(0)
                     p.join()
 
-            if self.grid_options["_job_crashed"] is True:
-                print(
+            if self.population_options["_job_crashed"] is True:
+                self.vb_critical(
                     "A child process crashed or was killed : I will not join incomplete data"
                 )
                 self._kill_child_processes(processes)
                 return False
             else:
-                print("Joined all subprocesses.")
+                self.vb_info("Joined all subprocesses.")
 
         ############
         # Handle the results by merging all the dictionaries. How that merging happens exactly is
         # described in the merge_dicts description.
         #
         # If there is a preloaded_population, we add this first,
         # then we add the populations run just now
@@ -276,28 +268,30 @@
         # use preloaded population's data as a basis
         # for our combined_output_dict
         if self.preloaded_population:
             combined_output_dict = {
                 "ensemble_results": keys_to_floats(
                     self.preloaded_population.grid_ensemble_results
                 ),
-                "results": keys_to_floats(self.preloaded_population.grid_results),
+                "results": keys_to_floats(self.preloaded_population.population_results),
             }
 
             for x in self._metadata_keylist():
                 try:
-                    combined_output_dict[x] = self.preloaded_population.grid_options[x]
+                    combined_output_dict[
+                        x
+                    ] = self.preloaded_population.population_options[x]
                 except Exception as e:
-                    print(
+                    self.vb_error(
                         "Tried to set combined_output_dict key",
                         x,
                         "from preloaded_popuation, but this failed:",
                         e,
                     )
-            print(
+            self.vb_info(
                 "Pre-loaded data from {} stars".format(combined_output_dict["_count"])
             )
 
             # do not propagate _killed
             # combined_output_dict['results']['_killed'] = False
             # combined_output_dict['_killed'] = False
 
@@ -334,75 +328,94 @@
                 "ensemble"
             ] = format_ensemble_results(
                 combined_output_dict["ensemble_results"].get("ensemble", {})
             )
         gc.collect()
 
         # Put the values back as object properties
-        self.grid_results = combined_output_dict["results"]
+        self.population_results = combined_output_dict["results"]
 
         #################################
         # Put Ensemble results
         self.grid_ensemble_results = combined_output_dict[
             "ensemble_results"
         ]  # Ensemble results are also passed as output from that dictionary
 
         # Add metadata
         self.add_ensemble_metadata(combined_output_dict)
 
         # if we were killed, save snapshot
-        if self.grid_options["save_snapshots"] and self.grid_options["_killed"]:
-            self.custom_options["save_snapshot"] = True
+        if (
+            self.population_options["save_snapshots"]
+            and self.population_options["_killed"]
+        ):
+            self.population_options["save_snapshot"] = True
 
         # return True because all seems well
         return True
 
     def _evolve_system_mp(self, system_number, full_system_dict):
         """
         Function that the multiprocessing evolution method calls to evolve a system
 
         this function is called by _process_queue
         """
 
+        # Set up cmdline string and store current parameter dict in the custom options
         binary_cmdline_string = self._return_argline(full_system_dict)
+        self.custom_options["parameter_dict"] = full_system_dict
 
+        # Get persistent memory adress for ensemble output
         persistent_data_memaddr = -1
         if self.bse_options.get("ensemble", 0) == 1:
             persistent_data_memaddr = self.persistent_data_memory_dict[self.process_ID]
-            # print("thread {}: persistent_data_memaddr: ".format(self.process_ID), persistent_data_memaddr)
 
         # vb2 logging
-        if self.grid_options["verbosity"] >= 2:
+        if self.population_options["verbosity"] >= 2:
             self.vb2print(full_system_dict, binary_cmdline_string)
 
         # Get results binary_c
-        # print("running: {}".format(binary_cmdline_string))
         out = _binary_c_bindings.run_system(
             argstring=binary_cmdline_string,
-            custom_logging_func_memaddr=self.grid_options[
+            custom_logging_func_memaddr=self.population_options[
                 "custom_logging_func_memaddr"
             ],
-            store_memaddr=self.grid_options["_store_memaddr"],
+            store_memaddr=self.population_options["_store_memaddr"],
             population=1,  # since this system is part of a population, we set this flag to prevent the store from being freed
             persistent_data_memaddr=persistent_data_memaddr,
         )
 
         # Check for errors
         _ = self._check_binary_c_error(system_number, out, full_system_dict)
 
-        # Have some user-defined function do stuff with the data.
-        if self.grid_options["parse_function"]:
-            self.custom_options["parameter_dict"] = full_system_dict
-            system_result = self.grid_options["parse_function"](self, out)
+        # Check event logging parsing
+        if self.population_options["event_based_logging_handle_output"]:
+            self.population_options["event_based_logging_output_parser"](
+                self,
+                events_parameters_list_dict=self.population_options[
+                    "event_based_logging_parameter_list_dict"
+                ],
+                output_dir=self.population_options[
+                    "event_based_logging_output_directory"
+                ],
+                output=out,
+                separator=self.population_options[
+                    "event_based_logging_output_separator"
+                ],
+            )
+
+        # Pass output of binary_c to a user-defined parsing function
+        if self.population_options["parse_function"]:
+            system_result = self.population_options["parse_function"](self, out)
 
             return system_result
 
     def evolve_single(self, clean_up_custom_logging_files: bool = True) -> Any:
         """
-        Function to run a single system, based on the settings in the grid_options
+        Function to run a single system, based on the settings in the population_options
 
         The output of the run gets returned, unless a parse function is given to this function.
 
         Args:
             clean_up_custom_logging_files: whether the clean up all the custom_logging files.
 
         returns:
@@ -417,186 +430,181 @@
         # Handle single system evolution
 
         # Check if there are actually arguments passed:
         if self.bse_options:
             # Get argument line
             argline = self._return_argline(self.bse_options)
 
-            self.verbose_print(
-                "Running {}".format(argline), self.grid_options["verbosity"], 1
-            )
+            self.vb_info("Running {}".format(argline))
 
             # Run system
             out = _binary_c_bindings.run_system(
                 argstring=argline,
-                custom_logging_func_memaddr=self.grid_options[
+                custom_logging_func_memaddr=self.population_options[
                     "custom_logging_func_memaddr"
                 ],
-                store_memaddr=self.grid_options["_store_memaddr"],
+                store_memaddr=self.population_options["_store_memaddr"],
                 population=0,
             )
 
             # Clean up custom logging
             if clean_up_custom_logging_files:
                 self._clean_up_custom_logging(evol_type="single")
 
             # Parse output and return the result
-            if self.grid_options["parse_function"]:
-                return self.grid_options["parse_function"](self, out)
+            if self.population_options["parse_function"]:
+                return self.population_options["parse_function"](self, out)
 
             # Otherwise just return the raw output
             return out
 
         # Raise error if no evolution options are passed
         msg = "No actual evolution options passed to the evolve call. Aborting"
         raise ValueError(msg)
 
     ###################
     # queue and worker functions
-
     def _system_queue_handler(self, job_queue, result_queue, processes, num_processes):
         """
         Function that is responsible for keeping the queue filled.
 
         This will generate the systems until it is full, and then keeps trying to fill it.
         Will have to play with the size of this.
 
         This function is called as part of the parent process.
         """
 
         #######
         # Set up logging
-        stream_logger = self._get_stream_logger()
-        if self.grid_options["verbosity"] >= self._LOGGER_VERBOSITY_LEVEL:
-            stream_logger.debug("setting up the system_queue_filler now")
+        if self.population_options["verbosity"] >= self._LOGGER_VERBOSITY_LEVEL:
+            self.vb_error("setting up the system_queue_filler now")
 
         #######
         # Start up the generator
         generator = self._get_generator()
 
         #######
         # Start and handle start_at value
 
         # start_at can be an expression : we should eval it
         # prior to running the loop
-        self.grid_options["start_at"] = eval(str(self.grid_options["start_at"]))
-        if self.grid_options["start_at"] > 0:
-            print("Starting at model {} ".format(self.grid_options["start_at"]))
+        self.population_options["start_at"] = eval(
+            str(self.population_options["start_at"])
+        )
+        if self.population_options["start_at"] > 0:
+            self.vb_info(
+                "Starting at model {} ".format(self.population_options["start_at"])
+            )
 
         prev_process_check = None
 
         #######
         # Continuously fill the queue while we are allowed to.
         #   The loop terminates when:
         #       - the generator is exhausted
         #       - a signal to stop the queue is passed
-        #       - TODO: mass threshold met when monte_carlo sampling
         #       - TODO: custom threshold (e.g. type of system)
         for system_number, system_dict in enumerate(generator):
             # on stop, quit this loop
-            if self.grid_options["stop_queue"]:
+            if self.population_options["stop_queue"]:
                 break
 
             ########
             # Handle start_at and modulo
 
             # skip systems before start_at
-            elif system_number < self.grid_options["start_at"]:
-                self.verbose_print(
+            elif system_number < self.population_options["start_at"]:
+                self.vb_info(
                     "skip system {n} because < start_at = {start}".format(
-                        n=system_number, start=self.grid_options["start_at"]
+                        n=system_number, start=self.population_options["start_at"]
                     ),
-                    self.grid_options["verbosity"],
-                    3,
                 )
                 continue
 
             # apply modulo
             if not (
-                (system_number - self.grid_options["start_at"])
-                % self.grid_options["modulo"]
+                (system_number - self.population_options["start_at"])
+                % self.population_options["modulo"]
                 == 0
             ):
-                self.verbose_print(
+                self.vb_info(
                     "skip system {n} because modulo {mod} == {donemod}".format(
                         n=system_number,
-                        mod=self.grid_options["modulo"],
-                        donemod=(system_number - self.grid_options["start_at"])
-                        % self.grid_options["modulo"],
+                        mod=self.population_options["modulo"],
+                        donemod=(system_number - self.population_options["start_at"])
+                        % self.population_options["modulo"],
                     ),
-                    self.grid_options["verbosity"],
-                    3,
                 )
 
                 continue
 
             ######
             # check children are running every 1s
             # TODO: allow frequency change?
             _now = time.time()
             if prev_process_check is None or _now - prev_process_check > 1:
                 prev_process_check = _now
                 if self._all_children_running(processes) is False:
-                    self.grid_options["_job_crashed"] = True
+                    self.population_options["_job_crashed"] = True
                     return
 
             ######
             # Handle monte-carlo threshold based on evolved mass
-            elif self.grid_options["evolution_type"] == "monte_carlo":
+            elif self.population_options["evolution_type"] == "monte_carlo":
                 # Check based on mass threshold
                 self._monte_carlo_sampling_check_mass_threshold(system_dict)
 
+                # Check based on count threshold
+                self._monte_carlo_sampling_check_count_threshold()
+
                 # Check based on custom threshold, which uses the result_queue
-                # TODO: process the result_queue and pass this. How we do this (get only one, or get until the result queue is empty again)
                 self._monte_carlo_sampling_check_custom_threshold(result_queue)
 
             ######
             # Check if evolution threshold is reached.
-            #   this can be set in the _monte_carlo_sampling_check_mass_threshold function or via _monte_carlo_sampling_check_custom_threshold
-            if self.grid_options["_monte_carlo_threshold_reached"]:
-                self.verbose_print(
+            #   this can be set in the _monte_carlo_sampling_check_mass_threshold function,
+            #   the _monte_carlo_sampling_check_count_threshold function,
+            #   or via _monte_carlo_sampling_check_custom_threshold
+            if self.population_options["_monte_carlo_threshold_reached"]:
+                self.vb_warning(
                     "Monte-Carlo threshold reached. Signaling to stop processing the queue{}",
-                    self.grid_options["verbosity"],
-                    2,
                 )
 
                 # Queue is done:
-                self.grid_options["_queue_done"] = True
+                self.population_options["_queue_done"] = True
 
             ########
             # Put system in the job queue
             try:
                 job_queue.put((system_number, system_dict), block=True)
             except Exception:
                 # error on queueing : stop the queue
-                self.grid_options["stop_queue"] = True
+                self.population_options["stop_queue"] = True
 
             # Print some info
-            self.verbose_print(
+            self.vb_info(
                 "Queue produced system {}".format(system_number),
-                self.grid_options["verbosity"],
-                3,
             )
 
             ########
             # Handle stopping
-            if self.grid_options["_queue_done"]:
+            if self.population_options["_queue_done"]:
                 break
 
         # Signal queue is done
-        self.grid_options["_queue_done"] = True
+        self.population_options["_queue_done"] = True
 
         #######
         # Send closing signal to workers. When they receive this they will terminate
-        if True:  # not self.grid_options['stop_queue']:
+        if True:  # not self.population_options['stop_queue']:
             for _ in range(num_processes):
                 job_queue.put("STOP")
 
-        if self.grid_options["verbosity"] >= self._LOGGER_VERBOSITY_LEVEL:
-            stream_logger.debug("Signalling processes to stop")  # DEBUG
+        #
+        self.vb_critical("Signalling processes to stop")  # DEBUG
 
     def _process_queue(self, job_queue, result_queue, final_result_queue, ID):
         """
         Worker process that gets items from the job_queue and runs those systems.
         It keeps track of several things like failed systems, total time spent on systems etc.
 
         Input:
@@ -651,74 +659,68 @@
         total_time_calling_binary_c = 0
         total_mass_run = 0
         total_probability_weighted_mass_run = 0
 
         # variables for the statu bar prints
         start_grid_time = time.time()
         next_log_time = (
-            self.shared_memory["prev_log_time"][0] + self.grid_options["log_dt"]
+            self.shared_memory["prev_log_time"][0] + self.population_options["log_dt"]
         )
-        next_mem_update_time = start_grid_time + self.grid_options["log_dt"]
+        next_mem_update_time = start_grid_time + self.population_options["log_dt"]
 
         # Load store memory adress: TODO: this might be prohibitive if we run with MINT
-        self.grid_options["_store_memaddr"] = _binary_c_bindings.return_store_memaddr()
+        self.population_options[
+            "_store_memaddr"
+        ] = _binary_c_bindings.return_store_memaddr()
 
         # Set the ensemble memory address
         if self.bse_options.get("ensemble", 0) == 1:
             # set persistent data memory address if necessary.
             persistent_data_memaddr = (
                 _binary_c_bindings.return_persistent_data_memaddr()
             )
 
             self.persistent_data_memory_dict = {
                 self.process_ID: persistent_data_memaddr
             }
 
-            self.verbose_print(
+            self.vb_info(
                 "\tUsing persistent_data memaddr: {}".format(persistent_data_memaddr),
-                self.grid_options["verbosity"],
-                3,
             )
 
         #########
         # Log the starting of the process
+        self.vb_info(
+            f"Setting up processor: process-{self.process_ID}",
+        )
 
-        # Set up stream logger for the worker processes
-        stream_logger = self._get_stream_logger()
-        if self.grid_options["verbosity"] >= self._LOGGER_VERBOSITY_LEVEL:
-            stream_logger.debug(f"Setting up processor: process-{self.process_ID}")
-
-        self.verbose_print(
+        self.vb_info(
             "Process {} started at {}.\tUsing store memaddr {}".format(
                 ID,
                 now(),
-                self.grid_options["_store_memaddr"],
-            ),
-            self.grid_options["verbosity"],
-            3,
+                self.population_options["_store_memaddr"],
+            )
         )
 
         # Set status to running
         self.set_status("running")
 
         ############################################################
         # Run stellar systems in the queue
         ############################################################
         for system_number, system_dict in iter(job_queue.get, "STOP"):
-
-            if False:
-                print(
-                    "Child: Job Queue system_number = {}, dict={}, n={} check {}".format(
-                        system_number,
-                        system_dict,
-                        number_of_systems_run,
-                        self.grid_options["stop_queue"],
-                    )
+            #
+            self.vb_debug(
+                "Child: Job Queue system_number = {}, dict={}, n={} check {}".format(
+                    system_number,
+                    system_dict,
+                    number_of_systems_run,
+                    self.population_options["stop_queue"],
                 )
-                sys.stdout.flush()
+            )
 
             #########
             # Create full system dict and perform check
             full_system_dict = self.bse_options.copy()
             full_system_dict.update(system_dict)
 
             # Check if all keys are known to binary_c.
@@ -732,129 +734,141 @@
             # save the current time (used often)
             time_now = time.time()
 
             # update memory use stats every log_dt seconds (not every time, this is likely a bit expensive)
             if time_now > next_mem_update_time:
                 m = mem_use()
                 self.shared_memory["memory_use_per_thread"][ID] = m
-                next_mem_update_time = time_now + self.grid_options["log_dt"]
+                next_mem_update_time = time_now + self.population_options["log_dt"]
                 if m > self.shared_memory["max_memory_use_per_thread"][ID]:
                     self.shared_memory["max_memory_use_per_thread"][ID] = m
 
             # calculate the next logging time
             next_log_time = (
-                self.shared_memory["prev_log_time"][0] + self.grid_options["log_dt"]
+                self.shared_memory["prev_log_time"][0]
+                + self.population_options["log_dt"]
             )
 
             # Check if we need to log info again
             # TODO: Check if we can put this functionality elsewhere
             if time_now > next_log_time:
                 # we have exceeded the next log time : output and update timers
                 # Lock the threads. TODO: Do we need to release this?
                 lock = multiprocessing.Lock()  # noqa: F841
 
                 # Do the printing itself
                 self.vb1print(ID, time_now, system_number, system_dict)
 
                 # Set some values for next time
-                next_log_time = time_now + self.grid_options["log_dt"]
-
-                # print("PREV ",self.shared_memory["prev_log_time"])
-                # print("N LOG STATS",self.shared_memory["n_saved_log_stats"].value)
+                next_log_time = time_now + self.population_options["log_dt"]
 
                 # shift the arrays
                 self.shared_memory["prev_log_time"][
-                    -(self.grid_options["n_logging_stats"] - 1) :
+                    -(self.population_options["n_logging_stats"] - 1) :
                 ] = self.shared_memory["prev_log_time"][
-                    : (self.grid_options["n_logging_stats"] - 1)
+                    : (self.population_options["n_logging_stats"] - 1)
                 ]
                 self.shared_memory["prev_log_system_number"][
-                    -(self.grid_options["n_logging_stats"] - 1) :
+                    -(self.population_options["n_logging_stats"] - 1) :
                 ] = self.shared_memory["prev_log_system_number"][
-                    : (self.grid_options["n_logging_stats"] - 1)
+                    : (self.population_options["n_logging_stats"] - 1)
                 ]
 
                 # set the current time and system number
                 self.shared_memory["prev_log_time"][0] = time_now
                 self.shared_memory["prev_log_system_number"][0] = system_number
 
                 # increase the number of stats
                 self.shared_memory["n_saved_log_stats"].value = min(
                     self.shared_memory["n_saved_log_stats"].value + 1,
-                    self.grid_options["n_logging_stats"],
+                    self.population_options["n_logging_stats"],
                 )
 
-                # print("FIRST (0) ",self.shared_memory["prev_log_time"][0])
-                # print("LAST (",self.shared_memory["n_saved_log_stats"].value-1,")",self.shared_memory["prev_log_time"][self.shared_memory["n_saved_log_stats"].value-1])
-
             ###############
             # Log current system info
 
             # In some cases, the whole run crashes. To be able to figure out which system
             # that was on, we log each current system to a file (each thread has one).
             # Each new system overrides the previous
-            if self.grid_options["log_args"]:
+            if self.population_options["log_args"]:
                 argfile = os.path.join(
-                    self.grid_options["log_args_dir"],
+                    self.population_options["log_args_dir"],
                     "process_{}.txt".format(self.jobID()),
                 )
                 with self.open(
                     argfile,
                     "w",
                     encoding="utf-8",
                 ) as f:
                     binary_c_cmdline_string = self._return_argline(full_system_dict)
                     f.write(binary_c_cmdline_string)
                     f.close()
 
+            ###############
+            # pre-evolution hook
+            #   the user can provide a function here that accepts the system dict and
+            #   (potentially) returns (a modified) system dict. Useful for analysis or modifications
+            if self.population_options["pre_evolve_function_hook"]:
+                pre_evolve_hook_res = self.population_options[
+                    "pre_evolve_function_hook"
+                ](self, system_dict)
+                if pre_evolve_hook_res is not None:
+                    system_dict = pre_evolve_hook_res
+
             ##############
             # Running the system
             start_runtime_binary_c = time.time()
 
             # If we want to actually evolve the systems
-            if self.grid_options["_actually_evolve_system"]:
+            if self.population_options["_actually_evolve_system"]:
                 run_system = True
 
                 # Check option to ignore 0 probability systems
-                if not self.grid_options["run_zero_probability_system"]:
+                if not self.population_options["run_zero_probability_system"]:
                     if full_system_dict.get("probability", 1) == 0:
                         run_system = False
                         zero_prob_stars_skipped += 1
 
                 if run_system:
                     # Evolve the system
-                    _ = self._evolve_system_mp(system_number, full_system_dict)
-
-                    # # If we're doing monte-carlo sampling with a custom
-                    # if system_result is not None:
-                    #     # TODO: fix that this is only handle if user-defined function is given
-                    #     # TODO: perhaps we should always put things in the system_result dict if the parse_function gives back something
-                    #     # result_queue.put(
-                    #     #     {
-                    #     #         "system_result": system_result,
-                    #     #         "system_number": system_number,
-                    #     #         "full_system_dict": full_system_dict,
-                    #     #     }
-                    #     # )
+                    system_result = self._evolve_system_mp(
+                        system_number, full_system_dict
+                    )
 
-                    #     raise NotImplementedError("Functionality not implemented")
+                    # If we're doing monte-carlo sampling with a custom threshold function
+                    # NOTE: this will probably change a bit
+                    if system_result is not None:
+                        # Put results into the queue
+                        if (
+                            self.population_options["using_result_queue"]
+                            and self.population_options[
+                                "monte_carlo_custom_threshold_function"
+                            ]
+                        ):
+                            result_queue.put(
+                                {
+                                    "system_result": system_result,
+                                    "system_number": system_number,
+                                    "full_system_dict": full_system_dict,
+                                }
+                            )
 
             end_runtime_binary_c = time.time()
 
             # keep track of total binary_c call time
             total_time_calling_binary_c += end_runtime_binary_c - start_runtime_binary_c
 
             ############
             # Logging runtime
 
             # Debug line: logging all the lines
-            if self.grid_options["log_runtime_systems"] == 1:
+            if self.population_options["log_runtime_systems"] == 1:
                 with self.open(
                     os.path.join(
-                        self.grid_options["tmp_dir"],
+                        self.population_options["tmp_dir"],
                         "runtime_systems",
                         "process_{}.txt".format(self.process_ID),
                     ),
                     "a+",
                     encoding="utf-8",
                 ) as f:
                     binary_cmdline_string = self._return_argline(full_system_dict)
@@ -878,153 +892,148 @@
             # Tally up some numbers
             total_mass_system = calculate_total_mass_system(full_system_dict)
             total_mass_run += total_mass_system
             total_probability_weighted_mass_run += (
                 total_mass_system * full_system_dict.get("probability", 1)
             )
 
-            if self.grid_options["stop_queue"]:
-                print("Child: Stop queue at system {n}".format(n=number_of_systems_run))
+            #####################
+            # Handle termination of the queue
+            if self.population_options["stop_queue"]:
+                self.vb_info(
+                    "Child: Stop queue at system {n}".format(n=number_of_systems_run)
+                )
                 break
 
         ####################
         # Handle stopping of queue
 
-        if self.grid_options["stop_queue"]:
+        if self.population_options["stop_queue"]:
             # any remaining jobs should be ignored
             try:
                 while True:
                     job_queue.get_nowait()
             except queue.Empty:
                 pass
 
         ##########################
         # Clean up and return
 
         # Set status to finishing
         self.set_status("finishing")
-        if self.grid_options["verbosity"] >= self._LOGGER_VERBOSITY_LEVEL:
-            stream_logger.debug(f"Process-{self.process_ID} is finishing.")
+        self.vb_info(f"Process-{self.process_ID} is finishing.")
 
         # free store memory:
-        _binary_c_bindings.free_store_memaddr(self.grid_options["_store_memaddr"])
+        _binary_c_bindings.free_store_memaddr(self.population_options["_store_memaddr"])
 
-        self.verbose_print(
+        self.vb_info(
             "process {} free memory and return ".format(ID),
-            self.grid_options["verbosity"],
-            1,
         )
 
         # Handle ensemble outut
         ensemble_json = self._process_handle_ensemble_output(ID=ID)
 
         # Return a set of results and errors
         output_dict = {
-            "results": self.grid_results,
+            "results": self.population_results,
             "ensemble_results": ensemble_json,
-            "_failed_count": self.grid_options["_failed_count"],
-            "_failed_prob": self.grid_options["_failed_prob"],
-            "_failed_systems_error_codes": self.grid_options[
+            "_failed_count": self.population_options["_failed_count"],
+            "_failed_prob": self.population_options["_failed_prob"],
+            "_failed_systems_error_codes": self.population_options[
                 "_failed_systems_error_codes"
             ],
-            "_errors_exceeded": self.grid_options["_errors_exceeded"],
-            "_errors_found": self.grid_options["_errors_found"],
+            "_errors_exceeded": self.population_options["_errors_exceeded"],
+            "_errors_found": self.population_options["_errors_found"],
             "_probtot": probability_of_systems_run,
             "_count": number_of_systems_run,
             "_total_mass_run": total_mass_run,
             "_total_probability_weighted_mass_run": total_probability_weighted_mass_run,
             "_zero_prob_stars_skipped": zero_prob_stars_skipped,
-            "_killed": self.grid_options["_killed"],
+            "_killed": self.population_options["_killed"],
         }
 
         end_process_time = datetime.datetime.now()
 
         killed = self.was_killed()
 
         # thread end message
         colour = "cyan on black"
-        self.verbose_print(
-            self._boxed(
+        self.vb_critical(
+            "\n"
+            + self._boxed(
                 "{colour}Process {ID} finished:\ngenerator started at {start}\ngenerator finished at {end}\ntotal: {timesecs}\nof which {binary_c_secs} with binary_c\nRan {nsystems} systems\nwith a total probability of {psystems:g}\n{failcolour}This thread had {nfail} failing systems{colour}\n{failcolour}with a total failed probability of {pfail}{colour}\n{zerocolour}Skipped a total of {nzero} zero-probability systems{zeroreset}\n{failednotice}".format(
                     colour=self.ANSI_colours[colour],
                     ID=ID,
                     start=start_process_time.isoformat(),
                     end=end_process_time.isoformat(),
                     timesecs=timedelta(
                         (end_process_time - start_process_time).total_seconds()
                     ),
                     binary_c_secs=timedelta(total_time_calling_binary_c),
                     nsystems=number_of_systems_run,
                     psystems=probability_of_systems_run,
                     failcolour=self.ANSI_colours["red"]
-                    if self.grid_options["_failed_count"] > 0
+                    if self.population_options["_failed_count"] > 0
                     else "",
                     # failreset=self.ANSI_colours[colour]
-                    # if self.grid_options["_failed_count"] > 0
+                    # if self.population_options["_failed_count"] > 0
                     # else "",
-                    nfail=self.grid_options["_failed_count"],
-                    pfail=self.grid_options["_failed_prob"],
+                    nfail=self.population_options["_failed_count"],
+                    pfail=self.population_options["_failed_prob"],
                     nzero=zero_prob_stars_skipped,
                     zerocolour=self.ANSI_colours["yellow"]
                     if zero_prob_stars_skipped > 0
                     else "",
                     zeroreset=self.ANSI_colours[colour]
                     if zero_prob_stars_skipped > 0
                     else "",
                     failednotice=">>> Process was killed <<<\n" if killed else "",
                 ),
                 colour=colour,
             ),
-            self.grid_options["verbosity"],
-            1,
         )
 
         # Write summary
         summary_dict = {
-            "population_id": self.grid_options["_population_id"],
+            "population_id": self.population_options["_population_id"],
             "process_id": self.process_ID,
             "start_process_time": start_process_time.timestamp(),
             "end_process_time": end_process_time.timestamp(),
             "total_time_calling_binary_c": total_time_calling_binary_c,
             "number_of_systems_run": number_of_systems_run,
             "probability_of_systems_run": probability_of_systems_run,
-            "failed_systems": self.grid_options["_failed_count"],
-            "failed_probability": self.grid_options["_failed_prob"],
-            "failed_system_error_codes": self.grid_options[
+            "failed_systems": self.population_options["_failed_count"],
+            "failed_probability": self.population_options["_failed_prob"],
+            "failed_system_error_codes": self.population_options[
                 "_failed_systems_error_codes"
             ],
             "zero_prob_stars_skipped": zero_prob_stars_skipped,
         }
         with self.open(
             os.path.join(
-                self.grid_options["tmp_dir"],
+                self.population_options["tmp_dir"],
                 "process_summary",
                 "process_{}.json".format(self.process_ID),
             ),
             "w",
             encoding="utf-8",
         ) as f:
             json.dump(summary_dict, f, indent=4, ensure_ascii=False)
 
         # Set status to finished
         if self.was_killed():
             self.set_status("killed")
         else:
             self.set_status("finished")
 
-        self.verbose_print(
+        #
+        self.vb_info(
             "process {} queue put output_dict ".format(ID),
-            self.grid_options["verbosity"],
-            1,
         )
+        self.vb_info(f"Process-{self.process_ID} is finished.")
 
         final_result_queue.put(output_dict)
 
-        if self.grid_options["verbosity"] >= self._LOGGER_VERBOSITY_LEVEL:
-            stream_logger.debug(f"Process-{self.process_ID} is finished.")
+        # Signal to the result queue that we're stopping too
+        result_queue.put("STOP")
 
-        self.verbose_print(
-            "process {} return ".format(ID),
-            self.grid_options["verbosity"],
-            1,
-        )
         return
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/failing_systems_functions.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/failing_systems_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,22 +24,22 @@
         self, system_dict=None, system_number=None, process=None, exitcode=None
     ):
         """
         Log failing or crashed system to file in log_failed_systems_dir
         """
 
         if (
-            self.grid_options["log_failed_systems"]
-            and self.grid_options["log_failed_systems_dir"] is not None
+            self.population_options["log_failed_systems"]
+            and self.population_options["log_failed_systems_dir"] is not None
         ):
-            path = os.path.join(self.grid_options["log_failed_systems_dir"])
+            path = os.path.join(self.population_options["log_failed_systems_dir"])
             os.makedirs(path, exist_ok=True)
             if self.dir_ok(path):
                 failed_systems_file = os.path.join(
-                    self.grid_options["log_failed_systems_dir"],
+                    self.population_options["log_failed_systems_dir"],
                     "process_{}.txt".format(self.jobID()),
                 )
                 with self.open(
                     failed_systems_file, "a", encoding="utf-8"  # append
                 ) as f:
                     now = datetime.datetime.now()
                     now = now.strftime("%d/%m/%Y %H:%M:%S\n")
@@ -47,113 +47,106 @@
                         binary_c_cmdline_string = (
                             f"system {system_number} at {now} "
                             + self._return_argline(system_dict)
                             + "\n"
                         )
                         f.write(binary_c_cmdline_string)
                     if process:
-                        print(f"logged crashed process to {failed_systems_file}")
+                        self.vb_warning(
+                            f"logged crashed process to {failed_systems_file}"
+                        )
                         f.write(
                             f"Process {process} crashed at {now} with exit code {exitcode}."
                         )
         return
 
     def _check_binary_c_error(self, system_number, binary_c_output, system_dict):
         """
         Function to check whether binary_c throws an error and handle accordingly.
         """
 
         if binary_c_output:
             if (binary_c_output.splitlines()[0].startswith("SYSTEM_ERROR")) or (
                 binary_c_output.splitlines()[-1].startswith("SYSTEM_ERROR")
             ):
-                self.verbose_print(
+                self.vb_warning(
                     "FAILING SYSTEM FOUND",
-                    self.grid_options["verbosity"],
-                    0,
                 )
 
                 # Keep track of the amount of failed systems and their error codes
-                self.grid_options["_failed_prob"] += system_dict.get("probability", 1)
-                self.grid_options["_failed_count"] += 1
-                self.grid_options["_errors_found"] = True
+                self.population_options["_failed_prob"] += system_dict.get(
+                    "probability", 1
+                )
+                self.population_options["_failed_count"] += 1
+                self.population_options["_errors_found"] = True
 
                 try:
                     error_code = int(
                         binary_c_output.splitlines()[0]
                         .split("with error code")[-1]
                         .split(":")[0]
                         .strip()
                     )
-                    self.verbose_print(
+                    self.vb_warning(
                         f"Have error code {error_code}",
-                        self.grid_options["verbosity"],
-                        0,
                     )
                 except:
-                    self.verbose_print(
+                    self.vb_warning(
                         "Failed to extract error code",
-                        self.grid_options["verbosity"],
-                        0,
                     )
                     pass
 
                 # Try catching the error code and keep track of the unique ones.
                 try:
                     error_code = int(
                         binary_c_output.splitlines()[0]
                         .split("with error code")[-1]
                         .split(":")[0]
                         .strip()
                     )
 
                     if (
                         error_code
-                        not in self.grid_options["_failed_systems_error_codes"]
+                        not in self.population_options["_failed_systems_error_codes"]
                     ):
-                        print(f"Caught errr code {error_code}")
-                        self.grid_options["_failed_systems_error_codes"].append(
+                        self.vb_info(f"Caught errr code {error_code}")
+                        self.population_options["_failed_systems_error_codes"].append(
                             error_code
                         )
                 except ValueError:
                     error_code = None
-                    self.verbose_print(
+                    self.vb_warning(
                         "Failed to extract the error-code",
-                        self.grid_options["verbosity"],
-                        1,
                     )
 
                 # log failing args?
                 self._log_failure(system_dict=system_dict, system_number=system_number)
 
                 # Check if we have exceeded the number of errors
-                print(
-                    f"Check failed count {self.grid_options['_failed_count']} vs max {self.grid_options['failed_systems_threshold']}"
+                self.vb_info(
+                    f"Check failed count {self.population_options['_failed_count']} vs max {self.population_options['failed_systems_threshold']}"
                 )
                 if (
-                    self.grid_options["_failed_count"]
-                    > self.grid_options["failed_systems_threshold"]
+                    self.population_options["_failed_count"]
+                    > self.population_options["failed_systems_threshold"]
                 ):
 
                     # stop evolving systems
-                    self.grid_options["stop_queue"]
+                    self.population_options["stop_queue"]
 
                     # warn the user the first time we exceed failed_systems_threshold
-                    if not self.grid_options["_errors_exceeded"]:
-                        self.verbose_print(
-                            self._boxed(
+                    if not self.population_options["_errors_exceeded"]:
+                        self.vb_error(
+                            "\n"
+                            + self._boxed(
                                 "Process {} exceeded the maximum ({}) number of failing systems. Stopped logging them to files now".format(
                                     self.process_ID,
-                                    self.grid_options["failed_systems_threshold"],
+                                    self.population_options["failed_systems_threshold"],
                                 )
                             ),
-                            self.grid_options["verbosity"],
-                            1,
                         )
-                        self.grid_options["_errors_exceeded"] = True
+                        self.population_options["_errors_exceeded"] = True
 
         else:
-            self.verbose_print(
+            self.vb_warning(
                 "binary_c output nothing - this is strange. If there is ensemble output being generated then this is fine.",
-                self.grid_options["verbosity"],
-                3,
             )
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/grid_sampling.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/grid_sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,40 @@
 import importlib
 import os
 
 _count = 0  # used for file symlinking (for testing only)
 _numba = False  # activate experimental numba code?
 
 
+###########################
+# Some context managers
+class indentation_context_manager:
+    def __init__(self, population_object, indentation_delta=1):
+        self.population_object = population_object
+        self.indentation_delta = indentation_delta
+
+    def __enter__(self):
+        self.population_object._increment_indent_depth(+self.indentation_delta)
+
+    def __exit__(self, exc, value, exc_traceback):
+        self.population_object._increment_indent_depth(-self.indentation_delta)
+
+
+class boxed_context_manager:
+    def __init__(self, population_object, width_box=40):
+        self.population_object = population_object
+        self.width_box = width_box
+
+    def __enter__(self):
+        self.population_object._add_code("#" * self.width_box + "\n")
+
+    def __exit__(self, exc, value, exc_traceback):
+        self.population_object._add_code("#" * self.width_box + "\n")
+
+
 class grid_sampling:
     """
     Extension to the population grid object that contains functionality to handle the metadata that will be put in the ensemble
     """
 
     def __init__(self, **kwargs):
         """
@@ -37,15 +63,17 @@
         """
 
         # write generator
         self._generate_grid_code(dry_run=False)
 
         # load generator
         self._load_grid_function()
-        generator = self.grid_options["_system_generator"](self, print_results=False)
+        generator = self.population_options["_system_generator"](
+            self, print_results=False
+        )
 
         return generator
 
     def _grid_sampling_setup(self):
         """
         Setup function for the grid sampling sampling type
         """
@@ -53,96 +81,95 @@
         # Set up LRU cache
         self.setup_function_cache()
 
         ############################################################
         # Dry run and getting starcount
         ############################################################
         # Put in check
-        if len(self.grid_options["_sampling_variables"]) == 0:
-            print("Error: you haven't defined any grid variables! Aborting")
+        if len(self.population_options["_sampling_variables"]) == 0:
+            self.vb_error("Error: you haven't defined any grid variables! Aborting")
             raise ValueError
 
         # Set up the grid code with a dry run option to see total probability
-        print("Do dry run? {}".format(self.grid_options["do_dry_run"]))
-        if self.grid_options["do_dry_run"]:
-            print("Doing dry run to calculate total starcount and probability")
+        self.vb_info("Do dry run? {}".format(self.population_options["do_dry_run"]))
+        if self.population_options["do_dry_run"]:
+            self.vb_info("Doing dry run to calculate total starcount and probability")
             self._generate_grid_code(dry_run=True)
 
             # Load the grid code
             self._load_grid_function()
 
             # Do a dry run
             self._dry_run()
 
-            self.verbose_print(
-                self._boxed(
+            self.vb_critical(
+                "\n"
+                + self._boxed(
                     "Dry run",
                     "Total starcount is {starcount}".format(
-                        starcount=self.grid_options["_total_starcount"]
+                        starcount=self.population_options["_total_starcount"]
                     ),
                     "Total probability is {probtot:g}".format(
-                        probtot=self.grid_options["_probtot"]
+                        probtot=self.population_options["_probtot"]
                     ),
                 ),
-                self.grid_options["verbosity"],
-                0,
             )
-            if self.grid_options["exit_after_dry_run"]:
-                print(
+            if self.population_options["exit_after_dry_run"]:
+                self.vb_info(
                     "Exiting after dry run {}".format(
-                        self.grid_options["exit_after_dry_run"]
+                        self.population_options["exit_after_dry_run"]
                     )
                 )
                 self.exit(code=0)
-            elif self.grid_options["return_after_dry_run"]:
-                print(
+            elif self.population_options["return_after_dry_run"]:
+                self.vb_info(
                     "Returning after dry run {}".format(
-                        self.grid_options["exit_after_dry_run"]
+                        self.population_options["exit_after_dry_run"]
                     )
                 )
                 return False
 
         #######################
         # Reset values and prepare the grid function
-        self.grid_options[
+        self.population_options[
             "_probtot"
         ] = 0  # To make sure that the values are reset. TODO: fix this in a cleaner way
 
         # # Making sure the loaded grid code isn't lingering in the main PID
         # self._generate_grid_code(dry_run=False)
 
         # #
         # self._load_grid_function()
 
         #
-        self.grid_options["_system_generator"] = None
+        self.population_options["_system_generator"] = None
 
     ###################################################
     # Grid code functions
     #
     # Function below are used to run populations with
     # a variable grid
     ###################################################
     def _gridcode_filename(self):
         """
         Returns a filename for the gridcode.
         """
         if self.HPC_job():
             filename = os.path.join(
-                self.grid_options["tmp_dir"],
+                self.population_options["tmp_dir"],
                 "binary_c_grid_{population_id}.{jobid}.py".format(
-                    population_id=self.grid_options["_population_id"],
+                    population_id=self.population_options["_population_id"],
                     jobid=self.jobID(),
                 ),
             )
         else:
             filename = os.path.join(
-                self.grid_options["tmp_dir"],
+                self.population_options["tmp_dir"],
                 "binary_c_grid_{population_id}.py".format(
-                    population_id=self.grid_options["_population_id"]
+                    population_id=self.population_options["_population_id"]
                 ),
             )
         return filename
 
     def _add_code(self, *args, indent=0):
         """
         Function to add code to the grid code string
@@ -178,103 +205,160 @@
         dry_run: when True, it will return the starcount at the end so that we know
         what the total number of systems is.
 
         The phasevol values are handled by generating a second array
 
         Results in a generated file that contains a system_generator function.
 
-        # TODO: make sure running systems with multiplicity 3+ is also possible.
-        # TODO: there is a lot of things going on in this function. Make sure to describe clearly what happens here.
+        NOTE: this function is large and has many moving parts.
+            Broadly it constructs a nested dictionary with yield calls at different depths (if they are branch points)
+
+        TODO: make sure running systems with multiplicity 3+ is also possible.
+        TODO: there is a lot of things going on in this function. Make sure to describe clearly what happens here.
+        TODO: this code could very much benefit from context managers that handle indent and dedents
         """
-        self.verbose_print("Generating grid code", self.grid_options["verbosity"], 1)
 
-        total_sampling_variables = len(self.grid_options["_sampling_variables"])
+        self.vb_info("Generating grid code")
+
+        # turn vb to True to have debugging output
+        vb = False
+
+        ######################################
+        # First part:
+        #   The code below generats the import statements, and sets up the function.
+        self._grid_sampling_write_grid_generator_function_start()
+
+        #################################################################################
+        # Nested loop generation
+        #################################################################################
+        self._add_code("\n")
+
+        ######################################
+        # Second part:
+        #   The code below generates the nested structure of the sampling variables
+        #       calls to the distribution functions and the calculation of the probabilities.
+        #   This part does *not* generate the yield statements
+        self._grid_sampling_write_grid_generator_function_nesting(
+            dry_run=dry_run, vb=vb
+        )
+
+        self._add_code("\n")
+
+        ######################################
+        # Third part:
+        #   The code below generates the yield calls and handles the branch points at different nest levels.
+        #   The order is reverse, and it starts at the deepest nesting.
+        self._grid_sampling_write_grid_generator_function_denesting(dry_run=dry_run)
 
+        ######################################
+        # Fourth part:
+        #   The code below wraps up the function and writes statements that handle returning information and some statistics.
+        self._grid_sampling_write_grid_generator_function_end(dry_run=dry_run)
+
+    def _grid_sampling_write_grid_generator_function_start(self):
+        """
+        This function is responsible for setting up the file, handling the imports and writing the beginning of the function, initialising parameters etc.
+        """
+
+        total_sampling_variables = len(self.population_options["_sampling_variables"])
+
+        ###############
+        # Import packages
         self._add_code(
-            # Import packages
             "import math\n",
             "import numpy as np\n",
             "from collections import OrderedDict\n",
             "from binarycpython.utils.useful_funcs import *\n",
             "import numba" if _numba else "",
             "\n\n",
-            # Make the function
-            "def grid_code(self, print_results=True):\n",
         )
 
+        ###############
+        # Define the function
+        self._add_code("def grid_code(self, print_results=True):\n")
+
         # Increase indent_depth
         self._increment_indent_depth(+1)
 
+        ###############
+        # Write comments at docstring
         self._add_code(
-            # Write some info in the function
             "# Grid code generated on {}\n".format(datetime.datetime.now().isoformat()),
-            "# This function generates the systems that will be evolved with binary_c\n\n"
-            # Set some values in the generated code:
+            "# This function generates the systems that will be evolved with binary_c\n\n",
+        )
+
+        ###############
+        # Initialise parameters, lists and dictionaries
+        self._add_code(
             "# Set initial values\n",
             "_total_starcount = 0\n",
             "starcounts = [0 for i in range({})]\n".format(
                 total_sampling_variables + 1
             ),
-            "probabilities = {}\n",
-            "probabilities_list = [0 for i in range({})]\n".format(
-                total_sampling_variables + 1
-            ),
-            "probabilities_sum = [0 for i in range({})]\n".format(
-                total_sampling_variables + 1
-            ),
             "parameter_dict = {}\n",
             "phasevol = 1\n",
         )
 
+        ###############
         # Set up the system parameters
         self._add_code(
             "M_1 = None\n",
             "M_2 = None\n",
             "M_3 = None\n",
             "M_4 = None\n",
             "orbital_period = None\n",
             "orbital_period_triple = None\n",
             "orbital_period_quadruple = None\n",
             "eccentricity = None\n",
-            "eccentricity2 = None\n",
-            "eccentricity3 = None\n",
+            "eccentricity_triple = None\n",
+            "eccentricity_quadruple = None\n",
             "\n",
+        )
+
+        ###############
+        # Set up probability lists, dicts
+        self._add_code(
             # Prepare the probability
-            "# set probability lists\n",
+            "# set probability objects\n",
+            "probabilities = {}\n",
+            "probabilities_list = [0 for i in range({})]\n".format(
+                total_sampling_variables + 1
+            ),
+            "probabilities_sum = [0 for i in range({})]\n".format(
+                total_sampling_variables + 1
+            ),
         )
 
+        # Fill the probability dictionary with zeroes
         for sampling_variable_el in sorted(
-            self.grid_options["_sampling_variables"].items(),
+            self.population_options["_sampling_variables"].items(),
             key=lambda x: x[1]["sampling_variable_number"],
         ):
             # Make probabilities dict
             sampling_variable = sampling_variable_el[1]
             self._add_code(
                 'probabilities["{}"] = 0\n'.format(sampling_variable["name"])
             )
 
-        #################################################################################
-        # Start of code generation
-        #################################################################################
-        self._add_code("\n")
-
-        # turn vb to True to have debugging output
-        vb = False
+    def _grid_sampling_write_grid_generator_function_nesting(self, dry_run, vb):
+        """
+        This function generates the nested structure of the grid code generator.
+        Sets up the calculation of the sampling variables, calls to the distribution functions
+        and the calculation of the probabilities.
+        """
 
         # Generate code
         for loopnr, sampling_variable_el in enumerate(
             sorted(
-                self.grid_options["_sampling_variables"].items(),
+                self.population_options["_sampling_variables"].items(),
                 key=lambda x: x[1]["sampling_variable_number"],
             )
         ):
-            self.verbose_print(
+            self.vb_debug(
                 "Constructing/adding: {}".format(sampling_variable_el[0]),
-                self.grid_options["verbosity"],
-                2,
             )
             sampling_variable = sampling_variable_el[1]
 
             ####################
             # top code
             if sampling_variable["topcode"]:
                 self._add_code(sampling_variable["topcode"])
@@ -582,15 +666,15 @@
                     "if not {condition}:\n".format(
                         condition=sampling_variable["condition"]
                     ),
                     indent=0,
                 )
 
                 # Add condition failed action:
-                if self.grid_options["verbosity"] >= 4:
+                if self.population_options["verbosity"] >= 4:
                     self._add_code(
                         'print("Grid generator: Condition for {name} not met!")'.format(
                             name=sampling_variable["name"]
                         )
                         + "\n",
                         "continue" + "\n",
                         indent=1,
@@ -615,14 +699,15 @@
                         precode=sampling_variable["precode"].replace(
                             "\n", "\n" + self._indent_block(0)
                         )
                     )
                     + "\n"
                 )
 
+            #########################
             # Set phasevol
             self._add_code(
                 "phasevol *= dphasevol_{name}\n".format(
                     name=sampling_variable["name"],
                 )
             )
 
@@ -658,27 +743,27 @@
                         this=sampling_variable["sampling_variable_number"],
                         prev=sampling_variable["sampling_variable_number"] - 1,
                         name=sampling_variable["name"],
                     )
                     + "\n"
                 )
 
-            ##############
+            #########################
             # postcode
             if sampling_variable["postcode"]:
                 self._add_code(
                     "{postcode}".format(
                         postcode=sampling_variable["postcode"].replace(
                             "\n", "\n" + self._indent_block(0)
                         )
                     )
                     + "\n"
                 )
 
-            #######################
+            #########################
             # Increment starcount for this parameter
             self._add_code(
                 "\n",
                 "# Increment starcount for {name}\n".format(
                     name=sampling_variable["name"]
                 ),
                 "starcounts[{n}] += 1".format(
@@ -689,280 +774,289 @@
                 'parameter_dict["{name}"] = {name}'.format(
                     name=sampling_variable["parameter_name"]
                 )
                 + "\n",
                 "\n",
             )
 
-            self._increment_indent_depth(-1)
-
-            # The final parts of the code, where things are returned, are within the deepest loop,
-            # but in some cases code from a higher loop needs to go under it again
-            # SO I think its better to put an if statement here that checks
-            # whether this is the last loop.
-            if loopnr == len(self.grid_options["_sampling_variables"]) - 1:
+            #########################
+            # Construct system call
+            #   The final parts of the code, where things are returned, are within the deepest loop,
+            #   but in some cases code from a higher loop needs to go under it again
+            #   SO I think its better to put an if statement here that checks
+            #   whether this is the last loop.
+            if loopnr == len(self.population_options["_sampling_variables"]) - 1:
                 self._write_gridcode_system_call(
                     sampling_variable,
                     dry_run,
-                    sampling_variable["branchpoint"],
-                    sampling_variable["branchcode"],
                 )
 
-            # increment indent_depth
-            self._increment_indent_depth(+1)
-
             ####################
             # bottom code
             if sampling_variable["bottomcode"]:
                 self._add_code(sampling_variable["bottomcode"])
 
-        self._increment_indent_depth(-1)
-        self._add_code("\n")
+    def _grid_sampling_write_grid_generator_function_denesting(self, dry_run):
+        """
+        The code below generates the yield calls and handles the branch points at different nest levels.
+        The order is reverse, and it starts at the deepest nesting.
+        """
 
-        # Write parts to write below the part that yield the results.
-        # this has to go in a reverse order:
-        # Here comes the stuff that is put after the deepest nested part that calls returns stuff.
-        # Here we will have a
         reverse_sorted_sampling_variables = sorted(
-            self.grid_options["_sampling_variables"].items(),
+            self.population_options["_sampling_variables"].items(),
             key=lambda x: x[1]["sampling_variable_number"],
             reverse=True,
         )
         for loopnr, sampling_variable_el in enumerate(
             reverse_sorted_sampling_variables
         ):
             sampling_variable = sampling_variable_el[1]
 
-            self._increment_indent_depth(+1)
             self._add_code(
                 "#" * 40 + "\n",
-                "# Code below is for finalising the handling of this iteration of the parameter {name}\n".format(
+                "# Code below is for finalising the handling of this iteration of the parameter {name}\n\n".format(
                     name=sampling_variable["name"]
                 ),
             )
 
-            # Set phasevol
+            ################
+            # Check the branchpoint part here. The branchpoint makes sure that we can construct
+            # a grid with several multiplicities and still can make the system calls for each
+            # multiplicity without reconstructing the grid each time
+            self._grid_sampling_handle_branchpoint(
+                sampling_variable=sampling_variable, dry_run=dry_run, loopnr=loopnr
+            )
+
+            #############
+            # Unset phasevol
+            #   This happens in the same loop as the actual variable
             # TODO: fix. this isn't supposed to be the value that we give it here. discuss
             self._add_code(
                 "phasevol /= dphasevol_{name}\n\n".format(
                     name=sampling_variable["name"]
                 )
             )
 
-            self._increment_indent_depth(-2)
-
             if _numba and sampling_variable["dry_parallel"]:
                 self._add_code("__parallel_func(phasevol,_total_starcount)\n")
                 self._increment_indent_depth(-1)
 
-            # Check the branchpoint part here. The branchpoint makes sure that we can construct
-            # a grid with several multiplicities and still can make the system calls for each
-            # multiplicity without reconstructing the grid each time
-            if sampling_variable["branchpoint"] > 0:
-
-                self._increment_indent_depth(+1)
-
-                self._add_code(
-                    # Add comment
-                    "# Condition for branchpoint at {}".format(
-                        reverse_sorted_sampling_variables[loopnr + 1][1]["name"]
-                    )
-                    + "\n",
-                    # # Add condition check
-                    #     "if not {}:".format(sampling_variable["condition"])
-                    #     + "\n"
-                    # Add branchpoint
-                    "if multiplicity=={}:".format(sampling_variable["branchpoint"])
-                    + "\n",
-                )
+            # Decrement level
+            self._increment_indent_depth(-1)
 
-                self._write_gridcode_system_call(
-                    reverse_sorted_sampling_variables[loopnr + 1][1],
-                    dry_run,
-                    sampling_variable["branchpoint"],
-                    sampling_variable["branchcode"],
-                )
-                self._increment_indent_depth(-1)
-                self._add_code("\n")
+    def _grid_sampling_write_grid_generator_function_end(self, dry_run):
+        """
+        This function is responsible for wrapping up the grid code generator. It wraps up the function, writes statements
+        """
 
         ###############################
         # Finalise print statements
         #
-        self._increment_indent_depth(+1)
         self._add_code("\n", "#" * 40 + "\n", "if print_results:\n")
         self._add_code(
-            "print('Grid has handled {starcount} stars with a total probability of {probtot:g}'.format(starcount=_total_starcount,probtot=self.grid_options['_probtot']))\n",
+            "print('Grid has handled {starcount} stars with a total probability of {probtot:g}'.format(starcount=_total_starcount,probtot=self.population_options['_probtot']))\n",
             indent=1,
         )
 
-        ################
         # Finalise return statement for dry run.
-        #
         if dry_run:
             self._add_code("return _total_starcount\n")
 
-        self._increment_indent_depth(-1)
         #################################################################################
-        # Stop of code generation. Here the code is saved and written
+        # Stop of code generation.
+        #   Here the code is saved and written
 
-        # Save the grid code to the grid_options
-        self.verbose_print(
-            "Save grid code to grid_options", self.grid_options["verbosity"], 1
+        #########
+        # Save the grid code to the population_options
+        self.vb_info(
+            "Save grid code to population_options",
         )
 
-        self.grid_options["code_string"] = self.code_string
+        self.population_options["code_string"] = self.code_string
 
         # Write to file
         gridcode_filename = self._gridcode_filename()
 
-        self.grid_options["gridcode_filename"] = gridcode_filename
+        self.population_options["gridcode_filename"] = gridcode_filename
 
-        self.verbose_print(
+        self.vb_error(
             "{blue}Write grid code to {file} [dry_run = {dry}]{reset}".format(
                 blue=self.ANSI_colours["blue"],
                 file=gridcode_filename,
                 dry=dry_run,
                 reset=self.ANSI_colours["reset"],
             ),
-            self.grid_options["verbosity"],
-            1,
         )
 
+        # Write code
         with self.open(gridcode_filename, "w", encoding="utf-8") as file:
             file.write(self.code_string)
 
         # reset the code string
         self.code_string = ""
+        self.indent_depth = 0
 
         # perhaps create symlink
-        if not self.HPC_job() and self.grid_options["symlink_latest_gridcode"]:
+        if not self.HPC_job() and self.population_options["symlink_latest_gridcode"]:
             global _count
             symlink = os.path.join(
-                self.grid_options["tmp_dir"], "binary_c_grid-latest" + str(_count)
+                self.population_options["tmp_dir"], "binary_c_grid-latest" + str(_count)
             )
             _count += 1
             try:
                 os.unlink(symlink)
             except:
                 pass
 
             try:
                 os.symlink(gridcode_filename, symlink)
-                self.verbose_print(
+                self.vb_info(
                     "{blue}Symlinked grid code to {symlink} {reset}".format(
                         blue=self.ANSI_colours["blue"],
                         symlink=symlink,
                         reset=self.ANSI_colours["reset"],
                     ),
-                    self.grid_options["verbosity"],
-                    1,
                 )
             except OSError:
-                print("symlink failed")
+                self.vb_error("symlink failed")
+
+    def _grid_sampling_handle_branchpoint(self, sampling_variable, dry_run, loopnr):
+        """
+        Function to handle the branch point
+        """
+
+        # Check if there is a branchpoint and that this is not the deepest loop
+        if (sampling_variable["branchpoint"]) and (loopnr > 0):
+            ###########################
+            # Handle branch point
+            if sampling_variable["branchcode"]:
+                with boxed_context_manager(population_object=self):
+                    self._add_code("# Branch code\n")
+                    self._add_code(
+                        "if {branchcode}:\n".format(
+                            branchcode=sampling_variable["branchcode"]
+                        )
+                    )
+
+                    ###########################
+                    # Indent and write the grid system call
+                    with indentation_context_manager(population_object=self):
+                        ###########################
+                        # Handle system call
+                        self._write_gridcode_system_call(
+                            sampling_variable,
+                            dry_run,
+                        )
+
+                        self._add_code("\n")
+            else:
+                raise ValueError("Handling branch point but no branchcode provided")
 
-    def _write_gridcode_system_call(
-        self, sampling_variable, dry_run, branchpoint, branchcode
-    ):
+            #
+            self._add_code("\n")
+
+    def _write_gridcode_system_call(self, sampling_variable, dry_run):
         """
         Function to write the block of code (as string) that handles the setting the final probability, taking into account the weight and repeat settings, incrementing the total starcount and total probability.
 
         Then if the run is a dry run we implement the dry_run_hook or pass depending on the settings. If it is not a dry run we yield the system dict
         """
 
-        self._increment_indent_depth(+1)
-        self._add_code("#" * 40 + "\n")
-
-        if branchcode:
+        with boxed_context_manager(population_object=self):
             self._add_code(
-                "# Branch code\nif {branchcode}:\n".format(branchcode=branchcode)
+                "# grid sampling system call section ({})\n\n".format(
+                    sampling_variable["name"]
+                )
             )
 
-        if branchpoint:
+            ##################
+            # Write the code that handles the probability calculation
+
+            #########
+            # Weight probability by custom weight factor
             self._add_code(
-                "# Code below will get evaluated for every system at this level of multiplicity (last one of that being {name})\n".format(
-                    name=sampling_variable["name"]
-                )
+                "# Weigh the probability by a custom weighting factor\n",
+                'probability = self.population_options["weight"] * probabilities_list[{n}]\n'.format(
+                    n=sampling_variable["sampling_variable_number"]
+                ),
             )
-        else:
+
+            #########
+            # Take into account the multiplicity fraction:
             self._add_code(
-                "# Code below will get evaluated for every generated system\n"
+                "\n",
+                "# Factor the multiplicity fraction into the probability\n",
+                "probability *= self._calculate_multiplicity_fraction(parameter_dict)\n",
             )
 
-        # Factor in the custom weight input
-        self._add_code(
-            "\n",
-            "# Weigh the probability by a custom weighting factor\n",
-            'probability = self.grid_options["weight"] * probabilities_list[{n}]'.format(
-                n=sampling_variable["sampling_variable_number"]
-            )
-            + "\n",
-            # Take into account the multiplicity fraction:
-            "\n",
-            "# Factor the multiplicity fraction into the probability\n",
-            "probability *= self._calculate_multiplicity_fraction(parameter_dict)"
-            + "\n",
+            #########
             # Divide by number of repeats
-            "\n",
-            "# Divide the probability by the number of repeats\n",
-            'probability /= self.grid_options["repeat"]' + "\n",
-            # Now we yield the system self.grid_options["repeat"] times.
-            "\n",
-            "# Loop over the repeats\n",
-            'for _ in range(self.grid_options["repeat"]):' + "\n",
-        )
-        self._add_code(
-            "_total_starcount += 1\n",
-            # set probability and phasevol values into the system dict
-            'parameter_dict["{p}"] = {p}'.format(p="probability") + "\n",
-            'parameter_dict["{v}"] = {v}'.format(v="phasevol") + "\n",
-            # Increment total probability
-            "self._increment_probtot(probability)\n",
-            indent=1,
-        )
+            self._add_code(
+                "\n",
+                "# Divide the probability by the number of repeats\n",
+                'probability /= self.population_options["repeat"]\n',
+            )
 
-        if not dry_run:
-            # Handle what is returned, or what is not.
-            self._add_code("yield(parameter_dict)\n", indent=1)
+            #########
+            # Now we yield the system self.population_options["repeat"] times.
+            self._add_code(
+                "\n",
+                "# Loop over the repeats\n",
+                'for _ in range(self.population_options["repeat"]):\n',
+            )
+            with indentation_context_manager(population_object=self):
+                #########
+                # Increment starcount
+                self._add_code("_total_starcount += 1\n")
 
-        # If its a dry run, dont do anything with it
-        else:
-            # run the hook function, only if given
-            if self.grid_options["dry_run_hook"]:
+                #########
+                # set probability and phasevol values into the system dict
                 self._add_code(
-                    "self.grid_options['dry_run_hook'](self, parameter_dict)\n",
-                    indent=1,
+                    'parameter_dict["{p}"] = {p}'.format(p="probability") + "\n",
+                    'parameter_dict["{v}"] = {v}'.format(v="phasevol") + "\n",
                 )
-            else:
-                # or pass
-                self._add_code("pass\n", indent=1)
-
-        self._add_code("#" * 40 + "\n")
 
-        self._increment_indent_depth(-1)
+                #########
+                # Increment total probability
+                self._add_code(
+                    "self._increment_probtot(probability)\n",
+                )
 
-        return self.code_string
+            #########
+            # Handle dry run or actual call
+            if not dry_run:
+                # Handle what is returned, or what is not.
+                self._add_code("yield(parameter_dict)\n", indent=1)
+            else:
+                # run the hook function, only if given
+                if self.population_options["dry_run_hook"]:
+                    self._add_code(
+                        "self.population_options['dry_run_hook'](self, parameter_dict)\n",
+                        indent=1,
+                    )
+                else:
+                    # or pass
+                    self._add_code("pass\n", indent=1)
 
     def _load_grid_function(self):
         """
         Function that loads the grid code from file
         """
 
         # Code to load the
-        self.verbose_print(
+        self.vb_info(
             message="Load grid code function from {file}".format(
-                file=self.grid_options["gridcode_filename"]
+                file=self.population_options["gridcode_filename"]
             ),
-            verbosity=self.grid_options["verbosity"],
-            minimal_verbosity=1,
         )
 
         spec = importlib.util.spec_from_file_location(
             "binary_c_python_grid",
-            os.path.join(self.grid_options["gridcode_filename"]),
+            os.path.join(self.population_options["gridcode_filename"]),
         )
         grid_file = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(grid_file)
         generator = grid_file.grid_code
 
-        self.grid_options["_system_generator"] = generator
+        self.population_options["_system_generator"] = generator
 
-        self.verbose_print("Grid code loaded", self.grid_options["verbosity"], 1)
+        self.vb_info("Grid code loaded")
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/metadata.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,40 +64,42 @@
         self.grid_ensemble_results["metadata"]["duration"] = self.time_elapsed()
 
         # Calculate cpu time
         self.grid_ensemble_results["metadata"]["CPU_time"] = self.CPU_time()
 
     def add_ensemble_metadata(self, combined_output_dict):
         """
-        Function to add metadata to the grid_ensemble_results and grid_options
+        Function to add metadata to the grid_ensemble_results and population_options
         """
 
         self.grid_ensemble_results["metadata"] = {}
 
-        self.grid_ensemble_results["metadata"]["population_id"] = self.grid_options[
-            "_population_id"
-        ]
+        self.grid_ensemble_results["metadata"][
+            "population_id"
+        ] = self.population_options["_population_id"]
         self.grid_ensemble_results["metadata"][
             "total_probability_weighted_mass"
         ] = combined_output_dict["_total_probability_weighted_mass_run"]
         self.grid_ensemble_results["metadata"][
             "factored_in_probability_weighted_mass"
         ] = False
-        if self.grid_options["ensemble_factor_in_probability_weighted_mass"]:
+        if self.population_options["ensemble_factor_in_probability_weighted_mass"]:
             multiply_values_dict(
                 self.grid_ensemble_results["ensemble"],
                 1.0
                 / self.grid_ensemble_results["metadata"][
                     "total_probability_weighted_mass"
                 ],
             )
             self.grid_ensemble_results["metadata"][
                 "factored_in_probability_weighted_mass"
             ] = True
-        self.grid_ensemble_results["metadata"]["_killed"] = self.grid_options["_killed"]
+        self.grid_ensemble_results["metadata"]["_killed"] = self.population_options[
+            "_killed"
+        ]
 
         # Add settings of the populations
         all_info = self.return_all_info(
             include_population_settings=True,
             include_binary_c_defaults=True,
             include_binary_c_version_info=True,
             include_binary_c_help_all=True,
@@ -105,16 +107,16 @@
         self.grid_ensemble_results["metadata"]["settings"] = json.loads(
             json.dumps(all_info, default=binaryc_json_serializer, ensure_ascii=False)
         )
 
         ##############################
         # Update grid options
         for x in self._metadata_keylist():
-            self.grid_options[x] = combined_output_dict[x]
-        self.grid_options["_failed_systems_error_codes"] = list(
+            self.population_options[x] = combined_output_dict[x]
+        self.population_options["_failed_systems_error_codes"] = list(
             set(combined_output_dict["_failed_systems_error_codes"])
         )
 
     def _metadata_keylist(self):
         """
         Function that returns the list of metadata keys
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/miscellaneous_functions.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/miscellaneous_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,92 +89,85 @@
                 argtype = "list"
             else:
                 parameter = None
                 value = None
                 argtype = None
 
         if parameter:
-            if vb:
-                print(
-                    f"_match_arg_to_host: {parameter} = {value} (argtype = {argtype})"
-                )
+            self.vb_debug(
+                f"_match_arg_to_host: {parameter} = {value} (argtype = {argtype})"
+            )
             try:
-                if vb:
-                    print("Try to eval", value)
+                self.vb_debug("Try to eval", value)
                 if isinstance(value, str):
                     # string : eval it
                     _x = eval(value)
                 else:
                     _x = value
 
                 # if dict, match to hostnames or 'default'
                 if isinstance(_x, dict):
                     _match = None
                     for host in hostnameslist:
-                        if vb:
-                            print(f"check host={host}")
+                        self.vb_debug(f"check host={host}")
                         _match = _x.get(host, None)
                         if _match:
-                            if vb:
-                                print(
-                                    f"Parameter {parameter} matches a value set by host={host} -> {_match}"
-                                )
+                            self.vb_debug(
+                                f"Parameter {parameter} matches a value set by host={host} -> {_match}"
+                            )
                             break
 
                     # no match? try 'default'
                     if not _match:
                         _match = _x.get("default", None)
 
                     # no match? error
                     if not _match:
-                        print(
+                        self.vb_debug(
                             f"Parameter {parameter} is a dict {value} none of the keys or which matches our hostname ({hostnameslist}) or 'default'. Please update this parameter."
                         )
                         sys.exit(1)
                     else:
-                        if vb:
-                            print(f"Parameter {parameter} set to value {_match}")
+                        self.vb_debug(f"Parameter {parameter} set to value {_match}")
                         value = _match
             except:
                 pass
 
             if argtype == "list":
                 # return x=y type argument
                 new_arg = f"{parameter}={value}"
             else:
                 new_arg = value
 
-        if vb:
-            print("return arg", new_arg, "of type", type(value))
+        self.vb_debug("return arg {} of type {}".format(new_arg, type(value)))
         return new_arg
 
     def _set_nprocesses(self):
         """
         Function to set the number of processes used in multiprocessing.
 
-        Test the value of grid_options['num_cores']:
+        Test the value of population_options['num_cores']:
 
         * If 0 or 'logical' or 'all logical', use all logical cores.
 
         * If -1 or 'physical' or 'all physical', use all physical cores.
 
         * If integer >=1 use the number of cores given.
 
         * If  a dict, (key,value) pairs are (hostname,num_cores)
           for particular machines. We then try to match this machine to
           the (hostname,num_cores) pairs to set num_cores. If not found,
           default to either the dict "default" setting, or the number
           of logical cores available.
 
-        * If grid_options['num_cores'] is missing, all logical cores are used.
+        * If population_options['num_cores'] is missing, all logical cores are used.
 
         Exit if none of the above are satisfied.
 
         """
-        _vb = self.grid_options["verbosity"] >= 2
 
         def __nprocs(ncores):
             """
             Function to determine the number of processes
             """
 
             if type(ncores) is str:
@@ -182,106 +175,100 @@
                     # use all logical cores available to us
                     return max(1, psutil.cpu_count(logical=True))
                 elif ncores == "all physical" or ncores == "physical":
                     # use all physical cores available to us
                     return max(1, psutil.cpu_count(logical=False))
                 else:
                     # unknown string : fall back to one CPU
-                    print(
+                    self.vb_error(
                         f"grid_option['num_cores'] = \"{ncores}\" is not recognised.\nPlease consider either setting this option to a number, 'physical' or 'logical', or a dict of (host,num_cores) pairs."
                     )
                     self.exit(code=1)
 
             if type(ncores) is int:
                 if ncores == -1:
                     return max(1, psutil.cpu_count(logical=False))
                 elif ncores == 0:
                     return max(1, psutil.cpu_count(logical=True))
                 else:
                     return ncores
             else:
                 # ncores should be int or string, oops
-                print(
+                self.vb_error(
                     f"grid_option['num_cores'] = \"{ncores}\" is not recognised.\nPlease consider either setting this option to a number, 'physical' or 'logical', or a dict of (host,num_cores) pairs."
                 )
                 self.exit(code=1)
 
-        if _vb:
-            print(
-                f"NPROC: pre-eval \"{self.grid_options['num_cores']}\" type \"{type(self.grid_options['num_cores'])}\""
+            self.vb_info(
+                f"NPROC: pre-eval \"{self.population_options['num_cores']}\" type \"{type(self.population_options['num_cores'])}\""
             )
 
         # eval the incoming string if possible, it may be a JSON
         # representation of a dict, and if this works we
         # set the num_cores option to the eval'd version.
         # It may also be a normal string or int, so we can't just
         # use the JSON parser.
         try:
-            _x = eval(self.grid_options["num_cores"])
-            self.grid_options["num_cores"] = _x
+            _x = eval(self.population_options["num_cores"])
+            self.population_options["num_cores"] = _x
         except:
             pass
 
         # backwards compatibility
-        if "amt_cores" in self.grid_options:
-            self.grid_options["num_cores"] = self.grid_options["amt_cores"]
+        if "amt_cores" in self.population_options:
+            self.population_options["num_cores"] = self.population_options["amt_cores"]
 
-        if _vb:
-            print(
-                f"NPROC: \"{self.grid_options['num_cores']}\" type \"{type(self.grid_options['num_cores'])}\""
-            )
-
-        if "num_cores" in self.grid_options:
-            if _vb:
-                print("NPROC found in grid options")
-            if type(self.grid_options["num_cores"]) is dict:
+        self.vb_info(
+            f"NPROC: \"{self.population_options['num_cores']}\" type \"{type(self.population_options['num_cores'])}\""
+        )
+
+        if "num_cores" in self.population_options:
+            self.vb_info("NPROC found in grid options")
+            if type(self.population_options["num_cores"]) is dict:
                 # try to match hostname to the dict keys
                 hostnameslist = self.my_hostnames()
-                for host, ncores in self.grid_options["num_cores"].items():
+                for host, ncores in self.population_options["num_cores"].items():
                     # check if we are this host
                     if host in hostnameslist:
-                        self.grid_options["num_processes"] = __nprocs(ncores)
-                        if _vb:
-                            print(
-                                f"SET NPROC = {self.grid_options['num_processes']} FROM HOST {host}"
-                            )
+                        self.population_options["_num_processes"] = __nprocs(ncores)
+                        self.vb_info(
+                            f"SET NPROC = {self.population_options['_num_processes']} FROM HOST {host}"
+                        )
                         return
 
                 # no host match : use default number of cores
-                if "default" in self.grid_options["num_cores"]:
-                    self.grid_options["num_processes"] = __nprocs(
-                        self.grid_options["num_cores"]["default"]
+                if "default" in self.population_options["num_cores"]:
+                    self.population_options["_num_processes"] = __nprocs(
+                        self.population_options["num_cores"]["default"]
+                    )
+                    self.vb_info(
+                        f"SET NPROC = {self.population_options['_num_processes']} FROM default"
                     )
-                    if _vb:
-                        print(
-                            f"SET NPROC = {self.grid_options['num_processes']} FROM default"
-                        )
                     return
-            elif type(self.grid_options["num_cores"]) is str:
+            elif type(self.population_options["num_cores"]) is str:
                 # just use int passed in
-                self.grid_options["num_processes"] = __nprocs(
-                    self.grid_options["num_cores"]
+                self.population_options["_num_processes"] = __nprocs(
+                    self.population_options["num_cores"]
+                )
+                self.vb_info(
+                    f"SET NPROC = {self.population_options['_num_processes']} from string passed in"
                 )
-                if _vb:
-                    print(
-                        f"SET NPROC = {self.grid_options['num_processes']} from string passed in"
-                    )
                 return
-            elif type(self.grid_options["num_cores"]) is int:
+            elif type(self.population_options["num_cores"]) is int:
                 # just use int passed in
-                self.grid_options["num_processes"] = __nprocs(
-                    self.grid_options["num_cores"]
+                self.population_options["_num_processes"] = __nprocs(
+                    self.population_options["num_cores"]
+                )
+                self.vb_info(
+                    f"SET NPROC = {self.population_options['_num_processes']} from int passed in"
                 )
-                if _vb:
-                    print(
-                        f"SET NPROC = {self.grid_options['num_processes']} from int passed in"
-                    )
                 return
 
         # no host matched or no 'num_cores' option provided: use all available logical cores
-        self.grid_options["num_processes"] = max(1, psutil.cpu_count(logical=True))
-        if _vb:
-            print(
-                f"SET NPROC = {self.grid_options['num_processes']} because no option given"
-            )
+        self.population_options["_num_processes"] = max(
+            1, psutil.cpu_count(logical=True)
+        )
+        self.vb_info(
+            f"SET NPROC = {self.population_options['_num_processes']} because no option given"
+        )
 
         return
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/monte_carlo_sampling.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/monte_carlo_sampling.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,77 +32,106 @@
         return
 
     def _monte_carlo_sampling_cleanup(self):
         """
         Cleanup function for the Monte-Carlo sampling evolution type
         """
 
-        self.grid_options["_monte_carlo_threshold_reached"] = False
-        self.grid_options["_monte_carlo_current_total_mass_evolved"] = 0
+        self.population_options["_monte_carlo_threshold_reached"] = False
+        self.population_options["_monte_carlo_current_total_mass_evolved"] = 0
+        self.population_options["_monte_carlo_current_total_count_evolved"] = 0
 
     def _monte_carlo_sampling_check_mass_threshold(self, system_dict):
         """
         Function to handle checking the total mass evolved and signal to stop
         """
 
         # Only if the monte_carlo_mass_threshold is positive (default = -1)
-        if self.grid_options["monte_carlo_mass_threshold"] > 0:
+        if self.population_options["monte_carlo_mass_threshold"] > 0:
 
             # Add total mass of current system tot total mass evolved
-            self.grid_options[
+            self.population_options[
                 "_monte_carlo_current_total_mass_evolved"
             ] += calculate_total_mass_system(system_dict)
 
             # Check if exceeds threshold
             if (
-                self.grid_options["_monte_carlo_current_total_mass_evolved"]
-                > self.grid_options["monte_carlo_mass_threshold"]
+                self.population_options["_monte_carlo_current_total_mass_evolved"]
+                > self.population_options["monte_carlo_mass_threshold"]
             ):
-                self.grid_options["_monte_carlo_threshold_reached"] = True
+                self.population_options["_monte_carlo_threshold_reached"] = True
+
+    def _monte_carlo_sampling_check_count_threshold(self):
+        """
+        Function to handle checking the total count evolved and signal to stop
+        """
+
+        # Only if the monte_carlo_count_threshold is positive (default = -1)
+        if self.population_options["monte_carlo_count_threshold"] > 0:
+
+            # Add total mass of current system tot total count evolved
+            self.population_options["_monte_carlo_current_total_count_evolved"] += 1
+
+            # Check if exceeds threshold
+            if (
+                self.population_options["_monte_carlo_current_total_count_evolved"]
+                > self.population_options["monte_carlo_count_threshold"]
+            ):
+                self.population_options["_monte_carlo_threshold_reached"] = True
 
     def _monte_carlo_sampling_check_custom_threshold(self, result_queue):
         """
         Function to handle checking the content of the result queue and look for a
-        TODO: put in the user-defined custom threshold function
+
+        The user-defined function has access to the result_queue and is responsible for processing (and emptying it)
         """
 
-        # raise NotImplementedError("Functionality in not implemented")
-        pass
+        # Pass output of binary_c to a user-defined parsing function
+        if self.population_options["monte_carlo_custom_threshold_function"]:
+            self.population_options["monte_carlo_custom_threshold_function"](
+                self, result_queue
+            )
 
     ##############
     # Generator functions
 
     # Management
     def _monte_carlo_sampling_get_generator_filename(self):
         """
-        Returns a filename for the gridcode.
+        Returns a filename of the generator file for the monte-carlo sampling
+
+        Returns:
+            filename (str): filename of the generator file for the monte-carlo sampling.
         """
 
         if self.HPC_job():
             filename = os.path.join(
-                self.grid_options["tmp_dir"],
+                self.population_options["tmp_dir"],
                 "binary_c_monte_carlo_sampling_generator_{population_id}.{jobid}.py".format(
-                    population_id=self.grid_options["_population_id"],
+                    population_id=self.population_options["_population_id"],
                     jobid=self.jobID(),
                 ),
             )
         else:
             filename = os.path.join(
-                self.grid_options["tmp_dir"],
+                self.population_options["tmp_dir"],
                 "binary_c_monte_carlo_sampling_generator_{population_id}.py".format(
-                    population_id=self.grid_options["_population_id"]
+                    population_id=self.population_options["_population_id"]
                 ),
             )
         return filename
 
     def _monte_carlo_sampling_write_generator_file(self, dry_run=False):
         """
         Function to write the function that can generate the sample for the parameter
 
         Contrary to the grid sampling variable generator code, this code is not nested, but is linear.
+
+        Args:
+            dry_run (bool, optional): flag to build with dry-run functionality.
         """
 
         #########
         # Set up header and start of function
         self._add_code(
             # Import packages
             "import math\n",
@@ -127,15 +156,15 @@
             "# Set initial values\n",
             "_total_starcount = 0\n",
             "generating = True\n",
             "default_system_dict = {'multiplicity': 0}\n\n",
         )
 
         # Add method for the pre-calculation of the arrays
-        if self.grid_options["monte_carlo_use_pre_calculated_distributions"]:
+        if self.population_options["monte_carlo_use_pre_calculated_distributions"]:
             self._add_code("self.handle_pre_calc(self)\n")
 
         #########
         # Set up the loop and yield calls
         self._add_code(
             # Comment
             comment_line,
@@ -148,15 +177,15 @@
         self._increment_indent_depth(+1)
         self._add_code("system_dict = copy.copy(default_system_dict)\n\n")
 
         #########
         # Run loop of sampling variable setup
         for loopnr, sampling_variable_el in enumerate(
             sorted(
-                self.grid_options["_sampling_variables"].items(),
+                self.population_options["_sampling_variables"].items(),
                 key=lambda x: x[1]["sampling_variable_number"],
             )
         ):
             sampling_variable = sampling_variable_el[1]
 
             #########
             # Generate parameter lines
@@ -173,26 +202,24 @@
 
         #########
         # Write to file
         monte_carlo_sampling_generator_filename = (
             self._monte_carlo_sampling_get_generator_filename()
         )
 
-        self.grid_options[
+        self.population_options[
             "_monte_carlo_sampling_generator_filename"
         ] = monte_carlo_sampling_generator_filename
 
-        self.verbose_print(
+        self.vb_info(
             "{blue}Write grid code to {file} {reset}".format(
                 blue=self.ANSI_colours["blue"],
                 file=monte_carlo_sampling_generator_filename,
                 reset=self.ANSI_colours["reset"],
             ),
-            self.grid_options["verbosity"],
-            1,
         )
 
         with self.open(
             monte_carlo_sampling_generator_filename, "w", encoding="utf-8"
         ) as file:
             file.write(self.code_string)
         self.code_string = ""
@@ -216,31 +243,31 @@
                 )
                 self._increment_indent_depth(+1)
 
             # Factor in the custom weight input
             self._add_code(
                 "\n",
                 "# Loop over the repeats\n",
-                'for _ in range(self.grid_options["repeat"]):' + "\n",
+                'for _ in range(self.population_options["repeat"]):' + "\n",
             )
             self._add_code(
                 "_total_starcount += 1\n",
                 indent=1,
             )
 
             if not dry_run:
                 # Handle what is returned, or what is not.
                 self._add_code("yield system_dict\n\n", indent=1)
 
             # If its a dry run, dont do anything with it
             else:
                 # run the hook function, only if given
-                if self.grid_options["dry_run_hook"]:
+                if self.population_options["dry_run_hook"]:
                     self._add_code(
-                        "self.grid_options['dry_run_hook'](self, system_dict)\n\n",
+                        "self.population_options['dry_run_hook'](self, system_dict)\n\n",
                         indent=1,
                     )
                 else:
                     # or pass
                     self._add_code("pass\n\n", indent=1)
 
             self._increment_indent_depth(-1)
@@ -248,32 +275,28 @@
         return self.code_string
 
     def _monte_carlo_sampling_write_generator_parameter(self, sampling_variable):
         """
         Function to write the parameter lines and the pre and postcode around it to the monte carlo sampling generator function.
         """
 
-        self.verbose_print(
+        self.vb_debug(
             "Constructing/adding: {}".format(sampling_variable["parameter_name"]),
-            self.grid_options["verbosity"],
-            2,
         )
 
         ####################
         # Write comment
         self._add_code(
             comment_line, "# Sampling variable {}\n\n".format(sampling_variable["name"])
         )
 
-        self.verbose_print(
+        self.vb_debug(
             "Writing sampling variable {} to monte-carlo sampling generator".format(
                 sampling_variable["parameter_name"]
             ),
-            self.grid_options["verbosity"],
-            1,
         )
 
         ####################
         # Generate top code
         if sampling_variable["topcode"]:
             self._add_code(
                 comment_line,
@@ -319,42 +342,43 @@
     # Management
     def _monte_carlo_sampling_get_sampling_functions_filename(self):
         """
         Returns a filename for the file containing the function to generate values for the variables.
         """
 
         filename = os.path.join(
+            self.population_options["tmp_dir"],
             "binary_c_monte_carlo_sampling_sampling_functions_{population_id}.py".format(
-                population_id=self.grid_options["_population_id"]
+                population_id=self.population_options["_population_id"]
             ),
         )
 
         return filename
 
     def _monte_carlo_sampling_load_sampling_functions_file(self):
         """
         Function to load the sampling functions
         """
 
         # Code to load the generator code
-        self.verbose_print(
+        self.vb_debug(
             message="Load monte-carlo sampling functions from {file}".format(
-                file=self.grid_options[
+                file=self.population_options[
                     "_monte_carlo_sampling_sampling_functions_filename"
                 ]
             ),
-            verbosity=self.grid_options["verbosity"],
-            minimal_verbosity=1,
         )
 
         # Load the module from file and the functions in it.
         spec = importlib.util.spec_from_file_location(
             "binary_c_python_monte_carlo_sampling_functions",
             os.path.join(
-                self.grid_options["_monte_carlo_sampling_sampling_functions_filename"]
+                self.population_options[
+                    "_monte_carlo_sampling_sampling_functions_filename"
+                ]
             ),
         )
         monte_carlo_sampling_functions_file = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(monte_carlo_sampling_functions_file)
 
         # NOTE: the way we are loading and dynamically is i think not fully correct. I have to pass the self in twice.
         # TODO: fix the setting of these functions properly
@@ -377,31 +401,34 @@
                 # Set function as class function
                 setattr(self, obj, getattr(monte_carlo_sampling_functions_file, obj))
                 # Add to dict
                 self.monte_carlo_calc_pdf_cdf_value_array_dict_functions[
                     obj.replace("calc_pdf_cdf_value_array_dict_", "")
                 ] = getattr(monte_carlo_sampling_functions_file, obj)
 
-        # Load handler function
+        # Load calc_sampled_value handler function
         for obj in dir(monte_carlo_sampling_functions_file):
             if obj.startswith("handle_calc_sampled_value"):
                 self.handle_calc_sampled_value = getattr(
                     monte_carlo_sampling_functions_file, obj
                 )
                 break
 
-        # Load handler function
-        for obj in dir(monte_carlo_sampling_functions_file):
-            if obj.startswith("handle_pre_calc"):
-                self.handle_pre_calc = getattr(monte_carlo_sampling_functions_file, obj)
-                # setattr(self, obj, getattr(monte_carlo_sampling_functions_file, obj))
-                # MethodType(func, obj)
-                # MethodType(getattr(monte_carlo_sampling_functions_file, obj), self)
+        # Load pre_calc handler function
+        if self.population_options["monte_carlo_use_pre_calculated_distributions"]:
+            for obj in dir(monte_carlo_sampling_functions_file):
+                if obj.startswith("handle_pre_calc"):
+                    self.handle_pre_calc = getattr(
+                        monte_carlo_sampling_functions_file, obj
+                    )
+                    # setattr(self, obj, getattr(monte_carlo_sampling_functions_file, obj))
+                    # MethodType(func, obj)
+                    # MethodType(getattr(monte_carlo_sampling_functions_file, obj), self)
 
-                break
+                    break
 
     def _monte_carlo_sampling_write_sampling_functions_file(self, dry_run=False):
         """
         Function to write the functions that handle generating the values for each variable
         """
 
         #########
@@ -416,15 +443,15 @@
             "\n\n",
         )
 
         #########
         # Write functions to calculate the values for each parameter.
         for loopnr, sampling_variable_el in enumerate(
             sorted(
-                self.grid_options["_sampling_variables"].items(),
+                self.population_options["_sampling_variables"].items(),
                 key=lambda x: x[1]["sampling_variable_number"],
             )
         ):
 
             sampling_variable = sampling_variable_el[1]
 
             ######################
@@ -437,48 +464,46 @@
             # Call to function to write the calc_sample_value function
             self._monte_carlo_sampling_write_calc_sampled_value_function(
                 sampling_variable
             )
 
             ######################
             # Call to function to write the pre_calc_sample_value function
-            if self.grid_options["monte_carlo_use_pre_calculated_distributions"]:
+            if self.population_options["monte_carlo_use_pre_calculated_distributions"]:
                 self._monte_carlo_sampling_write_pre_calc_function(sampling_variable)
 
         ######################
         # Call to function to write the handle_calc_sample_value wrapper function
         self._monte_carlo_sampling_write_handle_calc_sampled_value_function()
 
         ######################
         # Call to function to write the handle_pre_calc function and other functions
-        if self.grid_options["monte_carlo_use_pre_calculated_distributions"]:
+        if self.population_options["monte_carlo_use_pre_calculated_distributions"]:
             self._monte_carlo_sampling_write_handle_pre_calc_function()
 
             self._monte_carlo_sampling_write_bin_function()
 
             self._monte_carlo_sampling_write_center_function()
 
         #########
         # Write to file
         monte_carlo_sampling_sampling_functions_filename = (
             self._monte_carlo_sampling_get_sampling_functions_filename()
         )
 
-        self.grid_options[
+        self.population_options[
             "_monte_carlo_sampling_sampling_functions_filename"
         ] = monte_carlo_sampling_sampling_functions_filename
 
-        self.verbose_print(
+        self.vb_debug(
             "{blue}Write sampling functions code to {file} {reset}".format(
                 blue=self.ANSI_colours["blue"],
                 file=monte_carlo_sampling_sampling_functions_filename,
                 reset=self.ANSI_colours["reset"],
             ),
-            self.grid_options["verbosity"],
-            1,
         )
 
         with self.open(
             monte_carlo_sampling_sampling_functions_filename, "w", encoding="utf-8"
         ) as file:
             file.write(self.code_string)
 
@@ -566,20 +591,28 @@
         )
 
     def _monte_carlo_sampling_write_bin_function(self):
         """
         Function to write the bin function
         """
 
+        # self._add_code(
+        #     comment_line,
+        #     "def bin(parameter_value_array, parameter_value):\n",
+        #     "    index = np.digitize(parameter_value, bins=parameter_value_array, right=False)-1\n",
+        #     "    center_value = (parameter_value_array[index+1]+parameter_value_array[index])/2\n",
+        #     "    return center_value\n",
+        # )
+
         self._add_code(
             comment_line,
             "def bin(parameter_value_array, parameter_value):\n",
             "    index = np.digitize(parameter_value, bins=parameter_value_array, right=False)-1\n",
-            "    center_value = (parameter_value_array[index+1]+parameter_value_array[index])/2\n",
-            "    return center_value\n",
+            "    binned_value = parameter_value_array[index+1]\n",
+            "    return binned_value\n",
         )
 
     def _monte_carlo_sampling_write_center_function(self):
         """
         Function to write the center function
         """
 
@@ -609,15 +642,15 @@
             "self.pre_calculated_pdf_cdf_value_array_dicts = {}\n",
         )
 
         #######
         # Loop over variables and call them to set the pre-calculated pdf cdf information in the dictionary
         for loopnr, sampling_variable_el in enumerate(
             sorted(
-                self.grid_options["_sampling_variables"].items(),
+                self.population_options["_sampling_variables"].items(),
                 key=lambda x: x[1]["sampling_variable_number"],
             )
         ):
             sampling_variable = sampling_variable_el[1]
 
             #######
             # Write call to specific functions to pre-calculate each pdf/cdf dict
@@ -660,35 +693,35 @@
         )
         self._increment_indent_depth(+1)
 
         #######
         # Call to pdf_cdf_value_array_dict function
         self._add_code(
             comment_line,
-            "if self.grid_options['monte_carlo_use_pre_calculated_distributions']:\n",
+            "if self.population_options['monte_carlo_use_pre_calculated_distributions']:\n",
         )
 
         ######
         # Add calls to the dependency variable's pre-calculated parameter_value_array
         if sampling_variable["dependency_variables"]:
             for dependency_variable in sampling_variable["dependency_variables"]:
                 # Create string for getting the parameter value array
                 string = "self.pre_calculated_pdf_cdf_value_array_dicts['{}']".format(
                     dependency_variable
                 )
 
-                if self.grid_options["_sampling_variables_parameter_names"][
+                if self.population_options["_sampling_variables_parameter_names"][
                     dependency_variable
                 ]["dependency_variables"]:
                     for depth in range(
                         0,
                         len(
-                            self.grid_options["_sampling_variables_parameter_names"][
-                                dependency_variable
-                            ]["dependency_variables"]
+                            self.population_options[
+                                "_sampling_variables_parameter_names"
+                            ][dependency_variable]["dependency_variables"]
                         ),
                     ):
                         string += "['{{:.6f}}'.format(binned_{})]".format(
                             sampling_variable["dependency_variables"][depth]
                         )
 
                 # Add code to get the binned value of the current dependency value
@@ -887,15 +920,15 @@
             self._add_code(
                 comment_line,
                 "nested_pdf_cdf_value_array_dict = {}\n\n",
             )
 
             sampling_variable_dict_based_on_parameter_name = {
                 sampling_variable_el["parameter_name"]: sampling_variable_el
-                for sampling_variable_el in self.grid_options[
+                for sampling_variable_el in self.population_options[
                     "_sampling_variables"
                 ].values()
             }
             dependency_variable_list = [
                 sampling_variable_dict_based_on_parameter_name[dependency_variable_key]
                 for dependency_variable_key in sampling_variable["dependency_variables"]
             ]
@@ -931,17 +964,18 @@
                     "value_array_{} = {}\n\n".format(
                         dependency_variable["name"], dependency_variable["samplerfunc"]
                     ),
                 )
 
                 #######
                 # Set up loop for sampling the distribution function
+                # NOTE: previously there was a center statement here (for {} in center(value_array_{})). Not sure why i did that. I removed it now.
                 self._add_code(
                     comment_line,
-                    "for {} in center(value_array_{}):\n\n".format(
+                    "for {} in value_array_{}:\n\n".format(
                         dependency_variable["name"], dependency_variable["name"]
                     ),
                 )
                 self._increment_indent_depth(+1)
 
                 self._add_code(
                     "{}\n".format(
@@ -1013,15 +1047,15 @@
     def _sample_multiplicity(self, system_dict):
         """
         Function to calculate the multiplicity based on grid choices and random guess
         """
 
         ##############
         # If we choose to use no multiplicity fraction function then we always return multiplicity of 1
-        if self.grid_options["multiplicity_fraction_function"] in [0, "None"]:
+        if self.population_options["multiplicity_fraction_function"] in [0, "None"]:
             return 1
 
         # Otherwise we will get the multiplicity fraction dict sample a random value to determine which multiplicty we have
         multiplicity_dict = self._get_multiplicity_dict(system_dict)
 
         # TODO: this can probably be a oneliner
         multiplicity_list, probability_list = [], []
@@ -1048,44 +1082,53 @@
     # Management functions
     def _monte_carlo_sampling_load_generator(self):
         """
         Function to load the monte_carlo grid
         """
 
         # Code to load the generator code
-        self.verbose_print(
+        self.vb_info(
             message="Load monte-carlo generator function from {file}".format(
-                file=self.grid_options["_monte_carlo_sampling_generator_filename"]
+                file=self.population_options["_monte_carlo_sampling_generator_filename"]
             ),
-            verbosity=self.grid_options["verbosity"],
-            minimal_verbosity=1,
         )
 
         spec = importlib.util.spec_from_file_location(
             "binary_c_python_monte_carlo_sampling_generator",
-            os.path.join(self.grid_options["_monte_carlo_sampling_generator_filename"]),
+            os.path.join(
+                self.population_options["_monte_carlo_sampling_generator_filename"]
+            ),
         )
         monte_carlo_sampling_generator_file = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(monte_carlo_sampling_generator_file)
         generator = monte_carlo_sampling_generator_file.monte_carlo_generator
 
-        self.grid_options["_monte_carlo_sampling_generator"] = generator
-
-        self.verbose_print("Grid code loaded", self.grid_options["verbosity"], 1)
+        self.population_options["_monte_carlo_sampling_generator"] = generator
 
-        # raise NotImplementedError("This functionality is not available yet")
+        self.vb_info("Monte-carlo system generator")
 
     def _monte_carlo_sampling_setup(self):
         """
         Function to prepate the class for a monte-carlo sampling simulation
         """
 
-        print("setup mc sampling")
+        self.vb_info("setup mc sampling")
 
-        # raise NotImplementedError("This functionality is not available yet")
+        # Put in check
+        if len(self.population_options["_sampling_variables"]) == 0:
+            msg = "Error: you haven't defined any sampling variables! Aborting"
+            raise ValueError(msg)
+
+        # Make a dictionary with the names of the sampling variables
+        self.population_options["_sampling_variables_parameter_names"] = {
+            sampling_variable[1]["parameter_name"]: sampling_variable[1]
+            for sampling_variable in self.population_options[
+                "_sampling_variables"
+            ].items()
+        }
 
     def _monte_carlo_sampling_get_generator(self):
         """
         Function to get the generator for the source_file sampling method. Called by _get_generator and used in the actual evolution loop.
         """
 
         # Write the sampling functions file
@@ -1097,15 +1140,15 @@
         # Write generator file
         self._monte_carlo_sampling_write_generator_file()
 
         # Load generator
         self._monte_carlo_sampling_load_generator()
 
         # Get generator file
-        generator = self.grid_options["_monte_carlo_sampling_generator"](
+        generator = self.population_options["_monte_carlo_sampling_generator"](
             self, print_results=False
         )
 
         return generator
 
     ##############
     # misc
@@ -1120,15 +1163,15 @@
         TODO: this can be merged with the original write_binary_c_calls to file ... Have the get_generator handle the setup
         """
 
         #######
         # Start up the generator
         generator = self._get_generator()
 
-        if not self.grid_options["monte_carlo_mass_threshold"] > 0:
+        if not self.population_options["monte_carlo_mass_threshold"] > 0:
             raise ValueError("Cant write MC sampling to file without a mass threshold")
 
         # then if the _system_generator is present, we go through it
         if generator:
             # Write to file
             with self.open(output_file, "w", encoding="utf-8") as file:
                 # Get defaults and clean them, then overwrite them with the set values.
@@ -1142,26 +1185,26 @@
 
                 for system_number, system_dict in enumerate(generator):
                     # update values with current system values
                     full_system_dict.update(system_dict)
 
                     ######
                     # Handle monte-carlo threshold based on evolved mass
-                    if self.grid_options["evolution_type"] == "monte_carlo":
+                    if self.population_options["evolution_type"] == "monte_carlo":
                         # Check based on mass threshold
                         self._monte_carlo_sampling_check_mass_threshold(
                             full_system_dict
                         )
 
                         ######
                         # Check if evolution threshold is reached.
-                        if self.grid_options["_monte_carlo_threshold_reached"]:
+                        if self.population_options["_monte_carlo_threshold_reached"]:
                             break
 
                     #
                     binary_cmdline_string = self._return_argline(full_system_dict)
                     file.write(binary_cmdline_string + "\n")
         else:
-            print("Error. No grid function found!")
+            self.vb_error("Error. No grid function found!")
             raise ValueError
 
         return output_file
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/return_functions.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/return_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     def return_population_settings(self) -> dict:
         """
         Function that returns all the options that have been set.
 
         Can be combined with JSON to make a nice file.
 
         Returns:
-            dictionary containing "bse_options", "grid_options", "custom_options"
+            dictionary containing "bse_options", "population_options", "custom_options"
         """
         options = {
             "bse_options": self.bse_options,
-            "grid_options": self.grid_options,
+            "population_options": self.population_options,
             "custom_options": self.custom_options,
         }
 
         return options
 
     def return_binary_c_defaults(self):
         """
@@ -172,25 +172,20 @@
                 # Check directory, make if necessary
                 os.makedirs(self.custom_options["data_dir"], exist_ok=True)
 
                 settings_fullname = os.path.join(
                     self.custom_options["data_dir"], settings_name
                 )
 
-                print("ok")
-
                 # open locked settings file, then output if we get the lock
                 (f, lock) = self.locked_open_for_write(settings_fullname, vb=True)
-                print("ok")
 
                 if lock and f:
-                    self.verbose_print(
+                    self.vb_info(
                         "Writing settings to {}".format(settings_fullname),
-                        self.grid_options["verbosity"],
-                        1,
                     )
                     json.dump(
                         all_info_cleaned,
                         f,
                         indent=indent,
                         default=binaryc_json_serializer,
                         ensure_ascii=ensure_ascii,
@@ -199,24 +194,20 @@
                 return settings_fullname
 
             # TODO: turn it around and have the exception be within the if statement
             msg = "Exporting all info without passing a value for `outfile` requires custom_options['data_dir'] to be present. That is not the cause. Either set the `data_dir` or pass a value for `outfile` "
             raise ValueError(msg)
 
         else:
-            self.verbose_print(
+            self.vb_info(
                 "Writing settings to {}".format(outfile),
-                self.grid_options["verbosity"],
-                1,
             )
             if not outfile.endswith("json"):
-                self.verbose_print(
+                self.vb_critical(
                     "Error: outfile ({}) must end with .json".format(outfile),
-                    self.grid_options["verbosity"],
-                    0,
                 )
                 raise ValueError
 
             with self.open(outfile, "w") as file:
                 json.dump(
                     all_info_cleaned,
                     file,
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/sampling_variables.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/sampling_variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Main script to provide the sampling variable class extension. Here the sampling variable codebase is defined.
 """
 
 # pylint: disable=E1101
 import json
 from typing import Union
+from warnings import warn
 
 
 class sampling_variables:
     """
     Extension for the Population class containing the code for the sampling variable.
     """
 
@@ -22,27 +23,29 @@
     def _last_sampling_variable(self):
         """
         Function that returns the last sampling variable (i.e. the one with the highest sampling_variable_number)
 
         """
 
         # Get total number of sampling variables
-        number = len(self.grid_options["_sampling_variables"])
+        number = len(self.population_options["_sampling_variables"])
 
         # Get dictionary of grid variable numbers
         # RGI: broken?
-        #sampling_variable_dict = {
+        # sampling_variable_dict = {
         #    sampling_variable["sampling_variable_number"]: sampling_variable
-        #    for sampling_variable in self.grid_options["_sampling_variables"]
-        #}
+        #    for sampling_variable in self.population_options["_sampling_variables"]
+        # }
 
         # Get dictionary of grid variable numbers
         sampling_variable_dict = {
-            self.grid_options['_sampling_variables'][sampling_variable]["sampling_variable_number"]: sampling_variable
-            for sampling_variable in self.grid_options["_sampling_variables"]
+            self.population_options["_sampling_variables"][sampling_variable][
+                "sampling_variable_number"
+            ]: sampling_variable
+            for sampling_variable in self.population_options["_sampling_variables"]
         }
 
         #
         return sampling_variable_dict[number - 1]
 
     def update_sampling_variable(self, name: str, **kwargs) -> None:
         """
@@ -51,26 +54,24 @@
         Args:
             name:
                 name of the grid variable to be changed.
             **kwargs:
                 key-value pairs to override the existing grid variable data. See add_sampling_variable for these names.
         """
 
-        if name in self.grid_options["_sampling_variables"]:
-            sampling_variable = self.grid_options["_sampling_variables"][name]
+        if name in self.population_options["_sampling_variables"]:
+            sampling_variable = self.population_options["_sampling_variables"][name]
 
             # Set the value and print
             for key, value in kwargs.items():
                 sampling_variable[key] = value
-                self.verbose_print(
+                self.vb_info(
                     "Updated grid variable: {}".format(
                         json.dumps(sampling_variable, indent=4, ensure_ascii=False)
                     ),
-                    self.grid_options["verbosity"],
-                    1,
                 )
         else:
             msg = "Unknown sampling variable {} - please create it with the add_sampling_variable() method.".format(
                 name
             )
             raise KeyError(msg)
 
@@ -82,55 +83,51 @@
         Function to delete a sampling variable with the given name.
 
         Args:
             name:
                 name of the sampling variable to be deleted.
         """
 
-        if name in self.grid_options["_sampling_variables"]:
-            del self.grid_options["_sampling_variables"][name]
-            self.verbose_print(
+        if name in self.population_options["_sampling_variables"]:
+            del self.population_options["_sampling_variables"][name]
+            self.vb_info(
                 "Deleted sampling variable: {}".format(name),
-                self.grid_options["verbosity"],
-                1,
             )
         else:
             msg = (
                 "Failed to remove sampling variable {}: please check it exists.".format(
                     name
                 )
             )
             raise ValueError(msg)
 
     def rename_sampling_variable(self, oldname: str, newname: str) -> None:
         """
         Function to rename a sampling variable.
 
         note: this does NOT alter the order
-        of the self.grid_options["_sampling_variables"] dictionary.
+        of the self.population_options["_sampling_variables"] dictionary.
 
         The order in which the sampling variables are loaded into the grid is based on their
         `sampling_variable_number` property
 
         Args:
             oldname:
                 old name of the sampling variable
             newname:
                 new name of the sampling variable
         """
 
-        if oldname in self.grid_options["_sampling_variables"]:
-            self.grid_options["_sampling_variables"][newname] = self.grid_options[
-                "_sampling_variables"
-            ].pop(oldname)
-            self.grid_options["_sampling_variables"][newname]["name"] = newname
-            self.verbose_print(
+        if oldname in self.population_options["_sampling_variables"]:
+            self.population_options["_sampling_variables"][
+                newname
+            ] = self.population_options["_sampling_variables"].pop(oldname)
+            self.population_options["_sampling_variables"][newname]["name"] = newname
+            self.vb_info(
                 "Rename sampling variable: {} to {}".format(oldname, newname),
-                self.grid_options["verbosity"],
-                1,
             )
         else:
             msg = "Failed to rename sampling variable {} to {}.".format(
                 oldname, newname
             )
             raise ValueError(msg)
 
@@ -151,15 +148,15 @@
         topcode: Union[str, None] = None,
         bottomcode: Union[str, None] = None,
         condition: Union[str, None] = None,
         dry_parallel: Union[bool, None] = False,
         dependency_variables: Union[list, None] = None,
     ) -> None:
         """
-        Function to add sampling variables to the grid_options.
+        Function to add sampling variables to the population_options.
 
         The execution of the sampling generation will be through a nested for loop.
         Each of the grid variables will get create a deeper for loop.
 
         The real function that generates the numbers will get written to a new file in the TMP_DIR,
         and then loaded imported and evaluated.
         beware that if you insert some destructive piece of code, it will be executed anyway.
@@ -235,15 +232,15 @@
                     dphasevol = 'dlnM_1'
 
             condition:
                 condition that has to be met in order for the grid generation to continue
 
                 Examples::
 
-                    condition = "self.grid_options['binary']==1"
+                    condition = "self.population_options['binary']==1"
 
             gridtype:
                 Method on how the value range is sampled. Can be either 'edge' (steps starting at
                 the lower edge of the value range) or 'centred'
                 (steps starting at ``lower edge + 0.5 * stepsize``).
 
             dry_parallel:
@@ -258,15 +255,15 @@
             dependency_variables:
                 TODO: describe
         """
 
         # check parameters
         # if False and dphasevol != -1.0 and gridtype == "discrete":
         if dphasevol != -1.0 and gridtype == "discrete":
-            print(
+            self.vb_error(
                 "Error making grid: you have set the phasevol to be not -1 and gridtype to discrete, but a discrete grid has no phasevol calculation. You should only set the gridtype to discrete and not set the phasevol in this case."
             )
 
             self.exit(code=1)
 
         # Add sampling_variable
         sampling_variable = {
@@ -281,15 +278,17 @@
             "dphasevol": dphasevol,
             "condition": condition,
             "gridtype": gridtype,
             "branchpoint": branchpoint,
             "branchcode": branchcode,
             "topcode": topcode,
             "bottomcode": bottomcode,
-            "sampling_variable_number": len(self.grid_options["_sampling_variables"]),
+            "sampling_variable_number": len(
+                self.population_options["_sampling_variables"]
+            ),
             "dry_parallel": dry_parallel,
             "dependency_variables": dependency_variables,
         }
 
         # Check for gridtype input
         allowed_gridtypes = [
             "edge",
@@ -305,25 +304,23 @@
 
         if gridtype not in allowed_gridtypes:
             msg = "Unknown gridtype {gridtype}. Please choose one of: ".format(
                 gridtype=gridtype
             ) + ",".join(allowed_gridtypes)
             raise ValueError(msg)
 
-        # Load it into the grid_options
-        self.grid_options["_sampling_variables"][
+        # Load it into the population_options
+        self.population_options["_sampling_variables"][
             sampling_variable["name"]
         ] = sampling_variable
 
-        self.verbose_print(
+        self.vb_error(
             "Added sampling variable: {}".format(
                 json.dumps(sampling_variable, indent=4, ensure_ascii=False)
             ),
-            self.grid_options["verbosity"],
-            2,
         )
 
     ######################################################################
     # Functions to maintain compatibility with older scripts
     ######################################################################
     def _last_grid_variable(self):
         """
@@ -368,15 +365,15 @@
     def rename_grid_variable(self, oldname: str, newname: str) -> None:
         """
         NOTE: this function exists for backward compatability with older scripts. Please use rename_sampling_variable from now on.
 
         Function to rename a sampling variable. Calls rename_sampling_variable()
 
         note: this does NOT alter the order
-        of the self.grid_options["_sampling_variables"] dictionary.
+        of the self.population_options["_sampling_variables"] dictionary.
 
         The order in which the sampling variables are loaded into the grid is based on their
         `sampling_variable_number` property
 
         Args:
             oldname:
                 old name of the sampling variable
@@ -404,15 +401,15 @@
         bottomcode: Union[str, None] = None,
         condition: Union[str, None] = None,
         dry_parallel: Union[bool, None] = False,
     ) -> None:
         """
         NOTE: this function exists for backward compatability with older scripts. Please use add_sampling_variable from now on.
 
-        Function to add sampling variables to the grid_options. Calls add_sampling_variable().
+        Function to add sampling variables to the population_options. Calls add_sampling_variable().
 
         The execution of the sampling generation will be through a nested for loop.
         Each of the grid variables will get create a deeper for loop.
 
         The real function that generates the numbers will get written to a new file in the TMP_DIR,
         and then loaded imported and evaluated.
         beware that if you insert some destructive piece of code, it will be executed anyway.
@@ -488,15 +485,15 @@
                     dphasevol = 'dlnM_1'
 
             condition:
                 condition that has to be met in order for the grid generation to continue
 
                 Examples::
 
-                    condition = "self.grid_options['binary']==1"
+                    condition = "self.population_options['binary']==1"
 
             gridtype:
                 Method on how the value range is sampled. Can be either 'edge' (steps starting at
                 the lower edge of the value range) or 'centred'
                 (steps starting at ``lower edge + 0.5 * stepsize``).
 
             dry_parallel:
@@ -505,14 +502,20 @@
             topcode:
                 Code added at the very top of the block.
 
             bottomcode:
                 Code added at the very bottom of the block.
         """
 
+        warn(
+            "This function is getting deprecated soon. please use add_sampling_variable",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         self.add_sampling_variable(
             name=name,
             parameter_name=parameter_name,
             longname=longname,
             valuerange=valuerange,
             samplerfunc=samplerfunc,
             probdist=probdist,
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/signal_handling.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/signal_handling.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,33 +28,33 @@
         if sigstring in self.signal_count:
             self.signal_count[sigstring] += 1
         else:
             self.signal_count[sigstring] = 1
 
         # if we receive the signal three times, exit
         if self.signal_count[sigstring] > 3:
-            print("caught > 3 times : exit")
+            self.vb_critical("caught > 3 times : exit")
             self.exit(code=2)
 
-        print(
+        self.vb_info(
             "Child signal {} caught (count {}) handler set in {} [ keys {} ]".format(
                 sigstring,
                 self.signal_count[sigstring],
                 signal_data["where"],
                 ",".join(signal_data.keys()),
             )
         )
 
         # SIGINT should stop the queue nicely
         if signum == signal.SIGINT:
-            self.grid_options["stop_queue"] = True
-            self.grid_options["_killed"] = True
+            self.population_options["stop_queue"] = True
+            self.population_options["_killed"] = True
 
         # propagate signal to parent
-        os.kill(self.grid_options["_main_pid"], signum)
+        os.kill(self.population_options["_main_pid"], signum)
 
     def _parent_signal_handler(self, signal_data, signum, frame):
         """
         Signal handling function for the parent process.
         """
 
         # this function is called by both queues when they
@@ -63,34 +63,34 @@
 
         if sigstring in self.signal_count:
             self.signal_count[sigstring] += 1
         else:
             self.signal_count[sigstring] = 1
 
         if self.signal_count[sigstring] > 3:
-            print("caught > 3 times : exit")
+            self.vb_error("caught > 3 times : exit")
             self.exit(code=2)
 
         # tell the user what has happened
-        print(
+        self.vb_info(
             "Parent signal {} caught (count {}) handler set in {} [ keys {} ]".format(
                 sigstring,
                 self.signal_count[sigstring],
                 signal_data["where"],
                 ",".join(signal_data.keys()),
             )
         )
 
         # set status files
         self.set_status("signal {sig}".format(sig=sigstring))
 
         if signum == signal.SIGINT:
             # caught SIGINT: e.g. CTRL-C or HPC job manager
             # shutting us down
-            print("Parent set stop_queue to True")
-            self.grid_options["stop_queue"] = True
-            self.custom_options["save_snapshot"] = True
-            self.grid_options["_killed"] = True
+            self.vb_info("Parent set stop_queue to True")
+            self.population_options["stop_queue"] = True
+            self.population_options["save_snapshot"] = True
+            self.population_options["_killed"] = True
             return
         else:
             # what to do?
             return
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/slurm.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/slurm.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,56 +29,56 @@
         Init function for the slurm class
         """
 
         return
 
     def slurmID(self, jobid=None, jobarrayindex=None):
         """
-        Function to return a Slurm job ID as a string, [jobid].[jobarrayindex]. The jobid and jobarrayindex passed in are used if given, otherwise we default to the jobid and jobarrayindex in grid_options.
+        Function to return a Slurm job ID as a string, [jobid].[jobarrayindex]. The jobid and jobarrayindex passed in are used if given, otherwise we default to the jobid and jobarrayindex in population_options.
         """
         if jobid is None:
-            jobid = self.grid_options["slurm_jobid"]
+            jobid = self.population_options["slurm_jobid"]
         if jobarrayindex is None:
-            jobarrayindex = self.grid_options["slurm_jobarrayindex"]
+            jobarrayindex = self.population_options["slurm_jobarrayindex"]
         return "{jobid}.{jobarrayindex}".format(
             jobid=jobid, jobarrayindex=jobarrayindex
         )
 
     def slurmpath(self, path, slurm_dir=None):
         """
         Function to return the full slurm directory path.
         """
         if slurm_dir is None:
-            slurm_dir = self.grid_options["slurm_dir"]
+            slurm_dir = self.population_options["slurm_dir"]
 
         return os.path.abspath(os.path.join(slurm_dir, path))
 
     def slurm_status_file(self, jobid=None, jobarrayindex=None, slurm_dir=None):
         """
-        Return the slurm status file corresponding to the jobid and jobarrayindex, which default to grid_options slurm_jobid and slurm_jobarrayindex, respectively.
+        Return the slurm status file corresponding to the jobid and jobarrayindex, which default to population_options slurm_jobid and slurm_jobarrayindex, respectively.
         """
         return os.path.join(
             self.slurmpath("status", slurm_dir=slurm_dir),
             self.slurmID(jobid=jobid, jobarrayindex=jobarrayindex),
         )
 
     def slurm_check_requirements(self):
         """
-        Function to check whether the slurm parameters in grid_options have been set appropriately.
+        Function to check whether the slurm parameters in population_options have been set appropriately.
         """
 
-        if self.grid_options["slurm"] > 0 and (
-            self.grid_options["slurm_dir"] is None
-            or not os.path.isdir(self.grid_options["slurm_dir"])
+        if self.population_options["slurm"] > 0 and (
+            self.population_options["slurm_dir"] is None
+            or not os.path.isdir(self.population_options["slurm_dir"])
         ):
             return (
                 False,
                 "You have set slurm={slurm} but not set slurm_dir ({slurm_dir}) correctly. Please set it and try again.".format(
-                    slurm=self.grid_options["slurm"],
-                    slurm_dir=self.grid_options["slurm_dir"],
+                    slurm=self.population_options["slurm"],
+                    slurm_dir=self.population_options["slurm_dir"],
                 ),
             )
         return (True, "")
 
     def slurm_dirs(self):
         """
         Directories associated specifically with this slurm job.
@@ -91,45 +91,47 @@
 
         Args:
             string : the status string to be set
             slurm_dir : the directory in which the status directory is held. If not set, this defaults to the HPC directory (e.g. slurm_dir or condor_dir).
         """
         # save slurm jobid to file
         if slurm_dir is None:
-            slurm_dir = self.grid_options["slurm_dir"]
+            slurm_dir = self.population_options["slurm_dir"]
 
         idfile = os.path.join(slurm_dir, "jobid")
         if not os.path.exists(idfile):
             with self.open(idfile, "w", encoding="utf-8") as fjobid:
-                fjobid.write("{jobid}\n".format(jobid=self.grid_options["slurm_jobid"]))
+                fjobid.write(
+                    "{jobid}\n".format(jobid=self.population_options["slurm_jobid"])
+                )
                 fjobid.close()
                 self.NFS_flush_hack(idfile)
 
         # save slurm status
         status_file = self.slurm_status_file(slurm_dir=slurm_dir)
         if status_file:
             with self.open(status_file, "w", encoding="utf-8") as f:
                 f.write(string)
                 f.close()
                 self.NFS_flush_hack(status_file)
 
-        print("Have set status in", status_file, "to", string)
+        self.vb_info("Have set status in {} to {}".format(status_file, string))
         with self.open(status_file, "r", encoding="utf-8") as f:
-            print("Contents")
-            print(f.readlines())
+            self.vb_info("Contents")
+            self.vb_info(f.readlines())
             f.close()
 
     def get_slurm_status(self, jobid=None, jobarrayindex=None, slurm_dir=None):
         """
         Get and return the slurm status string corresponing to the self object, or jobid.jobarrayindex if they are passed in. If no status is found, returns an empty string.
         """
         if jobid is None:
-            jobid = self.grid_options["slurm_jobid"]
+            jobid = self.population_options["slurm_jobid"]
         if jobarrayindex is None:
-            jobarrayindex = self.grid_options["slurm_jobarrayindex"]
+            jobarrayindex = self.population_options["slurm_jobarrayindex"]
         if jobid is None or jobarrayindex is None:
             return None
         try:
 
             path = pathlib.Path(
                 self.slurm_status_file(
                     slurm_dir=slurm_dir, jobid=jobid, jobarrayindex=jobarrayindex
@@ -147,30 +149,30 @@
         """
         return a standard filename for the slurm chunk files
         """
         file = "{id}.gz".format(
             id=self.slurmID(),
         )
         if slurm_dir is None:
-            slurm_dir = self.grid_options["slurm_dir"]
+            slurm_dir = self.population_options["slurm_dir"]
         return os.path.abspath(os.path.join(slurm_dir, "results", file))
 
     def make_slurm_dirs(self, slurm_dir=None):
         """
         Function to create the necessary slurm directories
         """
 
         # TODO: replace the code block below with a function call to slurmpath
         # make the slurm directories
         if slurm_dir is None:
-            slurm_dir = self.grid_options["slurm_dir"]
+            slurm_dir = self.population_options["slurm_dir"]
 
         if not slurm_dir:
-            print(
-                "You must set self.grid_options['slurm_dir'] (or pass slurm_dir=whatever to make_slurm_dirs()) to a directory which we can use to set up binary_c-python's Slurm files. This should be unique to your set of grids."
+            self.vb_error(
+                "You must set self.population_options['slurm_dir'] (or pass slurm_dir=whatever to make_slurm_dirs()) to a directory which we can use to set up binary_c-python's Slurm files. This should be unique to your set of grids."
             )
             os.exit()
 
         # make a list of directories, these contain the various slurm
         # output, status files, etc.
         dirs = []
         for slurm_subdir in ["stdout", "stderr", "results", "status", "snapshots"]:
@@ -181,15 +183,15 @@
         for d in dirs:
             try:
                 pathlib.Path(self.slurmpath(d, slurm_dir=slurm_dir)).mkdir(
                     exist_ok=False, parents=True
                 )
             # TODO: fix this bare exception
             except:
-                print(
+                self.vb_error(
                     "Tried to make the directory {d} but it already exists. When you launch a set of binary_c jobs on Slurm, you need to set your slurm_dir to be a fresh directory with no contents.".format(
                         d=d
                     )
                 )
                 self.exit(code=1)
 
         # check that they have been made and exist: we need this
@@ -198,123 +200,123 @@
         fail = True
         count = 0
         count_warn = 10
         while fail is True:
             fail = False
             count += 1
             if count > count_warn:
-                print(
+                self.vb_warning(
                     "Warning: Have been waiting about {count} seconds for Slurm directories to be made, there seems to be significant delay...".format(
                         count=count
                     )
                 )
             for d in dirs:
                 if os.path.isdir(d) is False:
                     fail = True
                     time.sleep(1)
                     break
 
     def slurm_grid(self):  # pragma: no cover
         """
-        function to be called when running grids when grid_options['slurm']>=1
+        function to be called when running grids when population_options['slurm']>=1
 
-        if grid_options['slurm']==1, we set up the slurm script and launch the jobs, then return True to exit.
-        if grid_options['slurm']==2, we run the stars, which means we return False to continue.
-        if grid_options['slurm']==3, we are being called from the jobs to run the grids, return False to continue.
+        if population_options['slurm']==1, we set up the slurm script and launch the jobs, then return True to exit.
+        if population_options['slurm']==2, we run the stars, which means we return False to continue.
+        if population_options['slurm']==3, we are being called from the jobs to run the grids, return False to continue.
 
         TODO: split this function into some parts
         TODO: Comment this function better
         """
 
-        if self.grid_options["slurm"] == 2:
+        if self.population_options["slurm"] == 2:
             # run a grid of stars only, leaving the results
             # in the appropriate outfile
             return False
 
-        if self.grid_options["slurm"] == 3:
+        if self.population_options["slurm"] == 3:
             # joining : set the evolution type to "join" and return
             # False to continue
-            self.grid_options["evolution_type"] = "join"
+            self.population_options["evolution_type"] = "join"
             return False
 
-        if self.grid_options["slurm"] == 1:
+        if self.population_options["slurm"] == 1:
             # if slurm=1,  we should have no evolution type, we
             # set up the Slurm scripts and get them evolving
             # in a Slurm array
-            self.grid_options["evolution_type"] = None
+            self.population_options["evolution_type"] = None
 
             # make dirs
             self.make_slurm_dirs()
 
             # check we're not using too much RAM
-            if datasize.DataSize(self.grid_options["slurm_memory"]) > datasize.DataSize(
-                self.grid_options["slurm_warn_max_memory"]
-            ):
-                print(
+            if datasize.DataSize(
+                self.population_options["slurm_memory"]
+            ) > datasize.DataSize(self.population_options["slurm_warn_max_memory"]):
+                self.vb_error(
                     "WARNING: you want to use {slurm_memory} MB of RAM : this is unlikely to be correct. If you believe it is, set slurm_warn_max_memory to something very large (it is currently {slurm_warn_max_memory} MB)\n".format(
-                        slurm_memory=self.grid_options["slurm_memory"],
-                        slurm_warn_max_memory=self.grid_options[
+                        slurm_memory=self.population_options["slurm_memory"],
+                        slurm_warn_max_memory=self.population_options[
                             "slurm_warn_max_memory"
                         ],
                     )
                 )
                 self.exit(code=1)
 
             # set up slurm_array
-            if not self.grid_options["slurm_array_max_jobs"]:
-                self.grid_options["slurm_array_max_jobs"] = self.grid_options[
-                    "slurm_njobs"
-                ]
-                slurm_array = self.grid_options[
+            if not self.population_options["slurm_array_max_jobs"]:
+                self.population_options[
+                    "slurm_array_max_jobs"
+                ] = self.population_options["slurm_njobs"]
+                slurm_array = self.population_options[
                     "slurm_array"
                 ] or "1-{njobs}%{max_jobs}".format(
-                    njobs=self.grid_options["slurm_njobs"],
-                    max_jobs=self.grid_options["slurm_array_max_jobs"],
+                    njobs=self.population_options["slurm_njobs"],
+                    max_jobs=self.population_options["slurm_array_max_jobs"],
                 )
 
             # get job array index
-            jobarrayindex = self.grid_options["slurm_jobarrayindex"]
+            jobarrayindex = self.population_options["slurm_jobarrayindex"]
             if jobarrayindex is None:
                 jobarrayindex = "$SLURM_ARRAY_TASK_ID"
 
-            if self.grid_options["slurm_njobs"] == 0:
-                print(
+            if self.population_options["slurm_njobs"] == 0:
+                self.vb_error(
                     "binary_c-python Slurm : You must set grid_option slurm_njobs to be non-zero"
                 )
                 self.exit(code=1)
 
             # build the grid command
             grid_command = (
                 [
-                    str(self.grid_options["slurm_env"]),
+                    str(self.population_options["slurm_env"]),
                     sys.executable,
                     str(lib_programname.get_path_executed_script()),
                 ]
                 + sys.argv[1:]
                 + [
                     "start_at=$((" + str(jobarrayindex) + "-1))",
-                    "modulo=" + str(self.grid_options["slurm_njobs"]),
-                    "slurm_njobs=" + str(self.grid_options["slurm_njobs"]),
-                    "slurm_dir=" + self.grid_options["slurm_dir"],
-                    "verbosity=" + str(self.grid_options["verbosity"]),
-                    "num_cores=" + str(self.grid_options["num_processes"]),
+                    "modulo=" + str(self.population_options["slurm_njobs"]),
+                    "slurm_njobs=" + str(self.population_options["slurm_njobs"]),
+                    "slurm_dir=" + self.population_options["slurm_dir"],
+                    "verbosity=" + str(self.population_options["verbosity"]),
+                    "num_cores=" + str(self.population_options["_num_processes"]),
                 ]
             )
 
             # wrap command arguments in quotes
             grid_command = command_string_from_list(grid_command)
 
             # make slurm script
             scriptpath = self.slurmpath("slurm_script")
             try:
                 script = self.open(scriptpath, "w", encoding="utf-8")
             except IOError:
-                print(
+                self.vb_warning(
                     "Could not open Slurm script at {path} for writing: please check you have set {slurm_dir} correctly (it is currently {slurm_dir} and can write to this directory.".format(
-                        path=scriptpath, slurm_dir=self.grid_options["slurm_dir"]
+                        path=scriptpath, slurm_dir=self.population_options["slurm_dir"]
                     )
                 )
 
             slurmscript = """#!{bash}
 # Slurm launch script created by binary_c-python
 
 # Slurm options
@@ -324,28 +326,28 @@
 #SBATCH --partition={slurm_partition}
 #SBATCH --time={slurm_time}
 #SBATCH --mem={slurm_memory}
 #SBATCH --ntasks={slurm_ntasks}
 #SBATCH --array={slurm_array}
 #SBATCH --cpus-per-task={ncpus}
 """.format(
-                bash=self.grid_options["slurm_bash"],
-                slurm_dir=self.grid_options["slurm_dir"],
-                slurm_jobname=self.grid_options["slurm_jobname"],
-                slurm_partition=self.grid_options["slurm_partition"],
-                slurm_time=self.grid_options["slurm_time"],
-                slurm_ntasks=self.grid_options["slurm_ntasks"],
-                slurm_memory=self.grid_options["slurm_memory"],
+                bash=self.population_options["slurm_bash"],
+                slurm_dir=self.population_options["slurm_dir"],
+                slurm_jobname=self.population_options["slurm_jobname"],
+                slurm_partition=self.population_options["slurm_partition"],
+                slurm_time=self.population_options["slurm_time"],
+                slurm_ntasks=self.population_options["slurm_ntasks"],
+                slurm_memory=self.population_options["slurm_memory"],
                 slurm_array=slurm_array,
-                ncpus=self.grid_options["num_processes"],
+                ncpus=self.population_options["_num_processes"],
             )
 
-            for key in self.grid_options["slurm_extra_settings"]:
+            for key in self.population_options["slurm_extra_settings"]:
                 slurmscript += "#SBATCH --{key} = {value}\n".format(
-                    key=key, value=self.grid_options["slurm_extra_settings"][key]
+                    key=key, value=self.population_options["slurm_extra_settings"][key]
                 )
 
             slurmscript += """
 
 export BINARY_C_PYTHON_ORIGINAL_CMD_LINE={cmdline}
 export BINARY_C_PYTHON_ORIGINAL_WD=`{pwd}`
 export BINARY_C_PYTHON_ORIGINAL_SUBMISSION_TIME=`{date}`
@@ -354,25 +356,25 @@
 echo \"running\" > "{slurm_dir}/status/$SLURM_ARRAY_JOB_ID.$SLURM_ARRAY_TASK_ID"
 
 # make list of files which is checked for joining
 # echo "{slurm_dir}/results/$SLURM_ARRAY_JOB_ID.$SLURM_ARRAY_TASK_ID.gz" >> "{slurm_dir}/results/$SLURM_ARRAY_JOB_ID.all"
 
 # run grid of stars and, if this returns 0, set status to finished
 {grid_command} "slurm=2" "evolution_type=grid" "slurm_jobid=$SLURM_ARRAY_JOB_ID" "slurm_jobarrayindex=$SLURM_ARRAY_TASK_ID" "save_population_object={slurm_dir}/results/$SLURM_ARRAY_JOB_ID.$SLURM_ARRAY_TASK_ID.gz" && echo -n \"finished\" > "{slurm_dir}/status/$SLURM_ARRAY_JOB_ID.$SLURM_ARRAY_TASK_ID" && echo """.format(
-                slurm_dir=self.grid_options["slurm_dir"],
+                slurm_dir=self.population_options["slurm_dir"],
                 grid_command=grid_command,
-                cmdline=repr(self.grid_options["command_line"]),
-                date=self.grid_options["slurm_date"],
-                pwd=self.grid_options["slurm_pwd"],
+                cmdline=repr(self.population_options["command_line"]),
+                date=self.population_options["slurm_date"],
+                pwd=self.population_options["slurm_pwd"],
             )
 
-            if not self.grid_options["slurm_postpone_join"]:
+            if not self.population_options["slurm_postpone_join"]:
                 slurmscript += """&& echo \"Checking if we can join...\" && echo && {grid_command} "slurm=3" "evolution_type=join" "joinlist={slurm_dir}/results/$SLURM_ARRAY_JOB_ID.all" "slurm_jobid=$SLURM_ARRAY_JOB_ID" "slurm_jobarrayindex=$SLURM_ARRAY_TASK_ID"
                 """.format(
-                    slurm_dir=self.grid_options["slurm_dir"],
+                    slurm_dir=self.population_options["slurm_dir"],
                     grid_command=grid_command,
                 )
             else:
                 slurmscript += "\n"
 
             # write to script, close it and make it executable by
             # all (so the slurm user can pick it up)
@@ -385,17 +387,17 @@
                 | stat.S_IEXEC
                 | stat.S_IRGRP
                 | stat.S_IXGRP
                 | stat.S_IROTH
                 | stat.S_IXOTH,
             )
 
-            if not self.grid_options["slurm_postpone_sbatch"]:
+            if not self.population_options["slurm_postpone_sbatch"]:
                 # call sbatch to launch the jobs
-                cmd = [self.grid_options["slurm_sbatch"], scriptpath]
+                cmd = [self.population_options["slurm_sbatch"], scriptpath]
 
                 with subprocess.Popen(
                     cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE
                 ) as pipes:
 
                     std_out, std_err = pipes.communicate()
                     if pipes.returncode != 0:
@@ -405,45 +407,45 @@
                             code=pipes.returncode,
                             red=self.ANSI_colours["red"],
                             reset=self.ANSI_colours["reset"],
                         )
                         raise Exception(err_msg)
 
                 if len(std_err):
-                    print(
+                    self.vb_info(
                         "{red}{err}{reset}".format(
                             red=self.ANSI_colours["red"],
                             reset=self.ANSI_colours["reset"],
                             err=std_err.strip().decode("utf-8"),
                         )
                     )
 
-                print(
+                self.vb_info(
                     "{yellow}{out}{reset}".format(
                         yellow=self.ANSI_colours["yellow"],
                         reset=self.ANSI_colours["reset"],
                         out=std_out.strip().decode("utf-8"),
                     )
                 )
             else:
                 # just say we would have (use this for testing)
-                print(
+                self.vb_warning(
                     "Slurm script is at {path} but has not been launched".format(
                         path=scriptpath
                     )
                 )
 
         # some messages to the user, then return
-        if self.grid_options["slurm_postpone_sbatch"] == 1:
-            print(
+        if self.population_options["slurm_postpone_sbatch"] == 1:
+            self.vb_info(
                 "Slurm script written, but launching the jobs with sbatch was postponed."
             )
         else:
-            print("Slurm jobs launched")
-            print("All done in slurm_grid().")
+            self.vb_info("Slurm jobs launched")
+            self.vb_info("All done in slurm_grid().")
 
         # return True so we exit immediately
         return True
 
     def slurm_queue_stats(self):  # pragma: no cover
         """
         Function to XXX
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/spacing_functions.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/spacing_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from typing import Union
 
 import cachetools
 import diskcache
 import numpy as np
 import py_rinterpolate
 
+from binarycpython.utils.functions import output_lines
+
 
 class spacing_functions:
     """
     Extension for the Population class containing the code for spacing functions
     """
 
     def __init__(self, **kwargs):
@@ -195,15 +197,15 @@
             fsample: a global sampling (Shannon-like) factor (<1) to improve resolution (default 1.0, set to smaller to improve resolution)
             factor: all masses generated are multiplied by this after generation
             showtable: if True, the mass list and times are shown to stdout after generation
             showlist: if True, show the mass list once generated
             logmasses: if True, the masses are logged with math.log()
             log10masses: if True, the masses are logged with math.log10()
             usecache: if True (the default) uses cached results if they are saved (in cachedir) and cachedir is not None
-            cachedir: where the cache is stored. if None, defaults to grid_options['cache_dir']+'/const_dt_cache'
+            cachedir: where the cache is stored. if None, defaults to population_options['cache_dir']+'/const_dt_cache'
             vb : verbose logging flag (default False)
 
         Returns:
             Array of masses.
 
         Example:
             these are lines set as options to Population.add_grid_value(...)::
@@ -214,24 +216,24 @@
                 # logarithmic spacing in time, generally suitable for Galactic chemical evolution yield grids.
                 samplerfunc="self.const_dt(self,dlogt=0.1,nres=100,mmin=0.07,mmax=80.0,maxdm=((0.07,1.0,0.1),(1.0,10.0,1.0),(10.0,80.0,2.0)),showtable=True,logspacing=True,fsample=1.0/4.0)"
 
         """
 
         if usecache:
             if cachedir is None:
-                cachedir = self.grid_options["cache_dir"]
+                cachedir = self.population_options["cache_dir"]
 
             if cachedir is not None:
                 cachedir += "/const_dt_cache"
                 cache = diskcache.Cache(cachedir)
-                print(
+                self.vb_info(
                     "Use const_dt cache in {} [cache object {}]".format(cachedir, cache)
                 )
             else:
-                print("const_dt uses no cache")
+                self.vb_info("const_dt uses no cache")
                 cache = None
 
         def _const_dt_wrapper(
             cachedir=None,
             num_cores=None,
             bse_options=None,
             dt=1000.0,
@@ -254,15 +256,15 @@
             usecache=True,
             vb=False,
         ):
             """
             Wrapper function for the const_dt funtion which handles verbose logging and filtering of arguments
             """
 
-            print(
+            self.vb_debug(
                 "call _const_dt num_cores={} dt={} dlogt={} mmin={} mmax={} nres={} logspacing={} tmin={} mindm={} maxdm={} fsample={} factor={} logmasses={} log10masses={} showlist={} usecache={} [cache={} vb={}]".format(
                     num_cores,
                     dt,
                     dlogt,
                     mmin,
                     mmax,
                     nres,
@@ -295,15 +297,15 @@
 
             # make a JSON string of the options (this can be
             # used to check the cache)
             bse_options_json = json.dumps(
                 bse_stripped, sort_keys=True, ensure_ascii=False
             )
             if vb:
-                print("BSE options JSON:", bse_options_json)
+                self.vb_info("BSE options JSON:", bse_options_json)
 
             return _const_dt(
                 cachedir=cachedir,
                 num_cores=num_cores,
                 bse_options_json=bse_options_json,
                 dt=dt,
                 dlogt=dlogt,
@@ -435,76 +437,84 @@
             # set up the parse function
             def _parse_function(self, output):
                 """
                 Parse function for the const_dt binary_c calls
                 """
 
                 if output:
-                    for line in output.splitlines():
+                    for line in output_lines(output):
                         data = line.split()
                         if data[0] == "SINGLE_STAR_LIFETIME":
                             # append (log10(mass), log10(lifetime)) tuples
                             logm = math.log10(float(data[1]))
                             logt = math.log10(float(data[2]))
-                            # print(line)
-                            # print("logM=",logm,"M=",10.0**logm," -> logt=",logt)
-                            self.grid_results["interpolation table m->t"][logm] = logt
-                            self.grid_results["interpolation table t->m"][logt] = logm
+
+                            self.population_results["interpolation table m->t"][
+                                logm
+                            ] = logt
+                            self.population_results["interpolation table t->m"][
+                                logt
+                            ] = logm
 
             lifetime_population.set(
                 parse_function=_parse_function,
             )
 
             # run to build the interpolation table
-            print(
+            self.vb_info(
                 "Running population to make lifetime interpolation table, please wait"
             )
             lifetime_population.evolve()
-            # print("Data table",lifetime_population.grid_results['interpolation table t->m'])
 
             if (
-                "interpolation table t->m" not in lifetime_population.grid_results
+                "interpolation table t->m" not in lifetime_population.population_results
                 or len(
-                    lifetime_population.grid_results["interpolation table t->m"].keys()
+                    lifetime_population.population_results[
+                        "interpolation table t->m"
+                    ].keys()
                 )
                 == 0
             ):
-                print(
+                self.vb_error(
                     "\n\n\nError: The t->m lifetime table is empty. One usual cause for this is that the tmax or max_evolution_time option (currently passed in to const_dt as {tmax}) is too short for there to be any entries in the table before the first timestep. Try increasing tmax and max_evolution_time, shorten the timestep or, if using log times, set tstart to be closer to 0.\n".format(
                         tmax=tmax
                     )
                 )
                 sys.exit()
 
             # convert to nested lists for the interpolator
             #
             # make time -> mass table
             data_table_time_mass = []
             times = sorted(
-                lifetime_population.grid_results["interpolation table t->m"].keys()
+                lifetime_population.population_results[
+                    "interpolation table t->m"
+                ].keys()
             )
             for time in times:
-                mass = lifetime_population.grid_results["interpolation table t->m"][
-                    time
-                ]
+                mass = lifetime_population.population_results[
+                    "interpolation table t->m"
+                ][time]
                 # we have to make sure the time is monotonic (not guaranteed at high mass)
                 if len(data_table_time_mass) == 0:
                     data_table_time_mass.append([time, mass])
                 elif mass < data_table_time_mass[-1][1]:
                     data_table_time_mass.append([time, mass])
 
             # make mass -> time table
             data_table_mass_time = []
             masses = sorted(
-                lifetime_population.grid_results["interpolation table m->t"].keys()
+                lifetime_population.population_results[
+                    "interpolation table m->t"
+                ].keys()
             )
             for mass in masses:
-                time = lifetime_population.grid_results["interpolation table m->t"][
-                    mass
-                ]
+                time = lifetime_population.population_results[
+                    "interpolation table m->t"
+                ][mass]
                 data_table_mass_time.append([mass, time])
 
             # set up interpolators
             interpolator_time_mass = py_rinterpolate.Rinterpolate(
                 table=data_table_time_mass,
                 nparams=1,
                 ndata=1,
@@ -626,26 +636,26 @@
             if showtable:
                 twas = 0.0
                 logtwas = 0.0
                 for i, m in enumerate(mass_list):
                     t = _time_from_mass(m)
                     logt = math.log10(t)
                     if twas > 0.0:
-                        print(
+                        self.vb_debug(
                             "{i:4d} m={m:13g} t={t:13g} log10(t)={logt:13g} dt={dt:13g} dlog10(t)={dlogt:13g}".format(
                                 i=i,
                                 m=m,
                                 t=t,
                                 logt=logt,
                                 dt=twas - t,
                                 dlogt=logtwas - logt,
                             )
                         )
                     else:
-                        print(
+                        self.vb_debug(
                             "{i:4d} m={m:13g} t={t:13g} log10(t)={logt:13g}".format(
                                 i=i, m=m, t=t, logt=logt
                             )
                         )
                         twas = t
                         logtwas = logt
                     sys.exit()
@@ -667,18 +677,20 @@
         #       use the cached result.
         #
         # Note: we send a sorted JSON string instead of the
         #       bse_options dict to make sure the order is preserved
 
         mass_list = _const_dt_wrapper(
             cachedir=cachedir,
-            num_cores=self.grid_options["num_cores"],
+            num_cores=self.population_options["num_cores"],
             bse_options=self.bse_options,
             **kwargs,
         )
         if cache:
             cache.close()
 
         if kwargs.get("showlist", True):
-            print("const_dt mass list ({} masses)\n".format(len(mass_list)), mass_list)
+            self.vb_debug(
+                "const_dt mass list ({} masses)\n".format(len(mass_list)), mass_list
+            )
 
         return mass_list
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/termination_functions.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/termination_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,57 +21,61 @@
         return
 
     def was_killed(self):
         """
         Function to determine if the process was killed. Returns True if so, false otherwise.
         """
 
-        killed = self.grid_options["_killed"]
+        killed = self.population_options["_killed"]
 
         if "_killed" in self.grid_ensemble_results.get("metadata", {}):
             killed = killed or self.grid_ensemble_results["metadata"]["_killed"]
 
         return killed
 
     def exit(self, code=None, message=True, flush=True, stacktrace=False):
         """
         Exit function: use this to exit from a Population object.
         Really it's just a wrapper for sys.exit() to return the correct exit code,
         but also to post a message (if message is True, default is True)
         and perhaps a stacktrace (if stacktrace is True, default is False).
         """
+
         # if we've been killed, set exit code to 1
-        if self.grid_options["exit_code"] == 0 and self.grid_options["_killed"]:
-            self.grid_options["exit_code"] = 1
+        if (
+            self.population_options["exit_code"] == 0
+            and self.population_options["_killed"]
+        ):
+            self.population_options["exit_code"] = 1
         # but override with code passed in
         if code:
-            self.grid_options["exit_code"] = code
+            self.population_options["exit_code"] = code
         if message:
-            print(
+            self.vb_error(
                 "exit from binary_c-python Population with code {}".format(
-                    self.grid_options["exit_code"]
+                    self.population_options["exit_code"]
                 )
             )
         if flush:
             sys.stdout.flush()
-        if stacktrace or self.grid_options["print_stack_on_exit"]:
+        if stacktrace or self.population_options["print_stack_on_exit"]:
             traceback.print_stack()
-        sys.exit(self.grid_options["exit_code"])
+        sys.exit(self.population_options["exit_code"])
 
     def _all_children_running(self, processes):
         """
         Function to test if all child processes are running.
         """
 
         for p in processes:
             if p.is_alive() is False and p.exitcode != 0:
-                print(
-                    "Warning: process",
-                    p,
-                    "is no longer alive and hasn't returned good data.",
+                self.vb_warning(
+                    "Warning: process {} is no longer alive and hasn't returned good data.".format(
+                        p
+                    )
                 )
                 self._log_failure(process=p, exitcode=p.exitcode)
                 return False
 
         return True
 
     def _kill_child_processes(self, processes):
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/population_extensions/version_info.py` & `binarycpython-1.0.0/binarycpython/utils/population_extensions/version_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,64 +42,63 @@
             parsed: Boolean flag whether to parse the version_info output of binary_c. default = False
 
         Returns:
             Either the raw string of binary_c or a parsed version of this in the form of a nested
             dictionary
         """
 
-        found_prev = False
+        #####
+        # Check if the headers were previously defined
+        found_prev_MACRO_HEADER = False
         if "BINARY_C_MACRO_HEADER" in os.environ:
             # the env var is already present. lets save that and put that back later
-            found_prev = True
-            prev_value = os.environ["BINARY_C_MACRO_HEADER"]
+            found_prev_MACRO_HEADER = True
+            prev_value_MACRO_HEADER = os.environ["BINARY_C_MACRO_HEADER"]
 
-        #
+        found_prev_DEFLIST_HEADER = False
+        if "BINARY_C_DEFLIST_HEADER" in os.environ:
+            # the env var is already present. lets save that and put that back later
+            found_prev_DEFLIST_HEADER = True
+            prev_value_DEFLIST_HEADER = os.environ["BINARY_C_DEFLIST_HEADER"]
+
+        #############
+        # set new headers
         os.environ["BINARY_C_MACRO_HEADER"] = "macroxyz"
+        os.environ["BINARY_C_DEFLIST_HEADER"] = "deflist "
 
+        #############
         # Get version_info
         raw_version_info = _binary_c_bindings.return_version_info().strip()
 
-        # delete value
+        #############
+        # delete current headers
         del os.environ["BINARY_C_MACRO_HEADER"]
+        del os.environ["BINARY_C_DEFLIST_HEADER"]
 
-        # put stuff back if we found a previous one
-        if found_prev:
-            os.environ["BINARY_C_MACRO_HEADER"] = prev_value
+        #############
+        # put back previous headers
+        if found_prev_MACRO_HEADER:
+            os.environ["BINARY_C_MACRO_HEADER"] = prev_value_MACRO_HEADER
 
-        # parse if wanted
+        if found_prev_DEFLIST_HEADER:
+            os.environ["BINARY_C_DEFLIST_HEADER"] = prev_value_DEFLIST_HEADER
+
+        ##############
+        # return (parsed) version info
         if parsed:
             parsed_version_info = self.parse_binary_c_version_info(raw_version_info)
             return parsed_version_info
 
         return raw_version_info
 
-    def parse_binary_c_version_info(self, version_info_string: str) -> dict:
+    def _parse_binary_c_version_info_networks(self, networks):
         """
-        Function that parses the binary_c version info. Long function with a lot of branches
-
-        Args:
-            version_info_string: raw output of version_info call to binary_c
-
-        Returns:
-            Parsed version of the version info, which is a dictionary containing the keys: 'isotopes' for isotope info, 'argpairs' for argument pair info (TODO: explain), 'ensembles' for ensemble settings/info, 'macros' for macros, 'elements' for atomic element info, 'DTlimit' for (TODO: explain), 'nucleosynthesis_sources' for nucleosynthesis sources, and 'miscellaneous' for all those that were not caught by the previous groups. 'git_branch', 'git_build', 'revision' and 'email' are also keys, but its clear what those contain.
+        Function to parse the networks info
         """
 
-        version_info_dict = {}
-
-        # Clean data and put in correct shape
-        splitted = version_info_string.strip().splitlines()
-        cleaned = {el.strip() for el in splitted if not el == ""}
-
-        ##########################
-        # Network:
-        # Split off all the networks and parse the info.
-
-        networks = {el for el in cleaned if el.startswith("Network ")}
-        cleaned = cleaned - networks
-
         networks_dict = {}
         for el in networks:
             network_dict = {}
             split_info = el.split("Network ")[-1].strip().split("==")
 
             network_number = int(split_info[0])
             network_dict["network_number"] = network_number
@@ -120,21 +119,21 @@
                 )
                 if implementation:
                     network_dict["implemented_in"] = [
                         i.strip("()") for i in implementation.strip().split()
                     ]
 
             networks_dict[network_number] = copy.deepcopy(network_dict)
-        version_info_dict["networks"] = networks_dict if networks_dict else None
 
-        ##########################
-        # Isotopes:
-        # Split off
-        isotopes = {el for el in cleaned if el.startswith("Isotope ")}
-        cleaned -= isotopes
+        return networks_dict if networks_dict else None
+
+    def _parse_binary_c_version_info_isotopes(self, isotopes):
+        """
+        Function to parse the isotopes info
+        """
 
         isotope_dict = {}
         for el in isotopes:
             split_info = el.split("Isotope ")[-1].strip().split(" is ")
 
             isotope_info = split_info[-1]
             name = isotope_info.split(" ")[0].strip()
@@ -157,61 +156,56 @@
                 "name": name,
                 "Z": Z,
                 "A": A,
                 "mass_mev": mass_mev,
                 "mass_g": mass_g,
                 "mass_amu": mass_amu,
             }
-        version_info_dict["isotopes"] = isotope_dict if isotope_dict else None
 
-        ##########################
-        # Arg pairs:
-        # Split off
-        argpairs = {el for el in cleaned if el.startswith("ArgPair")}
-        cleaned -= argpairs
+        return isotope_dict if isotope_dict else None
+
+    def _parse_binary_c_version_info_argpairs(self, argpairs):
+        """
+        Function to parse the argpairs info
+        """
 
         argpair_dict = {}
         for el in sorted(argpairs):
             split_info = el.split("ArgPair ")[-1].split(" ")
 
             if not argpair_dict.get(split_info[0], None):
                 argpair_dict[split_info[0]] = {split_info[1]: split_info[2]}
             else:
                 argpair_dict[split_info[0]][split_info[1]] = split_info[2]
 
-        version_info_dict["argpairs"] = argpair_dict if argpair_dict else None
+        return argpair_dict if argpair_dict else None
 
-        ##########################
-        # ensembles:
-        # Split off
-        ensembles = {el for el in cleaned if el.startswith("Ensemble")}
-        cleaned -= ensembles
+    def _parse_binary_c_version_info_ensembles(self, ensembles):
+        """
+        Function to parse the ensembles info
+        """
 
         ensemble_dict = {}
         ensemble_filter_dict = {}
         for el in ensembles:
             split_info = el.split("Ensemble ")[-1].split(" is ")
 
             if len(split_info) > 1:
                 if not split_info[0].startswith("filter"):
                     ensemble_dict[int(split_info[0])] = split_info[-1]
                 else:
                     filter_no = int(split_info[0].replace("filter ", ""))
                     ensemble_filter_dict[filter_no] = split_info[-1]
 
-        version_info_dict["ensembles"] = ensemble_dict if ensemble_dict else None
-        version_info_dict["ensemble_filters"] = (
-            ensemble_filter_dict if ensemble_filter_dict else None
-        )
+        return ensemble_dict, ensemble_filter_dict
 
-        ##########################
-        # macros:
-        # Split off
-        macros = {el for el in cleaned if el.startswith("macroxyz")}
-        cleaned -= macros
+    def _parse_binary_c_version_info_macros(self, macros):
+        """
+        Function to parse the macros info
+        """
 
         param_type_dict = {
             "STRING": str,
             "FLOAT": float,
             "MACRO": str,
             "INT": int,
             "LONG_INT": int,
@@ -224,56 +218,48 @@
             param_type = split_info[0]
 
             new_split = "".join(split_info[1:]).split(" is ")
             param_name = new_split[0].strip()
             param_value = " is ".join(new_split[1:])
             param_value = param_value.strip()
 
-            # print("macro ",param_name,"=",param_value," float?",isfloat(param_value)," int?",isint(param_value))
-
             # If we're trying to set the value to "on", check that
             # it doesn't already exist. If it does, do nothing, as the
             # extra information is better than just "on"
             if param_name in macros_dict:
-                # print("already exists (is ",macros_dict[param_name]," float? ",isfloat(macros_dict[param_name]),", int? ",isint(macros_dict[param_name]),") : check that we can improve it")
                 if macros_dict[param_name] == "on":
                     # update with better value
                     store = True
                 elif (
                     isfloat(macros_dict[param_name]) is False
                     and isfloat(param_value) is True
                 ):
                     # store the number we now have to replace the non-number we had
                     store = True
                 else:
                     # don't override existing number
                     store = False
 
-                # if store:
-                #    print("Found improved macro value of param",param_name,", was ",macros_dict[param_name],", is",param_value)
-                # else:
-                #    print("Cannot improve: use old value")
             else:
                 store = True
 
             if store:
                 # Sometimes the macros have extra information behind it.
                 # Needs an update in outputting by binary_c (RGI: what does this mean David???)
                 try:
                     macros_dict[param_name] = param_type_dict[param_type](param_value)
                 except ValueError:
                     macros_dict[param_name] = str(param_value)
 
-        version_info_dict["macros"] = macros_dict if macros_dict else None
+        return macros_dict if macros_dict else None
 
-        ##########################
-        # Elements:
-        # Split off:
-        elements = {el for el in cleaned if el.startswith("Element")}
-        cleaned -= elements
+    def _parse_binary_c_version_info_elements(self, elements):
+        """
+        Function to parse the elements info
+        """
 
         # Fill dict:
         elements_dict = {}
         for el in elements:
             split_info = el.split("Element ")[-1].split(" : ")
             name_info = split_info[0].split(" is ")
 
@@ -288,49 +274,51 @@
 
             elements_dict[int(name_info[0])] = {
                 "name": name_info[-1],
                 "atomic_number": int(name_info[0]),
                 "amt_isotopes": len(isotopes),
                 "isotopes": isotopes,
             }
-        version_info_dict["elements"] = elements_dict if elements_dict else None
 
-        ##########################
-        # dt_limits:
-        # split off
-        dt_limits = {el for el in cleaned if el.startswith("DTlimit")}
-        cleaned -= dt_limits
+        return elements_dict if elements_dict else None
+
+    def _parse_binary_c_version_info_dt_limits(self, dt_limits):
+        """
+        Function to parse the dt_limits info
+        """
 
         # Fill dict
         dt_limits_dict = {}
         for el in dt_limits:
             split_info = el.split("DTlimit ")[-1].split(" : ")
             dt_limits_dict[split_info[1].strip()] = {
                 "index": int(split_info[0]),
                 "value": float(split_info[-1]),
             }
 
-        version_info_dict["dt_limits"] = dt_limits_dict if dt_limits_dict else None
+        return dt_limits_dict if dt_limits_dict else None
 
-        ##############################
-        # Units
+    def _parse_binary_c_version_info_units(self, unit, units):
+        """
+        Function to parse the units info
+
+        TODO: i'm not sure that this parsing is correct
+        """
 
-        units = {el for el in cleaned if el.startswith("Unit ")}
-        cleaned -= units
         units_dict = {}
-        for el in units:
+        for el in unit:
             split_info = el.split("Unit ")[-1].split(",")
             s = split_info[0].split(" is ")
 
             if len(s) == 2:
                 long, short = [i.strip().strip('"') for i in s]
             elif len(s) == 1:
                 long, short = None, s[0]
             else:
-                print("Warning: Failed to split unit string {}".format(el))
+                self.vb_warning("Warning: Failed to split unit string {}".format(el))
 
             to_cgs = (split_info[1].split())[3].strip().strip('"')
             code_units = split_info[2].split()
             code_unit_type_num = int(code_units[3].strip().strip('"'))
             code_unit_type = code_units[4].strip().strip('"')
             code_unit_cgs_value = code_units[9].strip().strip('"').strip(")")
             units_dict[long] = {
@@ -339,39 +327,236 @@
                 "to_cgs": to_cgs,
                 "code_unit_type_num": code_unit_type_num,
                 "code_unit_type": code_unit_type,
                 "code_unit_cgs_value": code_unit_cgs_value,
             }
 
         # Add the list of units
-        units = {el for el in cleaned if el.startswith("Units: ")}
-        cleaned -= units
         for el in units:
             el = el[7:]  # removes "Units: "
             units_dict["units list"] = el.strip("Units:")
 
-        version_info_dict["units"] = units_dict
+        return units_dict if units_dict else None
 
-        ##########################
-        # Nucleosynthesis sources:
-        # Split off
-        nucsyn_sources = {el for el in cleaned if el.startswith("Nucleosynthesis")}
-        cleaned -= nucsyn_sources
+    def _parse_binary_c_version_nucsyn_sources(self, nucsyn_sources):
+        """
+        Function to parse the nucsyn_sources info
+        """
 
         # Fill dict
         nucsyn_sources_dict = {}
         for el in nucsyn_sources:
             split_info = el.split("Nucleosynthesis source")[-1].strip().split(" is ")
             nucsyn_sources_dict[int(split_info[0])] = split_info[-1]
 
-        version_info_dict["nucleosynthesis_sources"] = (
-            nucsyn_sources_dict if nucsyn_sources_dict else None
+        return nucsyn_sources_dict if nucsyn_sources_dict else None
+
+    def _parse_binary_c_version_binary_c_error_codes(self, binary_c_error_codes):
+        """
+        Function to parse the binary_c_error_codes info
+        """
+
+        binary_c_error_codes_dict = {}
+        for el in binary_c_error_codes:
+            split_info = el.split("Error code")[-1].strip().split(" = ")
+
+            # extract info
+            number = int(split_info[1].split()[0])
+            name = str(split_info[0])
+            description = str(split_info[1].split()[1].replace('"', ""))
+
+            binary_c_error_codes_dict[number] = {
+                "number": number,
+                "name": name,
+                "description": description,
+            }
+
+        return binary_c_error_codes_dict if binary_c_error_codes_dict else None
+
+    def _parse_binary_c_version_deflists(self, deflists):
+        """
+        Function to parse the deflists info
+        """
+
+        deflist_dict = {}
+        for el in deflists:
+            split_info = el.split("deflist")[-1].strip().split()
+
+            # Extract data
+            deflist_type = split_info[0]
+            deflist_data = " ".join(split_info[1:])
+
+            # Check if current type is already known
+            if deflist_type not in deflist_dict:
+                deflist_dict[deflist_type] = {}
+
+            # store data in current type dict
+            deflist_data_split = deflist_data.split(" is ")
+            deflist_data_number = int(deflist_data_split[0])
+            deflist_data_name = str(deflist_data_split[1])
+
+            deflist_dict[deflist_type][deflist_data_number] = deflist_data_name
+
+        return deflist_dict if deflist_dict else None
+
+    def parse_binary_c_version_info(self, version_info_string: str) -> dict:
+        """
+        Function that parses the binary_c version info. Long function with a lot of branches
+
+        Args:
+            version_info_string: raw output of version_info call to binary_c
+
+        Returns:
+            Parsed version of the version info, which is a dictionary containing the keys: 'isotopes' for isotope info, 'argpairs' for argument pair info (TODO: explain), 'ensembles' for ensemble settings/info, 'macros' for macros, 'elements' for atomic element info, 'DTlimit' for (TODO: explain), 'nucleosynthesis_sources' for nucleosynthesis sources, and 'miscellaneous' for all those that were not caught by the previous groups. 'git_branch', 'git_build', 'revision' and 'email' are also keys, but its clear what those contain.
+        """
+
+        version_info_dict = {}
+
+        # Clean data and put in correct shape
+        splitted = version_info_string.strip().splitlines()
+        cleaned = {el.strip() for el in splitted if not el == ""}
+
+        ##########################
+        # Network:
+
+        # Split off all the networks
+        networks = {el for el in cleaned if el.startswith("Network ")}
+        cleaned = cleaned - networks
+
+        # and parse the info
+        version_info_dict["networks"] = self._parse_binary_c_version_info_networks(
+            networks
         )
 
         ##########################
+        # Isotopes:
+
+        # Split off all the isotopes
+        isotopes = {el for el in cleaned if el.startswith("Isotope ")}
+        cleaned -= isotopes
+
+        # and parse the info
+        version_info_dict["isotopes"] = self._parse_binary_c_version_info_isotopes(
+            isotopes
+        )
+
+        ##########################
+        # Arg pairs:
+
+        # Split off all the argpairs
+        argpairs = {el for el in cleaned if el.startswith("ArgPair")}
+        cleaned -= argpairs
+
+        # and parse the info
+        version_info_dict["argpairs"] = self._parse_binary_c_version_info_argpairs(
+            argpairs
+        )
+
+        ##########################
+        # ensembles:
+
+        # Split off all the ensembles
+        ensembles = {el for el in cleaned if el.startswith("Ensemble")}
+        cleaned -= ensembles
+
+        # and parse the info
+        (
+            ensemble_dict,
+            ensemble_filter_dict,
+        ) = self._parse_binary_c_version_info_ensembles(ensembles)
+
+        version_info_dict["ensembles"] = ensemble_dict if ensemble_dict else None
+        version_info_dict["ensemble_filters"] = (
+            ensemble_filter_dict if ensemble_filter_dict else None
+        )
+
+        ##########################
+        # macros:
+
+        # Split off of all the macros
+        macros = {el for el in cleaned if el.startswith("macroxyz")}
+        cleaned -= macros
+
+        # and parse the info
+        version_info_dict["macros"] = self._parse_binary_c_version_info_macros(macros)
+
+        ##########################
+        # Elements:
+
+        # Split off all the elements
+        elements = {el for el in cleaned if el.startswith("Element")}
+        cleaned -= elements
+
+        # and parse the info
+        version_info_dict["elements"] = self._parse_binary_c_version_info_elements(
+            elements
+        )
+
+        ##########################
+        # dt_limits:
+
+        # split off all the dt_limits
+        dt_limits = {el for el in cleaned if el.startswith("DTlimit")}
+        cleaned -= dt_limits
+
+        # and parse the info
+        version_info_dict["dt_limits"] = self._parse_binary_c_version_info_dt_limits(
+            dt_limits
+        )
+
+        ##############################
+        # Units
+
+        # split off all the units
+        unit = {el for el in cleaned if el.startswith("Unit ")}
+        cleaned -= unit
+
+        units = {el for el in cleaned if el.startswith("Units: ")}
+        cleaned -= units
+
+        # and parse the info
+        version_info_dict["units"] = self._parse_binary_c_version_info_units(
+            unit, units
+        )
+
+        ##########################
+        # Nucleosynthesis sources:
+
+        # Split off all the nucsyn sources
+        nucsyn_sources = {el for el in cleaned if el.startswith("Nucleosynthesis")}
+        cleaned -= nucsyn_sources
+
+        # and parse the info
+        version_info_dict[
+            "nucleosynthesis_sources"
+        ] = self._parse_binary_c_version_nucsyn_sources(nucsyn_sources)
+
+        ##########################
+        # binary_c_errors:
+
+        # Split off all the nucsyn sources
+        binary_c_error_codes = {el for el in cleaned if el.startswith("Error code")}
+        cleaned -= binary_c_error_codes
+
+        # and parse the info
+        version_info_dict[
+            "binary_c_error_codes"
+        ] = self._parse_binary_c_version_binary_c_error_codes(binary_c_error_codes)
+
+        ##########################
+        # deflist:
+
+        # Split off all the deflists
+        deflists = {el for el in cleaned if el.startswith("deflist")}
+        cleaned -= deflists
+
+        # and parse the info
+        version_info_dict["deflists"] = self._parse_binary_c_version_deflists(deflists)
+
+        ##########################
         # miscellaneous:
         # All those that I didn't catch with the above filters. Could try to get some more out though.
 
         misc_dict = {}
 
         # Filter out git revision
         git_revision = [el for el in cleaned if el.startswith("git revision")]
@@ -421,12 +606,13 @@
         version_info_dict["miscellaneous"] = misc_dict if misc_dict else None
         return version_info_dict
 
     def minimum_stellar_mass(self):
         """
         Function to return the minimum stellar mass (in Msun) from binary_c.
         """
-        if not self._minimum_stellar_mass:
+
+        if not hasattr(self, "_minimum_stellar_mass"):
             self._minimum_stellar_mass = self.return_binary_c_version_info(parsed=True)[
                 "macros"
             ]["BINARY_C_MINIMUM_STELLAR_MASS"]
         return self._minimum_stellar_mass
```

### Comparing `binarycpython-0.9.6/binarycpython/utils/run_system_wrapper.py` & `binarycpython-1.0.0/binarycpython/utils/run_system_wrapper.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/utils/stellar_types.py` & `binarycpython-1.0.0/binarycpython/utils/stellar_types.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/binarycpython/utils/useful_funcs.py` & `binarycpython-1.0.0/binarycpython/utils/useful_funcs.py`

 * *Files identical despite different names*

### Comparing `binarycpython-0.9.6/include/binary_c_python.h` & `binarycpython-1.0.0/include/binary_c_python.h`

 * *Files 4% similar despite different names*

```diff
@@ -21,71 +21,74 @@
                size_t * const nbytes);
 
 /* =================================================================== */
 /* Functions to call other API functionality like help and arglines    */
 /* =================================================================== */
 
 int return_arglines(char ** const outstring,
-                char ** const errorstring,
-                size_t * const nbytes);
+                    char ** const errorstring,
+                    size_t * const nbytes);
 
 int return_help_info(char * argstring,
-                char ** const outstring,
-                char ** const errorstring,
-                size_t * const nbytes);
-
-int return_help_all_info(char ** const outstring,
-                char ** const errorstring,
-                size_t * const nbytes);
+                     struct libbinary_c_store_t * store,
+                     char ** const outstring,
+                     char ** const errorstring,
+                     size_t * const nbytes);
+
+int return_help_all_info(char * argstring,
+                         struct libbinary_c_store_t * store,
+                         char ** const outstring,
+                         char ** const errorstring,
+                         size_t * const nbytes);
 
 int return_version_info(char ** const outstring,
-                char ** const errorstring,
-                size_t * const nbytes);
+                        char ** const errorstring,
+                        size_t * const nbytes);
 
 
 int return_minimum_orbit_for_RLOF(char * argstring,
-                                   struct libbinary_c_store_t * store,
-                                    char ** const buffer,
-                                    char ** const error_buffer,
-                                    size_t * const nbytes);
+                                  struct libbinary_c_store_t * store,
+                                  char ** const buffer,
+                                  char ** const error_buffer,
+                                  size_t * const nbytes);
 
 int return_maximum_mass_ratio_for_RLOF(char * argstring,
-                                   struct libbinary_c_store_t * store,
-                                   char ** buffer,
-                                   char ** error_buffer,
-                                   size_t * nbytes);
+                                       struct libbinary_c_store_t * store,
+                                       char ** buffer,
+                                       char ** error_buffer,
+                                       size_t * nbytes);
 
 /* =================================================================== */
 /* Functions to handle memory                                          */
 /* =================================================================== */
 
 struct libbinary_c_store_t * return_store_memaddr(char ** const buffer,
-               char ** const error_buffer,
-               size_t * const nbytes);
+        char ** const error_buffer,
+        size_t * const nbytes);
 
 struct persistent_data_t * return_persistent_data_memaddr(char ** const buffer,
-               char ** const error_buffer,
-               size_t * const nbytes);
+        char ** const error_buffer,
+        size_t * const nbytes);
 
 int free_store_memaddr(struct libbinary_c_store_t * store,
-               char ** const buffer,
-               char ** const error_buffer,
-               size_t * const nbytes);
+                       char ** const buffer,
+                       char ** const error_buffer,
+                       size_t * const nbytes);
 
 int free_persistent_data_memaddr_and_return_json_output(struct persistent_data_t * persistent_data,
-               char ** const buffer,
-               char ** const error_buffer,
-               size_t * const nbytes);
+        char ** const buffer,
+        char ** const error_buffer,
+        size_t * const nbytes);
 
 
 /* C macros */
 #define BINARY_C_APITEST_VERSION 0.1
 #define APIprint(...) APIprintf(__VA_ARGS__);
 #define NO_OUTPUT
 
 #ifdef BINARY_C_PYTHON_DEBUG
-  #define debug_printf(fmt, ...)  printf(fmt, ##__VA_ARGS__);
+#define debug_printf(fmt, ...)  printf(fmt, ##__VA_ARGS__);
 #else
-  #define debug_printf(fmt, ...)    /* Do nothing */
+#define debug_printf(fmt, ...)    /* Do nothing */
 #endif
 
 #endif // BINARY_C_C_PYTHON_H
```

### Comparing `binarycpython-0.9.6/setup.py` & `binarycpython-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Setup script for binarycpython
 """
+
 import distutils.command.build
 import os
 import re
 import subprocess
 import sys
 from distutils.core import Extension, setup
 
 #
 this_file = os.path.abspath(__file__)
 this_file_dir = os.path.dirname(this_file)
 
 ###
-REQUIRED_BINARY_C_VERSIONS = ["2.2.3"]
+REQUIRED_BINARY_C_VERSIONS = ["2.2.4"]
 
 ############################################################
 # Defining functionality
 ############################################################
 
 
 # Functions
@@ -250,15 +251,15 @@
     description="""This is a python API for binary_c (versions {}) by David Hendriks, Rob Izzard and collaborators. Based on the initial set up by Jeff andrews.""".format(
         ",".join(REQUIRED_BINARY_C_VERSIONS),
     ),
     author="David Hendriks",
     author_email="davidhendriks93@gmail.com",
     long_description=readme(),
     long_description_content_type="text/markdown",
-    url="https://gitlab.eps.surrey.ac.uk/ri0005/binary_c-python",
+    url="https://binary_c.gitlab.io/binary_c-python",
     license="gpl",
     keywords=[
         "binary_c",
         "astrophysics",
         "stellar evolution",
         "population synthesis",
     ],  # Keywords that define your package best
@@ -270,20 +271,21 @@
         "binarycpython.tests",
         "binarycpython.tests.tests_population_extensions",
     ],
     install_requires=requirements(this_file_dir),
     include_package_data=True,
     ext_modules=[BINARY_C_PYTHON_API_MODULE],  # binary_c must be loaded
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Programming Language :: C",
         "Topic :: Education",
+        "Topic :: Scientific/Engineering :: Astronomy",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     cmdclass={"build": CustomBuildCommand},
 )
```

### Comparing `binarycpython-0.9.6/src/binary_c_python.c` & `binarycpython-1.0.0/src/binary_c_python.c`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  * This module will be available as _binary_c_bindings, as a part of the binarycpython package.
  *
  * The first section contains the functions that will be available
  * to python as part of the submodule _binary_c_bindings
  *
  * The second section is composed of the functions that interface with the binary_c API
  *
- * Written by David Hendriks (davidhendriks93@gmail.com), Robert Izzard (r.izzard@surrey.ac.uk).
+ * Written by David Hendriks (davidhendriks93@gmail.com), Robert Izzard (rob.izzard@gmail.com).
  * Based on initial work of Jeff Andrews
  * Remember: variables must be passed by references
  * (i.e. as pointers).
  *
  * See tests/python_API_test.py for an example of how to use these functions.
  *
  * Backup reading material for making C-extensions:
@@ -103,16 +103,16 @@
 /* Initialize pyobjects */
 
 // Evolution function headers
 static PyObject* python_run_system(PyObject *self, PyObject *args, PyObject *kwargs);
 
 // Utility function headers
 static PyObject* python_return_arglines(PyObject *self, PyObject *args);
-static PyObject* python_return_help_info(PyObject *self, PyObject *args);
-static PyObject* python_return_help_all_info(PyObject *self, PyObject *args);
+static PyObject* python_return_help_info(PyObject *self, PyObject *args, PyObject *kwargs);
+static PyObject* python_return_help_all_info(PyObject *self, PyObject *args, PyObject *kwargs);
 static PyObject* python_return_version_info(PyObject *self, PyObject *args);
 static PyObject* python_return_minimum_orbit_for_RLOF(PyObject *self, PyObject *args, PyObject *kwargs);
 static PyObject* python_return_maximum_mass_ratio_for_RLOF(PyObject *self, PyObject *args, PyObject *kwargs);
 
 // Other function headers
 static PyObject* python_return_store_memaddr(PyObject *self, PyObject *args);
 static PyObject* python_return_persistent_data_memaddr(PyObject *self, PyObject *args);
@@ -126,16 +126,16 @@
 static PyMethodDef module_methods[] =
 {
     // Wierdly, this casting to a PyCFunction, which usually takes only 2 args, now works when giving keywords. See https://stackoverflow.com/q/10264080
     {"run_system", (PyCFunction)python_run_system, METH_VARARGS | METH_KEYWORDS, run_system_docstring},
 
     //
     {"return_arglines", python_return_arglines, METH_VARARGS, return_arglines_docstring},
-    {"return_help", python_return_help_info, METH_VARARGS, return_help_info_docstring},
-    {"return_help_all", python_return_help_all_info, METH_VARARGS, return_help_all_info_docstring},
+    {"return_help", (PyCFunction)python_return_help_info, METH_VARARGS | METH_KEYWORDS, return_help_info_docstring},
+    {"return_help_all", (PyCFunction)python_return_help_all_info, METH_VARARGS | METH_KEYWORDS, return_help_all_info_docstring},
     {"return_version_info", python_return_version_info, METH_VARARGS, return_version_info_docstring},
     {"return_minimum_orbit_for_RLOF", (PyCFunction)python_return_minimum_orbit_for_RLOF, METH_VARARGS | METH_KEYWORDS, return_minimum_orbit_for_RLOF_docstring},
     {"return_maximum_mass_ratio_for_RLOF", (PyCFunction)python_return_maximum_mass_ratio_for_RLOF, METH_VARARGS | METH_KEYWORDS, return_maximum_mass_ratio_for_RLOF_docstring},
 
     // memory
     {"return_store_memaddr", python_return_store_memaddr, METH_VARARGS, return_store_memaddr_docstring},
     {"return_persistent_data_memaddr", python_return_persistent_data_memaddr, METH_NOARGS, return_persistent_data_memaddr_docstring},
@@ -296,28 +296,45 @@
 
     Safe_free(buffer);
     Safe_free(error_buffer);
 
     return return_string;
 }
 
-static PyObject* python_return_help_info(PyObject *self, PyObject *args)
+static PyObject* python_return_help_info(PyObject *self, PyObject *args, PyObject *kwargs)
 {
+
+    static char* keywords[] = {"argstring", "store_memaddr", NULL};
+
     /* Parse the input tuple */
     char *argstring;
+    PyObject *  store_capsule = NULL;
 
-    if (!PyArg_ParseTuple(args, "s", &argstring))
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|O", keywords, &argstring, &store_capsule))
     {
         return NULL;
     }
 
+    // Store
+    struct libbinary_c_store_t * store = NULL;
+    if (store_capsule != NULL)
+    {
+        if (PyCapsule_IsValid(store_capsule, "STORE"))
+        {
+            if (!(store = (struct libbinary_c_store_t *) PyCapsule_GetPointer(store_capsule, "STORE")))
+                return NULL;
+            debug_printf("Unpacked store pointer %p from capsule\n", store_capsule);
+        }
+    }
+
     char * buffer;
     char * error_buffer;
     size_t nbytes;
     int out MAYBE_UNUSED = return_help_info(argstring,
+                                            store,                // TODO: change. memory adress for the store object
                                             &buffer,
                                             &error_buffer,
                                             &nbytes);
 
     /* copy the buffer to a python string */
     PyObject * return_string = Py_BuildValue("s", buffer);
     PyObject * return_error_string MAYBE_UNUSED = Py_BuildValue("s", error_buffer);
@@ -331,22 +348,51 @@
 
     Safe_free(buffer);
     Safe_free(error_buffer);
 
     return return_string;
 }
 
-static PyObject* python_return_help_all_info(PyObject *self, PyObject *args)
+static PyObject* python_return_help_all_info(PyObject *self, PyObject *args, PyObject *kwargs)
 {
+
+    static char* keywords[] = {"store_memaddr", NULL};
+
+    /* Parse the input tuple */
+    char *argstring = NULL;
+    PyObject *  store_capsule = NULL;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|O", keywords, &store_capsule))
+    {
+        return NULL;
+    }
+
+    // Store
+    struct libbinary_c_store_t * store = NULL;
+    if (store_capsule != NULL)
+    {
+        if (PyCapsule_IsValid(store_capsule, "STORE"))
+        {
+            if (!(store = (struct libbinary_c_store_t *) PyCapsule_GetPointer(store_capsule, "STORE")))
+                return NULL;
+            debug_printf("Unpacked store pointer %p from capsule\n", store_capsule);
+        }
+    }
+
     char * buffer;
     char * error_buffer;
     size_t nbytes;
-    int out MAYBE_UNUSED = return_help_all_info(&buffer,
-                           &error_buffer,
-                           &nbytes);
+
+    int out MAYBE_UNUSED = return_help_all_info(
+                               argstring,
+                               store,                // TODO: change. memory adress for the store object
+                               &buffer,
+                               &error_buffer,
+                               &nbytes
+                           );
 
     /* copy the buffer to a python string */
     PyObject * return_string = Py_BuildValue("s", buffer);
     PyObject * return_error_string MAYBE_UNUSED = Py_BuildValue("s", error_buffer);
 
     if (error_buffer != NULL && strlen(error_buffer) > 0)
     {
@@ -934,20 +980,28 @@
                         );
 
     return 0;
 }
 
 
 int return_help_info(char * argstring,
+                     struct libbinary_c_store_t * store,
                      char ** const buffer,
                      char ** const error_buffer,
                      size_t * const nbytes)
 {
     struct libbinary_c_stardata_t *stardata = NULL;
-    struct libbinary_c_store_t *store = NULL;
+
+    /* Determine whether to free the store memory adress*/
+    Boolean free_store = FALSE;
+    if (store == NULL)
+    {
+        debug_printf("Decided to free the store memaddr\n");
+        free_store = TRUE;
+    }
 
     /* Set up new system */
     binary_c_new_system(&stardata,          // stardata
                         NULL,               // previous_stardatas
                         NULL,               // preferences
                         &store,             // store
                         NULL,               // persistent_data
@@ -968,31 +1022,41 @@
     /* get error buffer pointer */
     binary_c_error_buffer(stardata, error_buffer);
 
     /* free stardata (except the buffer) */
     binary_c_free_memory(&stardata, // Stardata
                          TRUE,                       // free_preferences
                          TRUE,                       // free_stardata
-                         TRUE,                       // free_store
+                         free_store,                       // free_store
                          FALSE,                      // free_raw_buffer
                          TRUE                        // free_persistent
                         );
 
     return 0;
 }
 
 
-int return_help_all_info(char ** const buffer,
-                         char ** const error_buffer,
-                         size_t * const nbytes)
+int return_help_all_info(
+    char * argstring,
+    struct libbinary_c_store_t * store,
+    char ** const buffer,
+    char ** const error_buffer,
+    size_t * const nbytes)
 {
     struct libbinary_c_stardata_t *stardata = NULL;
-    struct libbinary_c_store_t *store = NULL;
     char * empty_str = "";
 
+    /* Determine whether to free the store memory adress*/
+    Boolean free_store = FALSE;
+    if (store == NULL)
+    {
+        debug_printf("Decided to free the store memaddr\n");
+        free_store = TRUE;
+    }
+
     /* Set up new system */
     binary_c_new_system(&stardata,          // stardata
                         NULL,               // previous_stardatas
                         NULL,               // preferences
                         &store,             // store
                         NULL,               // persistent_data
                         &empty_str,         // argv
@@ -1012,15 +1076,15 @@
     /* get error buffer pointer */
     binary_c_error_buffer(stardata, error_buffer);
 
     /* free stardata (except the buffer) */
     binary_c_free_memory(&stardata, // Stardata
                          TRUE,                       // free_preferences
                          TRUE,                       // free_stardata
-                         TRUE,                       // free_store
+                         free_store,                 // free_store
                          FALSE,                      // free_raw_buffer
                          TRUE                        // free_persistent
                         );
 
     return 0;
 }
```

