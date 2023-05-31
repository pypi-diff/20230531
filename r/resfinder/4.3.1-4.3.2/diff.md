# Comparing `tmp/resfinder-4.3.1.tar.gz` & `tmp/resfinder-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resfinder-4.3.1.tar", last modified: Fri Mar  3 09:14:55 2023, max compression
+gzip compressed data, was "resfinder-4.3.2.tar", last modified: Wed May 31 08:45:41 2023, max compression
```

## Comparing `resfinder-4.3.1.tar` & `resfinder-4.3.2.tar`

### file list

```diff
@@ -1,66 +1,64 @@
--rw-r--r--   0        0        0      623 2023-02-06 08:36:49.871379 resfinder-4.3.1/LICENSE
--rw-r--r--   0        0        0    15342 2023-02-06 08:36:49.871637 resfinder-4.3.1/README.md
--rw-r--r--   0        0        0      904 2023-02-06 08:36:49.872095 resfinder-4.3.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-03 09:03:17.777998 resfinder-4.3.1/src/resfinder/__init__.py
--rw-r--r--   0        0        0      101 2023-02-06 08:36:49.873095 resfinder-4.3.1/src/resfinder/__main__.py
--rw-r--r--   0        0        0    12626 2023-02-06 08:36:49.873165 resfinder-4.3.1/src/resfinder/amr_abbreviations.md
--rw-r--r--   0        0        0        0 2023-02-06 08:36:49.873234 resfinder-4.3.1/src/resfinder/cge/__init__.py
--rw-r--r--   0        0        0    19840 2023-02-08 09:07:14.241596 resfinder-4.3.1/src/resfinder/cge/config.py
--rw-r--r--   0        0        0        0 2023-02-06 08:36:49.873592 resfinder-4.3.1/src/resfinder/cge/output/__init__.py
--rw-r--r--   0        0        0      639 2023-02-06 08:36:49.873693 resfinder-4.3.1/src/resfinder/cge/output/exceptions.py
--rw-r--r--   0        0        0     8007 2023-03-03 09:03:17.778341 resfinder-4.3.1/src/resfinder/cge/output/gene_result.py
--rw-r--r--   0        0        0     2897 2023-02-06 08:36:49.873868 resfinder-4.3.1/src/resfinder/cge/output/orderedset.py
--rw-r--r--   0        0        0     5654 2023-02-08 09:07:14.242108 resfinder-4.3.1/src/resfinder/cge/output/phenotype_result.py
--rw-r--r--   0        0        0     5272 2023-02-06 08:36:49.874019 resfinder-4.3.1/src/resfinder/cge/output/seq_variation_result.py
--rw-r--r--   0        0        0     7423 2023-02-08 09:07:14.242339 resfinder-4.3.1/src/resfinder/cge/output/std_results.py
--rw-r--r--   0        0        0    18361 2023-02-06 08:36:49.874237 resfinder-4.3.1/src/resfinder/cge/output/table.py
--rw-r--r--   0        0        0        0 2023-02-06 08:36:49.874321 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/__init__.py
--rw-r--r--   0        0        0      667 2023-02-06 08:36:49.874392 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/abclassdef.py
--rw-r--r--   0        0        0     1315 2023-02-06 08:36:49.874457 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/dbhit.py
--rw-r--r--   0        0        0     9421 2023-02-06 08:36:49.874530 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/feature.py
--rw-r--r--   0        0        0    21739 2023-03-03 09:03:17.778775 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/isolate.py
--rw-r--r--   0        0        0     6106 2023-02-06 08:36:49.874732 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/phenodbpoint.py
--rw-r--r--   0        0        0     1501 2023-02-06 08:36:49.874791 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/phenotype.py
--rw-r--r--   0        0        0    42668 2023-02-08 09:07:14.242523 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/res_profile.py
--rw-r--r--   0        0        0    10559 2023-02-06 08:36:49.875073 resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/res_sumtable.py
--rw-r--r--   0        0        0    94910 2023-03-03 09:03:17.779639 resfinder-4.3.1/src/resfinder/cge/pointfinder.py
--rw-r--r--   0        0        0    24720 2023-02-06 08:36:49.875635 resfinder-4.3.1/src/resfinder/cge/resfinder.py
--rw-r--r--   0        0        0        0 2023-02-06 08:36:49.875694 resfinder-4.3.1/src/resfinder/cge/runinfo.py
--rw-r--r--   0        0        0     1366 2023-02-06 08:36:49.875765 resfinder-4.3.1/src/resfinder/environment_variables.md
--rw-r--r--   0        0        0    24618 2023-03-03 08:23:41.702888 resfinder-4.3.1/src/resfinder/run_resfinder.py
--rw-r--r--   0        0        0     1476 2023-02-06 08:36:49.876149 resfinder-4.3.1/src/resfinder/species_abbreviations.md
--rw-r--r--   0        0        0     6148 2023-02-10 09:59:43.646518 resfinder-4.3.1/tests/.DS_Store
--rw-r--r--   0        0        0      230 2023-02-06 08:36:49.876321 resfinder-4.3.1/tests/data/env_var_test_fail.md
--rw-r--r--   0        0        0    14926 2023-02-06 08:36:49.876442 resfinder-4.3.1/tests/data/test_isolate_01.fa
--rw-r--r--   0        0        0   158542 2023-02-06 08:36:49.877004 resfinder-4.3.1/tests/data/test_isolate_01_1.fq
--rw-r--r--   0        0        0   158542 2023-02-06 08:36:49.877747 resfinder-4.3.1/tests/data/test_isolate_01_2.fq
--rw-r--r--   0        0        0      931 2023-02-06 08:36:49.877843 resfinder-4.3.1/tests/data/test_isolate_02.fa
--rw-r--r--   0        0        0    14152 2023-02-06 08:36:49.877895 resfinder-4.3.1/tests/data/test_isolate_03.fa
--rw-r--r--   0        0        0    16924 2023-02-06 08:36:49.877952 resfinder-4.3.1/tests/data/test_isolate_05.fa
--rw-r--r--   0        0        0   181488 2023-02-06 08:36:49.878696 resfinder-4.3.1/tests/data/test_isolate_05_1.fq
--rw-r--r--   0        0        0   181488 2023-02-06 08:36:49.879323 resfinder-4.3.1/tests/data/test_isolate_05_2.fq
--rw-r--r--   0        0        0     2687 2023-02-06 08:36:49.879407 resfinder-4.3.1/tests/data/test_isolate_09a.fa
--rw-r--r--   0        0        0    84352 2023-02-06 08:36:49.879824 resfinder-4.3.1/tests/data/test_isolate_09a_1.fq
--rw-r--r--   0        0        0    84352 2023-02-06 08:36:49.880111 resfinder-4.3.1/tests/data/test_isolate_09a_2.fq
--rw-r--r--   0        0        0     2690 2023-02-06 08:36:49.880161 resfinder-4.3.1/tests/data/test_isolate_09b.fa
--rw-r--r--   0        0        0    85117 2023-02-06 08:36:49.880414 resfinder-4.3.1/tests/data/test_isolate_09b_1.fq
--rw-r--r--   0        0        0    85117 2023-02-06 08:36:49.880704 resfinder-4.3.1/tests/data/test_isolate_09b_2.fq
--rw-r--r--   0        0        0     2698 2023-02-06 08:36:49.880756 resfinder-4.3.1/tests/data/test_isolate_10.fa
--rw-r--r--   0        0        0     1563 2023-02-06 08:36:49.880816 resfinder-4.3.1/tests/data/test_isolate_11.fa
--rw-r--r--   0        0        0    16497 2023-02-06 08:36:49.880914 resfinder-4.3.1/tests/data/test_isolate_11_1.fq
--rw-r--r--   0        0        0    16497 2023-02-06 08:36:49.881003 resfinder-4.3.1/tests/data/test_isolate_11_2.fq
--rw-r--r--   0        0        0     1317 2023-03-03 09:03:17.780129 resfinder-4.3.1/tests/data/test_isolate_12.fa
--rw-r--r--   0        0        0      680 2023-02-06 08:36:49.881059 resfinder-4.3.1/tests/data/wdl_input.tsv
--rw-r--r--   0        0        0    12075 2023-02-06 08:36:49.881169 resfinder-4.3.1/tests/deprecated/functional_tests.py
--rw-r--r--   0        0        0     1719 2023-02-06 08:36:49.881240 resfinder-4.3.1/tests/deprecated/unit_tests.py
--rw-r--r--   0        0        0     4668 2023-02-08 09:07:14.243613 resfinder-4.3.1/tests/resfinder/cge/output/test_gene_result.md
--rw-r--r--   0        0        0     7156 2023-02-08 09:07:14.243842 resfinder-4.3.1/tests/resfinder/cge/output/test_phenotype_result.md
--rw-r--r--   0        0        0     4160 2023-02-06 08:36:49.881527 resfinder-4.3.1/tests/resfinder/cge/output/test_seq_variation_result.md
--rw-r--r--   0        0        0    10615 2023-02-09 08:40:36.491835 resfinder-4.3.1/tests/resfinder/cge/output/test_std_results.md
--rw-r--r--   0        0        0     1486 2023-02-06 08:36:49.881717 resfinder-4.3.1/tests/resfinder/cge/phenotype2genotype/test_antibiotics.md
--rw-r--r--   0        0        0     8329 2023-02-08 09:07:14.244318 resfinder-4.3.1/tests/resfinder/cge/phenotype2genotype/test_isolate.md
--rw-r--r--   0        0        0     7941 2023-02-08 09:07:14.244420 resfinder-4.3.1/tests/resfinder/cge/test_config.md
--rw-r--r--   0        0        0      470 2023-02-06 08:36:49.881912 resfinder-4.3.1/tests/resfinder/cge/test_pointfinder.md
--rw-r--r--   0        0        0     1824 2023-02-08 13:13:28.640168 resfinder-4.3.1/tests/resfinder/test_run_resfinder.md
--rw-r--r--   0        0        0    17173 2023-03-03 08:50:10.210106 resfinder-4.3.1/tests/tmp_out/tmp/out_beta-lactam.xml
--rw-r--r--   0        0        0    15747 1970-01-01 00:00:00.000000 resfinder-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0      623 2023-05-31 07:54:33.820171 resfinder-4.3.2/LICENSE
+-rw-r--r--   0        0        0    15342 2023-05-31 07:54:33.820388 resfinder-4.3.2/README.md
+-rw-r--r--   0        0        0      904 2023-05-31 07:54:33.821030 resfinder-4.3.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-31 07:55:20.604721 resfinder-4.3.2/src/resfinder/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-31 07:54:33.822272 resfinder-4.3.2/src/resfinder/__main__.py
+-rw-r--r--   0        0        0    12626 2023-05-31 07:54:33.822377 resfinder-4.3.2/src/resfinder/amr_abbreviations.md
+-rw-r--r--   0        0        0        0 2023-05-31 07:54:33.822452 resfinder-4.3.2/src/resfinder/cge/__init__.py
+-rw-r--r--   0        0        0    19840 2023-05-31 07:54:33.822632 resfinder-4.3.2/src/resfinder/cge/config.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:54:33.822728 resfinder-4.3.2/src/resfinder/cge/output/__init__.py
+-rw-r--r--   0        0        0      639 2023-05-31 07:54:33.822826 resfinder-4.3.2/src/resfinder/cge/output/exceptions.py
+-rw-r--r--   0        0        0     8007 2023-05-31 07:54:33.822934 resfinder-4.3.2/src/resfinder/cge/output/gene_result.py
+-rw-r--r--   0        0        0     2897 2023-05-31 07:54:33.823023 resfinder-4.3.2/src/resfinder/cge/output/orderedset.py
+-rw-r--r--   0        0        0     5654 2023-05-31 07:54:33.823131 resfinder-4.3.2/src/resfinder/cge/output/phenotype_result.py
+-rw-r--r--   0        0        0     5272 2023-05-31 07:54:33.823225 resfinder-4.3.2/src/resfinder/cge/output/seq_variation_result.py
+-rw-r--r--   0        0        0     7423 2023-05-31 07:54:33.823355 resfinder-4.3.2/src/resfinder/cge/output/std_results.py
+-rw-r--r--   0        0        0    18361 2023-05-31 07:54:33.823484 resfinder-4.3.2/src/resfinder/cge/output/table.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:54:33.823569 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/__init__.py
+-rw-r--r--   0        0        0      667 2023-05-31 07:54:33.823644 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/abclassdef.py
+-rw-r--r--   0        0        0     1315 2023-05-31 07:54:33.823715 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/dbhit.py
+-rw-r--r--   0        0        0     9421 2023-05-31 07:54:33.823808 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/feature.py
+-rw-r--r--   0        0        0    21739 2023-05-31 07:54:33.823941 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/isolate.py
+-rw-r--r--   0        0        0     6106 2023-05-31 07:54:33.824041 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/phenodbpoint.py
+-rw-r--r--   0        0        0     1501 2023-05-31 07:54:33.824119 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/phenotype.py
+-rw-r--r--   0        0        0    42668 2023-05-31 07:54:33.824303 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/res_profile.py
+-rw-r--r--   0        0        0    10559 2023-05-31 07:54:33.824421 resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/res_sumtable.py
+-rw-r--r--   0        0        0    93293 2023-05-31 07:54:33.824823 resfinder-4.3.2/src/resfinder/cge/pointfinder.py
+-rw-r--r--   0        0        0    24720 2023-05-31 07:54:33.825005 resfinder-4.3.2/src/resfinder/cge/resfinder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:54:33.825066 resfinder-4.3.2/src/resfinder/cge/runinfo.py
+-rw-r--r--   0        0        0     1366 2023-05-31 07:54:33.825162 resfinder-4.3.2/src/resfinder/environment_variables.md
+-rw-r--r--   0        0        0    24618 2023-05-31 07:54:33.825390 resfinder-4.3.2/src/resfinder/run_resfinder.py
+-rw-r--r--   0        0        0     1476 2023-05-31 07:54:33.825502 resfinder-4.3.2/src/resfinder/species_abbreviations.md
+-rw-r--r--   0        0        0      230 2023-05-31 07:54:33.825664 resfinder-4.3.2/tests/data/env_var_test_fail.md
+-rw-r--r--   0        0        0    14926 2023-05-31 07:54:33.825825 resfinder-4.3.2/tests/data/test_isolate_01.fa
+-rw-r--r--   0        0        0   158542 2023-05-31 07:54:33.826625 resfinder-4.3.2/tests/data/test_isolate_01_1.fq
+-rw-r--r--   0        0        0   158542 2023-05-31 07:54:33.827666 resfinder-4.3.2/tests/data/test_isolate_01_2.fq
+-rw-r--r--   0        0        0      931 2023-05-31 07:54:33.827767 resfinder-4.3.2/tests/data/test_isolate_02.fa
+-rw-r--r--   0        0        0    14152 2023-05-31 07:54:33.827828 resfinder-4.3.2/tests/data/test_isolate_03.fa
+-rw-r--r--   0        0        0    16924 2023-05-31 07:54:33.827889 resfinder-4.3.2/tests/data/test_isolate_05.fa
+-rw-r--r--   0        0        0   181488 2023-05-31 07:54:33.828575 resfinder-4.3.2/tests/data/test_isolate_05_1.fq
+-rw-r--r--   0        0        0   181488 2023-05-31 07:54:33.829452 resfinder-4.3.2/tests/data/test_isolate_05_2.fq
+-rw-r--r--   0        0        0     2687 2023-05-31 07:54:33.829543 resfinder-4.3.2/tests/data/test_isolate_09a.fa
+-rw-r--r--   0        0        0    84352 2023-05-31 07:54:33.829989 resfinder-4.3.2/tests/data/test_isolate_09a_1.fq
+-rw-r--r--   0        0        0    84352 2023-05-31 07:54:33.830303 resfinder-4.3.2/tests/data/test_isolate_09a_2.fq
+-rw-r--r--   0        0        0     2690 2023-05-31 07:54:33.830362 resfinder-4.3.2/tests/data/test_isolate_09b.fa
+-rw-r--r--   0        0        0    85117 2023-05-31 07:54:33.830648 resfinder-4.3.2/tests/data/test_isolate_09b_1.fq
+-rw-r--r--   0        0        0    85117 2023-05-31 07:54:33.830987 resfinder-4.3.2/tests/data/test_isolate_09b_2.fq
+-rw-r--r--   0        0        0     2698 2023-05-31 07:54:33.831051 resfinder-4.3.2/tests/data/test_isolate_10.fa
+-rw-r--r--   0        0        0     1563 2023-05-31 07:54:33.831116 resfinder-4.3.2/tests/data/test_isolate_11.fa
+-rw-r--r--   0        0        0    16497 2023-05-31 07:54:33.831224 resfinder-4.3.2/tests/data/test_isolate_11_1.fq
+-rw-r--r--   0        0        0    16497 2023-05-31 07:54:33.831322 resfinder-4.3.2/tests/data/test_isolate_11_2.fq
+-rw-r--r--   0        0        0     1317 2023-05-31 07:54:33.831381 resfinder-4.3.2/tests/data/test_isolate_12.fa
+-rw-r--r--   0        0        0      680 2023-05-31 07:54:33.831438 resfinder-4.3.2/tests/data/wdl_input.tsv
+-rw-r--r--   0        0        0    12075 2023-05-31 07:54:33.831555 resfinder-4.3.2/tests/deprecated/functional_tests.py
+-rw-r--r--   0        0        0     1719 2023-05-31 07:54:33.831626 resfinder-4.3.2/tests/deprecated/unit_tests.py
+-rw-r--r--   0        0        0     4668 2023-05-31 07:54:33.831821 resfinder-4.3.2/tests/resfinder/cge/output/test_gene_result.md
+-rw-r--r--   0        0        0     7156 2023-05-31 07:54:33.831911 resfinder-4.3.2/tests/resfinder/cge/output/test_phenotype_result.md
+-rw-r--r--   0        0        0     4160 2023-05-31 07:54:33.831989 resfinder-4.3.2/tests/resfinder/cge/output/test_seq_variation_result.md
+-rw-r--r--   0        0        0    10615 2023-05-31 07:54:33.832110 resfinder-4.3.2/tests/resfinder/cge/output/test_std_results.md
+-rw-r--r--   0        0        0     1486 2023-05-31 07:54:33.832208 resfinder-4.3.2/tests/resfinder/cge/phenotype2genotype/test_antibiotics.md
+-rw-r--r--   0        0        0     8329 2023-05-31 07:54:33.832329 resfinder-4.3.2/tests/resfinder/cge/phenotype2genotype/test_isolate.md
+-rw-r--r--   0        0        0     7941 2023-05-31 07:54:33.832424 resfinder-4.3.2/tests/resfinder/cge/test_config.md
+-rw-r--r--   0        0        0      470 2023-05-31 07:54:33.832490 resfinder-4.3.2/tests/resfinder/cge/test_pointfinder.md
+-rw-r--r--   0        0        0     1824 2023-05-31 07:54:33.832673 resfinder-4.3.2/tests/resfinder/test_run_resfinder.md
+-rw-r--r--   0        0        0    15747 1970-01-01 00:00:00.000000 resfinder-4.3.2/PKG-INFO
```

### Comparing `resfinder-4.3.1/LICENSE` & `resfinder-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/README.md` & `resfinder-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/pyproject.toml` & `resfinder-4.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "cgecore==1.5.6",
     "tabulate>=0.8.9",
     "pandas>=1.4.2",
     "biopython>=1.79",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "4.3.1"
+version = "4.3.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 
 [tool.pdm.version]
```

### Comparing `resfinder-4.3.1/src/resfinder/amr_abbreviations.md` & `resfinder-4.3.2/src/resfinder/amr_abbreviations.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/config.py` & `resfinder-4.3.2/src/resfinder/cge/config.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/output/exceptions.py` & `resfinder-4.3.2/src/resfinder/cge/output/exceptions.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/output/gene_result.py` & `resfinder-4.3.2/src/resfinder/cge/output/gene_result.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/output/orderedset.py` & `resfinder-4.3.2/src/resfinder/cge/output/orderedset.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/output/phenotype_result.py` & `resfinder-4.3.2/src/resfinder/cge/output/phenotype_result.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/output/seq_variation_result.py` & `resfinder-4.3.2/src/resfinder/cge/output/seq_variation_result.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/output/std_results.py` & `resfinder-4.3.2/src/resfinder/cge/output/std_results.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/output/table.py` & `resfinder-4.3.2/src/resfinder/cge/output/table.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/abclassdef.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/abclassdef.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/dbhit.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/dbhit.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/feature.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/feature.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/isolate.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/isolate.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/phenodbpoint.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/phenodbpoint.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/phenotype.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/phenotype.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/res_profile.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/res_profile.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/phenotype2genotype/res_sumtable.py` & `resfinder-4.3.2/src/resfinder/cge/phenotype2genotype/res_sumtable.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/cge/pointfinder.py` & `resfinder-4.3.2/src/resfinder/cge/pointfinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -747,16 +747,14 @@
                 # Gene not found! go to next gene
                 GENES[gene] = 'No hit found'
                 continue
 
             # Check coverage for each hit, patch together partial genes hits
             for hit_id, hit in hits.items():
 
-                hit_dict = []
-
                 # Save hits start and end positions in subject, total subject
                 # len, and subject and query sequences of each hit
                 hits_found += [(hit['sbjct_start'], hit['sbjct_end'],
                                 hit['sbjct_string'], hit['query_string'],
                                 hit['sbjct_length'], hit['homo_string'],
                                 hit_id)]
 
@@ -900,46 +898,14 @@
                 GENES[gene]['alternative_overlaps'] = alternative_overlaps
                 mismatches = self.find_mismatches(gene=gene,
                                                   sbjct_start=all_start,
                                                   sbjct_seq=final_sbjct,
                                                   qry_seq=final_qry)
                 GENES[gene]['mis_matches'] = mismatches
 
-                # the above addition of GENES[gene] may be redundant as we now add
-                # the following dict to GENES[gene]['hits']
-
-                gene_accession = hit_id
-
-                if 'pre_id' in locals() and gene_accession in pre_id + next_id:
-                    hit_dict = {
-                                'evalue': 'NA',
-                                'sbjct_header': gene_accession,
-                                'bit': 'NA',
-                                'perc_ident': identity,
-                                'sbjct_length': sbjct_len,
-                                'sbjct_start': all_start,
-                                'sbjct_end': current_end,
-                                'gaps': no_call,
-                                'query_string': final_qry,
-                                'homo_string': final_homol,
-                                'subjct_string': final_sbjct,
-                                'contig_name': ", ".join(contigs),
-                                'query_start': 'NA',
-                                'query_end': 'NA',
-                                'HSP_length': len(final_qry),
-                                'coverage': coverage,
-                                'cal_score': ", ".join(scores),
-                                'hit_id': pre_id + next_id,
-                                'strand': 'NA',
-                                'perc_coverage': coverage * 100,
-                                'mis_matches': mismatches
-                    }
-
-                    GENES[gene]['hits'][combined_id] = hit_dict
-
             else:
                 # Gene not found above given coverage
                 GENES[gene] = ('Gene found with coverage, %f, below '
                                'minimum coverage threshold: %s' % (coverage,
                                                                    min_cov))
         return GENES
```

### Comparing `resfinder-4.3.1/src/resfinder/cge/resfinder.py` & `resfinder-4.3.2/src/resfinder/cge/resfinder.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/environment_variables.md` & `resfinder-4.3.2/src/resfinder/environment_variables.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/run_resfinder.py` & `resfinder-4.3.2/src/resfinder/run_resfinder.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/src/resfinder/species_abbreviations.md` & `resfinder-4.3.2/src/resfinder/species_abbreviations.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_01.fa` & `resfinder-4.3.2/tests/data/test_isolate_01.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_01_1.fq` & `resfinder-4.3.2/tests/data/test_isolate_01_1.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_01_2.fq` & `resfinder-4.3.2/tests/data/test_isolate_01_2.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_02.fa` & `resfinder-4.3.2/tests/data/test_isolate_02.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_03.fa` & `resfinder-4.3.2/tests/data/test_isolate_03.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_05.fa` & `resfinder-4.3.2/tests/data/test_isolate_05.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_05_1.fq` & `resfinder-4.3.2/tests/data/test_isolate_05_1.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_05_2.fq` & `resfinder-4.3.2/tests/data/test_isolate_05_2.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_09a.fa` & `resfinder-4.3.2/tests/data/test_isolate_09a.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_09a_1.fq` & `resfinder-4.3.2/tests/data/test_isolate_09a_1.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_09a_2.fq` & `resfinder-4.3.2/tests/data/test_isolate_09a_2.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_09b.fa` & `resfinder-4.3.2/tests/data/test_isolate_09b.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_09b_1.fq` & `resfinder-4.3.2/tests/data/test_isolate_09b_1.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_09b_2.fq` & `resfinder-4.3.2/tests/data/test_isolate_09b_2.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_10.fa` & `resfinder-4.3.2/tests/data/test_isolate_10.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_11.fa` & `resfinder-4.3.2/tests/data/test_isolate_11.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_11_1.fq` & `resfinder-4.3.2/tests/data/test_isolate_11_1.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_11_2.fq` & `resfinder-4.3.2/tests/data/test_isolate_11_2.fq`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/test_isolate_12.fa` & `resfinder-4.3.2/tests/data/test_isolate_12.fa`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/data/wdl_input.tsv` & `resfinder-4.3.2/tests/data/wdl_input.tsv`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/deprecated/functional_tests.py` & `resfinder-4.3.2/tests/deprecated/functional_tests.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/deprecated/unit_tests.py` & `resfinder-4.3.2/tests/deprecated/unit_tests.py`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/cge/output/test_gene_result.md` & `resfinder-4.3.2/tests/resfinder/cge/output/test_gene_result.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/cge/output/test_phenotype_result.md` & `resfinder-4.3.2/tests/resfinder/cge/output/test_phenotype_result.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/cge/output/test_seq_variation_result.md` & `resfinder-4.3.2/tests/resfinder/cge/output/test_seq_variation_result.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/cge/output/test_std_results.md` & `resfinder-4.3.2/tests/resfinder/cge/output/test_std_results.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/cge/phenotype2genotype/test_antibiotics.md` & `resfinder-4.3.2/tests/resfinder/cge/phenotype2genotype/test_antibiotics.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/cge/phenotype2genotype/test_isolate.md` & `resfinder-4.3.2/tests/resfinder/cge/phenotype2genotype/test_isolate.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/cge/test_config.md` & `resfinder-4.3.2/tests/resfinder/cge/test_config.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/tests/resfinder/test_run_resfinder.md` & `resfinder-4.3.2/tests/resfinder/test_run_resfinder.md`

 * *Files identical despite different names*

### Comparing `resfinder-4.3.1/PKG-INFO` & `resfinder-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resfinder
-Version: 4.3.1
+Version: 4.3.2
 Summary: ResFinder identifies acquired genes and/or finds chromosomal /
                  mutations mediating antimicrobial resistance in total or /
                  partial DNA sequence of bacteria.
 License: Apache-2.0
 Author-email: Center for Genomic Epidemiology <food-cgehelp@dtu.dk>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

