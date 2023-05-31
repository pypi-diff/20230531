# Comparing `tmp/gencove-2.4.6.tar.gz` & `tmp/gencove-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gencove-2.4.6.tar", last modified: Thu Mar 30 21:33:52 2023, max compression
+gzip compressed data, was "dist/gencove-2.4.7.tar", last modified: Wed May 31 20:26:00 2023, max compression
```

## Comparing `gencove-2.4.6.tar` & `gencove-2.4.7.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-03-30 21:33:52.000000 gencove-2.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-03-30 21:33:05.000000 gencove-2.4.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    32228 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6009 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2536 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/autoimports/create/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/biosamples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/biosamples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/biosamples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/projects/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1959 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/basespace_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/basespace/projects/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/common_cli_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/download/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/download/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/download/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/download/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14731 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/download/main.py
--rw-rw-rw-   0 root         (0) root         (0)    10579 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/download/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/files/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/files/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/files/main.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/files/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/create_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/create_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1740 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/create_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/delete_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/delete_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/delete_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/delete_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/get_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/get_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/get_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/get_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/get_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/get_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/get_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/get_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/import_existing_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/import_existing_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/import_existing_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/import_existing_samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2474 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/import_existing_samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/import_existing_samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2859 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/list_batch_types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batch_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batch_types/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batch_types/main.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batch_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/list_batches/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batches/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2504 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batches/main.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_batches/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/list_pipeline_capabilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipeline_capabilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipeline_capabilities/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipeline_capabilities/main.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipeline_capabilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/list_pipelines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipelines/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipelines/main.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/list_pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/restore_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/restore_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/restore_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/restore_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/run_prefix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/run_prefix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/run_prefix/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/run_prefix/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5056 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/run_prefix/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2389 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/projects/status_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/status_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/status_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/status_merged_vcf/main.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/projects/status_merged_vcf/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/autoimports/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/s3_imports/s3_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/s3_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/s3_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/s3_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/s3_imports/s3_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/samples/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/samples/download_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/download_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/download_file/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/download_file/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4930 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/download_file/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/download_file/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/samples/get_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/get_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/get_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/get_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/samples/set_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/set_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/set_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/samples/set_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/upload/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/upload/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/upload/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/upload/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    16178 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/upload/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/upload/multi_file_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     7601 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/upload/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/uploads/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/uploads/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/uploads/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/uploads/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/uploads/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/uploads/list/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/uploads/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/uploads/list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/webhook/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/webhook/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/command/webhook/verify/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/webhook/verify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/webhook/verify/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/command/webhook/verify/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3691 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/description/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/description/pypi_readme.md
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3205 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7755 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/basespace/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/basespace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/basespace/test_basespace_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/basespace/test_basespace_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7257 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/basespace/test_basespace_biosamples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6335 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/basespace/test_basespace_projects_import.py
--rw-rw-rw-   0 root         (0) root         (0)     5955 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/basespace/test_basespace_projects_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/basespace/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/basespace/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3328 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/download/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36754 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/download/test_cli_download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/download/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/download/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/download/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4371 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/files/test_file_types_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/files/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/files/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4519 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/projects/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_batch_get.py
--rw-rw-rw-   0 root         (0) root         (0)     4502 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_batch_types_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8993 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_batches_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4601 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_batches_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4380 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9109 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_create_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     8901 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_delete_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    12017 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_get_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     6387 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_import_existing_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    10605 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6511 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_pipelines_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7328 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_restore_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    13391 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_run_prefix.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_samples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6469 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/test_projects_status_merged_vcf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/projects/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11910 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/projects/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/s3_imports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6470 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/s3_imports/test_s3_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4163 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/s3_imports/test_s3_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     5270 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/s3_imports/test_s3_uri_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/s3_imports/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/s3_imports/vcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8865 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/samples/test_samples_download_file.py
--rw-rw-rw-   0 root         (0) root         (0)     7024 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/samples/test_samples_get_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/samples/test_samples_set_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/samples/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/samples/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/samples/vcr/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/test_logger.py
--rw-rw-rw-   0 root         (0) root         (0)    17615 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35553 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/upload/test_cli_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/upload/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/upload/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4000 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/upload/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/uploads/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4357 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/uploads/test_uploads_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/uploads/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/uploads/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/tests/webhook/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/tests/webhook/test_webhook_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     5174 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove/version/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/version/A-major
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/version/B-minor
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/version/C-patch
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-03-30 21:33:05.000000 gencove-2.4.6/gencove/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 21:33:52.000000 gencove-2.4.6/gencove.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-03-30 21:33:51.000000 gencove-2.4.6/gencove.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10251 2023-03-30 21:33:51.000000 gencove-2.4.6/gencove.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 21:33:51.000000 gencove-2.4.6/gencove.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-30 21:33:51.000000 gencove-2.4.6/gencove.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-03-30 21:33:51.000000 gencove-2.4.6/gencove.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-30 21:33:51.000000 gencove-2.4.6/gencove.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-30 21:33:52.000000 gencove-2.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-03-30 21:33:05.000000 gencove-2.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-05-31 20:26:00.000000 gencove-2.4.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-05-31 20:25:28.000000 gencove-2.4.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    32228 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6009 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/autoimports/create/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/biosamples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/biosamples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/basespace_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/basespace/projects/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/common_cli_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/download/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14731 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    10579 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/download/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/files/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/files/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/create_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/create_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/delete_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/delete_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/delete_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/delete_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/get_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/get_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/import_existing_samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batch_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_batches/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_batches/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/list_pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/restore_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/restore_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/restore_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/restore_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/run_prefix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5056 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/run_prefix/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2454 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/projects/status_merged_vcf/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/autoimports/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/s3_imports/s3_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/download_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4930 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/download_file/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/get_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/get_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/get_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/get_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/samples/set_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/set_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/set_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/samples/set_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/upload/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    16178 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/multi_file_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7601 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/upload/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/uploads/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/uploads/list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/command/webhook/verify/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/verify/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/verify/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/command/webhook/verify/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3691 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/description/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/description/pypi_readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7778 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_biosamples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6335 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     5955 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/basespace/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/basespace/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/download/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36754 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/test_cli_download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/download/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/download/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/files/test_file_types_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/files/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/files/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/projects/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batch_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     4502 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batch_types_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8993 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batches_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_batches_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9109 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_create_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     8901 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_delete_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    12017 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_get_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6387 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_import_existing_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    10605 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6511 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_pipelines_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7328 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_restore_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    13391 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_run_prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_samples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6469 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/test_projects_status_merged_vcf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/projects/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11910 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/projects/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6470 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4163 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     5270 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/test_s3_uri_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/s3_imports/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/s3_imports/vcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8865 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/test_samples_download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     7024 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/test_samples_get_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/test_samples_set_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/samples/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/samples/vcr/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/test_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    17615 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35553 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/test_cli_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/upload/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4000 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/upload/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4357 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/uploads/test_uploads_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/uploads/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/uploads/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/tests/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/tests/webhook/test_webhook_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     5174 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove/version/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version/A-major
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version/B-minor
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version/C-patch
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-05-31 20:25:28.000000 gencove-2.4.7/gencove/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10251 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-31 20:26:00.000000 gencove-2.4.7/gencove.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-31 20:26:00.000000 gencove-2.4.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-05-31 20:25:28.000000 gencove-2.4.7/setup.py
```

### Comparing `gencove-2.4.6/PKG-INFO` & `gencove-2.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.4.6
+Version: 2.4.7
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.4.6/README.md` & `gencove-2.4.7/README.md`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/cli.py` & `gencove-2.4.7/gencove/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/client.py` & `gencove-2.4.7/gencove/client.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/base.py` & `gencove-2.4.7/gencove/command/base.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/cli.py` & `gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/main.py` & `gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/autoimports/autoimport_list/utils.py` & `gencove-2.4.7/gencove/command/basespace/autoimports/autoimport_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/autoimports/create/cli.py` & `gencove-2.4.7/gencove/command/basespace/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/autoimports/create/main.py` & `gencove-2.4.7/gencove/command/basespace/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/cli.py` & `gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/main.py` & `gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/biosamples/biosamples_list/utils.py` & `gencove-2.4.7/gencove/command/basespace/biosamples/biosamples_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/projects/basespace_import/cli.py` & `gencove-2.4.7/gencove/command/basespace/projects/basespace_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/projects/basespace_import/main.py` & `gencove-2.4.7/gencove/command/basespace/projects/basespace_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/projects/basespace_list/cli.py` & `gencove-2.4.7/gencove/command/basespace/projects/basespace_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/projects/basespace_list/main.py` & `gencove-2.4.7/gencove/command/basespace/projects/basespace_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/basespace/projects/basespace_list/utils.py` & `gencove-2.4.7/gencove/command/basespace/projects/basespace_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/common_cli_options.py` & `gencove-2.4.7/gencove/command/common_cli_options.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/download/cli.py` & `gencove-2.4.7/gencove/command/download/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/download/constants.py` & `gencove-2.4.7/gencove/command/download/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/download/main.py` & `gencove-2.4.7/gencove/command/download/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/download/utils.py` & `gencove-2.4.7/gencove/command/download/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/files/cli.py` & `gencove-2.4.7/gencove/command/files/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/files/main.py` & `gencove-2.4.7/gencove/command/files/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/cli.py` & `gencove-2.4.7/gencove/command/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/create/cli.py` & `gencove-2.4.7/gencove/command/projects/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/create/main.py` & `gencove-2.4.7/gencove/command/projects/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/create_batch/cli.py` & `gencove-2.4.7/gencove/command/projects/create_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/create_batch/main.py` & `gencove-2.4.7/gencove/command/projects/create_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/create_merged_vcf/cli.py` & `gencove-2.4.7/gencove/command/projects/create_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/create_merged_vcf/main.py` & `gencove-2.4.7/gencove/command/projects/create_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/delete_samples/cli.py` & `gencove-2.4.7/gencove/command/projects/delete_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/delete_samples/main.py` & `gencove-2.4.7/gencove/command/projects/delete_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/get_batch/cli.py` & `gencove-2.4.7/gencove/command/projects/get_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/get_batch/main.py` & `gencove-2.4.7/gencove/command/projects/get_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/get_merged_vcf/cli.py` & `gencove-2.4.7/gencove/command/projects/get_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/get_merged_vcf/main.py` & `gencove-2.4.7/gencove/command/projects/get_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/import_existing_samples/cli.py` & `gencove-2.4.7/gencove/command/projects/import_existing_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/import_existing_samples/main.py` & `gencove-2.4.7/gencove/command/projects/import_existing_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list/main.py` & `gencove-2.4.7/gencove/command/projects/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list/utils.py` & `gencove-2.4.7/gencove/command/projects/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_batch_types/cli.py` & `gencove-2.4.7/gencove/command/projects/list_batch_types/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_batch_types/main.py` & `gencove-2.4.7/gencove/command/projects/list_batch_types/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_batches/cli.py` & `gencove-2.4.7/gencove/command/projects/list_batches/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_batches/main.py` & `gencove-2.4.7/gencove/command/projects/list_batches/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_pipeline_capabilities/cli.py` & `gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_pipeline_capabilities/main.py` & `gencove-2.4.7/gencove/command/projects/list_pipeline_capabilities/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_pipelines/cli.py` & `gencove-2.4.7/gencove/command/projects/list_pipelines/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/list_pipelines/main.py` & `gencove-2.4.7/gencove/command/projects/list_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/restore_samples/cli.py` & `gencove-2.4.7/gencove/command/projects/restore_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/restore_samples/main.py` & `gencove-2.4.7/gencove/command/projects/restore_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/run_prefix/cli.py` & `gencove-2.4.7/gencove/command/projects/run_prefix/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/run_prefix/main.py` & `gencove-2.4.7/gencove/command/projects/run_prefix/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/samples/cli.py` & `gencove-2.4.7/gencove/command/projects/samples/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,22 +25,36 @@
 )
 @click.option(
     "--archive-status",
     help="Get samples with specific archive status",
     type=click.Choice(enum_as_dict(SampleArchiveStatus).values()),
     default=SampleArchiveStatus.ALL.value,
 )
+@click.option(
+    "--include-run/--no-include-run",
+    help="Include run id",
+    default=False,
+)
 @add_options(common_options)
 def list_project_samples(  # pylint: disable=E0012,C0330,R0913
-    project_id, search, status, archive_status, host, email, password, api_key
+    project_id,
+    search,
+    status,
+    archive_status,
+    include_run,
+    host,
+    email,
+    password,
+    api_key,
 ):
     """List samples in a project."""
     ListSamples(
         project_id,
         Credentials(email=email, password=password, api_key=api_key),
         SamplesOptions(
             host=host,
             status=status,
             archive_status=archive_status,
             search=search,
+            include_run=include_run,
         ),
     ).run()
```

### Comparing `gencove-2.4.6/gencove/command/projects/samples/main.py` & `gencove-2.4.7/gencove/command/projects/samples/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     def __init__(self, project_id, credentials, options):
         super().__init__(credentials, options)
         self.project_id = project_id
         self.sample_status = options.status
         self.sample_archive_status = options.archive_status
         self.search_term = options.search
+        self.include_run = options.include_run
 
     def initialize(self):
         """Initialize list subcommand."""
         self.login()
 
     def validate(self):
         """Validate command input."""
@@ -35,15 +36,15 @@
         try:
             for samples in self.get_paginated_samples():
                 if not samples:
                     self.echo_debug("No matching samples were found.")
                     return
 
                 for sample in samples:
-                    self.echo_data(get_line(sample))
+                    self.echo_data(get_line(sample, self.include_run))
         except APIClientError as err:
             if err.status_code == 404:
                 self.echo_error(f"Project {self.project_id} does not exist.")
             raise
 
     def get_paginated_samples(self):
         """Paginate over all sample sheets for the destination.
```

### Comparing `gencove-2.4.6/gencove/command/projects/status_merged_vcf/cli.py` & `gencove-2.4.7/gencove/command/projects/status_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/projects/status_merged_vcf/main.py` & `gencove-2.4.7/gencove/command/projects/status_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/s3_imports/autoimports/autoimport_list/cli.py` & `gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/s3_imports/autoimports/autoimport_list/main.py` & `gencove-2.4.7/gencove/command/s3_imports/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/s3_imports/autoimports/create/cli.py` & `gencove-2.4.7/gencove/command/s3_imports/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/s3_imports/autoimports/create/main.py` & `gencove-2.4.7/gencove/command/s3_imports/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/s3_imports/s3_import/cli.py` & `gencove-2.4.7/gencove/command/s3_imports/s3_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/s3_imports/s3_import/main.py` & `gencove-2.4.7/gencove/command/s3_imports/s3_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/samples/download_file/cli.py` & `gencove-2.4.7/gencove/command/samples/download_file/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/samples/download_file/main.py` & `gencove-2.4.7/gencove/command/samples/download_file/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/samples/download_file/utils.py` & `gencove-2.4.7/gencove/command/samples/download_file/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/samples/get_metadata/cli.py` & `gencove-2.4.7/gencove/command/samples/get_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/samples/get_metadata/main.py` & `gencove-2.4.7/gencove/command/samples/get_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/samples/set_metadata/cli.py` & `gencove-2.4.7/gencove/command/samples/set_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/samples/set_metadata/main.py` & `gencove-2.4.7/gencove/command/samples/set_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/upload/cli.py` & `gencove-2.4.7/gencove/command/upload/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/upload/constants.py` & `gencove-2.4.7/gencove/command/upload/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/upload/main.py` & `gencove-2.4.7/gencove/command/upload/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/upload/multi_file_reader.py` & `gencove-2.4.7/gencove/command/upload/multi_file_reader.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/upload/utils.py` & `gencove-2.4.7/gencove/command/upload/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/uploads/list/cli.py` & `gencove-2.4.7/gencove/command/uploads/list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/uploads/list/main.py` & `gencove-2.4.7/gencove/command/uploads/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/uploads/list/utils.py` & `gencove-2.4.7/gencove/command/uploads/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/utils.py` & `gencove-2.4.7/gencove/command/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/webhook/verify/cli.py` & `gencove-2.4.7/gencove/command/webhook/verify/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/command/webhook/verify/utils.py` & `gencove-2.4.7/gencove/command/webhook/verify/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/constants.py` & `gencove-2.4.7/gencove/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/description/pypi_readme.md` & `gencove-2.4.7/gencove/description/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/logger.py` & `gencove-2.4.7/gencove/logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/models.py` & `gencove-2.4.7/gencove/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 
 
 class SampleDetails(GencoveBaseModel):
     """SampleDetails model"""
 
     created: Optional[datetime]
     modified: Optional[datetime]
+    run: Optional[str]
     client_id: Optional[str]
     physical_id: Optional[str]
     legacy_id: Optional[str]
     last_status: Optional[GencoveStatus]
     archive_last_status: Optional[GencoveStatus]
     files: Optional[List[SampleFile]]
```

### Comparing `gencove-2.4.6/gencove/tests/basespace/test_basespace_autoimports_create.py` & `gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/basespace/test_basespace_autoimports_list.py` & `gencove-2.4.7/gencove/tests/basespace/test_basespace_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/basespace/test_basespace_biosamples_list.py` & `gencove-2.4.7/gencove/tests/basespace/test_basespace_biosamples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/basespace/test_basespace_projects_import.py` & `gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/basespace/test_basespace_projects_list.py` & `gencove-2.4.7/gencove/tests/basespace/test_basespace_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/conftest.py` & `gencove-2.4.7/gencove/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/decorators.py` & `gencove-2.4.7/gencove/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/download/test_cli_download.py` & `gencove-2.4.7/gencove/tests/download/test_cli_download.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/download/vcr/filters.py` & `gencove-2.4.7/gencove/tests/download/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/files/test_file_types_list.py` & `gencove-2.4.7/gencove/tests/files/test_file_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/filters.py` & `gencove-2.4.7/gencove/tests/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_batch_get.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_batch_get.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_batch_types_list.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_batch_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_batches_create.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_batches_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_batches_list.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_batches_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_create.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_create_merged_vcf.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_create_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_delete_samples.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_delete_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_get_merged_vcf.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_get_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_import_existing_samples.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_import_existing_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_list.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_pipeline_capabilities_list.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_pipeline_capabilities_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_pipelines_list.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_pipelines_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_restore_samples.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_restore_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_run_prefix.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_run_prefix.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_samples_list.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_samples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/test_projects_status_merged_vcf.py` & `gencove-2.4.7/gencove/tests/projects/test_projects_status_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/projects/vcr/filters.py` & `gencove-2.4.7/gencove/tests/projects/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/s3_imports/test_s3_autoimports_create.py` & `gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/s3_imports/test_s3_autoimports_list.py` & `gencove-2.4.7/gencove/tests/s3_imports/test_s3_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/s3_imports/test_s3_uri_import.py` & `gencove-2.4.7/gencove/tests/s3_imports/test_s3_uri_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/samples/test_samples_download_file.py` & `gencove-2.4.7/gencove/tests/samples/test_samples_download_file.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/samples/test_samples_get_metadata.py` & `gencove-2.4.7/gencove/tests/samples/test_samples_get_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/samples/test_samples_set_metadata.py` & `gencove-2.4.7/gencove/tests/samples/test_samples_set_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/samples/vcr/filters.py` & `gencove-2.4.7/gencove/tests/samples/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/test_logger.py` & `gencove-2.4.7/gencove/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/test_utils.py` & `gencove-2.4.7/gencove/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/upload/test_cli_upload.py` & `gencove-2.4.7/gencove/tests/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/upload/vcr/filters.py` & `gencove-2.4.7/gencove/tests/upload/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/uploads/test_uploads_list.py` & `gencove-2.4.7/gencove/tests/uploads/test_uploads_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/utils.py` & `gencove-2.4.7/gencove/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/tests/webhook/test_webhook_verify.py` & `gencove-2.4.7/gencove/tests/webhook/test_webhook_verify.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove/utils.py` & `gencove-2.4.7/gencove/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/gencove.egg-info/PKG-INFO` & `gencove-2.4.7/gencove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.4.6
+Version: 2.4.7
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.4.6/gencove.egg-info/SOURCES.txt` & `gencove-2.4.7/gencove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gencove-2.4.6/setup.py` & `gencove-2.4.7/setup.py`

 * *Files identical despite different names*

