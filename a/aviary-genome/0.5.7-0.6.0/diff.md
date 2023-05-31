# Comparing `tmp/aviary-genome-0.5.7.tar.gz` & `tmp/aviary-genome-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aviary-genome-0.5.7.tar", last modified: Tue Dec 20 22:42:39 2022, max compression
+gzip compressed data, was "aviary-genome-0.6.0.tar", last modified: Wed May 31 02:10:39 2023, max compression
```

## Comparing `aviary-genome-0.5.7.tar` & `aviary-genome-0.6.0.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47729 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/aviary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/checkm.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      401 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/checkm2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/coverm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/groopm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/gtdbtk.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/singlem.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/envs/webpage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/modules/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/annotation/annotation.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/modules/annotation/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/annotation/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/annotation/envs/busco.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       97 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/annotation/envs/eggnog.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/modules/annotation/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/annotation/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.273285 aviary-genome-0.5.7/aviary/modules/assembly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26928 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/assembly.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/assembly/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/circlator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/final_assembly.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/flye.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/medaka.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/megahit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/mfqe.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/pilon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/pysam.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/racon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/seqtk.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/envs/spades.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/isolate.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/assembly/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3543 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/assemble_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/assemble_short_reads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      667 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/combine_assemblies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3540 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/filter_illumina_assembly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/filter_illumina_reference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/filter_read_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2807 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/generate_pilon_sort.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4062 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/get_binned_reads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/pool_reads.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/racon_polish.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/assembly/scripts/run_flye.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/benchmarking/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/benchmarking/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51233 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/benchmarking/benchmarking.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/benchmarking/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/benchmarking/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/benchmarking/envs/magpurify.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/benchmarking/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/benchmarking/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/binning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33233 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/binning.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/binning/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/concoct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/das_tool.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/maxbin2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/metabat2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/rosella.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      392 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/semibin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/envs/vamb.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/binning/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/scripts/get_abundances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/scripts/get_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/scripts/make_long_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/scripts/prepare_rosella_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8118 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/scripts/rosella_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/binning/scripts/write_vamb_bins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/cluster/clustering.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/cluster/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/cluster/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/cluster/envs/pggb.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/cluster/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/cluster/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25736 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.277285 aviary-genome-0.5.7/aviary/modules/quality_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/quality_control/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/envs/fastqc.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/envs/filtlong.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/envs/nanoplot.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/envs/quast.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     7727 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/qc.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/quality_control/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1931 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/scripts/fraction_recovered.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/quality_control/scripts/run_fastqc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/strain_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/strain_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/strain_analysis/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/strain_analysis/envs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/strain_analysis/envs/lorikeet.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/strain_analysis/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/strain_analysis/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/strain_analysis/scripts/run_lorikeet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/strain_analysis/strain_analysis.smk
--rw-r--r--   0 runner    (1001) docker     (123)      701 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/template_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/viral_analysis/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/viral_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/viral_analysis/envs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/viral_analysis/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/viral_analysis/envs/virfinder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/viral_analysis/envs/virsorter.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/modules/viral_analysis/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/viral_analysis/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      622 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/modules/viral_analysis/viral_analysis.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   211909 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/scripts/create_aviary_webpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/scripts/process_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/scripts/process_viral_batch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/scripts/run_busco.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/scripts/run_virfinder.R
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/aviary/scripts/singlem_reads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/aviary_genome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2022-12-20 22:42:39.000000 aviary-genome-0.5.7/aviary_genome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2022-12-20 22:42:39.000000 aviary-genome-0.5.7/aviary_genome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 22:42:39.000000 aviary-genome-0.5.7/aviary_genome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-20 22:42:39.000000 aviary-genome-0.5.7/aviary_genome.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 22:42:39.000000 aviary-genome-0.5.7/aviary_genome.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-20 22:42:39.000000 aviary-genome-0.5.7/aviary_genome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-20 22:42:39.000000 aviary-genome-0.5.7/aviary_genome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:42:39.281285 aviary-genome-0.5.7/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2147 2022-12-20 22:42:36.000000 aviary-genome-0.5.7/test/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.924999 aviary-genome-0.6.0/aviary/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50402 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/aviary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.924999 aviary-genome-0.6.0/aviary/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.924999 aviary-genome-0.6.0/aviary/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/checkm.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/checkm2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/coverm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/groopm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/gtdbtk.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/singlem.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/envs/webpage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.924999 aviary-genome-0.6.0/aviary/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.924999 aviary-genome-0.6.0/aviary/modules/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/annotation/annotation.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.924999 aviary-genome-0.6.0/aviary/modules/annotation/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/annotation/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/annotation/envs/busco.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/annotation/envs/eggnog.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.924999 aviary-genome-0.6.0/aviary/modules/annotation/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/annotation/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.928999 aviary-genome-0.6.0/aviary/modules/assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27057 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/assembly.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.928999 aviary-genome-0.6.0/aviary/modules/assembly/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/circlator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/final_assembly.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/flye.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/medaka.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/megahit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/mfqe.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/pilon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/polishing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/pysam.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/seqtk.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/envs/spades.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/isolate.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.932999 aviary-genome-0.6.0/aviary/modules/assembly/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3543 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/assemble_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/assemble_short_reads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/combine_assemblies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3540 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/filter_illumina_assembly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/filter_illumina_reference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/filter_read_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2807 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/generate_pilon_sort.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4062 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/get_binned_reads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/polish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/pool_reads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      843 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/assembly/scripts/run_flye.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.932999 aviary-genome-0.6.0/aviary/modules/benchmarking/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/benchmarking/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51233 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/benchmarking/benchmarking.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.932999 aviary-genome-0.6.0/aviary/modules/benchmarking/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/benchmarking/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/benchmarking/envs/magpurify.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.932999 aviary-genome-0.6.0/aviary/modules/benchmarking/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/benchmarking/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.932999 aviary-genome-0.6.0/aviary/modules/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33233 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/binning.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/binning/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/concoct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/das_tool.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/maxbin2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/metabat2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/rosella.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      392 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/semibin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/envs/vamb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/binning/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/scripts/get_abundances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/scripts/get_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/scripts/make_long_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/scripts/prepare_rosella_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8118 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/scripts/rosella_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/binning/scripts/write_vamb_bins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/cluster/clustering.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/cluster/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/cluster/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/cluster/envs/pggb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/cluster/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/cluster/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25877 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/quality_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/quality_control/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/envs/fastqc.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/envs/filtlong.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/envs/nanoplot.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/envs/quast.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7726 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/qc.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/quality_control/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/scripts/fraction_recovered.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/quality_control/scripts/run_fastqc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.936999 aviary-genome-0.6.0/aviary/modules/strain_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/strain_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/aviary/modules/strain_analysis/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/strain_analysis/envs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/strain_analysis/envs/lorikeet.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/aviary/modules/strain_analysis/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/strain_analysis/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/strain_analysis/scripts/run_lorikeet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/strain_analysis/strain_analysis.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/template_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/aviary/modules/viral_analysis/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/viral_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/aviary/modules/viral_analysis/envs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/viral_analysis/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/viral_analysis/envs/virfinder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/viral_analysis/envs/virsorter.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/aviary/modules/viral_analysis/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/viral_analysis/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      622 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/modules/viral_analysis/viral_analysis.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/aviary/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   211909 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/scripts/create_aviary_webpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/scripts/process_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/scripts/process_viral_batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/scripts/run_busco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/scripts/run_virfinder.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/aviary/scripts/singlem_reads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/aviary_genome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-31 02:10:39.000000 aviary-genome-0.6.0/aviary_genome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-31 02:10:39.000000 aviary-genome-0.6.0/aviary_genome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:10:39.000000 aviary-genome-0.6.0/aviary_genome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 02:10:39.000000 aviary-genome-0.6.0/aviary_genome.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 02:10:39.000000 aviary-genome-0.6.0/aviary_genome.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 02:10:39.000000 aviary-genome-0.6.0/aviary_genome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 02:10:39.000000 aviary-genome-0.6.0/aviary_genome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 02:10:39.948999 aviary-genome-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 02:10:39.944999 aviary-genome-0.6.0/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2147 2023-05-31 02:10:35.000000 aviary-genome-0.6.0/test/test_integration.py
```

### Comparing `aviary-genome-0.5.7/LICENSE` & `aviary-genome-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/PKG-INFO` & `aviary-genome-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviary-genome
-Version: 0.5.7
+Version: 0.6.0
 Summary: aviary - metagenomics pipeline using long and short reads
 Home-page: https://github.com/rhysnewell/aviary
 Author: Rhys Newell
 Author-email: rhys.newell94@gmail.com
 License: GPL-3.0
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `aviary-genome-0.5.7/README.md` & `aviary-genome-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/aviary.py` & `aviary-genome-0.6.0/aviary/aviary.py`

 * *Files 8% similar despite different names*

```diff
@@ -389,19 +389,46 @@
         nargs='*',
         default="none"
     )
 
     long_read_group.add_argument(
         '-z', '--longread-type', '--longread_type', '--long_read_type', '--long-read-type',
         help='Whether the sequencing platform and technology for the longreads. \n'
-             '"rs" for PacBio RSII, "sq" for PacBio Sequel, "ccs" for PacBio CCS \n'
+             '"rs" for PacBio RSII, "sq" for PacBio Sequel, "ccs" for PacBio CCS, "hifi" for PacBio HiFi \n'
              'reads, "ont" for Oxford Nanopore and "ont_hq" for Oxford Nanopore high quality reads (Guppy5+ or Q20) \n',
         dest='longread_type',
         default="ont",
-        choices=["ont","ont_hq", "rs", "sq", "ccs"],
+        choices=["ont","ont_hq", "rs", "sq", "ccs", "hifi"],
+    )
+
+    long_read_group.add_argument(
+        '--medaka-model', '--medaka_model',
+        help='Medaka model to use for polishing long reads. \n',
+        dest='medaka_model',
+        default="r941_min_hac_g507",
+        choices=[
+            "r103_fast_g507", "r103_fast_snp_g507", "r103_fast_variant_g507", "r103_hac_g507", "r103_hac_snp_g507",
+            "r103_hac_variant_g507", "r103_min_high_g345", "r103_min_high_g360", "r103_prom_high_g360", "r103_prom_snp_g3210",
+            "r103_prom_variant_g3210", "r103_sup_g507", "r103_sup_snp_g507", "r103_sup_variant_g507", "r1041_e82_260bps_fast_g632",
+            "r1041_e82_260bps_fast_variant_g632", "r1041_e82_260bps_hac_g632", "r1041_e82_260bps_hac_variant_g632", "r1041_e82_260bps_sup_g632",
+            "r1041_e82_260bps_sup_variant_g632", "r1041_e82_400bps_fast_g615", "r1041_e82_400bps_fast_g632",
+            "r1041_e82_400bps_fast_variant_g615", "r1041_e82_400bps_fast_variant_g632", "r1041_e82_400bps_hac_g615",
+            "r1041_e82_400bps_hac_g632", "r1041_e82_400bps_hac_variant_g615", "r1041_e82_400bps_hac_variant_g632", "r1041_e82_400bps_sup_g615",
+            "r1041_e82_400bps_sup_variant_g615", "r104_e81_fast_g5015", "r104_e81_fast_variant_g5015", "r104_e81_hac_g5015",
+            "r104_e81_hac_variant_g5015", "r104_e81_sup_g5015", "r104_e81_sup_g610", "r104_e81_sup_variant_g610", "r10_min_high_g303",
+            "r10_min_high_g340", "r941_e81_fast_g514", "r941_e81_fast_variant_g514", "r941_e81_hac_g514", "r941_e81_hac_variant_g514",
+            "r941_e81_sup_g514", "r941_e81_sup_variant_g514", "r941_min_fast_g303", "r941_min_fast_g507", "r941_min_fast_snp_g507",
+            "r941_min_fast_variant_g507", "r941_min_hac_g507", "r941_min_hac_snp_g507", "r941_min_hac_variant_g507", "r941_min_high_g303",
+            "r941_min_high_g330", "r941_min_high_g340_rle", "r941_min_high_g344", "r941_min_high_g351", "r941_min_high_g360", "r941_min_sup_g507",
+            "r941_min_sup_snp_g507", "r941_min_sup_variant_g507", "r941_prom_fast_g303", "r941_prom_fast_g507", "r941_prom_fast_snp_g507",
+            "r941_prom_fast_variant_g507", "r941_prom_hac_g507", "r941_prom_hac_snp_g507", "r941_prom_hac_variant_g507", "r941_prom_high_g303",
+            "r941_prom_high_g330", "r941_prom_high_g344", "r941_prom_high_g360", "r941_prom_high_g4011", "r941_prom_snp_g303", "r941_prom_snp_g322",
+            "r941_prom_snp_g360", "r941_prom_sup_g507", "r941_prom_sup_snp_g507", "r941_prom_sup_variant_g507", "r941_prom_variant_g303",
+            "r941_prom_variant_g322", "r941_prom_variant_g360", "r941_sup_plant_g610", "r941_sup_plant_variant_g610"
+        ]
     )
 
     long_read_group.add_argument(
         '--min-percent-read-identity-long', '--min_percent_read_identity_long',
         help='Minimum percent read identity used by CoverM for long-reads'
              'when calculating genome abundances.',
         dest='long_percent_identity',
@@ -649,46 +676,46 @@
 
     assemble_group.add_argument(
         '--min-cov-long', '--min_cov_long',
         help='Automatically include Flye contigs with long read coverage greater than or equal to this. \n'
              'High long read coverage during assembly indicates that the overlap layout consensus algorithm \n'
              'is more likely to be correct.',
         dest='min_cov_long',
-        default=20
+        default=5
     )
 
     assemble_group.add_argument(
         '--min-cov-short', '--min_cov_short',
         help='Automatically include Flye contigs with short read coverage less than or equal to this. \n'
              'Low coverage via short reads indicates that metaSPAdes will not be able to better assemble this contig.',
         dest='min_cov_short',
-        default=3
+        default=5
     )
 
     assemble_group.add_argument(
         '--exclude-contig-cov', '--exclude_contig_cov',
         help='Automatically exclude Flye contigs with long read coverage less than or equal to this \n'
              'and less than or equal to `--exclude-contig-size`',
         dest='exclude_contig_cov',
-        default=100
+        default=10
     )
 
     assemble_group.add_argument(
         '--exclude-contig-size', '--exclude_contig_size',
         help='Automatically exclude Flye contigs with length less than or equal to this \n'
              'and long read coverage less than or equal to `--exclude-contig-cov`',
         dest='exclude_contig_size',
-        default=25000
+        default=2500
     )
 
     assemble_group.add_argument(
         '--include-contig-size', '--include_contig_size',
-        help='Automatically include Flye contigs with length less than or equal to this',
+        help='Automatically include Flye contigs with length greater than or equal to this',
         dest='include_contig_size',
-        default=100000
+        default=10000
     )
 
     #~#~#~#~#~#~#~#~#~#~#~#~#~   sub-parsers   ~#~#~#~#~#~#~#~#~#~#~#~#~#
     ##########################  ~ ASSEMBLE ~  ###########################
 
     assemble_options = subparsers.add_parser('assemble',
                                               description='Step-down hybrid assembly using long and short reads, or assembly using only short or long reads.',
@@ -705,15 +732,15 @@
 
 
     assemble_options.add_argument(
         '-w', '--workflow',
         help='Main workflow to run',
         dest='workflow',
         nargs="+",
-        default=['complete_assembly'],
+        default=['complete_assembly_with_qc'],
     )
 
     ##########################  ~ RECOVER ~   ###########################
 
     recover_options = subparsers.add_parser('recover',
                                             description='The aviary binning pipeline',
                                             formatter_class=CustomHelpFormatter,
```

### Comparing `aviary-genome-0.5.7/aviary/config/config.py` & `aviary-genome-0.6.0/aviary/config/config.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/Snakefile` & `aviary-genome-0.6.0/aviary/modules/Snakefile`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/annotation/annotation.smk` & `aviary-genome-0.6.0/aviary/modules/annotation/annotation.smk`

 * *Files 5% similar despite different names*

```diff
@@ -58,28 +58,26 @@
         'logs/download_eggnog.log'
     shell:
         'mkdir -p {params.eggnog_db}; '
         'download_eggnog_data.py --data_dir {params.eggnog_db} -y 2> {log} '
 
 rule download_gtdb:
     params:
-        gtdbtk_folder = os.path.expanduser(config['gtdbtk_folder']),
-        gtdbtk_version = '207.0'
+        gtdbtk_folder = os.path.expanduser(config['gtdbtk_folder'])
     conda:
         '../../envs/gtdbtk.yaml'
     threads: 1
     log:
         'logs/download_gtdb.log'
     shell:
         'GTDBTK_DATA_PATH={params.gtdbtk_folder}; '
         'mkdir -p {params.gtdbtk_folder}; '
         # Configuration
-        'N_FILES_IN_TAR=139919; '
-        'DB_URL="https://data.gtdb.ecogenomic.org/releases/release207/207.0/auxillary_files/gtdbtk_r207_v2_data.tar.gz"; '
-        'TARGET_TAR_NAME="gtdbtk_r207_v2_data.tar.gz"; '
+        'DB_URL="https://data.gtdb.ecogenomic.org/releases/latest/auxillary_files/gtdbtk_data.tar.gz"; '
+        'TARGET_TAR_NAME="gtdbtk_data.tar.gz"; '
 
         # Script variables (no need to configure)
         'TARGET_DIR=${{1:-$GTDBTK_DATA_PATH}}; '
         'TARGET_TAR="${{TARGET_DIR}}/${{TARGET_TAR_NAME}}"; '
 
         # Check if this is overriding an existing version
         'mkdir -p "$TARGET_DIR"; '
@@ -95,15 +93,15 @@
         # Start the download process
         # Note: When this URL is updated, ensure that the "--total" flag of TQDM below is also updated
         'echo "[INFO] - Downloading the GTDB-Tk database to: ${{TARGET_DIR}}"; '
         'wget $DB_URL -O "$TARGET_TAR"; '
 
         # Uncompress and pipe output to TQDM
         'echo "[INFO] - Extracting archive..."; '
-        'tar xvzf "$TARGET_TAR" -C "${{TARGET_DIR}}" --strip 1 | tqdm --unit=file --total=$N_FILES_IN_TAR --smoothing=0.1 >/dev/null; '
+        'tar xvzf "$TARGET_TAR" -C "${{TARGET_DIR}}" --strip 1; '
 
         # Remove the file after successful extraction
         'rm "$TARGET_TAR"; '
         'echo "[INFO] - The GTDB-Tk database has been successfully downloaded and extracted."; '
 
         # Set the environment variable
         'if conda env config vars set TARGET_DIR="$TARGET_DIR"; then '
@@ -188,15 +186,15 @@
         "../../envs/gtdbtk.yaml"
     threads:
         config["max_threads"]
     benchmark:
         'benchmarks/gtdbtk.benchmark.txt'
     shell:
         "export GTDBTK_DATA_PATH={params.gtdbtk_folder} && "
-        "gtdbtk classify_wf --cpus {threads} --pplacer_cpus {params.pplacer_threads} --extension {params.extension} "
+        "gtdbtk classify_wf --skip_ani_screen --cpus {threads} --pplacer_cpus {params.pplacer_threads} --extension {params.extension} "
         "--genome_dir {input.mag_folder} --out_dir data/gtdbtk && touch data/gtdbtk/done"
 
 rule annotate:
     input:
          'data/gtdbtk/done',
          'data/eggnog/done',
     output:
```

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/assembly.smk` & `aviary-genome-0.6.0/aviary/modules/assembly/assembly.smk`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,20 @@
     group: 'assembly'
     output:
         temp("data/raw_mapped_ref.bam")
     conda:
         "../../envs/coverm.yaml"
     benchmark:
         "benchmarks/map_reads_ref.benchmark.txt"
+    params:
+        mapper = "map-ont" if config["long_read_type"] in ["ont", "ont-hq"] else "map-pb"
     threads:
          config["max_threads"]
     shell:
-        "minimap2 -ax map-ont --split-prefix=tmp -t {threads} {input.reference_filter} {input.fastq} | samtools view -@ {threads} -b > {output}"
+        "minimap2 -ax {params.mapper} --split-prefix=tmp -t {threads} {input.reference_filter} {input.fastq} | samtools view -@ {threads} -b > {output}"
 
 
 # Get a list of reads that don't map to genome you want to filter
 rule get_umapped_reads_ref:
     input:
         "data/raw_mapped_ref.bam"
     group: 'assembly'
@@ -125,38 +127,38 @@
         "benchmarks/flye_assembly.benchmark.txt"
     threads:
         config["max_threads"]
     script:
         "scripts/run_flye.py"
 
 
-# Polish the long reads assembly with Racon
-rule polish_metagenome_racon:
+# Polish the long reads assembly with Racon or Medaka
+rule polish_metagenome_flye:
     input:
         fastq = "data/long_reads.fastq.gz",
         fasta = "data/flye/assembly.fasta",
     conda:
-        "envs/racon.yaml"
+        "envs/polishing.yaml"
     threads:
         config["max_threads"]
     params:
-        prefix = "racon",
+        prefix = "polished",
         maxcov = 200,
         rounds = 3,
         illumina = False,
         coassemble = config["coassemble"]
     resources:
         mem_mb=int(config["max_memory"])*1024
     group: 'assembly'
     output:
         fasta = "data/assembly.pol.rac.fasta"
     benchmark:
-        "benchmarks/polish_metagenome_racon.benchmark.txt"
+        "benchmarks/polish_metagenome_flye.benchmark.txt"
     script:
-        "scripts/racon_polish.py"
+        "scripts/polish.py"
 
 
 ### Filter illumina reads against provided reference
 rule filter_illumina_ref:
     input:
         reference_filter = config["reference_filter"]
     group: 'assembly'
@@ -228,40 +230,40 @@
 rule polish_meta_racon_ill:
     input:
         fastq = config['short_reads_1'], # check short reads are here
         fasta = "data/assembly.pol.pil.fasta"
     group: 'assembly'
     output:
         fasta = "data/assembly.pol.fin.fasta",
-        paf = temp("data/racon_polishing/alignment.racon_ill.0.paf")
+        paf = temp("data/polishing/alignment.racon_ill.0.paf")
     resources:
         mem_mb=int(config["max_memory"])*1024
     threads:
         config["max_threads"]
     conda:
-        "envs/racon.yaml"
+        "envs/polishing.yaml"
     params:
         prefix = "racon_ill",
         maxcov = 200,
         rounds = 1,
         illumina = True,
         coassemble = config["coassemble"]
     benchmark:
         "benchmarks/polish_meta_racon_ill.benchmark.txt"
     script:
-        "scripts/racon_polish.py"
+        "scripts/polish.py"
 
 
 # High coverage contigs are identified
 rule get_high_cov_contigs:
     input:
         info = "data/flye/assembly_info.txt",
         fasta = "data/assembly.pol.fin.fasta",
         graph = "data/flye/assembly_graph.gfa",
-        paf = "data/racon_polishing/alignment.racon_ill.0.paf"
+        paf = "data/polishing/alignment.racon_ill.0.paf"
     group: 'assembly'
     output:
         fasta = "data/flye_high_cov.fasta"
     benchmark:
         "benchmarks/get_high_cov_contigs.benchmark.txt"
     params:
         min_cov_long = int(config["min_cov_long"]),
@@ -719,15 +721,16 @@
         sizes = "www/assembly_stats.txt"
     shell:
         'mkdir -p www/; '
         'stats.sh {input.fasta} > {output.sizes}; '
         'mkdir -p assembly; '
         'cd assembly; '
         'ln -s ../data/final_contigs.fasta ./; '
-        'rm -rf data/racon_polishing; '
+        'cd ../;'
+        'rm -rf data/polishing; '
 
 rule complete_assembly_with_qc:
     input:
         fasta = 'data/final_contigs.fasta',
         qc_done = 'data/qc_done'
     group: 'assembly'
     output:
@@ -735,15 +738,16 @@
         sizes = "www/assembly_stats.txt"
     shell:
         'mkdir -p www/; '
         'stats.sh {input.fasta} > {output.sizes}; '
         'mkdir -p assembly; '
         'cd assembly; '
         'ln -s ../data/final_contigs.fasta ./; '
-        'rm -rf data/racon_polishing; '
+        'cd ../;'
+        'rm -rf data/polishing; '
 
 rule reset_to_spades_assembly:
     output:
          temp('data/reset_spades')
     shell:
          'rm -rf data/spades*; '
          'rm -rf assembly/; '
```

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/isolate.smk` & `aviary-genome-0.6.0/aviary/modules/assembly/isolate.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/assemble_pools.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/assemble_pools.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/assemble_short_reads.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/assemble_short_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/combine_assemblies.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/combine_assemblies.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/filter_illumina_assembly.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/filter_illumina_assembly.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/filter_illumina_reference.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/filter_illumina_reference.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/filter_read_list.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/filter_read_list.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/generate_pilon_sort.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/generate_pilon_sort.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/get_binned_reads.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/get_binned_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/pool_reads.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/pool_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/racon_polish.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/polish.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
+import sys
 import subprocess
 import random
 import shutil
 import logging
 
-out = "data/racon_polishing"
+out = "data/polishing"
 max_cov = snakemake.params.maxcov
 
 try:
     os.makedirs(out)
 except FileExistsError:
     pass
 
@@ -60,134 +61,150 @@
                 subprocess.Popen(f"pigz -p {snakemake.threads} --fast data/short_reads.1.fastq",
                                  shell=True).wait()
             pe1 = "data/short_reads.1.fastq.gz"
         reads = [pe1]
 else:
     reads = snakemake.input.fastq
 
-for rounds in range(snakemake.params.rounds):
-    paf = os.path.join(out, 'alignment.%s.%d.paf') % (snakemake.params.prefix, rounds)
-    print("Generating PAF file: %s for racon round %d..." % (paf, rounds))
-
-    # Generate PAF mapping files
-    if not os.path.exists(paf): # Check if mapping already exists
-        if snakemake.params.illumina:
-            if reads != "data/short_reads.fastq.gz":
-                subprocess.Popen("minimap2 -t %d -x sr %s %s > %s" % (snakemake.threads, reference, ' '.join(reads), paf),
-                                 shell=True).wait()
-            else:
-                subprocess.Popen("minimap2 -t %d -x sr %s %s > %s" % (snakemake.threads, reference, reads, paf),
-                                 shell=True).wait()
-        elif snakemake.config["long_read_type"] in ['ont', 'ont_hq']:
-            subprocess.Popen("minimap2 -t %d -x map-ont %s %s > %s" % (snakemake.threads, reference, reads, paf), shell=True).wait()
-        else:
-            subprocess.Popen("minimap2 -t %d -x map-pb %s %s > %s" % (snakemake.threads, reference, reads, paf), shell=True).wait()
+# use racon when using illumina or pacbio data
+if snakemake.params.illumina or snakemake.config["long_read_type"] not in ['ont', 'ont_hq']:
+    for rounds in range(snakemake.params.rounds):
+        paf = os.path.join(out, 'alignment.%s.%d.paf') % (snakemake.params.prefix, rounds)
+        print("Generating PAF file: %s for racon round %d..." % (paf, rounds))
 
-    cov_dict = {}
-    # Populate coverage dictionary,
-    with open(paf) as f:
-        for line in f:
-            qname, qlen, qstart, qstop, strand, ref, rlen, rstart, rstop = line.split()[:9]
-            qlen, qstart, qstop, rlen, rstart, rstop = map(int, [qlen, qstart, qstop, rlen, rstart, rstop])
-            if ref in cov_dict:
-                cov_dict[ref] += (rstop - rstart) / rlen
+        # Generate PAF mapping files
+        if not os.path.exists(paf): # Check if mapping already exists
+            if snakemake.params.illumina:
+                if reads != "data/short_reads.fastq.gz":
+                    subprocess.Popen("minimap2 -t %d -x sr %s %s > %s" % (snakemake.threads, reference, ' '.join(reads), paf),
+                                    shell=True).wait()
+                else:
+                    subprocess.Popen("minimap2 -t %d -x sr %s %s > %s" % (snakemake.threads, reference, reads, paf),
+                                    shell=True).wait()
+            elif snakemake.config["long_read_type"] in ['ont', 'ont_hq']:
+                sys.exit("ONT reads are not supported for racon polishing")
             else:
-                cov_dict[ref] = (rstop - rstart) / rlen
+                subprocess.Popen("minimap2 -t %d -x map-pb %s %s > %s" % (snakemake.threads, reference, reads, paf), shell=True).wait()
 
-    high_cov = set()
-    low_cov = set()
-    for i in cov_dict:
-        if cov_dict[i] >= max_cov:
-            high_cov.add(i)
-        else:
-            low_cov.add(i)
+        cov_dict = {}
+        # Populate coverage dictionary,
+        with open(paf) as f:
+            for line in f:
+                qname, qlen, qstart, qstop, strand, ref, rlen, rstart, rstop = line.split()[:9]
+                qlen, qstart, qstop, rlen, rstart, rstop = map(int, [qlen, qstart, qstop, rlen, rstart, rstop])
+                if ref in cov_dict:
+                    cov_dict[ref] += (rstop - rstart) / rlen
+                else:
+                    cov_dict[ref] = (rstop - rstart) / rlen
+
+        high_cov = set()
+        low_cov = set()
+        for i in cov_dict:
+            if cov_dict[i] >= max_cov:
+                high_cov.add(i)
+            else:
+                low_cov.add(i)
 
-    no_cov = set()
-    with open(reference) as ref_file, open(os.path.join(out, "filtered.%s.%d.fa" % (snakemake.params.prefix, rounds)), 'w') as o:
-        for line in ref_file:
-            if line.startswith('>'):
-                name = line.split()[0][1:]
-                if name in low_cov or name in high_cov:
+        no_cov = set()
+        with open(reference) as ref_file, open(os.path.join(out, "filtered.%s.%d.fa" % (snakemake.params.prefix, rounds)), 'w') as o:
+            for line in ref_file:
+                if line.startswith('>'):
+                    name = line.split()[0][1:]
+                    if name in low_cov or name in high_cov:
+                        o.write(line)
+                        getseq = True
+                    else:
+                        no_cov.add(name)
+                        getseq = False
+                elif getseq:
                     o.write(line)
-                    getseq = True
-                else:
-                    no_cov.add(name)
-                    getseq = False
-            elif getseq:
-                o.write(line)
-
-    included_reads = set()
-    excluded_reads = set()
-    with open(paf) as f, open(os.path.join(out, "filtered.%s.%d.paf" % (snakemake.params.prefix, rounds)), 'w') as paf_file:
-        for line in f:
-            qname, qlen, qstart, qstop, strand, ref, rlen, rstart, rstop = line.split()[:9]
-            qlen, qstart, qstop, rlen, rstart, rstop = map(int, [qlen, qstart, qstop, rlen, rstart, rstop])
-            if snakemake.params.illumina:
-                if qname[:-2] in ['/1', '/2']:
-                    qname = qname[:-2]
-            if ref in low_cov:
-                paf_file.write(line)
-                included_reads.add(qname)
-            elif ref in high_cov:
-                # Down sample reads from high coverage contigs
-                sample_rate = max_cov / cov_dict[ref]
-                if qname in excluded_reads:
-                    pass
-                elif qname in included_reads:
+
+        included_reads = set()
+        excluded_reads = set()
+        with open(paf) as f, open(os.path.join(out, "filtered.%s.%d.paf" % (snakemake.params.prefix, rounds)), 'w') as paf_file:
+            for line in f:
+                qname, qlen, qstart, qstop, strand, ref, rlen, rstart, rstop = line.split()[:9]
+                qlen, qstart, qstop, rlen, rstart, rstop = map(int, [qlen, qstart, qstop, rlen, rstart, rstop])
+                if snakemake.params.illumina:
+                    if qname[:-2] in ['/1', '/2']:
+                        qname = qname[:-2]
+                if ref in low_cov:
                     paf_file.write(line)
-                elif random.random() < sample_rate:
                     included_reads.add(qname)
-                    paf_file.write(line)
+                elif ref in high_cov:
+                    # Down sample reads from high coverage contigs
+                    sample_rate = max_cov / cov_dict[ref]
+                    if qname in excluded_reads:
+                        pass
+                    elif qname in included_reads:
+                        paf_file.write(line)
+                    elif random.random() < sample_rate:
+                        included_reads.add(qname)
+                        paf_file.write(line)
+                    else:
+                        excluded_reads.add(qname)
+        with open(os.path.join(out, "reads.%s.%d.lst" % (snakemake.params.prefix, rounds)), "w") as o:
+            for i in included_reads:
+                if (reads == 'data/short_reads.fastq.gz' or snakemake.config['short_reads_2'] == 'none') and snakemake.params.illumina:
+                    o.write(i + '/1\n')
+                    o.write(i + '/2\n')
                 else:
-                    excluded_reads.add(qname)
-    with open(os.path.join(out, "reads.%s.%d.lst" % (snakemake.params.prefix, rounds)), "w") as o:
-        for i in included_reads:
-            if (reads == 'data/short_reads.fastq.gz' or snakemake.config['short_reads_2'] == 'none') and snakemake.params.illumina:
-                o.write(i + '/1\n')
-                o.write(i + '/2\n')
-            else:
-                o.write(i + '\n')
-    logging.info("Retrieving reads...")
-    if not isinstance(reads, str):
-        for read in reads:
-            seqkit_command = f"seqkit -j {snakemake.threads} grep --pattern-file {out}/reads.{snakemake.params.prefix}.{rounds}.lst {read} | pigz -p {snakemake.threads} >> {out}/reads.{snakemake.params.prefix}.{rounds}.fastq.gz"
+                    o.write(i + '\n')
+        logging.info("Retrieving reads...")
+        if not isinstance(reads, str):
+            for read in reads:
+                seqkit_command = f"seqkit -j {snakemake.threads} grep --pattern-file {out}/reads.{snakemake.params.prefix}.{rounds}.lst {read} | pigz -p {snakemake.threads} >> {out}/reads.{snakemake.params.prefix}.{rounds}.fastq.gz"
+                print(seqkit_command)
+                subprocess.Popen(seqkit_command, shell=True).wait()
+        else:
+            seqkit_command = f"seqkit -j {snakemake.threads} grep --pattern-file {out}/reads.{snakemake.params.prefix}.{rounds}.lst {reads} | pigz -p {snakemake.threads} >> {out}/reads.{snakemake.params.prefix}.{rounds}.fastq.gz"
             print(seqkit_command)
             subprocess.Popen(seqkit_command, shell=True).wait()
-    else:
-        seqkit_command = f"seqkit -j {snakemake.threads} grep --pattern-file {out}/reads.{snakemake.params.prefix}.{rounds}.lst {reads} | pigz -p {snakemake.threads} >> {out}/reads.{snakemake.params.prefix}.{rounds}.fastq.gz"
-        print(seqkit_command)
-        subprocess.Popen(seqkit_command, shell=True).wait()
-
-    print("Performing round %d of racon polishing..." % rounds)
-    print("racon -m 8 -x -6 -g -8 -w 500 -t %d -u %s/reads.%s.%d.fastq.gz %s/filtered.%s.%d.paf %s/filtered.%s.%d.fa"
-                     " > %s/filtered.%s.%d.pol.fa" % (snakemake.threads, out, snakemake.params.prefix, rounds, out,
-                                                   snakemake.params.prefix, rounds, out, snakemake.params.prefix, rounds,
-                                                   out, snakemake.params.prefix, rounds))
-    subprocess.Popen("racon -m 8 -x -6 -g -8 -w 500 -t %d -u %s/reads.%s.%d.fastq.gz %s/filtered.%s.%d.paf %s/filtered.%s.%d.fa"
-                     " > %s/filtered.%s.%d.pol.fa" % (snakemake.threads, out, snakemake.params.prefix, rounds, out,
-                                                   snakemake.params.prefix, rounds, out, snakemake.params.prefix, rounds,
-                                                   out, snakemake.params.prefix, rounds), shell=True).wait()
-
-    with open(os.path.join(out, "combined.%s.%d.pol.fa" % (snakemake.params.prefix, rounds)), "w") as o:
-        with open(os.path.join(out, "filtered.%s.%d.pol.fa" % (snakemake.params.prefix, rounds))) as f:
-            gotten_set = set()
-            for line in f:
-                if line.startswith('>'):
-                    gotten_set.add(line.split()[0][1:])
-                o.write(line)
-        with open(reference) as f:
-            for line in f:
-                if line.startswith('>'):
-                    name = line.split()[0][1:]
-                    if name in gotten_set:
-                        get_line = False
-                    else:
-                        get_line = True
-                if get_line:
-                    o.write(line)
-    reference = os.path.join(out, "combined.%s.%d.pol.fa" % (snakemake.params.prefix, rounds))
 
+        print("Performing round %d of racon polishing..." % rounds)
+        print("racon -m 8 -x -6 -g -8 -w 500 -t %d -u %s/reads.%s.%d.fastq.gz %s/filtered.%s.%d.paf %s/filtered.%s.%d.fa"
+                        " > %s/filtered.%s.%d.pol.fa" % (snakemake.threads, out, snakemake.params.prefix, rounds, out,
+                                                    snakemake.params.prefix, rounds, out, snakemake.params.prefix, rounds,
+                                                    out, snakemake.params.prefix, rounds))
+        subprocess.Popen("racon -m 8 -x -6 -g -8 -w 500 -t %d -u %s/reads.%s.%d.fastq.gz %s/filtered.%s.%d.paf %s/filtered.%s.%d.fa"
+                        " > %s/filtered.%s.%d.pol.fa" % (snakemake.threads, out, snakemake.params.prefix, rounds, out,
+                                                    snakemake.params.prefix, rounds, out, snakemake.params.prefix, rounds,
+                                                    out, snakemake.params.prefix, rounds), shell=True).wait()
+
+        with open(os.path.join(out, "combined.%s.%d.pol.fa" % (snakemake.params.prefix, rounds)), "w") as o:
+            with open(os.path.join(out, "filtered.%s.%d.pol.fa" % (snakemake.params.prefix, rounds))) as f:
+                gotten_set = set()
+                for line in f:
+                    if line.startswith('>'):
+                        gotten_set.add(line.split()[0][1:])
+                    o.write(line)
+            with open(reference) as f:
+                for line in f:
+                    if line.startswith('>'):
+                        name = line.split()[0][1:]
+                        if name in gotten_set:
+                            get_line = False
+                        else:
+                            get_line = True
+                    if get_line:
+                        o.write(line)
+        reference = os.path.join(out, "combined.%s.%d.pol.fa" % (snakemake.params.prefix, rounds))
+else:
+    # polishing will be done by medaka
+    if snakemake.config["long_read_type"] not in ['ont', 'ont_hq']:
+        sys.exit("ERROR: long_read_type must be ont or ont_hq for medaka polishing")
+    
+    bam = os.path.join(out, 'alignment.%s.1.bam') % (snakemake.params.prefix)
+    print("Generating BAM file: %s for medaka..." % (bam))
+    # we just run medaka once: https://twitter.com/rrwick/status/1158278701819125760
+    # Twitter is a valid source of information :) do not question.
+    subprocess.Popen("minimap2 -t %d -x map-ont %s %s | samtools view -F 4 -b -@ %d %s" % 
+        (snakemake.threads, reference, reads, snakemake.threads - 1, bam), shell=True).wait()
+    
+    print("Running medaka...")
+    reference = os.path.join(out, "combined.%s.1.pol.fa" % (snakemake.params.prefix))
+    subprocess.Popen("medaka consensus -t %d -m %s %s %s" % (snakemake.threads, snakemake.config["medaka_model"], bam, reference), shell=True).wait()
 
 if os.path.exists("data/short_reads.racon.1.fastq.gz"):
     os.remove("data/short_reads.racon.1.fastq.gz")
     # os.remove("data/short_reads.racon.2.fastq.gz")
 shutil.copy2(reference, snakemake.output.fasta)
```

### Comparing `aviary-genome-0.5.7/aviary/modules/assembly/scripts/run_flye.py` & `aviary-genome-0.6.0/aviary/modules/assembly/scripts/run_flye.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     subprocess.Popen(
         "flye --nano-raw %s --meta -o data/flye -t %d" %
         (snakemake.input.fastq, snakemake.threads), shell=True).wait()
 elif snakemake.params.long_read_type == 'ont_hq':
     subprocess.Popen(
         "flye --nano-hq %s --meta -o data/flye -t %d" %
         (snakemake.input.fastq, snakemake.threads), shell=True).wait()
-elif snakemake.params.long_read_type == 'ccs':
+elif snakemake.params.long_read_type == 'ccs' or snakemake.params.long_read_type == 'hifi':
     subprocess.Popen(
         "flye --pacbio-hifi %s --meta -o data/flye -t %d" %
         (snakemake.input.fastq, snakemake.threads), shell=True).wait()
 else:
     subprocess.Popen(
         "flye --pacbio-raw %s --meta -o data/flye -t %d" %
         (snakemake.input.fastq, snakemake.threads), shell=True).wait()
```

### Comparing `aviary-genome-0.5.7/aviary/modules/benchmarking/benchmarking.smk` & `aviary-genome-0.6.0/aviary/modules/benchmarking/benchmarking.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/binning/binning.smk` & `aviary-genome-0.6.0/aviary/modules/binning/binning.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/binning/envs/rosella.yaml` & `aviary-genome-0.6.0/aviary/modules/binning/envs/rosella.yaml`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/binning/scripts/get_abundances.py` & `aviary-genome-0.6.0/aviary/modules/binning/scripts/get_abundances.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 if snakemake.config["long_reads"] != "none":
     if snakemake.config["long_read_type"][0] in ["ont", "ont_hq"]:
         subprocess.Popen("coverm genome -t %d -d bins/final_bins/ -m relative_abundance covered_fraction --single %s -p minimap2-ont --min-covered-fraction 0.0 -x fna %s > data/long_abundances.tsv" %
                          (snakemake.threads, " ".join(snakemake.config["long_reads"]),
                           '--bam-file-cache-directory data/reads_mapped_to_mags/long/ --discard-unmapped' if snakemake.config['strain_analysis'] is True else ''), shell=True).wait()
-    elif snakemake.config["long_read_type"][0] in ["rs", "sq", "ccs"]:
+    elif snakemake.config["long_read_type"][0] in ["rs", "sq", "ccs", "hifi"]:
         subprocess.Popen("coverm genome -t %d -d bins/final_bins/ -m relative_abundance covered_fraction --single %s -p minimap2-pb --min-covered-fraction 0.0 -x fna %s > data/long_abundances.tsv" %
                          (snakemake.threads, " ".join(snakemake.config["long_reads"]),
                           '--bam-file-cache-directory data/reads_mapped_to_mags/long/ --discard-unmapped' if snakemake.config['strain_analysis'] is True else ''), shell=True).wait()
     else:
         subprocess.Popen("coverm genome -t %d -d bins/final_bins/ -m relative_abundance covered_fraction --single %s -p minimap2-ont --min-covered-fraction 0.0 -x fna %s > data/long_abundances.tsv" %
                          (snakemake.threads, " ".join(snakemake.config["long_reads"]),
                           '--bam-file-cache-directory data/reads_mapped_to_mags/long/ --discard-unmapped' if snakemake.config['strain_analysis'] is True else ''), shell=True).wait()
```

### Comparing `aviary-genome-0.5.7/aviary/modules/binning/scripts/get_coverage.py` & `aviary-genome-0.6.0/aviary/modules/binning/scripts/get_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import subprocess
 import os
 
 if snakemake.config["long_reads"] != "none" and not os.path.exists("data/long_cov.tsv"):
     if snakemake.config["long_read_type"][0] in ["ont", "ont_hq"]:
         subprocess.Popen("TMPDIR=%s coverm contig -t %d -r %s --single %s -p minimap2-ont -m length trimmed_mean variance --bam-file-cache-directory data/binning_bams/ --discard-unmapped --min-read-percent-identity 0.85 > data/long_cov.tsv" %
                          (snakemake.params.tmpdir, snakemake.threads, snakemake.input.fasta, " ".join(snakemake.config["long_reads"])), shell=True).wait()
-    elif snakemake.config["long_read_type"][0] in ["rs", "sq", "ccs"]:
+    elif snakemake.config["long_read_type"][0] in ["rs", "sq", "ccs", "hifi"]:
         subprocess.Popen("TMPDIR=%s coverm contig -t %d -r %s --single %s -p minimap2-pb -m length trimmed_mean variance --bam-file-cache-directory data/binning_bams/ --discard-unmapped --min-read-percent-identity 0.9 > data/long_cov.tsv" %
                          (snakemake.params.tmpdir, snakemake.threads, snakemake.input.fasta, " ".join(snakemake.config["long_reads"])), shell=True).wait()
     else:
         subprocess.Popen(
             "TMPDIR=%s coverm contig -t %d -r %s --single %s -p minimap2-ont -m length trimmed_mean variance --bam-file-cache-directory data/binning_bams/ --discard-unmapped > data/long_cov.tsv" %
             (snakemake.params.tmpdir, snakemake.threads, snakemake.input.fasta, " ".join(snakemake.config["long_reads"])), shell=True).wait()
```

### Comparing `aviary-genome-0.5.7/aviary/modules/binning/scripts/make_long_cov.py` & `aviary-genome-0.6.0/aviary/modules/binning/scripts/make_long_cov.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/binning/scripts/rosella_refine.py` & `aviary-genome-0.6.0/aviary/modules/binning/scripts/rosella_refine.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/binning/scripts/write_vamb_bins.py` & `aviary-genome-0.6.0/aviary/modules/binning/scripts/write_vamb_bins.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/cluster/clustering.smk` & `aviary-genome-0.6.0/aviary/modules/cluster/clustering.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/processor.py` & `aviary-genome-0.6.0/aviary/modules/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,18 @@
             self.long_percent_identity = args.long_percent_identity
         except AttributeError:
             self.longreads = 'none'
             self.long_percent_identity = 'none'
 
         try:
             self.longread_type = args.longread_type
+            self.medaka_model = args.medaka_model
         except AttributeError:
             self.longread_type = 'none'
+            self.medaka_model = 'none'
 
         try:
             self.short_percent_identity = args.short_percent_identity
 
             if args.coupled != "none":
                 self.pe1 = args.coupled[::2]
                 self.pe2 = args.coupled[1::2]
@@ -311,14 +313,15 @@
         conf["max_threads"] = int(self.threads)
         conf["pplacer_threads"] = int(self.pplacer_threads)
         conf["max_memory"] = int(self.max_memory)
         conf["short_reads_1"] = self.pe1
         conf["short_reads_2"] = self.pe2
         conf["long_reads"] = self.longreads
         conf["long_read_type"] = self.longread_type
+        conf["medaka_model"] = self.medaka_model
         conf["kmer_sizes"] = self.kmer_sizes
         conf["use_megahit"] = self.use_megahit
         conf["coassemble"] = self.coassemble
         conf["min_cov_long"] = self.min_cov_long
         conf["min_cov_short"] = self.min_cov_short
         conf["exclude_contig_cov"] = self.exclude_contig_cov
         conf["exclude_contig_size"] = self.exclude_contig_size
```

### Comparing `aviary-genome-0.5.7/aviary/modules/quality_control/qc.smk` & `aviary-genome-0.6.0/aviary/modules/quality_control/qc.smk`

 * *Files 2% similar despite different names*

```diff
@@ -117,55 +117,55 @@
 #         '| pigz -p {threads} > {output.long}'
 
 
 rule fastqc:
     input:
         config['short_reads_1']
     output:
-        directory("www/fastqc/")
+        output = "www/fastqc/done"
     conda:
         "envs/fastqc.yaml"
     benchmark:
         "benchmarks/fastqc_short.benchmark.txt"
     group: 'qc'
     threads:
         config["max_threads"]
     script:
         "scripts/run_fastqc.py"
 
 rule fastqc_long:
     input:
         'data/long_reads.fastq.gz'
     output:
-        directory("www/fastqc_long/")
+        output = "www/fastqc_long/done"
     conda:
         "envs/fastqc.yaml"
     benchmark:
         "benchmarks/fastqc_long.benchmark.txt"
     group: 'qc'
     threads:
         config["max_threads"]
     shell:
-        "fastqc -o www/fastqc_long/ -t {threads} {input[0]}; touch www/fastqc_long/done"
+        "fastqc -o www/fastqc_long/ -t {threads} {input[0]}; touch {output.output}"
 
 rule nanoplot:
     input:
         long = config['long_reads']
          # "data/long_reads.fastq.gz"
     output:
-        directory("www/nanoplot/")
+        output = "www/nanoplot/done"
     conda:
         "envs/nanoplot.yaml"
     benchmark:
         "benchmarks/nanoplot.benchmark.txt"
     group: 'qc'
     threads:
         config["max_threads"]
     shell:
-        "NanoPlot -o www/nanoplot -p longReads -t {threads} --fastq {input.long}; touch www/nanoplot/done"
+        "NanoPlot -o www/nanoplot -p longReads -t {threads} --fastq {input.long}; touch {output.output}"
 
 rule metaquast:
     """
     MetaQuast on input assembly (one or more). Compare against GSA if one is provided
     """
     input:
         assembly = config['fasta']
```

### Comparing `aviary-genome-0.5.7/aviary/modules/quality_control/scripts/fraction_recovered.py` & `aviary-genome-0.6.0/aviary/modules/quality_control/scripts/fraction_recovered.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 os.makedirs('www/fraction_recovered', exist_ok=True)
 
 if snakemake.config["long_reads"] != "none" and not os.path.exists("data/long_cov.tsv"):
     if snakemake.config["long_read_type"][0] in ["ont", "ont_hq"]:
         subprocess.Popen("coverm genome -t %d -r %s --single %s -p minimap2-ont --min-read-percent-identity 0.85 > www/fraction_recovered/long_fraction_recovered.tsv" %
                          (snakemake.threads, snakemake.input.fasta, " ".join(snakemake.config["long_reads"])), shell=True).wait()
-    elif snakemake.config["long_read_type"][0] in ["rs", "sq", "ccs"]:
+    elif snakemake.config["long_read_type"][0] in ["rs", "sq", "ccs", "hifi"]:
         subprocess.Popen("coverm genome -t %d -r %s --single %s -p minimap2-pb --min-read-percent-identity 0.85 > www/fraction_recovered/long_fraction_recovered.tsv" %
                          (snakemake.threads, snakemake.input.fasta, " ".join(snakemake.config["long_reads"])), shell=True).wait()
     else:
         subprocess.Popen(
             "coverm genome -t %d -r %s --single %s -p minimap2-ont > www/fraction_recovered/long_fraction_recovered.tsv" %
             (snakemake.threads, snakemake.input.fasta, " ".join(snakemake.config["long_reads"])), shell=True).wait()
```

### Comparing `aviary-genome-0.5.7/aviary/modules/quality_control/scripts/run_fastqc.py` & `aviary-genome-0.6.0/aviary/modules/quality_control/scripts/run_fastqc.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/strain_analysis/scripts/run_lorikeet.py` & `aviary-genome-0.6.0/aviary/modules/strain_analysis/scripts/run_lorikeet.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/strain_analysis/strain_analysis.smk` & `aviary-genome-0.6.0/aviary/modules/strain_analysis/strain_analysis.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/modules/template_config.yaml` & `aviary-genome-0.6.0/aviary/modules/template_config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 fasta:
     none
 long_reads:
     none
 long_read_type:
     ont
+medaka_model:
+    r941_min_hac_g507
 short_reads_1:
     none
 short_reads_2:
     none
 min_contig_size:
     1500
 min_bin_size:
```

### Comparing `aviary-genome-0.5.7/aviary/modules/viral_analysis/viral_analysis.smk` & `aviary-genome-0.6.0/aviary/modules/viral_analysis/viral_analysis.smk`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/scripts/create_aviary_webpage.py` & `aviary-genome-0.6.0/aviary/scripts/create_aviary_webpage.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/scripts/process_batch.py` & `aviary-genome-0.6.0/aviary/scripts/process_batch.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/scripts/process_viral_batch.py` & `aviary-genome-0.6.0/aviary/scripts/process_viral_batch.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary/scripts/singlem_reads.py` & `aviary-genome-0.6.0/aviary/scripts/singlem_reads.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/aviary_genome.egg-info/PKG-INFO` & `aviary-genome-0.6.0/aviary_genome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviary-genome
-Version: 0.5.7
+Version: 0.6.0
 Summary: aviary - metagenomics pipeline using long and short reads
 Home-page: https://github.com/rhysnewell/aviary
 Author: Rhys Newell
 Author-email: rhys.newell94@gmail.com
 License: GPL-3.0
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `aviary-genome-0.5.7/aviary_genome.egg-info/SOURCES.txt` & `aviary-genome-0.6.0/aviary_genome.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,29 +32,29 @@
 aviary/modules/assembly/envs/circlator.yaml
 aviary/modules/assembly/envs/final_assembly.yaml
 aviary/modules/assembly/envs/flye.yaml
 aviary/modules/assembly/envs/medaka.yaml
 aviary/modules/assembly/envs/megahit.yml
 aviary/modules/assembly/envs/mfqe.yaml
 aviary/modules/assembly/envs/pilon.yaml
+aviary/modules/assembly/envs/polishing.yaml
 aviary/modules/assembly/envs/pysam.yaml
-aviary/modules/assembly/envs/racon.yaml
 aviary/modules/assembly/envs/seqtk.yaml
 aviary/modules/assembly/envs/spades.yaml
 aviary/modules/assembly/scripts/__init__.py
 aviary/modules/assembly/scripts/assemble_pools.py
 aviary/modules/assembly/scripts/assemble_short_reads.py
 aviary/modules/assembly/scripts/combine_assemblies.py
 aviary/modules/assembly/scripts/filter_illumina_assembly.py
 aviary/modules/assembly/scripts/filter_illumina_reference.py
 aviary/modules/assembly/scripts/filter_read_list.py
 aviary/modules/assembly/scripts/generate_pilon_sort.py
 aviary/modules/assembly/scripts/get_binned_reads.py
+aviary/modules/assembly/scripts/polish.py
 aviary/modules/assembly/scripts/pool_reads.py
-aviary/modules/assembly/scripts/racon_polish.py
 aviary/modules/assembly/scripts/run_flye.py
 aviary/modules/benchmarking/__init__.py
 aviary/modules/benchmarking/benchmarking.smk
 aviary/modules/benchmarking/envs/__init__.py
 aviary/modules/benchmarking/envs/magpurify.yaml
 aviary/modules/benchmarking/scripts/__init__.py
 aviary/modules/binning/__init__.py
```

### Comparing `aviary-genome-0.5.7/setup.py` & `aviary-genome-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `aviary-genome-0.5.7/test/test_integration.py` & `aviary-genome-0.6.0/test/test_integration.py`

 * *Files identical despite different names*

