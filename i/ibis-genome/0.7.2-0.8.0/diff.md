# Comparing `tmp/ibis-genome-0.7.2.tar.gz` & `tmp/ibis-genome-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis-genome-0.7.2.tar", last modified: Thu May 18 01:14:15 2023, max compression
+gzip compressed data, was "ibis-genome-0.8.0.tar", last modified: Wed May 31 01:53:30 2023, max compression
```

## Comparing `ibis-genome-0.7.2.tar` & `ibis-genome-0.8.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.502722 ibis-genome-0.7.2/ibis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.502722 ibis-genome-0.7.2/ibis/config/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/config/template_coassemble.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/config/template_evaluate.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    37806 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/ibis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/coassemble.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis/workflow/env/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/aviary.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/coverm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/kingfisher.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/prodigal.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/r.yml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/env/singlem.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/evaluate.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis/workflow/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/aviary_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/cluster_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/collect_reference_bins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10121 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/no_genomes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3715 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/query_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/separate_SingleM_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/summarise_coassemblies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/ibis/workflow/scripts/target_elusive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.506723 ibis-genome-0.7.2/ibis_genome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44009 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 01:14:15.000000 ibis-genome-0.7.2/ibis_genome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 01:14:15.510722 ibis-genome-0.7.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_cluster_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    45532 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_coassemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_collect_reference_bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_evaluate_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_iterate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_no_genomes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_query_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_target_elusive.py
--rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-05-18 01:14:04.000000 ibis-genome-0.7.2/test/test_unmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.858384 ibis-genome-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44664 2023-05-31 01:53:30.858384 ibis-genome-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.854384 ibis-genome-0.8.0/ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.854384 ibis-genome-0.8.0/ibis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/config/template_coassemble.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/config/template_evaluate.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41498 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/ibis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.854384 ibis-genome-0.8.0/ibis/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/coassemble.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.854384 ibis-genome-0.8.0/ibis/workflow/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/env/aviary.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/env/coverm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/env/kingfisher.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/env/prodigal.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/env/r.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/env/singlem.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/evaluate.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.858384 ibis-genome-0.8.0/ibis/workflow/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/aviary_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/cluster_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/collect_reference_bins.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10121 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3492 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/is_interleaved.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/no_genomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3715 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/query_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/separate_SingleM_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/summarise_coassemblies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3524 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/ibis/workflow/scripts/target_elusive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.858384 ibis-genome-0.8.0/ibis_genome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44664 2023-05-31 01:53:30.000000 ibis-genome-0.8.0/ibis_genome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-31 01:53:30.000000 ibis-genome-0.8.0/ibis_genome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:53:30.000000 ibis-genome-0.8.0/ibis_genome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 01:53:30.000000 ibis-genome-0.8.0/ibis_genome.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 01:53:30.000000 ibis-genome-0.8.0/ibis_genome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 01:53:30.000000 ibis-genome-0.8.0/ibis_genome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:53:30.858384 ibis-genome-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:53:30.858384 ibis-genome-0.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_cluster_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45719 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_coassemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_collect_reference_bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_evaluate_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_is_interleaved.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_no_genomes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_query_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_target_elusive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19591 2023-05-31 01:53:13.000000 ibis-genome-0.8.0/test/test_update.py
```

### Comparing `ibis-genome-0.7.2/LICENSE` & `ibis-genome-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/PKG-INFO` & `ibis-genome-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-genome
-Version: 0.7.2
+Version: 0.8.0
 Summary: Ibis (Australian bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,14 +683,16 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ibis
 
+[<img src="ibis_logo.png" width="50%" />](ibis_logo.png)
+
 Ibis (bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly.
 
 ## Installation options
 
 ### Install from pip
 
 Install latest release via pip.
@@ -717,47 +719,56 @@
 Creates graph with samples as nodes and the number of overlapping sequences provided by SingleM.
 The taxa of the considered sequences can be filtered to target a specific taxon (e.g. the phylum Planctomycetota).
 The graph is clustered using the Girvan-Newman algorithm to provide sample groupings.
 Aviary assemble/recover commands are generated based on proposed coassemblies.
 Optionally, reads can be mapped to the matched bins with only unmapped reads being assembled.
 
 ```bash
+# Example: cluster reads into proposed coassemblies
+ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --no-genomes
+
 # Example: cluster reads into proposed coassemblies based on unbinned sequences
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 
 # Example: cluster reads into proposed coassemblies based on unbinned sequences and coassemble only unbinned reads
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --assemble-unmapped
 
 # Example: cluster reads into proposed coassemblies based on unbinned sequences from a specific taxa
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --taxa-of-interest "p__Planctomycetota"
 
 # Example: find relevant samples for differential coverage binning (no coassembly)
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --single-assembly
 ```
 
+## Ibis evaluate
+
+Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
+Compares the recovery by phyla and by single-copy marker gene.
+
+```bash
+# Example: evaluate a completed coassembly
+ibis evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
+```
+
 ## Ibis iterate
 
 Run a further iteration of coassemble, including newly recovered bins.
 
 ```bash
 # Example: rerun coassemble, adding new bins to database
 ibis iterate --aviary-outputs coassembly_0_dir ... --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 ```
 
-## Ibis evaluate
+## Ibis update
 
-Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
-Compares the recovery by phyla and by single-copy marker gene.
+Applies further processing to a previous Ibis coassemble run: downloading SRA reads, generating unmapped reads files, and/or running Aviary commands.
 
 ```bash
-# Example: evaluate a completed coassembly
-ibis evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
-```
+# Example: update previous run to download SRA reads
+ibis update --sra --coassemble-output coassemble_dir --forward SRA000001 ... --reverse SRA000001 ... --genomes genome_1.fna ...
 
-## Ibis unmap
+# Example: update previous run to perform unmapping
+ibis update --assemble-unmapped --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 
-Applies unmapping to a previous Ibis coassemble run, generating unmapped reads files and Aviary commands.
-
-```bash
-# Example: generate unmapped reads and commands for completed coassembly
-ibis unmap --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
+# Example: update previous run to run specific coassemblies
+ibis update --run-aviary --coassemblies coassembly_0 ... --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 ```
```

### Comparing `ibis-genome-0.7.2/README.md` & `ibis-genome-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Ibis
 
+[<img src="ibis_logo.png" width="50%" />](ibis_logo.png)
+
 Ibis (bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly.
 
 ## Installation options
 
 ### Install from pip
 
 Install latest release via pip.
@@ -30,47 +32,56 @@
 Creates graph with samples as nodes and the number of overlapping sequences provided by SingleM.
 The taxa of the considered sequences can be filtered to target a specific taxon (e.g. the phylum Planctomycetota).
 The graph is clustered using the Girvan-Newman algorithm to provide sample groupings.
 Aviary assemble/recover commands are generated based on proposed coassemblies.
 Optionally, reads can be mapped to the matched bins with only unmapped reads being assembled.
 
 ```bash
+# Example: cluster reads into proposed coassemblies
+ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --no-genomes
+
 # Example: cluster reads into proposed coassemblies based on unbinned sequences
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 
 # Example: cluster reads into proposed coassemblies based on unbinned sequences and coassemble only unbinned reads
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --assemble-unmapped
 
 # Example: cluster reads into proposed coassemblies based on unbinned sequences from a specific taxa
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --taxa-of-interest "p__Planctomycetota"
 
 # Example: find relevant samples for differential coverage binning (no coassembly)
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --single-assembly
 ```
 
+## Ibis evaluate
+
+Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
+Compares the recovery by phyla and by single-copy marker gene.
+
+```bash
+# Example: evaluate a completed coassembly
+ibis evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
+```
+
 ## Ibis iterate
 
 Run a further iteration of coassemble, including newly recovered bins.
 
 ```bash
 # Example: rerun coassemble, adding new bins to database
 ibis iterate --aviary-outputs coassembly_0_dir ... --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 ```
 
-## Ibis evaluate
+## Ibis update
 
-Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
-Compares the recovery by phyla and by single-copy marker gene.
+Applies further processing to a previous Ibis coassemble run: downloading SRA reads, generating unmapped reads files, and/or running Aviary commands.
 
 ```bash
-# Example: evaluate a completed coassembly
-ibis evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
-```
+# Example: update previous run to download SRA reads
+ibis update --sra --coassemble-output coassemble_dir --forward SRA000001 ... --reverse SRA000001 ... --genomes genome_1.fna ...
 
-## Ibis unmap
+# Example: update previous run to perform unmapping
+ibis update --assemble-unmapped --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 
-Applies unmapping to a previous Ibis coassemble run, generating unmapped reads files and Aviary commands.
-
-```bash
-# Example: generate unmapped reads and commands for completed coassembly
-ibis unmap --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
+# Example: update previous run to run specific coassemblies
+ibis update --run-aviary --coassemblies coassembly_0 ... --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 ```
```

### Comparing `ibis-genome-0.7.2/ibis/ibis.py` & `ibis-genome-0.8.0/ibis/ibis.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .__init__ import __version__
 __author__ = "Samuel Aroney"
 
 import os
 import sys
 import logging
 import subprocess
+import extern
 import importlib.resources
 import bird_tool_utils as btu
 import polars as pl
 from snakemake.io import load_configfile
 from ruamel.yaml import YAML
 import copy
 
@@ -106,26 +107,80 @@
 
     config_path = make_config(
         importlib.resources.files("ibis.config").joinpath("template_coassemble.yaml"),
         args.output,
         config_items
         )
 
+    if "mock_sra=True" in args.snakemake_args:
+        target_rule = "mock_download_sra"
+    else:
+        target_rule = "download_sra"
+
     run_workflow(
         config = config_path,
         workflow = "coassemble.smk",
         output_dir = args.output,
         cores = args.cores,
         dryrun = args.dryrun,
         conda_prefix = args.conda_prefix,
-        snakemake_args = args.snakemake_args + " -- download_sra" if args.snakemake_args else "-- download_sra",
+        snakemake_args = args.snakemake_args + " -- " + target_rule if args.snakemake_args else "-- " + target_rule,
     )
 
     sra_dir = args.output + "/coassemble/sra/"
     SRA_SUFFIX = ".fastq.gz"
+    expected_forward = [sra_dir + f + "_1" + SRA_SUFFIX for f in args.forward]
+    expected_reverse = [sra_dir + f + "_2" + SRA_SUFFIX for f in args.forward]
+
+    # Fix single file outputs if interleaved or error if unpaired
+    if not args.dryrun:
+        for f, r in zip(expected_forward, expected_reverse):
+            if os.path.isfile(f) & os.path.isfile(r):
+                continue
+
+            if os.path.isfile(f) | os.path.isfile(r):
+                raise Exception(f"Mismatched downloads with {f} and {r}")
+
+            u = f.replace("_1", "")
+            if not os.path.isfile(u):
+                raise Exception(f"Missing downloads: {f} and {r}")
+
+            logging.info(f"Checking single-file download for interleaved: {u}")
+            cmd = (
+                "python {script} "
+                "--input {input} "
+                "--start-check-pairs {start_check_pairs} "
+                "--end-check-pairs {end_check_pairs} "
+            ).format(
+                script = importlib.resources.files("ibis.workflow.scripts").joinpath("is_interleaved.py"),
+                input = u,
+                start_check_pairs = 5,
+                end_check_pairs = 5,
+            )
+            output = extern.run(cmd).strip().split("\t")
+
+            if output[0] != "True":
+                raise Exception(f"Download {u} was not interleaved: {output[1]}")
+
+            logging.info(f"Download {u} was interleaved: {output[1]}")
+            logging.info(f"Deinterleaving {u}")
+            cmd = (
+                "gunzip -c {input} | "
+                "paste - - - - - - - - | "
+                "tee >(cut -f 1-4 | tr '\t' '\n' | pigz --best --processes {threads} > {output_f}) "
+                "| cut -f 5-8 | tr '\t' '\n' | pigz --best --processes {threads} > {output_r}"
+            ).format(
+                input = u,
+                output_f = f,
+                output_r = r,
+                threads = max(1, args.cores // 2),
+            )
+            extern.run(cmd)
+
+
     # Need to convince Snakemake that the SRA data predates the completed outputs
     # Otherwise it will rerun all the rules with reason "updated input files"
     # Using Jan 1 2000 as pre-date
     os.makedirs(sra_dir, exist_ok=True)
     for sra in [f + s for f in args.forward for s in ["_1", "_2"]]:
         subprocess.check_call(f"touch -t 200001011200 {sra_dir + sra + SRA_SUFFIX}", shell=True)
 
@@ -152,15 +207,14 @@
     args.single_assembly = False
     args.no_genomes = False
     args.num_coassembly_samples = 1
     args.max_coassembly_samples = None
     args.max_coassembly_size = None
     args.max_recovery_samples = 1
     args.prodigal_meta = False
-    args.assemble_unmapped = True
 
     return(args)
 
 def evaluate_bins(aviary_outputs, checkm_version, min_completeness, max_contamination, iteration=None):
     logging.info(f"Evaluating bins using CheckM{str(checkm_version)} with completeness >= {str(min_completeness)} and contamination <= {str(max_contamination)}")
     recovered_bins = {
         os.path.basename(coassembly.rstrip("/")): 
@@ -288,18 +342,21 @@
         "max_coassembly_size": args.max_coassembly_size,
         "max_recovery_samples": args.max_recovery_samples,
         "prodigal_meta": args.prodigal_meta,
         # Coassembly config
         "assemble_unmapped": args.assemble_unmapped,
         "unmapping_min_appraised": args.unmapping_min_appraised,
         "unmapping_max_identity": args.unmapping_max_identity,
+        "unmapping_max_alignment": args.unmapping_max_alignment,
         "run_aviary": args.run_aviary,
-        "aviary_conda": args.aviary_conda,
+        "aviary_gtdbtk": args.aviary_gtdbtk_dir,
+        "aviary_checkm2": args.aviary_checkm2_dir,
         "aviary_threads": args.aviary_cores,
         "aviary_memory": args.aviary_memory,
+        "conda_prefix": args.conda_prefix,
     }
 
     config_path = make_config(
         importlib.resources.files("ibis.config").joinpath("template_coassemble.yaml"),
         args.output,
         config_items
         )
@@ -361,15 +418,15 @@
         output_dir = args.output,
         cores = args.cores,
         dryrun = args.dryrun,
         conda_prefix = args.conda_prefix,
         snakemake_args = args.snakemake_args,
     )
 
-def unmap(args):
+def update(args):
     logging.info("Loading Ibis coassemble info")
     if args.coassemble_output:
         args.elusive_clusters = os.path.join(args.coassemble_output, "target", "elusive_clusters.tsv")
         args.appraise_binned = os.path.join(args.coassemble_output, "appraise", "binned.otu_table.tsv")
         args.appraise_unbinned = os.path.join(args.coassemble_output, "appraise", "unbinned.otu_table.tsv")
     if args.elusive_clusters and not args.coassemblies:
         copy_input(
@@ -488,18 +545,26 @@
             ],
             "evaluate": [
                 btu.Example(
                     "evaluate a completed coassembly",
                     "ibis evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ..."
                 ),
             ],
-            "unmap": [
+            "update": [
+                btu.Example(
+                    "update previous run to download SRA reads",
+                    "ibis update --sra --coassemble-output coassemble_dir --forward SRA000001 ... --reverse SRA000001 ... --genomes genome_1.fna ..."
+                ),
+                btu.Example(
+                    "update previous run to perform unmapping",
+                    "ibis update --assemble-unmapped --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ..."
+                ),
                 btu.Example(
-                    "generate unmapped reads and commands for completed coassembly",
-                    "ibis unmap --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ..."
+                    "update previous run to run specific coassemblies",
+                    "ibis update --run-aviary --coassemblies coassembly_0 ... --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ..."
                 ),
             ],
             "iterate": [
                 btu.Example(
                     "rerun coassemble, adding new bins to database",
                     "ibis iterate --aviary-outputs coassembly_0_dir ... --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ..."
                 ),
@@ -525,16 +590,17 @@
 
     def add_evaluation_options(argument_group):
         argument_group.add_argument("--checkm-version", type=int, help="CheckM version to use to quality cutoffs [default: 2]", default=2)
         argument_group.add_argument("--min-completeness", type=int, help="Include bins with at least this minimum completeness [default: 70]", default=70)
         argument_group.add_argument("--max-contamination", type=int, help="Include bins with at most this maximum contamination [default: 10]", default=10)
 
     def add_aviary_options(argument_group):
-        argument_group.add_argument("--run-aviary", action="store_true", help="Run Aviary commands for all identified coassemblies")
-        argument_group.add_argument("--aviary-conda", help="Pre-built Aviary conda env path")
+        argument_group.add_argument("--run-aviary", action="store_true", help="Run Aviary commands for all identified coassemblies (unless specified)")
+        argument_group.add_argument("--aviary-gtdbtk-dir", help="Path to GTDB-Tk database directory for Aviary")
+        argument_group.add_argument("--aviary-checkm2-dir", help="Path to CheckM2 database directory for Aviary")
         argument_group.add_argument("--aviary-cores", type=int, help="Maximum number of cores for Aviary to use", default=16)
         argument_group.add_argument("--aviary-memory", type=int, help="Maximum amount of memory for Aviary to use (Gigabytes)", default=250)
 
     ###########################################################################
 
     coassemble_parser = main_parser.new_subparser("coassemble", "Coassemble reads clustered by unbinned single-copy marker genes")
 
@@ -568,14 +634,15 @@
         coassemble_clustering.add_argument("--max-recovery-samples", type=int, help="Upper bound for number of related samples to use for differential abundance binning [default: 20]", default=20)
         coassemble_clustering.add_argument("--prodigal-meta", action="store_true", help="Use prodigal \"-p meta\" argument (for testing)")
         # Coassembly options
         coassemble_coassembly = parser.add_argument_group("Coassembly options")
         coassemble_coassembly.add_argument("--assemble-unmapped", action="store_true", help="Only assemble reads that do not map to reference genomes")
         coassemble_coassembly.add_argument("--unmapping-min-appraised", type=int, help="Minimum fraction of sequences binned to justify unmapping [default: 0.1]", default=0.1)
         coassemble_coassembly.add_argument("--unmapping-max-identity", type=float, help="Maximum sequence identity of mapped sequences kept for coassembly [default: 99%]", default=99)
+        coassemble_coassembly.add_argument("--unmapping-max-alignment", type=float, help="Maximum percent alignment of mapped sequences kept for coassembly [default: 99%]", default=99)
         add_aviary_options(coassemble_coassembly)
         # General options
         coassemble_general = parser.add_argument_group("General options")
         add_general_snakemake_options(coassemble_general)
 
     add_coassemble_arguments(coassemble_parser)
 
@@ -598,32 +665,34 @@
     evaluate_cluster.add_argument("--genomes-list", help="Original genomes used as references for coassemble subcommand newline separated")
     # General options
     evaluate_general = evaluate_parser.add_argument_group("General options")
     add_general_snakemake_options(evaluate_general)
 
     ###########################################################################
 
-    unmap_parser = main_parser.new_subparser("unmap", "Coassemble pre-clustered reads")
+    update_parser = main_parser.new_subparser("update", "Coassemble pre-clustered reads")
     # Base arguments
-    unmap_base = unmap_parser.add_argument_group("Input arguments")
-    add_base_arguments(unmap_base)
-    unmap_base.add_argument("--sra", action="store_true", help="Download reads from SRA (read argument still required)")
+    update_base = update_parser.add_argument_group("Input arguments")
+    add_base_arguments(update_base)
+    update_base.add_argument("--sra", action="store_true", help="Download reads from SRA (read argument still required)")
     # Coassembly options
-    unmap_coassembly = unmap_parser.add_argument_group("Coassembly options")
-    unmap_coassembly.add_argument("--coassemble-output", help="Output dir from cluster subcommand")
-    unmap_coassembly.add_argument("--appraise-binned", help="SingleM appraise binned output from Ibis coassemble (alternative to --coassemble-output)")
-    unmap_coassembly.add_argument("--appraise-unbinned", help="SingleM appraise unbinned output from Ibis coassemble (alternative to --coassemble-output)")
-    unmap_coassembly.add_argument("--elusive-clusters", help="Elusive clusters output from Ibis coassemble (alternative to --coassemble-output)")
-    unmap_coassembly.add_argument("--coassemblies", nargs='+', help="Choose specific coassemblies from elusive clusters (e.g. coassembly_0)")
-    unmap_coassembly.add_argument("--unmapping-min-appraised", type=float, help="Minimum fraction of sequences binned to justify unmapping [default: 0.1]", default=0.1)
-    unmap_coassembly.add_argument("--unmapping-max-identity", type=float, help="Maximum sequence identity of mapped sequences kept for coassembly [default: 95%]", default=95)
-    add_aviary_options(unmap_coassembly)
+    update_coassembly = update_parser.add_argument_group("Coassembly options")
+    update_coassembly.add_argument("--coassemble-output", help="Output dir from cluster subcommand")
+    update_coassembly.add_argument("--appraise-binned", help="SingleM appraise binned output from Ibis coassemble (alternative to --coassemble-output)")
+    update_coassembly.add_argument("--appraise-unbinned", help="SingleM appraise unbinned output from Ibis coassemble (alternative to --coassemble-output)")
+    update_coassembly.add_argument("--elusive-clusters", help="Elusive clusters output from Ibis coassemble (alternative to --coassemble-output)")
+    update_coassembly.add_argument("--coassemblies", nargs='+', help="Choose specific coassemblies from elusive clusters (e.g. coassembly_0)")
+    update_coassembly.add_argument("--assemble-unmapped", action="store_true", help="Only assemble reads that do not map to reference genomes")
+    update_coassembly.add_argument("--unmapping-min-appraised", type=float, help="Minimum fraction of sequences binned to justify unmapping [default: 0.1]", default=0.1)
+    update_coassembly.add_argument("--unmapping-max-identity", type=float, help="Maximum sequence identity of mapped sequences kept for coassembly [default: 95%]", default=95)
+    update_coassembly.add_argument("--unmapping-max-alignment", type=float, help="Maximum percent alignment of mapped sequences kept for coassembly [default: 90%]", default=90)
+    add_aviary_options(update_coassembly)
     # General options
-    unmap_general = unmap_parser.add_argument_group("General options")
-    add_general_snakemake_options(unmap_general)
+    update_general = update_parser.add_argument_group("General options")
+    add_general_snakemake_options(update_general)
 
     ###########################################################################
 
     iterate_parser = main_parser.new_subparser("iterate", "Iterate coassemble using new bins")
     # Iterate options
     iterate_iteration = iterate_parser.add_argument_group("Iteration options")
     iterate_iteration.add_argument("--iteration", help="Iteration number used for unique bin naming", default="0")
@@ -668,35 +737,35 @@
             raise Exception("General, list and directory arguments are mutually exclusive")
         if args.max_coassembly_samples:
             if args.max_coassembly_samples > args.max_recovery_samples:
                 raise Exception("Max recovery samples (--max-recovery-samples) must be greater than or equal to max coassembly samples (--max-coassembly-samples)")
         else:
             if args.num_coassembly_samples > args.max_recovery_samples:
                 raise Exception("Max recovery samples (--max-recovery-samples) must be greater than or equal to number of coassembly samples (--num-coassembly-samples)")
-        if args.run_aviary and not args.aviary_conda:
-            raise Exception("Run Aviary (--run-aviary) requires pre-build conda env path to be provided (--aviary-conda)")
+        if args.run_aviary and not (args.aviary_gtdbtk_dir and args.aviary_checkm2_dir):
+            raise Exception("Run Aviary (--run-aviary) requires paths to GTDB-Tk and CheckM2 databases to be provided (--aviary-gtdbtk-dir and --aviary-checkm2-dir)")
 
     if args.subparser_name == "coassemble":
         coassemble_argument_verification(args)
         coassemble(args)
 
     elif args.subparser_name == "evaluate":
         if not args.singlem_metapackage and not os.environ['SINGLEM_METAPACKAGE_PATH']:
             raise Exception("SingleM metapackage (--singlem-metapackage or SINGLEM_METAPACKAGE_PATH environment variable, see SingleM data) must be provided")
         if args.cluster and not (args.genomes or args.genomes_list):
             raise Exception("Reference genomes must be provided to cluster with new genomes")
         evaluate(args)
 
-    elif args.subparser_name == "unmap":
+    elif args.subparser_name == "update":
         base_argument_verification(args)
         if not args.coassemble_output and not (args.appraise_binned and args.appraise_unbinned and args.elusive_clusters):
             raise Exception("Either Ibis coassemble output (--coassemble-output) or specific input files (--appraise-binned and --elusive-clusters) must be provided")
-        if args.run_aviary and not args.aviary_conda:
-            raise Exception("Run Aviary (--run-aviary) requires pre-build conda env path to be provided (--aviary-conda)")
-        unmap(args)
+        if args.run_aviary and not (args.aviary_gtdbtk_dir and args.aviary_checkm2_dir):
+            raise Exception("Run Aviary (--run-aviary) requires paths to GTDB-Tk and CheckM2 databases to be provided (--aviary-gtdbtk-dir and --aviary-checkm2-dir)")
+        update(args)
 
     elif args.subparser_name == "iterate":
         if args.sample_query or args.sample_query_list or args.sample_query_dir:
             raise Exception("Query arguments are incompatible with Ibis iterate")
         if args.sample_singlem_dir or args.sample_query_dir:
             raise Exception("Directory arguments are incompatible with Ibis iterate")
         if args.single_assembly:
```

### Comparing `ibis-genome-0.7.2/ibis/workflow/coassemble.smk` & `ibis-genome-0.8.0/ibis/workflow/coassemble.smk`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #############
 ### Setup ###
 #############
 ruleorder: no_genomes > query_processing > singlem_appraise_filtered
+ruleorder: mock_download_sra > download_sra
 
 import os
 import pandas as pd
 
 output_dir = os.path.abspath("coassemble")
 logs_dir = output_dir + "/logs"
 
 mapped_reads_1 = {read: output_dir + f"/mapping/{read}_unmapped.1.fq.gz" for read in config["reads_1"]}
 mapped_reads_2 = {read: output_dir + f"/mapping/{read}_unmapped.2.fq.gz" for read in config["reads_2"]}
 
 def get_reads(wildcards, forward=True, version=None):
     version = version if version else wildcards.version
-    if version == "":
+    if version == "" or version == "whole":
         if forward:
             return config["reads_1"]
         else:
             return config["reads_2"]
     elif version == "unmapped_":
         if forward:
             return mapped_reads_1
         else:
             return mapped_reads_2
     else:
-        raise ValueError("Version should be empty or unmapped")
+        raise ValueError("Version should be empty, 'whole' or 'unmapped'")
 
 def get_cat(wildcards):
     return "zcat" if [r for r in get_reads(wildcards).values()][0].endswith(".gz") else "cat"
 
 def get_reads_coassembly(wildcards, forward=True, recover=False):
     checkpoint_output = checkpoints.cluster_graph.get(**wildcards).output[0]
     elusive_clusters = pd.read_csv(checkpoint_output, sep = "\t")
@@ -40,15 +41,15 @@
         sample_names = elusive_clusters[elusive_clusters["coassembly"] == wildcards.coassembly]["samples"].iloc[0]
 
     sample_names = sample_names.split(",")
 
     if config["assemble_unmapped"]:
         version = "unmapped_"
     else:
-        version = ""
+        version = "whole"
 
     reads = get_reads(wildcards, forward=forward, version=version)
     return [reads[n] for n in sample_names]
 
 def get_coassemblies(wildcards):
     checkpoint_output = checkpoints.cluster_graph.get().output[0]
     elusive_clusters = pd.read_csv(checkpoint_output, sep = "\t")
@@ -302,18 +303,38 @@
         logs_dir + "/sra/kingfisher.log"
     shell:
         "mkdir -p {output} && "
         "cd {output} && "
         "kingfisher get "
         "-r {params.sra} "
         "-f fastq.gz "
-        "-m ena-ascp ena-ftp prefetch aws-http aws-cp "
+        "-m ena-ftp prefetch ena-ascp aws-http aws-cp "
         "-t {threads} "
         "&> {log} "
 
+rule mock_download_sra:
+    output:
+        directory(output_dir + "/sra") if config["mock_sra"] else []
+    threads:
+        64
+    params:
+        sra_f=" ".join([s + "_1.fastq.gz" for s in config["sra"][1:]]) if config["sra"] else "",
+        sra_r=" ".join([s + "_2.fastq.gz" for s in config["sra"][1:]]) if config["sra"] else "",
+        sra_u=config["sra"][0] + ".fastq.gz" if config["sra"] else "",
+        sra_basedir=workflow.basedir + "/../../test/data/sra",
+    conda:
+        "env/kingfisher.yml"
+    log:
+        logs_dir + "/sra/kingfisher.log"
+    shell:
+        "mkdir -p {output} && "
+        "cd {output} && "
+        "touch {params.sra_f} {params.sra_r} && "
+        "cp {params.sra_basedir}/{params.sra_u} {params.sra_u} "
+
 #####################################
 ### Map reads to matching genomes ###
 #####################################
 rule collect_genomes:
     input:
         appraise_binned=output_dir + "/appraise/binned.otu_table.tsv",
         appraise_unbinned=output_dir + "/appraise/unbinned.otu_table.tsv",
@@ -355,24 +376,27 @@
         temp(output_dir + "/mapping/{read}_unmapped.bam"),
     log:
         logs_dir + "/mapping/{read}_filter.log",
     params:
         genomes="{read}_reference.fna",
         reads_1=lambda wildcards: os.path.basename(config["reads_1"][wildcards.read]),
         sequence_identity=config["unmapping_max_identity"],
+        alignment_percent=config["unmapping_max_alignment"],
     threads:
         32
     conda:
         "env/coverm.yml"
     shell:
         "coverm filter "
         "-b {input}/{params.genomes}.{params.reads_1}.bam "
         "-o {output} "
         "--inverse "
-        "--min-read-percent-identity {params.sequence_identity} "
+        "--min-read-percent-identity-pair {params.sequence_identity} "
+        "--min-read-aligned-percent-pair {params.alignment_percent} "
+        "--proper-pairs-only "
         "&> {log}"
 
 rule bam_to_fastq:
     input:
         output_dir + "/mapping/{read}_unmapped.bam",
     output:
         reads_1=output_dir + "/mapping/{read}_unmapped.1.fq.gz",
@@ -436,57 +460,77 @@
     output:
         dir=directory(output_dir + "/coassemble/{coassembly}/assemble"),
         assembly=output_dir + "/coassemble/{coassembly}/assemble/assembly/final_contigs.fasta",
     params:
         reads_1 = lambda wildcards: get_reads_coassembly(wildcards),
         reads_2 = lambda wildcards: get_reads_coassembly(wildcards, forward=False),
         memory=config["aviary_memory"],
+        dryrun = "--dryrun" if config["aviary_dryrun"] else "",
+        drymkdir = "&& mkdir -p "+output_dir+"/coassemble/{coassembly}/assemble/assembly" if config["aviary_dryrun"] else "",
+        drytouch = "&& touch "+output_dir+"/coassemble/{coassembly}/assemble/assembly/final_contigs.fasta" if config["aviary_dryrun"] else "",
+        conda_prefix = config["conda_prefix"] if config["conda_prefix"] else ".",
     threads:
         threads=config["aviary_threads"]
     log:
         logs_dir + "/aviary/{coassembly}_assemble.log"
     conda:
-        config["aviary_conda"]
+        "env/aviary.yml"
     shell:
+        "GTDBTK_DATA_PATH=. "
+        "CHECKM2DB=. "
+        "EGGNOG_DATA_DIR=. "
+        "CONDA_ENV_PATH={params.conda_prefix} "
         "aviary assemble "
         "-1 {params.reads_1} "
         "-2 {params.reads_2} "
         "--output {output.dir} "
         "-n {threads} "
         "-t {threads} "
         "-m {params.memory} "
+        "{params.dryrun} "
         "&> {log} "
+        "{params.drymkdir} "
+        "{params.drytouch} "
 
 rule aviary_recover:
     input:
         assembly=output_dir + "/coassemble/{coassembly}/assemble/assembly/final_contigs.fasta",
         elusive_clusters=output_dir + "/target/elusive_clusters.tsv",
     output:
         directory(output_dir + "/coassemble/{coassembly}/recover")
     params:
         reads_1 = lambda wildcards: get_reads_coassembly(wildcards, recover=True),
         reads_2 = lambda wildcards: get_reads_coassembly(wildcards, forward=False, recover=True),
         memory=config["aviary_memory"],
         skip_binners = "--skip-binners rosella semibin metabat1 vamb concoct maxbin2 maxbin" if config["test"] else "",
+        dryrun = "--dryrun" if config["aviary_dryrun"] else "",
+        gtdbtk=config["aviary_gtdbtk"],
+        checkm2=config["aviary_checkm2"],
+        conda_prefix = config["conda_prefix"] if config["conda_prefix"] else ".",
     threads:
         config["aviary_threads"]
     log:
         logs_dir + "/aviary/{coassembly}_recover.log"
     conda:
-        config["aviary_conda"]
+        "env/aviary.yml"
     shell:
+        "GTDBTK_DATA_PATH={params.gtdbtk} "
+        "CHECKM2DB={params.checkm2} "
+        "EGGNOG_DATA_DIR=. "
+        "CONDA_ENV_PATH={params.conda_prefix} "
         "aviary recover "
         "--assembly {input.assembly} "
         "-1 {params.reads_1} "
         "-2 {params.reads_2} "
         "--output {output} "
         "{params.skip_binners} "
         "-n {threads} "
         "-t {threads} "
         "-m {params.memory} "
+        "{params.dryrun} "
         "&> {log} "
 
 rule aviary_combine:
     input:
         get_coassemblies,
         elusive_clusters=output_dir + "/target/elusive_clusters.tsv",
         mapping=output_dir + "/mapping/done" if config["assemble_unmapped"] else [],
```

### Comparing `ibis-genome-0.7.2/ibis/workflow/env/singlem.yml` & `ibis-genome-0.8.0/ibis/workflow/env/singlem.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 channels:
   - conda-forge
   - bioconda
-  - defaults
 dependencies:
   - python>=3.7
   - diamond>2.0.11,<2.1.3
   - biopython
   - hmmer
   - orfm
   - mfqe
```

### Comparing `ibis-genome-0.7.2/ibis/workflow/evaluate.smk` & `ibis-genome-0.8.0/ibis/workflow/evaluate.smk`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/aviary_commands.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/aviary_commands.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/cluster_graph.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/cluster_graph.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/collect_reference_bins.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/evaluate.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/no_genomes.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/no_genomes.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/query_processing.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/query_processing.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/separate_SingleM_seq.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/separate_SingleM_seq.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/summarise_coassemblies.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/summarise_coassemblies.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis/workflow/scripts/target_elusive.py` & `ibis-genome-0.8.0/ibis/workflow/scripts/target_elusive.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/ibis_genome.egg-info/PKG-INFO` & `ibis-genome-0.8.0/ibis_genome.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-genome
-Version: 0.7.2
+Version: 0.8.0
 Summary: Ibis (Australian bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,14 +683,16 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ibis
 
+[<img src="ibis_logo.png" width="50%" />](ibis_logo.png)
+
 Ibis (bin chicken) - targeted recovery of low abundance genomes through intelligent coassembly.
 
 ## Installation options
 
 ### Install from pip
 
 Install latest release via pip.
@@ -717,47 +719,56 @@
 Creates graph with samples as nodes and the number of overlapping sequences provided by SingleM.
 The taxa of the considered sequences can be filtered to target a specific taxon (e.g. the phylum Planctomycetota).
 The graph is clustered using the Girvan-Newman algorithm to provide sample groupings.
 Aviary assemble/recover commands are generated based on proposed coassemblies.
 Optionally, reads can be mapped to the matched bins with only unmapped reads being assembled.
 
 ```bash
+# Example: cluster reads into proposed coassemblies
+ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --no-genomes
+
 # Example: cluster reads into proposed coassemblies based on unbinned sequences
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 
 # Example: cluster reads into proposed coassemblies based on unbinned sequences and coassemble only unbinned reads
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --assemble-unmapped
 
 # Example: cluster reads into proposed coassemblies based on unbinned sequences from a specific taxa
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ... --taxa-of-interest "p__Planctomycetota"
 
 # Example: find relevant samples for differential coverage binning (no coassembly)
 ibis coassemble --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --single-assembly
 ```
 
+## Ibis evaluate
+
+Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
+Compares the recovery by phyla and by single-copy marker gene.
+
+```bash
+# Example: evaluate a completed coassembly
+ibis evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
+```
+
 ## Ibis iterate
 
 Run a further iteration of coassemble, including newly recovered bins.
 
 ```bash
 # Example: rerun coassemble, adding new bins to database
 ibis iterate --aviary-outputs coassembly_0_dir ... --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 ```
 
-## Ibis evaluate
+## Ibis update
 
-Evaluates the recovery of target genes by coassemblies suggested by above, finding the number of target genes present in the newly recovered genomes.
-Compares the recovery by phyla and by single-copy marker gene.
+Applies further processing to a previous Ibis coassemble run: downloading SRA reads, generating unmapped reads files, and/or running Aviary commands.
 
 ```bash
-# Example: evaluate a completed coassembly
-ibis evaluate --coassemble-output coassemble_dir --aviary-outputs coassembly_0_dir ...
-```
+# Example: update previous run to download SRA reads
+ibis update --sra --coassemble-output coassemble_dir --forward SRA000001 ... --reverse SRA000001 ... --genomes genome_1.fna ...
 
-## Ibis unmap
+# Example: update previous run to perform unmapping
+ibis update --assemble-unmapped --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 
-Applies unmapping to a previous Ibis coassemble run, generating unmapped reads files and Aviary commands.
-
-```bash
-# Example: generate unmapped reads and commands for completed coassembly
-ibis unmap --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
+# Example: update previous run to run specific coassemblies
+ibis update --run-aviary --coassemblies coassembly_0 ... --coassemble-output coassemble_dir --forward reads_1.1.fq ... --reverse reads_1.2.fq ... --genomes genome_1.fna ...
 ```
```

### Comparing `ibis-genome-0.7.2/ibis_genome.egg-info/SOURCES.txt` & `ibis-genome-0.8.0/ibis_genome.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ibis/workflow/env/prodigal.yml
 ibis/workflow/env/r.yml
 ibis/workflow/env/singlem.yml
 ibis/workflow/scripts/aviary_commands.py
 ibis/workflow/scripts/cluster_graph.py
 ibis/workflow/scripts/collect_reference_bins.py
 ibis/workflow/scripts/evaluate.py
+ibis/workflow/scripts/is_interleaved.py
 ibis/workflow/scripts/no_genomes.py
 ibis/workflow/scripts/query_processing.py
 ibis/workflow/scripts/separate_SingleM_seq.py
 ibis/workflow/scripts/summarise_coassemblies.py
 ibis/workflow/scripts/target_elusive.py
 ibis_genome.egg-info/PKG-INFO
 ibis_genome.egg-info/SOURCES.txt
@@ -30,12 +31,14 @@
 ibis_genome.egg-info/requires.txt
 ibis_genome.egg-info/top_level.txt
 test/test_cluster_graph.py
 test/test_coassemble.py
 test/test_collect_reference_bins.py
 test/test_evaluate.py
 test/test_evaluate_script.py
+test/test_is_interleaved.py
 test/test_iterate.py
+test/test_manual.py
 test/test_no_genomes.py
 test/test_query_processing.py
 test/test_target_elusive.py
-test/test_unmap.py
+test/test_update.py
```

### Comparing `ibis-genome-0.7.2/pyproject.toml` & `ibis-genome-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_cluster_graph.py` & `ibis-genome-0.8.0/test/test_cluster_graph.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_coassemble.py` & `ibis-genome-0.8.0/test/test_coassemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,29 +68,30 @@
             cmd = (
                 f"ibis coassemble "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--singlem-metapackage {METAPACKAGE} "
                 f"--assemble-unmapped "
-                f"--unmapping-max-identity 95 "
+                f"--unmapping-max-identity 99 "
+                f"--unmapping-max-alignment 90 "
                 f"--prodigal-meta "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
             )
             extern.run(cmd)
 
             config_path = os.path.join("test", "config.yaml")
             self.assertTrue(os.path.exists(config_path))
 
             read_size_path = os.path.join("test", "coassemble", "read_size.csv")
             self.assertTrue(os.path.exists(read_size_path))
             expected = "\n".join(
                 [
-                    ",".join(["sample_1", "3322"]),
+                    ",".join(["sample_1", "3624"]),
                     ",".join(["sample_2", "2416"]),
                     ",".join(["sample_3", "2416"]),
                     ""
                 ]
             )
             with open(read_size_path) as f:
                 self.assertEqual(expected, f.read())
@@ -116,15 +117,15 @@
                         "coassembly",
                     ]),
                     "\t".join([
                         "sample_1,sample_2",
                         "2",
                         "2",
                         "2",
-                        "5738",
+                        "6040",
                         "sample_1,sample_2,sample_3",
                         "coassembly_0"
                     ]),
                     ""
                 ]
             )
             with open(cluster_path) as f:
@@ -140,15 +141,15 @@
             self.assertFalse(os.path.exists(coverm_working_dir))
 
             unmapped_sample_1_path = os.path.join("test", "coassemble", "mapping", "sample_1_unmapped.1.fq.gz")
             self.assertTrue(os.path.exists(unmapped_sample_1_path))
             with gzip.open(unmapped_sample_1_path) as f:
                 file = f.read().decode()
                 self.assertTrue("@A00178:112:HMNM5DSXX:4:1622:16405:19194" in file)
-                self.assertTrue("@A00178:118:HTHTVDSXX:1:1249:16740:14105" not in file)
+                self.assertTrue("@A00178:112:HMNM5DSXX:4:9999:19126:17300" not in file)
 
             coassemble_path = os.path.join("test", "coassemble", "commands", "coassemble_commands.sh")
             self.assertTrue(os.path.exists(coassemble_path))
             test_dir = os.path.abspath("test")
             expected = "\n".join(
                 [
                     " ".join([
@@ -209,16 +210,16 @@
                     ]),
                     "\t".join([
                         "coassembly_0",
                         "sample_1,sample_2",
                         "2",
                         "2",
                         "2",
+                        "6040",
                         "5738",
-                        "4832",
                     ]),
                     ""
                 ]
             )
             with open(summary_path) as f:
                 self.assertEqual(expected, f.read())
 
@@ -489,15 +490,15 @@
                         "coassembly_1"
                     ]),
                     "\t".join([
                         "sample_1",
                         "1",
                         "0",
                         "0",
-                        "3322",
+                        "3624",
                         "sample_1,sample_2,sample_3",
                         "coassembly_2"
                     ]),
                     ""
                 ]
             )
             with open(cluster_path) as f:
@@ -555,15 +556,15 @@
                         "coassembly",
                     ]),
                     "\t".join([
                         "sample_1,sample_2",
                         "2",
                         "2",
                         "2",
-                        "5738",
+                        "6040",
                         "sample_1,sample_2,sample_3",
                         "coassembly_0"
                     ]),
                     ""
                 ]
             )
             with open(cluster_path) as f:
@@ -718,15 +719,16 @@
             self.assertTrue("aviary_commands" in output)
 
     def test_coassemble_run_aviary(self):
         with in_tempdir():
             cmd = (
                 f"ibis coassemble "
                 f"--run-aviary "
-                f"--aviary-conda aviary "
+                f"--aviary-gtdbtk-dir gtdb_release "
+                f"--aviary-checkm2-dir CheckM2_database "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--genome-transcripts {GENOME_TRANSCRIPTS} "
                 f"--sample-singlem {SAMPLE_SINGLEM} "
                 f"--sample-read-size {SAMPLE_READ_SIZE} "
                 f"--genome-singlem {GENOME_SINGLEM} "
@@ -758,15 +760,16 @@
 
     def test_coassemble_run_aviary_unmapped(self):
         with in_tempdir():
             cmd = (
                 f"ibis coassemble "
                 f"--assemble-unmapped "
                 f"--run-aviary "
-                f"--aviary-conda aviary "
+                f"--aviary-gtdbtk-dir gtdb_release "
+                f"--aviary-checkm2-dir CheckM2_database "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--genome-transcripts {GENOME_TRANSCRIPTS} "
                 f"--sample-singlem {SAMPLE_SINGLEM} "
                 f"--sample-read-size {SAMPLE_READ_SIZE} "
                 f"--genome-singlem {GENOME_SINGLEM} "
```

### Comparing `ibis-genome-0.7.2/test/test_collect_reference_bins.py` & `ibis-genome-0.8.0/test/test_collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_evaluate.py` & `ibis-genome-0.8.0/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_evaluate_script.py` & `ibis-genome-0.8.0/test/test_evaluate_script.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_iterate.py` & `ibis-genome-0.8.0/test/test_iterate.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_no_genomes.py` & `ibis-genome-0.8.0/test/test_no_genomes.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_query_processing.py` & `ibis-genome-0.8.0/test/test_query_processing.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_target_elusive.py` & `ibis-genome-0.8.0/test/test_target_elusive.py`

 * *Files identical despite different names*

### Comparing `ibis-genome-0.7.2/test/test_unmap.py` & `ibis-genome-0.8.0/test/test_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import unittest
 import os
 import gzip
 from bird_tool_utils import in_tempdir
 import extern
+from snakemake.io import load_configfile
 
 path_to_data = os.path.join(os.path.dirname(os.path.realpath(__file__)),'data')
 path_to_conda = os.path.join(path_to_data,'.conda')
 
 SAMPLE_READS_FORWARD = " ".join([
     os.path.join(path_to_data, "sample_1.1.fq"),
     os.path.join(path_to_data, "sample_2.1.fq"),
@@ -29,18 +30,19 @@
 APPRAISE_BINNED = os.path.join(MOCK_COASSEMBLE, "appraise", "binned.otu_table.tsv")
 APPRAISE_UNBINNED = os.path.join(MOCK_COASSEMBLE, "appraise", "unbinned.otu_table.tsv")
 ELUSIVE_CLUSTERS = os.path.join(MOCK_COASSEMBLE, "target", "elusive_clusters.tsv")
 ELUSIVE_CLUSTERS_TWO = os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_two.tsv')
 
 
 class Tests(unittest.TestCase):
-    def test_unmap(self):
+    def test_update(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
+                f"ibis update "
+                f"--assemble-unmapped "
                 f"--coassemble-output {MOCK_COASSEMBLE} "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
             )
@@ -59,15 +61,15 @@
             self.assertFalse(os.path.exists(coverm_working_dir))
 
             unmapped_sample_1_path = os.path.join("test", "coassemble", "mapping", "sample_1_unmapped.1.fq.gz")
             self.assertTrue(os.path.exists(unmapped_sample_1_path))
             with gzip.open(unmapped_sample_1_path) as f:
                 file = f.read().decode()
                 self.assertTrue("@A00178:112:HMNM5DSXX:4:1622:16405:19194" in file)
-                self.assertTrue("@A00178:118:HTHTVDSXX:1:1249:16740:14105" not in file)
+                self.assertTrue("@A00178:112:HMNM5DSXX:4:9999:19126:17300" not in file)
 
             coassemble_path = os.path.join("test", "coassemble", "commands", "coassemble_commands.sh")
             self.assertTrue(os.path.exists(coassemble_path))
             test_dir = os.path.abspath("test")
             expected = "\n".join(
                 [
                     " ".join([
@@ -109,18 +111,19 @@
                     ]),
                     ""
                 ]
             )
             with open(recover_path) as f:
                 self.assertEqual(expected, f.read())
 
-    def test_unmap_specified_files(self):
+    def test_update_specified_files(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
+                f"ibis update "
+                f"--assemble-unmapped "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--appraise-binned {APPRAISE_BINNED} "
                 f"--appraise-unbinned {APPRAISE_UNBINNED} "
                 f"--elusive-clusters {ELUSIVE_CLUSTERS} "
                 f"--output test "
@@ -141,19 +144,21 @@
             self.assertTrue("target_elusive" not in output)
             self.assertTrue("cluster_graph" not in output)
             self.assertTrue("collect_genomes" in output)
             self.assertTrue("map_reads" in output)
             self.assertTrue("finish_mapping" in output)
             self.assertTrue("aviary_commands" in output)
 
-    def test_unmap_read_identity(self):
+    def test_update_read_identity(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
+                f"ibis update "
+                f"--assemble-unmapped "
                 f"--unmapping-max-identity 99 "
+                f"--unmapping-max-alignment 90 "
                 f"--coassemble-output {MOCK_COASSEMBLE} "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
             )
@@ -174,18 +179,19 @@
             unmapped_sample_1_path = os.path.join("test", "coassemble", "mapping", "sample_1_unmapped.1.fq.gz")
             self.assertTrue(os.path.exists(unmapped_sample_1_path))
             with gzip.open(unmapped_sample_1_path) as f:
                 file = f.read().decode()
                 self.assertTrue("@A00178:112:HMNM5DSXX:4:1622:16405:19194" in file)
                 self.assertTrue("@A00178:118:HTHTVDSXX:1:1249:16740:14105" in file)
 
-    def test_unmap_sra_download(self):
+    def test_update_sra_download(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
+                f"ibis update "
+                f"--assemble-unmapped "
                 f"--forward SRR8334323 SRR8334324 "
                 f"--sra "
                 f"--genomes {GENOMES} "
                 f"--coassemble-output {MOCK_COASSEMBLE} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--dryrun "
@@ -209,52 +215,71 @@
             self.assertTrue("target_elusive" not in output)
             self.assertTrue("cluster_graph" not in output)
             self.assertTrue("collect_genomes" in output)
             self.assertTrue("map_reads" in output)
             self.assertTrue("finish_mapping" in output)
             self.assertTrue("aviary_commands" in output)
 
-    @unittest.skip("Downloads SRA data using Kingfisher. Test manually")
-    def test_unmap_sra_download_real(self):
+    def test_update_sra_download_mock(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
-                f"--forward SRR8334323 SRR8334324 "
+                f"ibis update "
+                f"--forward SRR3309137 SRR8334323 SRR8334324 "
                 f"--sra "
                 f"--genomes {GENOMES} "
                 f"--appraise-binned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'binned_sra.otu_table.tsv')} "
                 f"--appraise-unbinned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'unbinned_sra.otu_table.tsv')} "
-                f"--elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra.tsv')} "
+                f"--elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra_mock.tsv')} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
+                f"--snakemake-args \" --config mock_sra=True\" "
             )
             extern.run(cmd)
 
-            config_path = os.path.join("test", "config.yaml")
-            self.assertTrue(os.path.exists(config_path))
-
-            sra_1_path = os.path.join("test", "coassemble", "sra", "SRR8334323_1.fastq.gz")
+            sra_1_path = os.path.join("test", "coassemble", "sra", "SRR3309137_1.fastq.gz")
             self.assertTrue(os.path.exists(sra_1_path))
             with gzip.open(sra_1_path) as f:
                 file = f.readline().decode()
-                self.assertTrue("@SRR8334323.1 HS2:487:H80UEADXX:1:1101:1148:1986/1" in file)
-                self.assertTrue("@SRR8334323.2 HS2:487:H80UEADXX:1:1101:1148:1986/2" not in file)
+                self.assertTrue("@SRR3309137.1 HISEQ06:195:D1DRHACXX:5:1101:1597:2236/1" in file)
+                self.assertTrue("@SRR3309137.2 HISEQ06:195:D1DRHACXX:5:1101:1597:2236/1" not in file)
+
+            sra_2_path = os.path.join("test", "coassemble", "sra", "SRR3309137_2.fastq.gz")
+            self.assertTrue(os.path.exists(sra_2_path))
+            with gzip.open(sra_2_path) as f:
+                file = f.readline().decode()
+                self.assertTrue("@SRR3309137.2 HISEQ06:195:D1DRHACXX:5:1101:1597:2236/1" in file)
+                self.assertTrue("@SRR3309137.1 HISEQ06:195:D1DRHACXX:5:1101:1597:2236/1" not in file)
 
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334323_2.fastq.gz")))
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334324_1.fastq.gz")))
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334324_2.fastq.gz")))
+    def test_update_sra_download_mock_fail(self):
+        with in_tempdir():
+            cmd = (
+                f"ibis update "
+                f"--forward SRR3309137_mismatched SRR8334323 SRR8334324 "
+                f"--sra "
+                f"--genomes {GENOMES} "
+                f"--appraise-binned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'binned_sra.otu_table.tsv')} "
+                f"--appraise-unbinned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'unbinned_sra.otu_table.tsv')} "
+                f"--elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra_mock.tsv')} "
+                f"--output test "
+                f"--conda-prefix {path_to_conda} "
+                f"--snakemake-args \" --config mock_sra=True\" "
+            )
+            with self.assertRaises(Exception):
+                extern.run(cmd)
 
-    def test_unmap_aviary_run(self):
+    def test_update_aviary_run(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
+                f"ibis update "
+                f"--assemble-unmapped "
                 f"--forward SRR8334323 SRR8334324 "
                 f"--sra "
                 f"--run-aviary "
-                f"--aviary-conda aviary "
+                f"--aviary-gtdbtk-dir gtdb_release "
+                f"--aviary-checkm2-dir CheckM2_database "
                 f"--genomes {GENOMES} "
                 f"--appraise-binned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'binned_sra.otu_table.tsv')} "
                 f"--appraise-unbinned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'unbinned_sra.otu_table.tsv')} "
                 f"--elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra.tsv')} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
                 f"--dryrun "
@@ -281,58 +306,63 @@
             self.assertTrue("map_reads" in output)
             self.assertTrue("finish_mapping" in output)
             self.assertTrue("aviary_commands" not in output)
             self.assertTrue("aviary_assemble" in output)
             self.assertTrue("aviary_recover" in output)
             self.assertTrue("aviary_combine" in output)
 
-    @unittest.skip("Downloads SRA data using Kingfisher and runs Aviary. Test manually")
-    def test_unmap_aviary_run_real(self):
+    def test_update_aviary_dryrun(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
-                f"--forward SRR8334323 SRR8334324 "
-                f"--sra "
+                f"ibis update "
                 f"--run-aviary "
-                f"--cores 32 "
-                f"--aviary-cores 32 "
-                f"--aviary-memory 500 "
-                f"--aviary-conda /mnt/hpccs01/work/microbiome/conda/envs/aviary-v0.5.7 "
+                f"--aviary-gtdbtk-dir gtdb_release "
+                f"--aviary-checkm2-dir CheckM2_database "
+                f"--coassemble-output {MOCK_COASSEMBLE} "
+                f"--forward {SAMPLE_READS_FORWARD} "
+                f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
-                f"--appraise-binned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'binned_sra.otu_table.tsv')} "
-                f"--appraise-unbinned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'unbinned_sra.otu_table.tsv')} "
-                f"--elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra.tsv')} "
                 f"--output test "
                 f"--conda-prefix {path_to_conda} "
-                f"--snakemake-args \" --config test=True\" "
+                f"--snakemake-args \" --config test=True aviary_dryrun=True\" "
             )
-            output = extern.run(cmd)
+            extern.run(cmd)
 
             config_path = os.path.join("test", "config.yaml")
             self.assertTrue(os.path.exists(config_path))
 
-            sra_1_path = os.path.join("test", "coassemble", "sra", "SRR8334323_1.fastq.gz")
-            self.assertTrue(os.path.exists(sra_1_path))
-            with gzip.open(sra_1_path) as f:
-                file = f.readline().decode()
-                self.assertTrue("@SRR8334323.1 1/1" in file)
-                self.assertTrue("@SRR8334323.1 1/2" not in file)
-
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334323_2.fastq.gz")))
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334324_1.fastq.gz")))
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334324_2.fastq.gz")))
+            coassembly_path = os.path.join("test", "coassemble", "coassemble", "coassembly_0")
+            contigs_path = os.path.join(coassembly_path, "assemble", "assembly", "final_contigs.fasta")
+            self.assertTrue(os.path.exists(contigs_path))
+
+            assembly_config_path = os.path.join(coassembly_path, "assemble", "config.yaml")
+            self.assertTrue(os.path.exists(assembly_config_path))
+            assembly_config = load_configfile(assembly_config_path)
+            forward_reads = SAMPLE_READS_FORWARD.split(" ")
+            self.assertTrue(forward_reads[0] in assembly_config["short_reads_1"])
+            self.assertTrue(forward_reads[1] in assembly_config["short_reads_1"])
+            self.assertFalse(forward_reads[2] in assembly_config["short_reads_1"])
+            self.assertTrue(assembly_config["coassemble"])
+
+            recovery_config_path = os.path.join(coassembly_path, "recover", "config.yaml")
+            self.assertTrue(os.path.exists(recovery_config_path))
+            recovery_config = load_configfile(recovery_config_path)
+            self.assertTrue(forward_reads[0] in recovery_config["short_reads_1"])
+            self.assertTrue(forward_reads[1] in recovery_config["short_reads_1"])
+            self.assertTrue(forward_reads[2] in recovery_config["short_reads_1"])
+            self.assertEqual(recovery_config["fasta"][0], os.path.abspath(contigs_path))
+            self.assertEqual(recovery_config["checkm2_db_folder"], "CheckM2_database")
+            self.assertEqual(recovery_config["gtdbtk_folder"], "gtdb_release")
+            self.assertEqual(recovery_config["eggnog_folder"], ".")
 
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "coassemble", "coassembly_0", "assemble", "assembly", "final_contigs.fna")))
-
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "coassemble", "coassembly_0", "recover", "bins", "checkm_minimal.tsv")))
-
-    def test_unmap_specific_coassembly(self):
+    def test_update_specific_coassembly(self):
         with in_tempdir():
             cmd = (
-                f"ibis unmap "
+                f"ibis update "
+                f"--assemble-unmapped "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
                 f"--appraise-binned {APPRAISE_BINNED} "
                 f"--appraise-unbinned {APPRAISE_UNBINNED} "
                 f"--elusive-clusters {ELUSIVE_CLUSTERS_TWO} "
                 f"--coassemblies coassembly_0 "
@@ -349,44 +379,10 @@
             self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "mapping", "sample_2_unmapped.1.fq.gz")))
             self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "mapping", "sample_2_unmapped.2.fq.gz")))
             self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "mapping", "sample_3_unmapped.1.fq.gz")))
             self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "mapping", "sample_3_unmapped.2.fq.gz")))
             self.assertFalse(os.path.exists(os.path.join("test", "coassemble", "mapping", "sample_4_unmapped.1.fq.gz")))
             self.assertFalse(os.path.exists(os.path.join("test", "coassemble", "mapping", "sample_4_unmapped.2.fq.gz")))
 
-    @unittest.skip("Downloads SRA data using Kingfisher. Test manually")
-    def test_unmap_specific_coassembly_sra(self):
-        with in_tempdir():
-            cmd = (
-                f"ibis unmap "
-                f"--forward SRR8334323 SRR8334324 "
-                f"--sra "
-                f"--genomes {GENOMES} "
-                f"--appraise-binned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'binned_sra.otu_table.tsv')} "
-                f"--appraise-unbinned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'unbinned_sra.otu_table.tsv')} "
-                f"--elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra_two.tsv')} "
-                f"--coassemblies coassembly_0 "
-                f"--output test "
-                f"--conda-prefix {path_to_conda} "
-            )
-            output = extern.run(cmd)
-
-            config_path = os.path.join("test", "config.yaml")
-            self.assertTrue(os.path.exists(config_path))
-
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334323_1.fastq.gz")))
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334323_2.fastq.gz")))
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334324_1.fastq.gz")))
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334324_2.fastq.gz")))
-
-            self.assertFalse(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334320_1.fastq.gz")))
-            self.assertFalse(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334320_2.fastq.gz")))
-            self.assertFalse(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334321_1.fastq.gz")))
-            self.assertFalse(os.path.exists(os.path.join("test", "coassemble", "sra", "SRR8334321_2.fastq.gz")))
-
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "coassemble", "coassembly_0", "assemble", "assembly", "final_contigs.fna")))
-
-            self.assertTrue(os.path.exists(os.path.join("test", "coassemble", "coassemble", "coassembly_0", "recover", "bins", "checkm_minimal.tsv")))
-
 
 if __name__ == '__main__':
     unittest.main()
```

