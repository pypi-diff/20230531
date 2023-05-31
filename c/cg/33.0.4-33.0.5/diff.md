# Comparing `tmp/cg-33.0.4.tar.gz` & `tmp/cg-33.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-33.0.4.tar", last modified: Tue May 30 13:47:44 2023, max compression
+gzip compressed data, was "dist/cg-33.0.5.tar", last modified: Wed May 31 09:00:13 2023, max compression
```

## Comparing `cg-33.0.4.tar` & `cg-33.0.5.tar`

### file list

```diff
@@ -1,1266 +1,1270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 13:47:33.000000 cg-33.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-30 13:47:44.000000 cg-33.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-30 13:47:33.000000 cg-33.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 13:47:33.000000 cg-33.0.4/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/dragen_demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/db/models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sample_sheet/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/lims/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-30 13:47:33.000000 cg-33.0.4/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/demultiplex/sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/set/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/taxprofiler/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-30 13:47:33.000000 cg-33.0.4/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 13:47:33.000000 cg-33.0.4/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-30 13:47:33.000000 cg-33.0.4/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-30 13:47:33.000000 cg-33.0.4/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-30 13:47:33.000000 cg-33.0.4/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/taxprofiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 13:47:33.000000 cg-33.0.4/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-30 13:47:33.000000 cg-33.0.4/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-30 13:47:33.000000 cg-33.0.4/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-30 13:47:33.000000 cg-33.0.4/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 13:47:33.000000 cg-33.0.4/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38700 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-05-30 13:47:33.000000 cg-33.0.4/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 13:47:33.000000 cg-33.0.4/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-30 13:47:43.000000 cg-33.0.4/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40457 2023-05-30 13:47:43.000000 cg-33.0.4/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:47:43.000000 cg-33.0.4/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 13:47:43.000000 cg-33.0.4/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:47:43.000000 cg-33.0.4/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-30 13:47:43.000000 cg-33.0.4/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-30 13:47:43.000000 cg-33.0.4/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 13:47:33.000000 cg-33.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-30 13:47:33.000000 cg-33.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:47:44.000000 cg-33.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-30 13:47:33.000000 cg-33.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/demultiplex/test_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/lims/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/lims/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-30 13:47:33.000000 cg-33.0.4/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/test_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-30 13:47:33.000000 cg-33.0.4/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    63110 2023-05-30 13:47:33.000000 cg-33.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/io/example_json.json
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/io/example_xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-30 13:47:33.000000 cg-33.0.4/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-30 13:47:33.000000 cg-33.0.4/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-30 13:47:33.000000 cg-33.0.4/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-30 13:47:33.000000 cg-33.0.4/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-30 13:47:33.000000 cg-33.0.4/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-30 13:47:33.000000 cg-33.0.4/tests/io/test_io_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-30 13:47:33.000000 cg-33.0.4/tests/io/test_io_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-30 13:47:33.000000 cg-33.0.4/tests/io/test_validate_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/gisaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-30 13:47:33.000000 cg-33.0.4/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-30 13:47:33.000000 cg-33.0.4/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-30 13:47:33.000000 cg-33.0.4/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 13:47:33.000000 cg-33.0.4/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-30 13:47:33.000000 cg-33.0.4/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 13:47:33.000000 cg-33.0.4/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 13:47:33.000000 cg-33.0.4/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    38171 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-05-30 13:47:33.000000 cg-33.0.4/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-30 13:47:33.000000 cg-33.0.4/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:44.000000 cg-33.0.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:33.000000 cg-33.0.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-30 13:47:33.000000 cg-33.0.4/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-30 13:47:33.000000 cg-33.0.4/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-30 13:47:33.000000 cg-33.0.4/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-30 13:47:33.000000 cg-33.0.4/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-30 13:47:33.000000 cg-33.0.4/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-30 13:47:33.000000 cg-33.0.4/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-31 09:00:03.000000 cg-33.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-31 09:00:13.000000 cg-33.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-31 09:00:03.000000 cg-33.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 09:00:03.000000 cg-33.0.5/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/dragen_demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/db/models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sample_sheet/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-31 09:00:03.000000 cg-33.0.5/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/demultiplex/sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/set/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/taxprofiler/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 09:00:03.000000 cg-33.0.5/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 09:00:03.000000 cg-33.0.5/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-31 09:00:03.000000 cg-33.0.5/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-31 09:00:03.000000 cg-33.0.5/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-31 09:00:03.000000 cg-33.0.5/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/rnafusion/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/rnafusion/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/taxprofiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-31 09:00:03.000000 cg-33.0.5/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-31 09:00:03.000000 cg-33.0.5/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 09:00:03.000000 cg-33.0.5/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-31 09:00:03.000000 cg-33.0.5/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-31 09:00:03.000000 cg-33.0.5/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38700 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-05-31 09:00:03.000000 cg-33.0.5/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-31 09:00:03.000000 cg-33.0.5/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40585 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-31 09:00:13.000000 cg-33.0.5/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 09:00:03.000000 cg-33.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-31 09:00:03.000000 cg-33.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:00:13.000000 cg-33.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 09:00:03.000000 cg-33.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/demultiplex/test_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/lims/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/lims/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-31 09:00:03.000000 cg-33.0.5/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/test_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-31 09:00:03.000000 cg-33.0.5/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-05-31 09:00:03.000000 cg-33.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/io/example_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/io/example_xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-31 09:00:03.000000 cg-33.0.5/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-31 09:00:03.000000 cg-33.0.5/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-31 09:00:03.000000 cg-33.0.5/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-31 09:00:03.000000 cg-33.0.5/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-31 09:00:03.000000 cg-33.0.5/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-31 09:00:03.000000 cg-33.0.5/tests/io/test_io_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-31 09:00:03.000000 cg-33.0.5/tests/io/test_io_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-31 09:00:03.000000 cg-33.0.5/tests/io/test_validate_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/test_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/report/test_rnafusion_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/gisaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-31 09:00:03.000000 cg-33.0.5/tests/meta/workflow/test_rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-31 09:00:03.000000 cg-33.0.5/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-31 09:00:03.000000 cg-33.0.5/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-31 09:00:03.000000 cg-33.0.5/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-31 09:00:03.000000 cg-33.0.5/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 09:00:03.000000 cg-33.0.5/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-31 09:00:03.000000 cg-33.0.5/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38171 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-05-31 09:00:03.000000 cg-33.0.5/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-31 09:00:03.000000 cg-33.0.5/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:13.000000 cg-33.0.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:03.000000 cg-33.0.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 09:00:03.000000 cg-33.0.5/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-31 09:00:03.000000 cg-33.0.5/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-31 09:00:03.000000 cg-33.0.5/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-31 09:00:03.000000 cg-33.0.5/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-31 09:00:03.000000 cg-33.0.5/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-31 09:00:03.000000 cg-33.0.5/tests/utils/test_utils.py
```

### Comparing `cg-33.0.4/PKG-INFO` & `cg-33.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 33.0.4
+Version: 33.0.5
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-33.0.4/README.md` & `cg-33.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/crud/create.py` & `cg-33.0.5/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/crud/delete.py` & `cg-33.0.5/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/crud/find.py` & `cg-33.0.5/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/base.py` & `cg-33.0.5/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/datasource.py` & `cg-33.0.5/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/demux.py` & `cg-33.0.5/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/demux_sample.py` & `cg-33.0.5/cg/apps/cgstats/db/models/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/dragen_demux_sample.py` & `cg-33.0.5/cg/apps/cgstats/db/models/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/sample.py` & `cg-33.0.5/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/support_params.py` & `cg-33.0.5/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/unaligned.py` & `cg-33.0.5/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/db/models/version.py` & `cg-33.0.5/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-33.0.5/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-33.0.5/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/parsers/demux_stats.py` & `cg-33.0.5/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-33.0.5/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-33.0.5/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/parsers/run_info.py` & `cg-33.0.5/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/cgstats/stats.py` & `cg-33.0.5/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/coverage/api.py` & `cg-33.0.5/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/crunchy/crunchy.py` & `cg-33.0.5/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/crunchy/files.py` & `cg-33.0.5/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/crunchy/sbatch.py` & `cg-33.0.5/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/demultiplex_api.py` & `cg-33.0.5/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/demux_report.py` & `cg-33.0.5/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/sample_sheet/create.py` & `cg-33.0.5/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-33.0.5/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/sample_sheet/index.py` & `cg-33.0.5/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/sample_sheet/models.py` & `cg-33.0.5/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-33.0.5/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/sample_sheet/validate.py` & `cg-33.0.5/cg/apps/demultiplex/sample_sheet/validate.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/demultiplex/sbatch.py` & `cg-33.0.5/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/gens.py` & `cg-33.0.5/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/gt.py` & `cg-33.0.5/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/hermes/hermes_api.py` & `cg-33.0.5/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/hermes/models.py` & `cg-33.0.5/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/housekeeper/hk.py` & `cg-33.0.5/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/invoice/render.py` & `cg-33.0.5/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-33.0.5/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-33.0.5/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-33.0.5/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-33.0.5/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/lims/api.py` & `cg-33.0.5/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/lims/batch.py` & `cg-33.0.5/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/lims/order.py` & `cg-33.0.5/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/lims/sample_sheet.py` & `cg-33.0.5/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/loqus.py` & `cg-33.0.5/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/madeline/api.py` & `cg-33.0.5/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/mip/confighandler.py` & `cg-33.0.5/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/mutacc_auto.py` & `cg-33.0.5/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/orderform/excel_orderform_parser.py` & `cg-33.0.5/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/orderform/json_orderform_parser.py` & `cg-33.0.5/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/orderform/orderform_parser.py` & `cg-33.0.5/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/osticket.py` & `cg-33.0.5/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/scout/scout_export.py` & `cg-33.0.5/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/scout/scoutapi.py` & `cg-33.0.5/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-33.0.5/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-33.0.5/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py` & `cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-33.0.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-33.0.5/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/slurm/sbatch.py` & `cg-33.0.5/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/slurm/slurm_api.py` & `cg-33.0.5/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/tb/api.py` & `cg-33.0.5/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/tb/models.py` & `cg-33.0.5/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/apps/vogue.py` & `cg-33.0.5/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/add.py` & `cg-33.0.5/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/backup.py` & `cg-33.0.5/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/base.py` & `cg-33.0.5/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/clean.py` & `cg-33.0.5/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/compress/base.py` & `cg-33.0.5/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/compress/fastq.py` & `cg-33.0.5/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/compress/helpers.py` & `cg-33.0.5/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/delete/base.py` & `cg-33.0.5/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/delete/case.py` & `cg-33.0.5/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/delete/cases.py` & `cg-33.0.5/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/delete/observations.py` & `cg-33.0.5/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/deliver/base.py` & `cg-33.0.5/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/demultiplex/add.py` & `cg-33.0.5/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/demultiplex/base.py` & `cg-33.0.5/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/demultiplex/demux.py` & `cg-33.0.5/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/demultiplex/finish.py` & `cg-33.0.5/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/demultiplex/report.py` & `cg-33.0.5/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/demultiplex/sample_sheet.py` & `cg-33.0.5/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/generate/report/base.py` & `cg-33.0.5/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/generate/report/options.py` & `cg-33.0.5/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/generate/report/utils.py` & `cg-33.0.5/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/get.py` & `cg-33.0.5/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/set/base.py` & `cg-33.0.5/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/set/case.py` & `cg-33.0.5/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/set/cases.py` & `cg-33.0.5/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/store/fastq.py` & `cg-33.0.5/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/store/store.py` & `cg-33.0.5/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/transfer.py` & `cg-33.0.5/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/base.py` & `cg-33.0.5/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/clinical_delivery.py` & `cg-33.0.5/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/coverage.py` & `cg-33.0.5/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/delivery_report.py` & `cg-33.0.5/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/fohm.py` & `cg-33.0.5/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/genotype.py` & `cg-33.0.5/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/gens.py` & `cg-33.0.5/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/gisaid.py` & `cg-33.0.5/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/mutacc.py` & `cg-33.0.5/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/nipt/base.py` & `cg-33.0.5/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/nipt/ftp.py` & `cg-33.0.5/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/nipt/statina.py` & `cg-33.0.5/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/observations/observations.py` & `cg-33.0.5/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/observations/utils.py` & `cg-33.0.5/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/scout.py` & `cg-33.0.5/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/utils.py` & `cg-33.0.5/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/validate.py` & `cg-33.0.5/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/upload/vogue.py` & `cg-33.0.5/cg/cli/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/balsamic/base.py` & `cg-33.0.5/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/balsamic/options.py` & `cg-33.0.5/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/balsamic/pon.py` & `cg-33.0.5/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/balsamic/qc.py` & `cg-33.0.5/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/balsamic/umi.py` & `cg-33.0.5/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/base.py` & `cg-33.0.5/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/commands.py` & `cg-33.0.5/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/fastq/base.py` & `cg-33.0.5/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/fluffy/base.py` & `cg-33.0.5/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/microsalt/base.py` & `cg-33.0.5/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/mip/base.py` & `cg-33.0.5/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/mip/options.py` & `cg-33.0.5/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/mip_dna/base.py` & `cg-33.0.5/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/mip_rna/base.py` & `cg-33.0.5/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/mutant/base.py` & `cg-33.0.5/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/nextflow/options.py` & `cg-33.0.5/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/rnafusion/base.py` & `cg-33.0.5/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/rnafusion/options.py` & `cg-33.0.5/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/cli/workflow/taxprofiler/base.py` & `cg-33.0.5/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/__init__.py` & `cg-33.0.5/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/bcl_convert_metrics.py` & `cg-33.0.5/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/compression.py` & `cg-33.0.5/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/constants.py` & `cg-33.0.5/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/delivery.py` & `cg-33.0.5/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/demultiplexing.py` & `cg-33.0.5/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/encryption.py` & `cg-33.0.5/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/gene_panel.py` & `cg-33.0.5/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/housekeeper_tags.py` & `cg-33.0.5/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/lims.py` & `cg-33.0.5/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/nextflow.py` & `cg-33.0.5/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/observations.py` & `cg-33.0.5/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/orderforms.py` & `cg-33.0.5/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/priority.py` & `cg-33.0.5/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/report.py` & `cg-33.0.5/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/rnafusion.py` & `cg-33.0.5/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/scout_upload.py` & `cg-33.0.5/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/sequencing.py` & `cg-33.0.5/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/constants/subject.py` & `cg-33.0.5/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/exc.py` & `cg-33.0.5/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/io/api.py` & `cg-33.0.5/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/io/controller.py` & `cg-33.0.5/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/io/csv.py` & `cg-33.0.5/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/io/json.py` & `cg-33.0.5/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/io/validate_path.py` & `cg-33.0.5/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/io/xml.py` & `cg-33.0.5/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/io/yaml.py` & `cg-33.0.5/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/archive/ddn_dataflow.py` & `cg-33.0.5/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/backup/backup.py` & `cg-33.0.5/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/backup/pdc.py` & `cg-33.0.5/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/clean/api.py` & `cg-33.0.5/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-33.0.5/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/clean/flow_cell_run_directories.py` & `cg-33.0.5/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/compress/compress.py` & `cg-33.0.5/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/compress/files.py` & `cg-33.0.5/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/deliver.py` & `cg-33.0.5/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/deliver_ticket.py` & `cg-33.0.5/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-33.0.5/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/demultiplex/demux_post_processing.py` & `cg-33.0.5/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/demultiplex/files.py` & `cg-33.0.5/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/encryption/encryption.py` & `cg-33.0.5/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/invoice.py` & `cg-33.0.5/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/meta.py` & `cg-33.0.5/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/observations/balsamic_observations_api.py` & `cg-33.0.5/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/observations/mip_dna_observations_api.py` & `cg-33.0.5/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/observations/observations_api.py` & `cg-33.0.5/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/api.py` & `cg-33.0.5/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/case_submitter.py` & `cg-33.0.5/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/fastq_submitter.py` & `cg-33.0.5/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/lims.py` & `cg-33.0.5/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/metagenome_submitter.py` & `cg-33.0.5/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/microbial_submitter.py` & `cg-33.0.5/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/pool_submitter.py` & `cg-33.0.5/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/sars_cov_2_submitter.py` & `cg-33.0.5/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/submitter.py` & `cg-33.0.5/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/orders/ticket_handler.py` & `cg-33.0.5/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/report/balsamic.py` & `cg-33.0.5/cg/meta/report/balsamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 )
 from cg.constants.scout_upload import BALSAMIC_CASE_TAGS
 from cg.meta.report.field_validators import get_million_read_pairs
 from cg.meta.workflow.balsamic import BalsamicAnalysisAPI
 from cg.meta.report.report_api import ReportAPI
 from cg.models.balsamic.analysis import BalsamicAnalysis
 from cg.models.balsamic.config import BalsamicVarCaller
-from cg.models.balsamic.metrics import BalsamicTargetedQCMetrics, BalsamicWGSQCMetrics
+from cg.models.balsamic.metrics import (
+    BalsamicTargetedQCMetrics,
+    BalsamicWGSQCMetrics,
+    BalsamicQCMetrics,
+)
 from cg.models.cg_config import CGConfig
 from cg.models.report.metadata import (
     BalsamicTargetedSampleMetadataModel,
     BalsamicWGSSampleMetadataModel,
 )
 from cg.models.report.report import CaseModel
 from cg.models.report.sample import SampleModel
@@ -39,40 +43,43 @@
 
 
 class BalsamicReportAPI(ReportAPI):
     """API to create BALSAMIC delivery reports."""
 
     def __init__(self, config: CGConfig, analysis_api: BalsamicAnalysisAPI):
         super().__init__(config=config, analysis_api=analysis_api)
-        self.analysis_api = analysis_api
+        self.analysis_api: BalsamicAnalysisAPI = analysis_api
 
     def get_sample_metadata(
         self, case: Family, sample: Sample, analysis_metadata: BalsamicAnalysis
     ) -> Union[BalsamicTargetedSampleMetadataModel, BalsamicWGSSampleMetadataModel]:
-        """Fetches the sample metadata to include in the report."""
-
-        sample_metrics = analysis_metadata.sample_metrics[sample.internal_id]
-        million_read_pairs = get_million_read_pairs(sample.reads)
-
-        if "wgs" in self.get_data_analysis_type(case):
-            return self.get_wgs_metadata(million_read_pairs, sample_metrics)
-
+        """Return the sample metadata to include in the report."""
+        sample_metrics: Dict[str, BalsamicQCMetrics] = analysis_metadata.sample_metrics[
+            sample.internal_id
+        ]
+        million_read_pairs: float = get_million_read_pairs(reads=sample.reads)
+        if "wgs" in self.get_data_analysis_type(case=case):
+            return self.get_wgs_metadata(
+                million_read_pairs=million_read_pairs, sample_metrics=sample_metrics
+            )
         return self.get_panel_metadata(
-            sample, million_read_pairs, sample_metrics, analysis_metadata
+            sample=sample,
+            million_read_pairs=million_read_pairs,
+            sample_metrics=sample_metrics,
+            analysis_metadata=analysis_metadata,
         )
 
     @staticmethod
     def get_panel_metadata(
         sample: Sample,
         million_read_pairs: float,
         sample_metrics: BalsamicTargetedQCMetrics,
         analysis_metadata: BalsamicAnalysis,
     ) -> BalsamicTargetedSampleMetadataModel:
         """Returns a report metadata for BALSAMIC TGS analysis."""
-
         return BalsamicTargetedSampleMetadataModel(
             bait_set=sample.capture_kit,
             bait_set_version=analysis_metadata.config.panel.capture_kit_version,
             million_read_pairs=million_read_pairs,
             median_target_coverage=sample_metrics.median_target_coverage
             if sample_metrics
             else None,
@@ -83,148 +90,144 @@
             fold_80=sample_metrics.fold_80_base_penalty if sample_metrics else None,
         )
 
     def get_wgs_metadata(
         self, million_read_pairs: float, sample_metrics: BalsamicWGSQCMetrics
     ) -> BalsamicWGSSampleMetadataModel:
         """Returns a report metadata for BALSAMIC WGS analysis."""
-
         return BalsamicWGSSampleMetadataModel(
             million_read_pairs=million_read_pairs,
             median_coverage=sample_metrics.median_coverage if sample_metrics else None,
             pct_15x=sample_metrics.pct_15x if sample_metrics else None,
             pct_60x=sample_metrics.pct_60x if sample_metrics else None,
-            duplicates=self.get_wgs_percent_duplication(sample_metrics),
+            duplicates=self.get_wgs_percent_duplication(sample_metrics=sample_metrics),
             mean_insert_size=sample_metrics.mean_insert_size if sample_metrics else None,
             fold_80=sample_metrics.fold_80_base_penalty if sample_metrics else None,
         )
 
     @staticmethod
     def get_wgs_percent_duplication(sample_metrics: BalsamicWGSQCMetrics):
         """Returns the duplication percentage taking into account both reads."""
-
         return (
             (sample_metrics.percent_duplication_r1 + sample_metrics.percent_duplication_r2) / 2
             if sample_metrics
             else None
         )
 
     def get_data_analysis_type(self, case: Family) -> Optional[str]:
         """Retrieves the data analysis type carried out."""
-
-        return self.analysis_api.get_bundle_deliverables_type(case.internal_id)
+        return self.analysis_api.get_bundle_deliverables_type(case_id=case.internal_id)
 
     def get_genome_build(self, analysis_metadata: BalsamicAnalysis) -> str:
         """Returns the build version of the genome reference of a specific case."""
-
         return analysis_metadata.config.reference.reference_genome_version
 
     def get_variant_callers(self, analysis_metadata: BalsamicAnalysis) -> list:
         """
         Extracts the list of BALSAMIC variant-calling filters and their versions (if available) from the
         config.json file.
         """
-
-        sequencing_type = analysis_metadata.config.analysis.sequencing_type
-        analysis_type = analysis_metadata.config.analysis.analysis_type
+        sequencing_type: str = analysis_metadata.config.analysis.sequencing_type
+        analysis_type: str = analysis_metadata.config.analysis.analysis_type
         var_callers: Dict[str, BalsamicVarCaller] = analysis_metadata.config.vcf
         tool_versions: Dict[str, list] = analysis_metadata.config.bioinfo_tools_version
-
         analysis_var_callers = list()
         for var_caller_name, var_caller_attributes in var_callers.items():
             if (
                 sequencing_type in var_caller_attributes.sequencing_type
                 and analysis_type in var_caller_attributes.analysis_type
             ):
-                version = self.get_variant_caller_version(var_caller_name, tool_versions)
+                version: str = self.get_variant_caller_version(
+                    var_caller_name=var_caller_name, var_caller_versions=tool_versions
+                )
                 analysis_var_callers.append(
                     f"{var_caller_name} (v{version})" if version else var_caller_name
                 )
-
         return analysis_var_callers
 
     @staticmethod
     def get_variant_caller_version(
-        var_caller_name: str,
-        var_caller_versions: dict,
+        var_caller_name: str, var_caller_versions: dict
     ) -> Optional[str]:
         """Returns the version of a specific BALSAMIC tool."""
-
         for tool_name, versions in var_caller_versions.items():
             if tool_name in var_caller_name:
                 return versions[0]
-
         return None
 
     def get_report_accreditation(
         self, samples: List[SampleModel], analysis_metadata: BalsamicAnalysis
     ) -> bool:
         """Checks if the report is accredited or not."""
-
         if analysis_metadata.config.analysis.sequencing_type == "targeted" and next(
             (
-                i
-                for i in BALSAMIC_REPORT_ACCREDITED_PANELS
-                if i in str(analysis_metadata.config.panel.capture_kit)
+                panel
+                for panel in BALSAMIC_REPORT_ACCREDITED_PANELS
+                if panel in str(analysis_metadata.config.panel.capture_kit)
             ),
             None,
         ):
             return True
-
         return False
 
     def get_required_fields(self, case: CaseModel) -> dict:
         """Retrieves a dictionary with the delivery report required fields for BALSAMIC."""
-
-        analysis_type = case.data_analysis.type
-        required_sample_metadata_fields = list()
-
+        analysis_type: str = case.data_analysis.type
+        required_sample_metadata_fields: List[str] = []
         if BALSAMIC_ANALYSIS_TYPE["tumor_wgs"] in analysis_type:
-            required_sample_metadata_fields = REQUIRED_SAMPLE_METADATA_BALSAMIC_TO_WGS_FIELDS
+            required_sample_metadata_fields: List[
+                str
+            ] = REQUIRED_SAMPLE_METADATA_BALSAMIC_TO_WGS_FIELDS
         elif BALSAMIC_ANALYSIS_TYPE["tumor_normal_wgs"] in analysis_type:
-            required_sample_metadata_fields = REQUIRED_SAMPLE_METADATA_BALSAMIC_TN_WGS_FIELDS
+            required_sample_metadata_fields: List[
+                str
+            ] = REQUIRED_SAMPLE_METADATA_BALSAMIC_TN_WGS_FIELDS
         elif (
             BALSAMIC_ANALYSIS_TYPE["tumor_panel"] in analysis_type
             or BALSAMIC_ANALYSIS_TYPE["tumor_normal_panel"] in analysis_type
         ):
-            required_sample_metadata_fields = REQUIRED_SAMPLE_METADATA_BALSAMIC_TARGETED_FIELDS
-
+            required_sample_metadata_fields: List[
+                str
+            ] = REQUIRED_SAMPLE_METADATA_BALSAMIC_TARGETED_FIELDS
         return {
             "report": REQUIRED_REPORT_FIELDS,
             "customer": REQUIRED_CUSTOMER_FIELDS,
             "case": REQUIRED_CASE_FIELDS,
-            "applications": self.get_application_required_fields(case, REQUIRED_APPLICATION_FIELDS),
+            "applications": self.get_application_required_fields(
+                case=case, required_fields=REQUIRED_APPLICATION_FIELDS
+            ),
             "data_analysis": REQUIRED_DATA_ANALYSIS_BALSAMIC_FIELDS,
-            "samples": self.get_sample_required_fields(case, REQUIRED_SAMPLE_BALSAMIC_FIELDS),
-            "methods": self.get_sample_required_fields(case, REQUIRED_SAMPLE_METHODS_FIELDS),
+            "samples": self.get_sample_required_fields(
+                case=case, required_fields=REQUIRED_SAMPLE_BALSAMIC_FIELDS
+            ),
+            "methods": self.get_sample_required_fields(
+                case=case, required_fields=REQUIRED_SAMPLE_METHODS_FIELDS
+            ),
             "timestamps": self.get_timestamp_required_fields(
-                case, REQUIRED_SAMPLE_TIMESTAMP_FIELDS
+                case=case, required_fields=REQUIRED_SAMPLE_TIMESTAMP_FIELDS
+            ),
+            "metadata": self.get_sample_required_fields(
+                case=case, required_fields=required_sample_metadata_fields
             ),
-            "metadata": self.get_sample_required_fields(case, required_sample_metadata_fields),
         }
 
     def get_template_name(self) -> str:
         """Retrieves the template name to render the delivery report."""
-
         return Pipeline.BALSAMIC + "_report.html"
 
     def get_upload_case_tags(self) -> dict:
         """Retrieves BALSAMIC upload case tags."""
-
         return BALSAMIC_CASE_TAGS
 
     def get_scout_uploaded_file_from_hk(self, case_id: str, scout_tag: str) -> Optional[str]:
         """Return the file path of the uploaded to Scout file given its tag."""
-
         version: Version = self.housekeeper_api.last_version(bundle=case_id)
         tags: list = self.get_hk_scout_file_tags(scout_tag=scout_tag)
         uploaded_file: File = self.housekeeper_api.get_latest_file(
             bundle=case_id, tags=tags, version=version.id
         )
-
         if not tags or not uploaded_file:
             LOG.warning(
                 f"No files were found for the following Scout Housekeeper tag: {scout_tag} (case: {case_id})"
             )
             return None
-
         return uploaded_file.full_path
```

### Comparing `cg-33.0.4/cg/meta/report/balsamic_umi.py` & `cg-33.0.5/cg/meta/report/balsamic_umi.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,13 +10,12 @@
 
 
 class BalsamicUmiReportAPI(BalsamicReportAPI):
     """API to create BALSAMIC UMI delivery reports."""
 
     def __init__(self, config: CGConfig, analysis_api: BalsamicUmiAnalysisAPI):
         super().__init__(config=config, analysis_api=analysis_api)
-        self.analysis_api = analysis_api
+        self.analysis_api: BalsamicUmiAnalysisAPI = analysis_api
 
     def get_upload_case_tags(self) -> dict:
         """Retrieves BALSAMIC UMI upload case tags."""
-
         return BALSAMIC_UMI_CASE_TAGS
```

### Comparing `cg-33.0.4/cg/meta/report/field_validators.py` & `cg-33.0.5/cg/meta/report/field_validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,102 +5,95 @@
 from cg.constants import NA_FIELD
 from cg.constants.constants import SCALE_TO_MILLION_READ_PAIRS
 from cg.models.report.report import ReportModel
 
 
 def get_million_read_pairs(reads: int) -> Optional[float]:
     """Represents the number of sequencing reads as millions of read pairs."""
-
     return (
         round(reads / SCALE_TO_MILLION_READ_PAIRS, 1) if reads or isinstance(reads, int) else None
     )
 
 
 def get_missing_fields(empty_fields: list, required_fields: list) -> list:
     """Extracts the missing fields that are required to generate successfully the delivery report."""
-
     missing_fields = list()
-
     for field in empty_fields:
         if field in required_fields:
             missing_fields.append(field)
-
     return missing_fields
 
 
 def get_empty_fields(report_data: dict) -> list:
     """Returns a list of empty report fields."""
-
     empty_fields = list()
-
     for field, value in report_data.items():
         if not value or value == NA_FIELD:
             if isinstance(value, bool):
                 continue
-
             empty_fields.append(field)
-
     return empty_fields
 
 
 def get_empty_report_data(report_data: ReportModel) -> dict:
     """Retrieve empty fields from a report data model."""
-
     empty_fields = {
-        "report": get_empty_fields(report_data.dict()),
-        "customer": get_empty_fields(report_data.customer.dict()),
-        "case": get_empty_fields(report_data.case.dict()),
+        "report": get_empty_fields(report_data=report_data.dict()),
+        "customer": get_empty_fields(report_data=report_data.customer.dict()),
+        "case": get_empty_fields(report_data=report_data.case.dict()),
         "applications": {
-            app.tag: get_empty_fields(app.dict())
+            app.tag: get_empty_fields(report_data=app.dict())
             for app in report_data.case.applications
-            if get_empty_fields(app.dict())
+            if get_empty_fields(report_data=app.dict())
         },
-        "data_analysis": get_empty_fields(report_data.case.data_analysis.dict()),
+        "data_analysis": get_empty_fields(report_data=report_data.case.data_analysis.dict()),
         "samples": {
-            sample.id: get_empty_fields(sample.dict())
+            sample.id: get_empty_fields(report_data=sample.dict())
             for sample in report_data.case.samples
-            if get_empty_fields(sample.dict())
+            if get_empty_fields(report_data=sample.dict())
         },
         "methods": {
-            sample.id: get_empty_fields(sample.methods.dict())
+            sample.id: get_empty_fields(report_data=sample.methods.dict())
             for sample in report_data.case.samples
-            if get_empty_fields(sample.methods.dict())
+            if get_empty_fields(report_data=sample.methods.dict())
         },
         "timestamps": {
-            sample.id: get_empty_fields(sample.timestamps.dict())
+            sample.id: get_empty_fields(report_data=sample.timestamps.dict())
             for sample in report_data.case.samples
-            if get_empty_fields(sample.timestamps.dict())
+            if get_empty_fields(report_data=sample.timestamps.dict())
         },
         "metadata": {
-            sample.id: get_empty_fields(sample.metadata.dict())
+            sample.id: get_empty_fields(report_data=sample.metadata.dict())
             for sample in report_data.case.samples
-            if get_empty_fields(sample.metadata.dict())
+            if get_empty_fields(report_data=sample.metadata.dict())
         },
     }
-
     # Clear empty values
     empty_fields = {k: v for k, v in empty_fields.items() if v}
-
     return empty_fields
 
 
 def get_missing_report_data(empty_fields: dict, required_fields: dict) -> dict:
     """Retrieve the missing required fields from a report data model."""
-
     nested_sources = ["applications", "samples", "methods", "timestamps", "metadata"]
     missing_fields = dict()
-
     for source in empty_fields:
         if source in nested_sources:
             # Associates application/sample tags/ids to missing fields
             missing_data = {
-                tag: get_missing_fields(empty_fields[source][tag], required_fields[source][tag])
+                tag: get_missing_fields(
+                    empty_fields=empty_fields[source][tag],
+                    required_fields=required_fields[source][tag],
+                )
                 for tag in empty_fields[source]
-                if get_missing_fields(empty_fields[source][tag], required_fields[source][tag])
+                if get_missing_fields(
+                    empty_fields=empty_fields[source][tag],
+                    required_fields=required_fields[source][tag],
+                )
             }
         else:
-            missing_data = get_missing_fields(empty_fields[source], required_fields[source])
-
+            missing_data = get_missing_fields(
+                empty_fields=empty_fields[source], required_fields=required_fields[source]
+            )
         if missing_data:
             missing_fields.update({source: missing_data})
-
     return missing_fields
```

### Comparing `cg-33.0.4/cg/meta/report/mip_dna.py` & `cg-33.0.5/cg/meta/report/mip_dna.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,143 +32,130 @@
 
 
 class MipDNAReportAPI(ReportAPI):
     """API to create Rare disease DNA delivery reports."""
 
     def __init__(self, config: CGConfig, analysis_api: MipDNAAnalysisAPI):
         super().__init__(config=config, analysis_api=analysis_api)
-        self.analysis_api = analysis_api
+        self.analysis_api: MipDNAAnalysisAPI = analysis_api
 
     def get_sample_metadata(
         self, case: Family, sample: Sample, analysis_metadata: MipAnalysis
     ) -> MipDNASampleMetadataModel:
         """Fetches the MIP DNA sample metadata to include in the report."""
-
         parsed_metrics = get_sample_id_metric(
             sample_id=sample.internal_id, sample_id_metrics=analysis_metadata.sample_id_metrics
         )
-        sample_coverage = self.get_sample_coverage(sample, case)
-
+        sample_coverage: dict = self.get_sample_coverage(sample=sample, case=case)
         return MipDNASampleMetadataModel(
             bait_set=self.lims_api.capture_kit(lims_id=sample.internal_id),
             gender=parsed_metrics.predicted_sex,
-            million_read_pairs=get_million_read_pairs(sample.reads),
+            million_read_pairs=get_million_read_pairs(reads=sample.reads),
             mapped_reads=parsed_metrics.mapped_reads,
             mean_target_coverage=sample_coverage.get("mean_coverage"),
             pct_10x=sample_coverage.get("mean_completeness"),
             duplicates=parsed_metrics.duplicate_reads,
         )
 
     def get_sample_coverage(self, sample: Sample, case: Family) -> dict:
         """Calculates coverage values for a specific sample."""
-
-        genes = self.get_genes_from_scout(case.panels)
-        sample_coverage = self.chanjo_api.sample_coverage(sample.internal_id, genes)
+        genes = self.get_genes_from_scout(panels=case.panels)
+        sample_coverage = self.chanjo_api.sample_coverage(
+            sample_id=sample.internal_id, panel_genes=genes
+        )
         if sample_coverage:
             return sample_coverage
-
         LOG.warning("Could not calculate sample coverage for: %s", sample.internal_id)
         return dict()
 
     def get_genes_from_scout(self, panels: list) -> list:
         """Extracts panel gene IDs information from Scout."""
-
         panel_genes = list()
         for panel in panels:
             panel_genes.extend(self.scout_api.get_genes(panel))
-
         panel_gene_ids = [gene.get("hgnc_id") for gene in panel_genes]
         return panel_gene_ids
 
     def get_data_analysis_type(self, case: Family) -> Optional[str]:
         """Retrieves the data analysis type carried out."""
-
         case_sample: Sample = self.status_db.get_case_samples_by_case_id(
             case_internal_id=case.internal_id
         )[0].sample
-        lims_sample = self.get_lims_sample(case_sample.internal_id)
+        lims_sample = self.get_lims_sample(sample_id=case_sample.internal_id)
         application: Application = self.status_db.get_application_by_tag(
             tag=lims_sample.get("application")
         )
-
         return application.analysis_type if application else None
 
     def get_genome_build(self, analysis_metadata: MipAnalysis) -> str:
         """Returns the build version of the genome reference of a specific case."""
-
         return analysis_metadata.genome_build
 
     def get_variant_callers(self, analysis_metadata: MipAnalysis = None) -> list:
         """Extracts the list of variant-calling filters used during analysis."""
-
         return []
 
     def get_report_accreditation(
         self, samples: List[SampleModel], analysis_metadata: MipAnalysis = None
     ) -> bool:
         """Checks if the report is accredited or not by evaluating each of the sample process accreditations."""
-
         for sample in samples:
             if not sample.application.accredited:
                 return False
-
         return True
 
     def get_required_fields(self, case: CaseModel) -> dict:
         """Retrieves a dictionary with the delivery report required fields for MIP DNA."""
-
         return {
             "report": REQUIRED_REPORT_FIELDS,
             "customer": REQUIRED_CUSTOMER_FIELDS,
             "case": REQUIRED_CASE_FIELDS,
-            "applications": self.get_application_required_fields(case, REQUIRED_APPLICATION_FIELDS),
+            "applications": self.get_application_required_fields(
+                case=case, required_fields=REQUIRED_APPLICATION_FIELDS
+            ),
             "data_analysis": REQUIRED_DATA_ANALYSIS_MIP_DNA_FIELDS,
-            "samples": self.get_sample_required_fields(case, REQUIRED_SAMPLE_MIP_DNA_FIELDS),
-            "methods": self.get_sample_required_fields(case, REQUIRED_SAMPLE_METHODS_FIELDS),
+            "samples": self.get_sample_required_fields(
+                case=case, required_fields=REQUIRED_SAMPLE_MIP_DNA_FIELDS
+            ),
+            "methods": self.get_sample_required_fields(
+                case=case, required_fields=REQUIRED_SAMPLE_METHODS_FIELDS
+            ),
             "timestamps": self.get_timestamp_required_fields(
-                case, REQUIRED_SAMPLE_TIMESTAMP_FIELDS
+                case=case, required_fields=REQUIRED_SAMPLE_TIMESTAMP_FIELDS
             ),
-            "metadata": self.get_sample_metadata_required_fields(case),
+            "metadata": self.get_sample_metadata_required_fields(case=case),
         }
 
     @staticmethod
     def get_sample_metadata_required_fields(case: CaseModel) -> dict:
         """Retrieves sample metadata required fields associated to a specific sample ID."""
-
         required_sample_metadata_fields = dict()
-
         for sample in case.samples:
             required_fields = (
                 REQUIRED_SAMPLE_METADATA_MIP_DNA_WGS_FIELDS
                 if "wgs" in sample.application.prep_category.lower()
                 else REQUIRED_SAMPLE_METADATA_MIP_DNA_FIELDS
             )
-
             required_sample_metadata_fields.update({sample.id: required_fields})
-
         return required_sample_metadata_fields
 
     def get_template_name(self) -> str:
         """Retrieves the template name to render the delivery report."""
-
         return Pipeline.MIP_DNA + "_report.html"
 
     def get_upload_case_tags(self) -> dict:
         """Retrieves MIP DNA upload case tags."""
-
         return MIP_CASE_TAGS
 
     def get_scout_uploaded_file_from_hk(self, case_id: str, scout_tag: str) -> Optional[str]:
         """Returns the file path of the uploaded to Scout file given its tag."""
-
         version: Version = self.housekeeper_api.last_version(bundle=case_id)
         tags: list = self.get_hk_scout_file_tags(scout_tag=scout_tag)
         uploaded_files: Iterable[File] = self.housekeeper_api.get_files(
             bundle=case_id, tags=tags, version=version.id
         )
         if not tags or not any(uploaded_files):
             LOG.info(
                 f"No files were found for the following Scout Housekeeper tag: {scout_tag} (case: {case_id})"
             )
             return None
-
         return uploaded_files[0].full_path
```

### Comparing `cg-33.0.4/cg/meta/report/report_api.py` & `cg-33.0.5/cg/meta/report/report_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,282 +26,255 @@
     CustomerModel,
     CaseModel,
     DataAnalysisModel,
     ScoutReportFiles,
 )
 from cg.models.report.sample import SampleModel, ApplicationModel, TimestampModel, MethodsModel
 from cg.store.models import Analysis, Application, Family, Sample, FamilySample
-from jinja2 import Environment, PackageLoader, select_autoescape
+from jinja2 import Environment, PackageLoader, select_autoescape, Template
 
 LOG = logging.getLogger(__name__)
 
 
 class ReportAPI(MetaAPI):
     """Common Delivery Report API."""
 
     def __init__(self, config: CGConfig, analysis_api: AnalysisAPI):
         super().__init__(config=config)
-        self.analysis_api = analysis_api
+        self.analysis_api: AnalysisAPI = analysis_api
 
     def create_delivery_report(
         self, case_id: str, analysis_date: datetime, force_report: bool
     ) -> str:
         """Generates the html contents of a delivery report."""
-
         report_data: ReportModel = self.get_report_data(
             case_id=case_id, analysis_date=analysis_date
         )
-        report_data: ReportModel = self.validate_report_fields(case_id, report_data, force_report)
-
-        rendered_report = self.render_delivery_report(report_data.dict())
+        report_data: ReportModel = self.validate_report_fields(
+            case_id=case_id, report_data=report_data, force_report=force_report
+        )
+        rendered_report: str = self.render_delivery_report(report_data=report_data.dict())
         return rendered_report
 
     def create_delivery_report_file(
         self, case_id: str, file_path: Path, analysis_date: datetime, force_report: bool
     ) -> TextIO:
         """Generates a temporary file containing a delivery report."""
-
         file_path.mkdir(parents=True, exist_ok=True)
-        delivery_report = self.create_delivery_report(
+        delivery_report: str = self.create_delivery_report(
             case_id=case_id, analysis_date=analysis_date, force_report=force_report
         )
-
-        report_file_path = Path(file_path / "delivery-report.html")
+        report_file_path: Path = Path(file_path / "delivery-report.html")
         with open(report_file_path, "w") as delivery_report_file:
             delivery_report_file.write(delivery_report)
-
         return delivery_report_file
 
     def add_delivery_report_to_hk(
         self, delivery_report_file: Path, case_id: str, analysis_date: datetime
     ) -> Optional[File]:
         """
         Adds a delivery report file, if it has not already been generated, to an analysis bundle for a specific case
         in HK and returns a pointer to it.
         """
-
         version = self.housekeeper_api.version(case_id, analysis_date)
         try:
             self.get_delivery_report_from_hk(case_id=case_id)
         except FileNotFoundError:
             LOG.info(f"Adding a new delivery report to housekeeper for {case_id}")
             file: File = self.housekeeper_api.add_file(
                 delivery_report_file.name, version, [case_id, HK_DELIVERY_REPORT_TAG]
             )
             self.housekeeper_api.include_file(file, version)
             self.housekeeper_api.add_commit(file)
             return file
-
         return None
 
     def get_delivery_report_from_hk(self, case_id: str) -> str:
         """Extracts the delivery reports of a specific case stored in HK."""
-
         version: Version = self.housekeeper_api.last_version(case_id)
         delivery_report: File = self.housekeeper_api.get_latest_file(
             bundle=case_id, tags=[HK_DELIVERY_REPORT_TAG], version=version.id
         )
-
         if not delivery_report:
             LOG.warning(f"No existing delivery report found in housekeeper for {case_id}")
             raise FileNotFoundError
-
         return delivery_report.full_path
 
     def get_scout_uploaded_file_from_hk(self, case_id: str, scout_tag: str) -> Optional[str]:
         """Return the file path of the uploaded to Scout file given its tag."""
-
         raise NotImplementedError
 
     def render_delivery_report(self, report_data: dict) -> str:
         """Renders the report on the Jinja template."""
-
-        env = Environment(
+        env: Environment = Environment(
             loader=PackageLoader("cg", "meta/report/templates"),
             autoescape=select_autoescape(["html", "xml"]),
         )
-        template_name = self.get_template_name()
-        template = env.get_template(template_name)
+        template: Template = env.get_template(self.get_template_name())
         return template.render(**report_data)
 
     def get_cases_without_delivery_report(self, pipeline: Pipeline) -> List[Family]:
         """Returns a list of cases that has been stored and need a delivery report."""
-
-        stored_cases = []
-        analyses: Query = self.status_db.analyses_to_delivery_report(pipeline)[
+        stored_cases: List[Family] = []
+        analyses: Query = self.status_db.analyses_to_delivery_report(pipeline=pipeline)[
             :MAX_ITEMS_TO_RETRIEVE
         ]
-
         for analysis_obj in analyses:
             case: Family = analysis_obj.family
-            last_version: Version = self.housekeeper_api.last_version(case.internal_id)
+            last_version: Version = self.housekeeper_api.last_version(bundle=case.internal_id)
             hk_file: File = self.housekeeper_api.get_files(
                 bundle=case.internal_id, version=last_version.id if last_version else None
             ).first()
 
             if hk_file and Path(hk_file.full_path).is_file():
                 stored_cases.append(case)
             else:
                 LOG.warning(
                     f"Case {case.internal_id} must be stored before creating a delivery report"
                 )
-
         return stored_cases
 
     def get_cases_without_uploaded_delivery_report(self, pipeline: Pipeline) -> List[Family]:
         """Returns a list of cases that need a delivery report to be uploaded."""
-
-        analyses: Query = self.status_db.analyses_to_upload_delivery_reports(pipeline)[
+        analyses: Query = self.status_db.analyses_to_upload_delivery_reports(pipeline=pipeline)[
             :MAX_ITEMS_TO_RETRIEVE
         ]
-
         return [analysis_obj.family for analysis_obj in analyses]
 
     def update_delivery_report_date(self, case: Family, analysis_date: datetime) -> None:
         """Updates the date when delivery report was created."""
-
         analysis: Analysis = self.status_db.get_analysis_by_case_entry_id_and_started_at(
             case_entry_id=case.id, started_at_date=analysis_date
         )
         analysis.delivery_report_created_at = datetime.now()
         self.status_db.session.commit()
 
     def get_report_data(self, case_id: str, analysis_date: datetime) -> ReportModel:
         """Fetches all the data needed to generate a delivery report."""
-
         case: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
         analysis: Analysis = self.status_db.get_analysis_by_case_entry_id_and_started_at(
             case_entry_id=case.id, started_at_date=analysis_date
         )
         analysis_metadata: AnalysisModel = self.analysis_api.get_latest_metadata(case.internal_id)
         case_model: CaseModel = self.get_case_data(case, analysis, analysis_metadata)
-
         return ReportModel(
-            customer=self.get_customer_data(case),
-            version=self.get_report_version(analysis),
+            customer=self.get_customer_data(case=case),
+            version=self.get_report_version(analysis=analysis),
             date=datetime.today(),
             case=case_model,
-            accredited=self.get_report_accreditation(case_model.samples, analysis_metadata),
+            accredited=self.get_report_accreditation(
+                samples=case_model.samples, analysis_metadata=analysis_metadata
+            ),
         )
 
     def validate_report_fields(
         self, case_id: str, report_data: ReportModel, force_report
     ) -> ReportModel:
         """Verifies that the required report fields are not empty."""
-
-        required_fields: dict = self.get_required_fields(report_data.case)
-        empty_report_fields: dict = get_empty_report_data(report_data)
-        missing_report_fields: dict = get_missing_report_data(empty_report_fields, required_fields)
-
+        required_fields: dict = self.get_required_fields(case=report_data.case)
+        empty_report_fields: dict = get_empty_report_data(report_data=report_data)
+        missing_report_fields: dict = get_missing_report_data(
+            empty_fields=empty_report_fields, required_fields=required_fields
+        )
         if missing_report_fields and not force_report:
             LOG.error(
                 f"Could not generate report data for {case_id}. "
                 f"Missing data: \n{WriteStream.write_stream_from_content(content=missing_report_fields, file_format=FileFormat.YAML)}"
             )
             raise DeliveryReportError
-
         if empty_report_fields:
             LOG.warning(
                 f"Empty report fields: \n{WriteStream.write_stream_from_content(content=empty_report_fields, file_format=FileFormat.YAML)}"
             )
-
         return report_data
 
     @staticmethod
     def get_customer_data(case: Family) -> CustomerModel:
         """Returns customer validated attributes retrieved from status DB."""
-
         return CustomerModel(
             name=case.customer.name,
             id=case.customer.internal_id,
             invoice_address=case.customer.invoice_address,
             scout_access=case.customer.scout_access,
         )
 
     @staticmethod
     def get_report_version(analysis: Analysis) -> int:
         """
         Returns the version of the given analysis. The version of the first analysis is 1 and subsequent reruns
         increase it by 1.
         """
-
         version = None
-
         if analysis:
             version = len(analysis.family.analyses) - analysis.family.analyses.index(analysis)
-
         return version
 
     def get_case_data(
         self,
         case: Family,
         analysis: Analysis,
         analysis_metadata: AnalysisModel,
     ) -> CaseModel:
         """Returns case associated validated attributes."""
-
-        samples: List[SampleModel] = self.get_samples_data(case, analysis_metadata)
-        unique_applications: List[ApplicationModel] = self.get_unique_applications(samples)
-
+        samples: List[SampleModel] = self.get_samples_data(
+            case=case, analysis_metadata=analysis_metadata
+        )
+        unique_applications: List[ApplicationModel] = self.get_unique_applications(samples=samples)
         return CaseModel(
             name=case.name,
             id=case.internal_id,
-            data_analysis=self.get_case_analysis_data(case, analysis, analysis_metadata),
+            data_analysis=self.get_case_analysis_data(
+                case=case, analysis=analysis, analysis_metadata=analysis_metadata
+            ),
             samples=samples,
             applications=unique_applications,
         )
 
     def get_samples_data(self, case: Family, analysis_metadata: AnalysisModel) -> List[SampleModel]:
         """Extracts all the samples associated to a specific case and their attributes."""
-
         samples = list()
         case_samples: List[FamilySample] = self.status_db.get_case_samples_by_case_id(
             case_internal_id=case.internal_id
         )
-
         for case_sample in case_samples:
             sample: Sample = case_sample.sample
-            lims_sample: Optional[dict] = self.get_lims_sample(sample.internal_id)
-
+            lims_sample: Optional[dict] = self.get_lims_sample(sample_id=sample.internal_id)
             samples.append(
                 SampleModel(
                     name=sample.name,
                     id=sample.internal_id,
                     ticket=sample.original_ticket,
                     gender=sample.sex,
                     source=lims_sample.get("source") if lims_sample else None,
                     tumour=sample.is_tumour,
-                    application=self.get_sample_application_data(lims_sample),
-                    methods=self.get_sample_methods_data(sample.internal_id),
+                    application=self.get_sample_application_data(lims_sample=lims_sample),
+                    methods=self.get_sample_methods_data(sample_id=sample.internal_id),
                     status=case_sample.status,
-                    metadata=self.get_sample_metadata(case, sample, analysis_metadata),
-                    timestamps=self.get_sample_timestamp_data(sample),
+                    metadata=self.get_sample_metadata(
+                        case=case, sample=sample, analysis_metadata=analysis_metadata
+                    ),
+                    timestamps=self.get_sample_timestamp_data(sample=sample),
                 )
             )
-
         return samples
 
     def get_lims_sample(self, sample_id: str) -> Optional[dict]:
         """Fetches sample data from LIMS. Returns an empty dictionary if the request was unsuccessful."""
-
         lims_sample = dict()
         try:
-            lims_sample = self.lims_api.sample(sample_id)
+            lims_sample: dict = self.lims_api.sample(sample_id)
         except requests.exceptions.HTTPError as ex:
             LOG.info("Could not fetch sample %s from LIMS: %s", sample_id, ex)
-
         return lims_sample
 
     def get_sample_application_data(self, lims_sample: dict) -> ApplicationModel:
         """Retrieves the analysis application attributes."""
-
         application: Application = self.status_db.get_application_by_tag(
             tag=lims_sample.get("application")
         )
-
         return (
             ApplicationModel(
                 tag=application.tag,
                 version=lims_sample.get("application_version"),
                 prep_category=application.prep_category,
                 description=application.description,
                 limitations=application.limitations,
@@ -311,155 +284,139 @@
             if application
             else ApplicationModel()
         )
 
     @staticmethod
     def get_unique_applications(samples: List[SampleModel]) -> List[ApplicationModel]:
         """Returns the unique case associated applications."""
-
         applications = list()
         for sample in samples:
             if sample.application not in applications:
                 applications.append(sample.application)
-
         return applications
 
     def get_sample_methods_data(self, sample_id: str) -> MethodsModel:
         """Fetches sample library preparation and sequencing methods from LIMS."""
-
         library_prep = None
         sequencing = None
         try:
-            library_prep = self.lims_api.get_prep_method(sample_id)
-            sequencing = self.lims_api.get_sequencing_method(sample_id)
+            library_prep = self.lims_api.get_prep_method(lims_id=sample_id)
+            sequencing = self.lims_api.get_sequencing_method(lims_id=sample_id)
         except requests.exceptions.HTTPError as ex:
             LOG.info("Could not fetch sample (%s) methods from LIMS: %s", sample_id, ex)
 
         return MethodsModel(library_prep=library_prep, sequencing=sequencing)
 
     def get_case_analysis_data(
         self,
         case: Family,
         analysis: Analysis,
         analysis_metadata: AnalysisModel,
     ) -> DataAnalysisModel:
         """Retrieves the pipeline attributes used for data analysis."""
-
         return DataAnalysisModel(
             customer_pipeline=case.data_analysis,
             data_delivery=case.data_delivery,
             pipeline=analysis.pipeline,
             pipeline_version=analysis.pipeline_version,
-            type=self.get_data_analysis_type(case),
-            genome_build=self.get_genome_build(analysis_metadata),
-            variant_callers=self.get_variant_callers(analysis_metadata),
+            type=self.get_data_analysis_type(case=case),
+            genome_build=self.get_genome_build(analysis_metadata=analysis_metadata),
+            variant_callers=self.get_variant_callers(analysis_metadata=analysis_metadata),
             panels=case.panels,
-            scout_files=self.get_scout_uploaded_files(case),
+            scout_files=self.get_scout_uploaded_files(case=case),
         )
 
     def get_scout_uploaded_files(self, case: Family) -> ScoutReportFiles:
         """Extracts the files that will be uploaded to Scout."""
-
         return ScoutReportFiles(
-            snv_vcf=self.get_scout_uploaded_file_from_hk(case.internal_id, "snv_vcf"),
-            sv_vcf=self.get_scout_uploaded_file_from_hk(case.internal_id, "sv_vcf"),
-            vcf_str=self.get_scout_uploaded_file_from_hk(case.internal_id, "vcf_str"),
-            smn_tsv=self.get_scout_uploaded_file_from_hk(case.internal_id, "smn_tsv"),
+            snv_vcf=self.get_scout_uploaded_file_from_hk(
+                case_id=case.internal_id, scout_tag="snv_vcf"
+            ),
+            sv_vcf=self.get_scout_uploaded_file_from_hk(
+                case_id=case.internal_id, scout_tag="sv_vcf"
+            ),
+            vcf_str=self.get_scout_uploaded_file_from_hk(
+                case_id=case.internal_id, scout_tag="vcf_str"
+            ),
+            smn_tsv=self.get_scout_uploaded_file_from_hk(
+                case_id=case.internal_id, scout_tag="smn_tsv"
+            ),
         )
 
     @staticmethod
     def get_sample_timestamp_data(sample: Sample) -> TimestampModel:
         """Retrieves the sample processing dates."""
-
         return TimestampModel(
             ordered_at=sample.ordered_at,
             received_at=sample.received_at,
             prepared_at=sample.prepared_at,
             sequenced_at=sample.sequenced_at,
         )
 
     def get_sample_metadata(
         self,
         case: Family,
         sample: Sample,
         analysis_metadata: AnalysisModel,
     ) -> SampleMetadataModel:
-        """Fetches the sample metadata to include in the report."""
-
+        """Return the sample metadata to include in the report."""
         raise NotImplementedError
 
     def get_data_analysis_type(self, case: Family) -> Optional[str]:
         """Retrieves the data analysis type carried out."""
-
         raise NotImplementedError
 
     def get_genome_build(self, analysis_metadata: AnalysisModel) -> str:
         """Returns the build version of the genome reference of a specific case."""
-
         raise NotImplementedError
 
     def get_variant_callers(self, analysis_metadata: AnalysisModel) -> list:
         """Extracts the list of variant-calling filters used during analysis."""
-
         raise NotImplementedError
 
     def get_report_accreditation(
         self, samples: List[SampleModel], analysis_metadata: AnalysisModel
     ) -> bool:
         """Checks if the report is accredited or not."""
-
         raise NotImplementedError
 
     def get_required_fields(self, case: CaseModel) -> dict:
         """Retrieves a dictionary with the delivery report required fields."""
-
         raise NotImplementedError
 
     def get_template_name(self) -> str:
         """Retrieves the pipeline specific template name."""
-
         raise NotImplementedError
 
     @staticmethod
     def get_application_required_fields(case: CaseModel, required_fields: list) -> dict:
         """Retrieves sample required fields."""
-
         required_sample_fields = dict()
-
         for application in case.applications:
             required_sample_fields.update({application.tag: required_fields})
-
         return required_sample_fields
 
     @staticmethod
     def get_sample_required_fields(case: CaseModel, required_fields: list) -> dict:
         """Retrieves sample required fields."""
-
         required_sample_fields = dict()
-
         for sample in case.samples:
             required_sample_fields.update({sample.id: required_fields})
-
         return required_sample_fields
 
     @staticmethod
     def get_timestamp_required_fields(case: CaseModel, required_fields: list) -> dict:
         """Retrieves sample timestamps required fields."""
-
         for sample in case.samples:
             if sample.application.external:
                 required_fields.remove("received_at")
                 break
-
-        return ReportAPI.get_sample_required_fields(case, required_fields)
+        return ReportAPI.get_sample_required_fields(case=case, required_fields=required_fields)
 
     def get_hk_scout_file_tags(self, scout_tag: str) -> Optional[list]:
         """Retrieves pipeline specific uploaded to Scout Housekeeper file tags given a Scout key."""
-
         tags = self.get_upload_case_tags().get(scout_tag)
-
         return list(tags) if tags else None
 
     def get_upload_case_tags(self):
         """Retrieves pipeline specific upload case tags."""
-
         raise NotImplementedError
```

### Comparing `cg-33.0.4/cg/meta/report/templates/balsamic_report.html` & `cg-33.0.5/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/report/templates/bootstrap.html` & `cg-33.0.5/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/report/templates/mip-dna_report.html` & `cg-33.0.5/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/rsync/rsync_api.py` & `cg-33.0.5/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/tar/tar.py` & `cg-33.0.5/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/transfer/external_data.py` & `cg-33.0.5/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/transfer/flowcell.py` & `cg-33.0.5/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/transfer/lims.py` & `cg-33.0.5/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/balsamic/balsamic.py` & `cg-33.0.5/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/coverage.py` & `cg-33.0.5/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/fohm/fohm.py` & `cg-33.0.5/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/gisaid/constants.py` & `cg-33.0.5/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/gisaid/gisaid.py` & `cg-33.0.5/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/gisaid/models.py` & `cg-33.0.5/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/gt.py` & `cg-33.0.5/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/mip/mip_dna.py` & `cg-33.0.5/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/mip/mip_rna.py` & `cg-33.0.5/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/mutacc.py` & `cg-33.0.5/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/nipt/nipt.py` & `cg-33.0.5/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/rnafusion/rnafusion.py` & `cg-33.0.5/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-33.0.5/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-33.0.5/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/scout/hk_tags.py` & `cg-33.0.5/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/scout/mip_config_builder.py` & `cg-33.0.5/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-33.0.5/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/scout/scout_config_builder.py` & `cg-33.0.5/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/scout/uploadscoutapi.py` & `cg-33.0.5/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/upload/upload_api.py` & `cg-33.0.5/cg/meta/upload/upload_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class UploadAPI(MetaAPI):
     """Upload API"""
 
     def __init__(self, config: CGConfig, analysis_api: AnalysisAPI):
         super().__init__(config=config)
-        self.analysis_api = analysis_api
+        self.analysis_api: AnalysisAPI = analysis_api
         self.scout_upload_api: UploadScoutAPI = UploadScoutAPI(
             hk_api=config.housekeeper_api,
             scout_api=config.scout_api,
             madeline_api=config.madeline_api,
             analysis_api=self.analysis_api,
             lims_api=config.lims_api,
             status_db=config.status_db,
```

### Comparing `cg-33.0.4/cg/meta/upload/vogue.py` & `cg-33.0.5/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/analysis.py` & `cg-33.0.5/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/balsamic.py` & `cg-33.0.5/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/balsamic_pon.py` & `cg-33.0.5/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/balsamic_qc.py` & `cg-33.0.5/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/balsamic_umi.py` & `cg-33.0.5/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/fastq.py` & `cg-33.0.5/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/fluffy.py` & `cg-33.0.5/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/microsalt.py` & `cg-33.0.5/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/mip.py` & `cg-33.0.5/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/mip_dna.py` & `cg-33.0.5/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/mip_rna.py` & `cg-33.0.5/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/mutant.py` & `cg-33.0.5/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/nextflow_common.py` & `cg-33.0.5/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/prepare_fastq.py` & `cg-33.0.5/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/rnafusion.py` & `cg-33.0.5/cg/meta/workflow/rnafusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module for Rnafusion Analysis API."""
 
 import logging
 from pathlib import Path
 from typing import Dict, List, Optional
 
+from cg.models.rnafusion.analysis import RnafusionAnalysis
 from pydantic import ValidationError
 
 from cg import resources
 from cg.constants import Pipeline
 from cg.constants.constants import FileFormat, WorkflowManager
 from cg.constants.nextflow import NFX_READ1_HEADER, NFX_READ2_HEADER, NFX_SAMPLE_HEADER
 from cg.constants.rnafusion import (
@@ -27,14 +28,15 @@
 from cg.models.deliverables.metric_deliverables import (
     MetricsBase,
     MetricsDeliverablesCondition,
     MultiqcDataJson,
 )
 from cg.models.nextflow.deliverables import NextflowDeliverables, replace_dict_values
 from cg.models.rnafusion.rnafusion_sample import RnafusionSample
+from cg.store.models import Family
 from cg.utils import Process
 
 LOG = logging.getLogger(__name__)
 
 
 class RnafusionAnalysisAPI(AnalysisAPI):
     """Handles communication between RNAFUSION processes
@@ -341,25 +343,27 @@
 
     def get_metrics_deliverables_path(self, case_id: str) -> Path:
         """Return a path where the <case>_metrics_deliverables.yaml file should be located."""
         return Path(self.root_dir, case_id, f"{case_id}_metrics_deliverables.yaml")
 
     def get_multiqc_json_metrics(self, case_id: str) -> List[MetricsBase]:
         """Get a multiqc_data.json file and returns metrics and values formatted."""
+        case: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
+        sample_id: str = case.links[0].sample.internal_id
         multiqc_json: MultiqcDataJson = MultiqcDataJson(
             **read_json(file_path=self.get_multiqc_json_path(case_id=case_id))
         )
         metrics_values: Dict = {}
         for key in multiqc_json.report_general_stats_data:
             if case_id in key:
                 metrics_values.update(list(key.values())[0])
         return [
             MetricsBase(
                 header=None,
-                id=case_id,
+                id=sample_id,
                 input="multiqc_data.json",
                 name=metric_name,
                 step="multiqc",
                 value=metric_value,
                 condition=RNAFUSION_METRIC_CONDITIONS.get(metric_name, None),
             )
             for metric_name, metric_value in metrics_values.items()
@@ -397,7 +401,23 @@
     def validate_qc_metrics(self, case_id: str) -> None:
         """Validate the information from a qc metrics deliverable file."""
         metrics_deliverables_path: Path = self.get_metrics_deliverables_path(case_id=case_id)
         qcmetrics_raw: dict = ReadFile.get_content_from_file(
             file_format=FileFormat.YAML, file_path=metrics_deliverables_path
         )
         MetricsDeliverablesCondition(**qcmetrics_raw)
+
+    def parse_analysis(self, qc_metrics_raw: List[MetricsBase], **kwargs) -> RnafusionAnalysis:
+        """Parse Rnafusion output analysis files and return analysis model."""
+        sample_metrics: Dict[str, dict] = {}
+        for metric in qc_metrics_raw:
+            metric.name = metric.name.replace("5_3_bias", "bias_5_3")
+            try:
+                sample_metrics[metric.id].update({metric.name.lower(): metric.value})
+            except KeyError:
+                sample_metrics[metric.id] = {metric.name.lower(): metric.value}
+        return RnafusionAnalysis(sample_metrics=sample_metrics)
+
+    def get_latest_metadata(self, case_id: str) -> RnafusionAnalysis:
+        """Return the latest metadata of a specific Rnafusion case."""
+        qc_metrics: List[MetricsBase] = self.get_multiqc_json_metrics(case_id)
+        return self.parse_analysis(qc_metrics_raw=qc_metrics)
```

### Comparing `cg-33.0.4/cg/meta/workflow/taxprofiler.py` & `cg-33.0.5/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/meta/workflow/tower_common.py` & `cg-33.0.5/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/balsamic/config.py` & `cg-33.0.5/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/balsamic/metrics.py` & `cg-33.0.5/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/cg_config.py` & `cg-33.0.5/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/cgstats/stats_sample.py` & `cg-33.0.5/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/compression_data.py` & `cg-33.0.5/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/deliverables/metric_deliverables.py` & `cg-33.0.5/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/demultiplex/demux_results.py` & `cg-33.0.5/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/demultiplex/flow_cell.py` & `cg-33.0.5/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/demultiplex/run_parameters.py` & `cg-33.0.5/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/demultiplex/sbatch.py` & `cg-33.0.5/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/file_data.py` & `cg-33.0.5/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/invoice/invoice.py` & `cg-33.0.5/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/lims/sample.py` & `cg-33.0.5/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/mip/mip_config.py` & `cg-33.0.5/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/mip/mip_metrics_deliverables.py` & `cg-33.0.5/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/mip/mip_sample_info.py` & `cg-33.0.5/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/nextflow/deliverables.py` & `cg-33.0.5/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/nextflow/sample.py` & `cg-33.0.5/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/observations/input_files.py` & `cg-33.0.5/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/orders/constants.py` & `cg-33.0.5/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/orders/excel_sample.py` & `cg-33.0.5/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/orders/json_sample.py` & `cg-33.0.5/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/orders/order.py` & `cg-33.0.5/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/orders/orderform_schema.py` & `cg-33.0.5/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/orders/sample_base.py` & `cg-33.0.5/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/orders/samples.py` & `cg-33.0.5/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/report/report.py` & `cg-33.0.5/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/report/sample.py` & `cg-33.0.5/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/report/validators.py` & `cg-33.0.5/cg/models/report/validators.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,96 +15,86 @@
     REPORT_GENDER,
 )
 
 LOG = logging.getLogger(__name__)
 
 
 def validate_empty_field(value: Union[int, str]) -> str:
-    """Formats an empty value to be included in the report as 'N/A'"""
-
+    """Formats an empty value to be included in the report as N/A."""
     return str(value) if value else NA_FIELD
 
 
 def validate_boolean(value: Union[bool, str]) -> str:
-    """Formats a boolean value for the delivery report"""
-
+    """Formats a boolean value for the delivery report."""
     if isinstance(value, bool) or value:
         if str(value) == "True":
             return YES_FIELD
         if str(value) == "False":
             return NO_FIELD
-
     return NA_FIELD
 
 
 def validate_float(value: Union[float, str]) -> str:
-    """Returns a processed float value"""
-
+    """Returns a processed float value."""
     return str(round(float(value), PRECISION)) if value or isinstance(value, float) else NA_FIELD
 
 
-def validate_date(date: datetime) -> str:
-    """Returns the date part (year, month, day) from a datetime object"""
+def validate_percentage(value: Union[float, str]) -> str:
+    """Returns a processed float value as a percentage."""
+    return validate_float(float(value) * 100) if value else NA_FIELD
 
+
+def validate_date(date: datetime) -> str:
+    """Returns the date part (year, month, day) from a datetime object."""
     return str(date.date()) if date else NA_FIELD
 
 
 def validate_list(value: list) -> str:
-    """Formats a list elements as comma separated individual values"""
-
+    """Formats a list elements as comma separated individual values."""
     return validate_empty_field(
         ", ".join(validate_empty_field(v) for v in value) if value else NA_FIELD
     )
 
 
 def validate_path(file_path: str) -> str:
-    """Returns the name of a specific file"""
-
+    """Returns the name of a specific file."""
     return Path(file_path).name if file_path and Path(file_path).is_file() else NA_FIELD
 
 
 def validate_gender(value: str) -> str:
-    """Formats the provided gender"""
-
+    """Formats the provided gender."""
     return validate_empty_field(REPORT_GENDER.get(value))
 
 
 def validate_rml_sample(prep_category: str) -> str:
-    """Checks if a specific sample is a RML one"""
-
+    """Checks if a specific sample is a RML one."""
     if prep_category == OrderType.RML:
         LOG.error("The delivery report generation does not support RML samples")
         raise ValueError
-
     return validate_empty_field(prep_category)
 
 
 def validate_balsamic_analysis_type(value: str) -> str:
-    """Translates the BALSAMIC analysis type string to an accepted value for the delivery report"""
-
+    """Translates the BALSAMIC analysis type string to an accepted value for the delivery report."""
     return validate_empty_field(BALSAMIC_ANALYSIS_TYPE.get(value))
 
 
 def validate_supported_pipeline(cls, values: dict) -> dict:
-    """Validates if the report generation supports a specific pipeline and analysis type"""
-
+    """Validates if the report generation supports a specific pipeline and analysis type."""
     if values and values.get("pipeline") and values.get("customer_pipeline"):
         # Checks that the requested analysis and the executed one match
         if values.get("pipeline") != values.get("customer_pipeline"):
             LOG.error(
                 f"The analysis requested by the customer ({values.get('customer_pipeline')}) does not match the one "
                 f"executed ({values.get('pipeline')})"
             )
             raise ValueError
-
         # Check that the generation of the report supports the data analysis executed on the case
         if values.get("pipeline") not in REPORT_SUPPORTED_PIPELINES:
             LOG.error(
                 f"The pipeline {values.get('pipeline')} does not support delivery report generation"
             )
             raise ValueError
-
     # Validates the analysis type
     if Pipeline.BALSAMIC in values.get("pipeline"):
         values["type"] = validate_balsamic_analysis_type(values["type"])
-
     return values
```

### Comparing `cg-33.0.4/cg/models/rnafusion/rnafusion_sample.py` & `cg-33.0.5/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/scout/scout_load_config.py` & `cg-33.0.5/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/slurm/sbatch.py` & `cg-33.0.5/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/models/workflow/mutant.py` & `cg-33.0.5/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/resources/20181012_Indices.csv` & `cg-33.0.5/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/resources/rnafusion_bundle_filenames.csv` & `cg-33.0.5/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/admin.py` & `cg-33.0.5/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/api.py` & `cg-33.0.5/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/app.py` & `cg-33.0.5/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/config.py` & `cg-33.0.5/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/ext.py` & `cg-33.0.5/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/invoices/templates/invoices/index.html` & `cg-33.0.5/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/invoices/templates/invoices/invoice.html` & `cg-33.0.5/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/invoices/templates/invoices/layout.html` & `cg-33.0.5/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/invoices/templates/invoices/new.html` & `cg-33.0.5/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/server/invoices/views.py` & `cg-33.0.5/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/api/add.py` & `cg-33.0.5/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/api/base.py` & `cg-33.0.5/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/api/core.py` & `cg-33.0.5/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/api/delete.py` & `cg-33.0.5/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/api/find_basic_data.py` & `cg-33.0.5/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/api/find_business_data.py` & `cg-33.0.5/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/api/status.py` & `cg-33.0.5/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_analysis_filters.py` & `cg-33.0.5/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_application_filters.py` & `cg-33.0.5/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_application_version_filters.py` & `cg-33.0.5/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_bed_filters.py` & `cg-33.0.5/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_bed_version_filters.py` & `cg-33.0.5/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_case_filters.py` & `cg-33.0.5/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_case_sample_filters.py` & `cg-33.0.5/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_collaboration_filters.py` & `cg-33.0.5/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_customer_filters.py` & `cg-33.0.5/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_flow_cell_filters.py` & `cg-33.0.5/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_invoice_filters.py` & `cg-33.0.5/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_organism_filters.py` & `cg-33.0.5/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_panel_filters.py` & `cg-33.0.5/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_pool_filters.py` & `cg-33.0.5/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_sample_filters.py` & `cg-33.0.5/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/filters/status_user_filters.py` & `cg-33.0.5/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/store/models.py` & `cg-33.0.5/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/checksum/checksum.py` & `cg-33.0.5/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/click/EnumChoice.py` & `cg-33.0.5/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/commands.py` & `cg-33.0.5/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/date.py` & `cg-33.0.5/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/dict.py` & `cg-33.0.5/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/dispatcher.py` & `cg-33.0.5/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/email.py` & `cg-33.0.5/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/flask/enum.py` & `cg-33.0.5/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg/utils/utils.py` & `cg-33.0.5/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/cg.egg-info/PKG-INFO` & `cg-33.0.5/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 33.0.4
+Version: 33.0.5
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-33.0.4/cg.egg-info/SOURCES.txt` & `cg-33.0.5/cg.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
 cg/meta/orders/ticket_handler.py
 cg/meta/report/__init__.py
 cg/meta/report/balsamic.py
 cg/meta/report/balsamic_umi.py
 cg/meta/report/field_validators.py
 cg/meta/report/mip_dna.py
 cg/meta/report/report_api.py
+cg/meta/report/rnafusion.py
 cg/meta/report/templates/balsamic_report.html
 cg/meta/report/templates/bootstrap.html
 cg/meta/report/templates/mip-dna_report.html
 cg/meta/rsync/__init__.py
 cg/meta/rsync/rsync_api.py
 cg/meta/rsync/sbatch.py
 cg/meta/tar/__init__.py
@@ -397,14 +398,16 @@
 cg/models/orders/samples.py
 cg/models/report/__init__.py
 cg/models/report/metadata.py
 cg/models/report/report.py
 cg/models/report/sample.py
 cg/models/report/validators.py
 cg/models/rnafusion/__init__.py
+cg/models/rnafusion/analysis.py
+cg/models/rnafusion/metrics.py
 cg/models/rnafusion/rnafusion_sample.py
 cg/models/scout/__init__.py
 cg/models/scout/scout_load_config.py
 cg/models/slurm/__init__.py
 cg/models/slurm/sbatch.py
 cg/models/taxprofiler/__init__.py
 cg/models/workflow/__init__.py
@@ -648,15 +651,14 @@
 tests/cli/workflow/mip/test_cli_mip_dna_panel.py
 tests/cli/workflow/mip/test_cli_mip_dna_run.py
 tests/cli/workflow/mip/test_cli_mip_dna_start.py
 tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
 tests/cli/workflow/mip/test_cli_mip_rna_link.py
 tests/cli/workflow/mip/test_cli_mip_rna_run.py
 tests/cli/workflow/mip/test_cli_mip_store.py
-tests/cli/workflow/rnafusion/conftest.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
 tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
 tests/cli/workflow/taxprofiler/conftest.py
@@ -862,14 +864,15 @@
 tests/meta/report/__init__.py
 tests/meta/report/conftest.py
 tests/meta/report/helper.py
 tests/meta/report/test_balsamic_api.py
 tests/meta/report/test_field_validators.py
 tests/meta/report/test_mip_dna_api.py
 tests/meta/report/test_report_api.py
+tests/meta/report/test_rnafusion_api.py
 tests/meta/rsync/__init__.py
 tests/meta/rsync/conftest.py
 tests/meta/rsync/test_rsync.py
 tests/meta/transfer/conftest.py
 tests/meta/transfer/test_external_data.py
 tests/meta/transfer/test_meta_transfer_flowcell.py
 tests/meta/transfer/test_meta_transfer_lims.py
@@ -899,14 +902,15 @@
 tests/meta/upload/vogue/test_upload_vogue.py
 tests/meta/workflow/__init__.py
 tests/meta/workflow/conftest.py
 tests/meta/workflow/test_analysis.py
 tests/meta/workflow/test_balsamic.py
 tests/meta/workflow/test_microsalt.py
 tests/meta/workflow/test_prepare_fastq_api.py
+tests/meta/workflow/test_rnafusion.py
 tests/mocks/__init__.py
 tests/mocks/balsamic_analysis_mock.py
 tests/mocks/crunchy.py
 tests/mocks/hk_mock.py
 tests/mocks/limsmock.py
 tests/mocks/madeline.py
 tests/mocks/mip_analysis_mock.py
```

### Comparing `cg-33.0.4/requirements.txt` & `cg-33.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/setup.py` & `cg-33.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="33.0.4",
+    version="33.0.5",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-33.0.4/tests/apps/cgstats/conftest.py` & `cg-33.0.5/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-33.0.5/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/cgstats/crud/test_delete.py` & `cg-33.0.5/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-33.0.5/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-33.0.5/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/cgstats/parsers/test_run_info.py` & `cg-33.0.5/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/cgstats/test_cgstats_create.py` & `cg-33.0.5/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/cgstats/test_stats.py` & `cg-33.0.5/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/conftest.py` & `cg-33.0.5/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/coverage/test_coverage.py` & `cg-33.0.5/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/crunchy/conftest.py` & `cg-33.0.5/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/crunchy/test_compress_fastq.py` & `cg-33.0.5/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/crunchy/test_config.py` & `cg-33.0.5/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/crunchy/test_crunchy.py` & `cg-33.0.5/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/crunchy/test_spring_decompression.py` & `cg-33.0.5/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/demultiplex/conftest.py` & `cg-33.0.5/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-33.0.5/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-33.0.5/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/demultiplex/test_sample_sheet.py` & `cg-33.0.5/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/demultiplex/test_validate_sample_sheet.py` & `cg-33.0.5/tests/apps/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/gens/test_gens_api.py` & `cg-33.0.5/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/gt/conftest.py` & `cg-33.0.5/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/gt/test_gt_api.py` & `cg-33.0.5/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/hk/conftest.py` & `cg-33.0.5/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/hk/test__getattr__.py` & `cg-33.0.5/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/hk/test_add_file.py` & `cg-33.0.5/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/hk/test_bundles.py` & `cg-33.0.5/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/hk/test_core.py` & `cg-33.0.5/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/hk/test_file.py` & `cg-33.0.5/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/hk/test_version.py` & `cg-33.0.5/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/lims/conftest.py` & `cg-33.0.5/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/lims/test_api.py` & `cg-33.0.5/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/lims/test_sample_sheet.py` & `cg-33.0.5/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/loqus/conftest.py` & `cg-33.0.5/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/loqus/test_loqusdb_api.py` & `cg-33.0.5/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/madeline/conftest.py` & `cg-33.0.5/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/madeline/test_madeline.py` & `cg-33.0.5/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/mip/conftest.py` & `cg-33.0.5/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/mip/test_config_mip.py` & `cg-33.0.5/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/mutacc_auto/conftest.py` & `cg-33.0.5/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-33.0.5/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/orderform/conftest.py` & `cg-33.0.5/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-33.0.5/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/orderform/test_excel_sample_schema.py` & `cg-33.0.5/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/orderform/test_json_orderform_parser.py` & `cg-33.0.5/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/orderform/test_orderform_parser.py` & `cg-33.0.5/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/scout/conftest.py` & `cg-33.0.5/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/scout/test_get_causative_variants.py` & `cg-33.0.5/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/scout/test_get_scout_cases.py` & `cg-33.0.5/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/scout/test_scout_load_config.py` & `cg-33.0.5/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/scout/test_scout_models.py` & `cg-33.0.5/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-33.0.5/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-33.0.5/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-33.0.5/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/slurm/conftest.py` & `cg-33.0.5/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/slurm/test_slurm_api.py` & `cg-33.0.5/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/test_apps_environ.py` & `cg-33.0.5/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/test_osticket.py` & `cg-33.0.5/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/vogue/conftest.py` & `cg-33.0.5/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/apps/vogue/test_vogue_api.py` & `cg-33.0.5/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/add/test_cli_add.py` & `cg-33.0.5/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/add/test_cli_add_customer.py` & `cg-33.0.5/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/add/test_cli_add_family.py` & `cg-33.0.5/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/add/test_cli_add_relationship.py` & `cg-33.0.5/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/add/test_cli_add_sample.py` & `cg-33.0.5/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/backup/conftest.py` & `cg-33.0.5/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/backup/test_backup_command.py` & `cg-33.0.5/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/clean/conftest.py` & `cg-33.0.5/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/clean/test_balsamic_clean.py` & `cg-33.0.5/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-33.0.5/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/clean/test_hk_bundle_files.py` & `cg-33.0.5/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-33.0.5/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/clean/test_microbial_clean.py` & `cg-33.0.5/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-33.0.5/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/compress/conftest.py` & `cg-33.0.5/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/compress/test_cli_compress_fastq.py` & `cg-33.0.5/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/compress/test_cli_decompress_spring.py` & `cg-33.0.5/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/compress/test_compress_helpers.py` & `cg-33.0.5/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/compress/test_store_fastq.py` & `cg-33.0.5/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/conftest.py` & `cg-33.0.5/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/delete/test_cli_delete_case.py` & `cg-33.0.5/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/delete/test_cli_delete_cases.py` & `cg-33.0.5/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/deliver/conftest.py` & `cg-33.0.5/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/deliver/test_deliver_base.py` & `cg-33.0.5/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/deliver/test_rsync_base.py` & `cg-33.0.5/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-33.0.5/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/demultiplex/conftest.py` & `cg-33.0.5/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/demultiplex/test_add_flowcell.py` & `cg-33.0.5/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-33.0.5/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-33.0.5/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/demultiplex/test_finish_demux.py` & `cg-33.0.5/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/demultiplex/test_stats_command.py` & `cg-33.0.5/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-33.0.5/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/generate/report/conftest.py` & `cg-33.0.5/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-33.0.5/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/generate/report/test_utils.py` & `cg-33.0.5/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/generate/test_cli_base.py` & `cg-33.0.5/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/get/test_cli_get.py` & `cg-33.0.5/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/get/test_cli_get_analysis.py` & `cg-33.0.5/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/get/test_cli_get_case.py` & `cg-33.0.5/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/get/test_cli_get_flow_cell.py` & `cg-33.0.5/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/get/test_cli_get_sample.py` & `cg-33.0.5/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/set/conftest.py` & `cg-33.0.5/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/set/test_cli_set_case.py` & `cg-33.0.5/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/set/test_cli_set_cases.py` & `cg-33.0.5/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/set/test_cli_set_flowcell.py` & `cg-33.0.5/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/set/test_cli_set_list_keys.py` & `cg-33.0.5/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/set/test_cli_set_sample.py` & `cg-33.0.5/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/set/test_cli_set_samples.py` & `cg-33.0.5/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/store/test_fastq.py` & `cg-33.0.5/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/test_base.py` & `cg-33.0.5/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/test_clean.py` & `cg-33.0.5/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/conftest.py` & `cg-33.0.5/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_scout.py` & `cg-33.0.5/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_auto.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_fastq.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_genotype.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_gens.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_nipt.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_observations.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/upload/test_cli_upload_vogue.py` & `cg-33.0.5/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/balsamic/conftest.py` & `cg-33.0.5/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-33.0.5/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-33.0.5/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/balsamic/test_link.py` & `cg-33.0.5/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-33.0.5/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/balsamic/test_run.py` & `cg-33.0.5/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-33.0.5/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/conftest.py` & `cg-33.0.5/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-33.0.5/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/fluffy/conftest.py` & `cg-33.0.5/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-33.0.5/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-33.0.5/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-33.0.5/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-33.0.5/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-33.0.5/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/microsalt/conftest.py` & `cg-33.0.5/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-33.0.5/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-33.0.5/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-33.0.5/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/conftest.py` & `cg-33.0.5/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-33.0.5/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-33.0.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-33.0.5/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/test_cli_workflow.py` & `cg-33.0.5/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-33.0.5/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/conftest.py` & `cg-33.0.5/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """Conftest file for pytest fixtures that needs to be shared for multiple tests."""
 import copy
+import gzip
 import http
 import logging
 import os
 import shutil
 from datetime import MAXYEAR, datetime, timedelta
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Tuple
 
 import pytest
+from cg.meta.workflow.rnafusion import RnafusionAnalysisAPI
 from housekeeper.store.models import File, Version
 from requests import Response
 
 from cg.apps.gens import GensAPI
 from cg.apps.gt import GenotypeAPI
 from cg.apps.hermes.hermes_api import HermesApi
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import FileExtensions, Pipeline
 from cg.constants.constants import CaseActions, FileFormat
 from cg.constants.demultiplexing import BclConverter, DemultiplexingDirsAndFiles
 from cg.constants.priority import SlurmQos
 from cg.constants.subject import Gender
-from cg.io.controller import ReadFile
+from cg.io.controller import ReadFile, WriteFile
+from cg.io.json import write_json, read_json
 from cg.meta.rsync import RsyncAPI
 from cg.meta.transfer.external_data import ExternalDataAPI
 from cg.models import CompressionData
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.demux_results import DemuxResults
 from cg.models.demultiplex.flow_cell import FlowCell
 from cg.store import Store
-from cg.store.models import Bed, BedVersion, Customer, Organism
+from cg.store.models import Bed, BedVersion, Customer, Organism, Family, Sample
 from tests.mocks.crunchy import MockCrunchyAPI
 from tests.mocks.hk_mock import MockHousekeeperAPI
 from tests.mocks.limsmock import MockLimsAPI
 from tests.mocks.madeline import MockMadelineAPI
 from tests.mocks.osticket import MockOsTicket
 from tests.mocks.process_mock import ProcessMock
 from tests.mocks.scout import MockScoutAPI
@@ -1917,7 +1920,237 @@
             case_id=case_id,
             data_analysis=pipeline.value,
             action=action.value,
             customer=customer,
         )
     store.session.commit()
     yield store
+
+
+# Rnafusion fixtures
+
+
+@pytest.fixture(name="rnafusion_dir")
+def fixture_rnafusion_dir(tmpdir_factory, apps_dir: Path) -> str:
+    """Return the path to the rnafusion apps dir."""
+    rnafusion_dir = tmpdir_factory.mktemp("rnafusion")
+    return Path(rnafusion_dir).absolute().as_posix()
+
+
+@pytest.fixture(name="rnafusion_case_id")
+def fixture_rnafusion_case_id() -> str:
+    """Returns a rnafusion case id."""
+    return "rnafusion_case_enough_reads"
+
+
+@pytest.fixture(name="no_sample_case_id")
+def fixture_no_sample_case_id() -> str:
+    """Returns a case id of a case with no samples."""
+    return "no_sample_case"
+
+
+@pytest.fixture(name="rnafusion_sample_id")
+def fixture_rnafusion_sample_id() -> str:
+    """Returns a rnafusion sample id."""
+    return "sample_rnafusion_case_enough_reads"
+
+
+@pytest.fixture(name="rnafusion_housekeeper_dir")
+def fixture_rnafusion_housekeeper_dir(tmpdir_factory, rnafusion_dir: Path) -> Path:
+    """Return the path to the rnafusion housekeeper bundle dir."""
+    return tmpdir_factory.mktemp("bundles")
+
+
+@pytest.fixture(name="rnafusion_fastq_file_l_1_r_1")
+def fixture_rnafusion_fastq_file_l_1_r_1(rnafusion_housekeeper_dir: Path) -> str:
+    fastq_filename = Path(
+        rnafusion_housekeeper_dir, "XXXXXXXXX_000000_S000_L001_R1_001.fastq.gz"
+    ).as_posix()
+    with gzip.open(fastq_filename, "wb") as wh:
+        wh.write(b"@A00689:73:XXXXXXXXX:1:1101:4806:1047 1:N:0:TCCTGGAACA+ACAACCAGTA")
+    return fastq_filename
+
+
+@pytest.fixture(name="rnafusion_fastq_file_l_1_r_2")
+def fixture_rnafusion_fastq_file_l_1_r_2(rnafusion_housekeeper_dir: Path) -> str:
+    fastq_filename = Path(
+        rnafusion_housekeeper_dir, "XXXXXXXXX_000000_S000_L001_R2_001.fastq.gz"
+    ).as_posix()
+    with gzip.open(fastq_filename, "wb") as wh:
+        wh.write(b"@A00689:73:XXXXXXXXX:1:1101:4806:1047 2:N:0:TCCTGGAACA+ACAACCAGTA")
+    return fastq_filename
+
+
+@pytest.fixture(name="rnafusion_mock_fastq_files")
+def fixture_rnafusion_mock_fastq_files(
+    rnafusion_fastq_file_l_1_r_1: Path, rnafusion_fastq_file_l_1_r_2: Path
+) -> List[Path]:
+    """Return list of all mock fastq files to commit to mock housekeeper"""
+    return [rnafusion_fastq_file_l_1_r_1, rnafusion_fastq_file_l_1_r_2]
+
+
+@pytest.fixture(scope="function", name="rnafusion_housekeeper")
+def fixture_rnafusion_housekeeper(
+    housekeeper_api: HousekeeperAPI,
+    helpers: StoreHelpers,
+    rnafusion_mock_fastq_files: List[Path],
+    rnafusion_sample_id: str,
+):
+    """Create populated housekeeper that holds files for all mock samples."""
+
+    bundle_data = {
+        "name": rnafusion_sample_id,
+        "created": datetime.now(),
+        "version": "1.0",
+        "files": [
+            {"path": f, "tags": ["fastq"], "archive": False} for f in rnafusion_mock_fastq_files
+        ],
+    }
+    helpers.ensure_hk_bundle(store=housekeeper_api, bundle_data=bundle_data)
+    return housekeeper_api
+
+
+@pytest.fixture(scope="function", name="rnafusion_context")
+def fixture_rnafusion_context(
+    cg_context: CGConfig,
+    helpers: StoreHelpers,
+    rnafusion_housekeeper: HousekeeperAPI,
+    trailblazer_api: MockTB,
+    hermes_api: HermesApi,
+    cg_dir: Path,
+    rnafusion_case_id: str,
+    rnafusion_sample_id: str,
+    no_sample_case_id: str,
+) -> CGConfig:
+    """context to use in cli"""
+    cg_context.housekeeper_api_ = rnafusion_housekeeper
+    cg_context.trailblazer_api_ = trailblazer_api
+    cg_context.meta_apis["analysis_api"] = RnafusionAnalysisAPI(config=cg_context)
+    status_db: Store = cg_context.status_db
+
+    # Create ERROR case with NO SAMPLES
+    helpers.add_case(status_db, internal_id=no_sample_case_id, name=no_sample_case_id)
+
+    # Create textbook case with enough reads
+    case_enough_reads: Family = helpers.add_case(
+        store=status_db,
+        internal_id=rnafusion_case_id,
+        name=rnafusion_case_id,
+        data_analysis=Pipeline.RNAFUSION,
+    )
+
+    sample_rnafusion_case_enough_reads: Sample = helpers.add_sample(
+        status_db,
+        internal_id=rnafusion_sample_id,
+        sequenced_at=datetime.now(),
+    )
+
+    helpers.add_relationship(
+        status_db,
+        case=case_enough_reads,
+        sample=sample_rnafusion_case_enough_reads,
+    )
+    return cg_context
+
+
+@pytest.fixture(name="deliverable_data")
+def fixture_deliverables_data(
+    rnafusion_dir: Path, rnafusion_case_id: str, rnafusion_sample_id: str
+) -> dict:
+    return {
+        "files": [
+            {
+                "path": f"{rnafusion_dir}/{rnafusion_case_id}/multiqc/multiqc_report.html",
+                "path_index": "",
+                "step": "report",
+                "tag": ["multiqc-html", "rna"],
+                "id": rnafusion_case_id,
+                "format": "html",
+                "mandatory": True,
+            },
+        ]
+    }
+
+
+@pytest.fixture
+def mock_deliverable(rnafusion_dir: Path, deliverable_data: dict, rnafusion_case_id: str) -> None:
+    """Create deliverable file with dummy data and files to deliver."""
+    Path.mkdir(
+        Path(rnafusion_dir, rnafusion_case_id),
+        parents=True,
+        exist_ok=True,
+    )
+    Path.mkdir(
+        Path(rnafusion_dir, rnafusion_case_id, "multiqc"),
+        parents=True,
+        exist_ok=True,
+    )
+    for report_entry in deliverable_data["files"]:
+        Path(report_entry["path"]).touch(exist_ok=True)
+    WriteFile.write_file_from_content(
+        content=deliverable_data,
+        file_format=FileFormat.JSON,
+        file_path=Path(rnafusion_dir, rnafusion_case_id, rnafusion_case_id + "_deliverables.yaml"),
+    )
+
+
+@pytest.fixture(name="hermes_deliverables")
+def fixture_hermes_deliverables(deliverable_data: dict, rnafusion_case_id: str) -> dict:
+    hermes_output: dict = {"pipeline": "rnafusion", "bundle_id": rnafusion_case_id, "files": []}
+    for file_info in deliverable_data["files"]:
+        tags: List[str] = []
+        if "html" in file_info["format"]:
+            tags.append("multiqc-html")
+        hermes_output["files"].append({"path": file_info["path"], "tags": tags, "mandatory": True})
+    return hermes_output
+
+
+@pytest.fixture(name="malformed_hermes_deliverables")
+def fixture_malformed_hermes_deliverables(hermes_deliverables: dict) -> dict:
+    malformed_deliverable: dict = hermes_deliverables.copy()
+    malformed_deliverable.pop("pipeline")
+
+    return malformed_deliverable
+
+
+@pytest.fixture(name="rnafusion_multiqc_json_metrics")
+def fixture_rnafusion_multiqc_json_metrics(rnafusion_analysis_dir) -> dict:
+    """Returns a the content of a mock multiqc json file."""
+    return read_json(file_path=Path(rnafusion_analysis_dir, "multiqc_data.json"))
+
+
+@pytest.fixture
+def mock_analysis_finish(
+    rnafusion_dir: Path, rnafusion_case_id: str, rnafusion_multiqc_json_metrics: dict
+) -> None:
+    """Create analysis_finish file for testing."""
+    Path.mkdir(Path(rnafusion_dir, rnafusion_case_id, "pipeline_info"), parents=True, exist_ok=True)
+    Path(rnafusion_dir, rnafusion_case_id, "pipeline_info", "software_versions.yml").touch(
+        exist_ok=True
+    )
+    Path(rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_samplesheet.csv").touch(
+        exist_ok=True
+    )
+    Path.mkdir(
+        Path(rnafusion_dir, rnafusion_case_id, "multiqc", "multiqc_data"),
+        parents=True,
+        exist_ok=True,
+    )
+    write_json(
+        content=rnafusion_multiqc_json_metrics,
+        file_path=Path(
+            rnafusion_dir,
+            rnafusion_case_id,
+            "multiqc",
+            "multiqc_data",
+            "multiqc_data.json",
+        ),
+    )
+
+
+@pytest.fixture
+def mock_config(rnafusion_dir: Path, rnafusion_case_id: str) -> None:
+    """Create samplesheet.csv file for testing"""
+    Path.mkdir(Path(rnafusion_dir, rnafusion_case_id), parents=True, exist_ok=True)
+    Path(rnafusion_dir, rnafusion_case_id, f"{rnafusion_case_id}_samplesheet.csv").touch(
+        exist_ok=True
+    )
```

### Comparing `cg-33.0.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-33.0.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-33.0.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-33.0.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-33.0.5/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/analysis/sample_coverage.bed` & `cg-33.0.5/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/balsamic/case/config.json` & `cg-33.0.5/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-33.0.5/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-33.0.5/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-33.0.5/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-33.0.5/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-33.0.5/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-33.0.5/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/madeline/madeline.xml` & `cg-33.0.5/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-33.0.5/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-33.0.5/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/scout/643594.config.yaml` & `cg-33.0.5/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/scout/case_export.json` & `cg-33.0.5/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/scout/export_causatives.json` & `cg-33.0.5/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/scout/none_case_export.json` & `cg-33.0.5/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/scout/other_sex_case.json` & `cg-33.0.5/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/scout/panel_export.bed` & `cg-33.0.5/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/scout/panel_export.csv` & `cg-33.0.5/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv` & `cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv` & `cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv` & `cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml` & `cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv` & `cg-33.0.5/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/balsamic.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/fastq.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/metagenome.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/microsalt.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/mip.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/rml.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-33.0.5/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/data/SampleSheet.csv` & `cg-33.0.5/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/data/cgfixture.db` & `cg-33.0.5/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/data/hkstore.db` & `cg-33.0.5/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/io/example_json.json` & `cg-33.0.5/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-33.0.5/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/NIPT-json.json` & `cg-33.0.5/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-33.0.5/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-33.0.5/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/report/case_data.json` & `cg-33.0.5/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/report/lims_exported_samples.json` & `cg-33.0.5/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/fixtures/report/lims_family.json` & `cg-33.0.5/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/io/conftest.py` & `cg-33.0.5/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/io/test_io_controller.py` & `cg-33.0.5/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/io/test_io_csv.py` & `cg-33.0.5/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/io/test_io_json.py` & `cg-33.0.5/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/io/test_io_xml.py` & `cg-33.0.5/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/io/test_io_yaml.py` & `cg-33.0.5/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/io/test_validate_path.py` & `cg-33.0.5/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/archive/conftest.py` & `cg-33.0.5/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/archive/test_archiving.py` & `cg-33.0.5/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/backup/conftest.py` & `cg-33.0.5/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/backup/test_meta_backup.py` & `cg-33.0.5/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/backup/test_meta_pdc.py` & `cg-33.0.5/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/clean/conftest.py` & `cg-33.0.5/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-33.0.5/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-33.0.5/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/compress/conftest.py` & `cg-33.0.5/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/compress/test_clean_fastq.py` & `cg-33.0.5/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/compress/test_compress_files.py` & `cg-33.0.5/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/compress/test_compress_meta_fastq.py` & `cg-33.0.5/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/compress/test_decompress_spring_meta.py` & `cg-33.0.5/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-33.0.5/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/conftest.py` & `cg-33.0.5/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/deliver/conftest.py` & `cg-33.0.5/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/deliver/test_deliver_ticket.py` & `cg-33.0.5/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/deliver/test_delivery_api.py` & `cg-33.0.5/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/demultiplex/conftest.py` & `cg-33.0.5/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-33.0.5/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-33.0.5/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/demultiplex/test_rename_files.py` & `cg-33.0.5/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/encryption/conftest.py` & `cg-33.0.5/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/encryption/test_encryption.py` & `cg-33.0.5/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/observations/conftest.py` & `cg-33.0.5/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/observations/test_meta_upload_observations.py` & `cg-33.0.5/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/conftest.py` & `cg-33.0.5/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-33.0.5/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-33.0.5/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-33.0.5/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-33.0.5/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_meta_orders_api.py` & `cg-33.0.5/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_meta_orders_lims.py` & `cg-33.0.5/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_meta_orders_status.py` & `cg-33.0.5/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/orders/test_ticket_handler.py` & `cg-33.0.5/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/report/conftest.py` & `cg-33.0.5/tests/meta/report/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from pathlib import Path
 
 from datetime import datetime, timedelta
-from typing import List
+from typing import List, Dict
 
 import pytest
+from cg.store import Store
+
+from cg.meta.report.rnafusion import RnafusionReportAPI
 from cgmodels.cg.constants import Pipeline
 
 from cg.constants.constants import FileFormat
 from cg.io.controller import ReadFile
 from cg.meta.report.balsamic import BalsamicReportAPI
 from cg.meta.report.mip_dna import MipDNAReportAPI
 from cg.models.cg_config import CGConfig
@@ -16,93 +19,121 @@
 from tests.mocks.balsamic_analysis_mock import MockBalsamicAnalysis
 from tests.mocks.limsmock import MockLimsAPI
 from tests.mocks.mip_analysis_mock import MockMipAnalysis
 from tests.mocks.report import MockChanjo, MockHousekeeperMipDNAReportAPI
 
 
 @pytest.fixture(scope="function", name="report_api_mip_dna")
-def report_api_mip_dna(cg_context: CGConfig, lims_samples, report_store) -> MipDNAReportAPI:
+def report_api_mip_dna(
+    cg_context: CGConfig, lims_samples: List[dict], report_store: Store
+) -> MipDNAReportAPI:
     """MIP DNA ReportAPI fixture."""
-
     cg_context.meta_apis["analysis_api"] = MockMipAnalysis()
     cg_context.status_db_ = report_store
     cg_context.lims_api_ = MockLimsAPI(cg_context, lims_samples)
     cg_context.chanjo_api_ = MockChanjo()
     cg_context.scout_api_ = MockScoutApi(cg_context)
     return MockHousekeeperMipDNAReportAPI(cg_context, cg_context.meta_apis["analysis_api"])
 
 
 @pytest.fixture(scope="function", name="report_api_balsamic")
-def report_api_balsamic(cg_context: CGConfig, lims_samples, report_store) -> BalsamicReportAPI:
+def report_api_balsamic(
+    cg_context: CGConfig, lims_samples: List[dict], report_store: Store
+) -> BalsamicReportAPI:
     """BALSAMIC ReportAPI fixture."""
-
     cg_context.meta_apis["analysis_api"] = MockBalsamicAnalysis(cg_context)
     cg_context.status_db_ = report_store
     cg_context.lims_api_ = MockLimsAPI(cg_context, lims_samples)
     cg_context.scout_api_ = MockScoutApi(cg_context)
     return BalsamicReportAPI(cg_context, cg_context.meta_apis["analysis_api"])
 
 
+@pytest.fixture(scope="function", name="report_api_rnafusion")
+def report_api_rnafusion(
+    rnafusion_context: CGConfig, lims_samples: List[dict]
+) -> RnafusionReportAPI:
+    """Rnafusion report API fixture."""
+    rnafusion_context.lims_api_ = MockLimsAPI(rnafusion_context, lims_samples)
+    rnafusion_context.scout_api_ = MockScoutApi(rnafusion_context)
+    return RnafusionReportAPI(rnafusion_context, rnafusion_context.meta_apis["analysis_api"])
+
+
 @pytest.fixture(scope="function", name="case_mip_dna")
-def case_mip_dna(case_id, report_api_mip_dna) -> Family:
+def case_mip_dna(case_id: str, report_api_mip_dna: MipDNAReportAPI) -> Family:
     """MIP DNA case instance."""
-
     return report_api_mip_dna.status_db.get_case_by_internal_id(internal_id=case_id)
 
 
 @pytest.fixture(scope="function", name="case_balsamic")
-def case_balsamic(case_id, report_api_balsamic) -> Family:
+def case_balsamic(case_id: str, report_api_balsamic: BalsamicReportAPI) -> Family:
     """BALSAMIC case instance."""
-
     return report_api_balsamic.status_db.get_case_by_internal_id(internal_id=case_id)
 
 
 @pytest.fixture(scope="function", name="case_samples_data")
-def case_samples_data(case_id, report_api_mip_dna):
+def case_samples_data(case_id: str, report_api_mip_dna: MipDNAReportAPI):
     """MIP DNA family sample object."""
-
     return report_api_mip_dna.status_db.get_case_samples_by_case_id(case_internal_id=case_id)
 
 
-@pytest.fixture(name="mip_analysis_api")
+@pytest.fixture(scope="function", name="mip_analysis_api")
 def mip_analysis_api() -> MockMipAnalysis:
     """MIP analysis mock data."""
-
     return MockMipAnalysis()
 
 
-@pytest.fixture(name="lims_family")
+@pytest.fixture(scope="session", name="lims_family")
 def fixture_lims_family(fixtures_dir: Path) -> dict:
     """Returns a lims-like case of samples."""
     return ReadFile.get_content_from_file(
         file_format=FileFormat.JSON, file_path=Path(fixtures_dir, "report", "lims_family.json")
     )
 
 
-@pytest.fixture(name="lims_samples")
+@pytest.fixture(scope="session", name="lims_samples")
 def fixture_lims_samples(lims_family: dict) -> List[dict]:
     """Returns the samples of a lims case."""
-
     return lims_family["samples"]
 
 
 @pytest.fixture(scope="function", autouse=True, name="report_store")
 def report_store(analysis_store, helpers, timestamp_yesterday):
     """A mock store instance for report testing."""
-
     case = analysis_store.get_cases()[0]
     helpers.add_analysis(
         analysis_store, case, pipeline=Pipeline.MIP_DNA, started_at=timestamp_yesterday
     )
     helpers.add_analysis(analysis_store, case, pipeline=Pipeline.MIP_DNA, started_at=datetime.now())
-
     # Mock sample dates to calculate processing times
     for family_sample in analysis_store.get_case_samples_by_case_id(
         case_internal_id=case.internal_id
     ):
         family_sample.sample.ordered_at = timestamp_yesterday - timedelta(days=2)
         family_sample.sample.received_at = timestamp_yesterday - timedelta(days=1)
         family_sample.sample.prepared_at = timestamp_yesterday
         family_sample.sample.sequenced_at = timestamp_yesterday
         family_sample.sample.delivered_at = datetime.now()
-
     return analysis_store
+
+
+@pytest.fixture(scope="session", name="rnafusion_validated_metrics")
+def fixture_rnafusion_validated_metrics() -> Dict[str, str]:
+    """Return Rnafusion raw analysis metrics dictionary."""
+    return {
+        "gc_content": "51.7",
+        "ribosomal_bases": "65.81",
+        "q20_rate": "97.48",
+        "q30_rate": "92.95",
+        "mapped_reads": "48.27",
+        "rin": "10.0",
+        "input_amount": "300.0",
+        "insert_size": "N/A",
+        "insert_size_peak": "N/A",
+        "mean_length_r1": "99.0",
+        "million_read_pairs": "75.0",
+        "bias_5_3": "1.07",
+        "pct_adapter": "12.01",
+        "duplicates": "14.86",
+        "mrna_bases": "85.97",
+        "pct_surviving": "99.42",
+        "uniquely_mapped_reads": "91.02",
+    }
```

### Comparing `cg-33.0.4/tests/meta/report/test_balsamic_api.py` & `cg-33.0.5/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/report/test_field_validators.py` & `cg-33.0.5/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/report/test_mip_dna_api.py` & `cg-33.0.5/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/report/test_report_api.py` & `cg-33.0.5/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/rsync/conftest.py` & `cg-33.0.5/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/rsync/test_rsync.py` & `cg-33.0.5/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/test_invoice.py` & `cg-33.0.5/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/transfer/conftest.py` & `cg-33.0.5/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/transfer/test_external_data.py` & `cg-33.0.5/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-33.0.5/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-33.0.5/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/balsamic/test_balsamic.py` & `cg-33.0.5/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/conftest.py` & `cg-33.0.5/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-33.0.5/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/mutacc/conftest.py` & `cg-33.0.5/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-33.0.5/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/nipt/conftest.py` & `cg-33.0.5/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-33.0.5/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/scout/conftest.py` & `cg-33.0.5/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/scout/test_generate_load_config.py` & `cg-33.0.5/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-33.0.5/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-33.0.5/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-33.0.5/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/test_meta_upload_coverage.py` & `cg-33.0.5/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/test_upload_api.py` & `cg-33.0.5/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/test_upload_genotypes_api.py` & `cg-33.0.5/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/vogue/conftest.py` & `cg-33.0.5/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-33.0.5/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/workflow/conftest.py` & `cg-33.0.5/tests/meta/workflow/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Fixtures for the workflow tests."""
 import datetime
 from pathlib import Path
-from typing import List
+from typing import List, Dict
 
 import pytest
 from cgmodels.cg.constants import Pipeline
 
 from cg.constants.constants import MicrosaltAppTags, MicrosaltQC
 from cg.meta.workflow.microsalt import MicrosaltAnalysisAPI
 
@@ -202,7 +202,27 @@
     store.get_application_by_tag(
         tag=MicrosaltAppTags.MWXNXTR003
     ).target_reads = MicrosaltQC.TARGET_READS
 
     cg_context.meta_apis["analysis_api"] = analysis_api
 
     return cg_context
+
+
+@pytest.fixture(name="rnafusion_metrics")
+def fixture_rnafusion_metrics() -> Dict[str, float]:
+    """Return Rnafusion raw analysis metrics dictionary."""
+    return {
+        "after_filtering_gc_content": 0.516984,
+        "after_filtering_q20_rate": 0.974834,
+        "after_filtering_q30_rate": 0.929476,
+        "after_filtering_read1_mean_length": 99.0,
+        "before_filtering_total_reads": 149984042.0,
+        "bias_5_3": 1.07,
+        "pct_adapter": 12.005654574904709,
+        "pct_mrna_bases": 85.9731,
+        "pct_ribosomal_bases": 0.6581,
+        "pct_surviving": 99.42004630065911,
+        "pct_duplication": 14.8643,
+        "reads_aligned": 72391566.0,
+        "uniquely_mapped_percent": 91.02,
+    }
```

### Comparing `cg-33.0.4/tests/meta/workflow/test_analysis.py` & `cg-33.0.5/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/workflow/test_balsamic.py` & `cg-33.0.5/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/workflow/test_microsalt.py` & `cg-33.0.5/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-33.0.5/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/balsamic_analysis_mock.py` & `cg-33.0.5/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/crunchy.py` & `cg-33.0.5/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/hk_mock.py` & `cg-33.0.5/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/limsmock.py` & `cg-33.0.5/tests/mocks/limsmock.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,7 +107,15 @@
 
     def get_received_date(self, lims_id: str):
         received_date = None
         for sample in self._samples:
             if sample.internal_id == lims_id:
                 received_date = sample.received_at
         return received_date
+
+    def get_sample_rin(self, sample_id: str) -> float:
+        """Mock return sample RIN value."""
+        return 10.0
+
+    def get_latest_rna_input_amount(self, sample_id: str) -> float:
+        """Mock return input amount used in the latest preparation of an RNA sample."""
+        return 300.0
```

### Comparing `cg-33.0.4/tests/mocks/madeline.py` & `cg-33.0.5/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/mip_analysis_mock.py` & `cg-33.0.5/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/osticket.py` & `cg-33.0.5/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/process_mock.py` & `cg-33.0.5/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/report.py` & `cg-33.0.5/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/scout.py` & `cg-33.0.5/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/store_model.py` & `cg-33.0.5/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/mocks/tb_mock.py` & `cg-33.0.5/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/balsamic/conftest.py` & `cg-33.0.5/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/balsamic/test_balsamic_analysis.py` & `cg-33.0.5/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/conftest.py` & `cg-33.0.5/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/demultiplexing/conftest.py` & `cg-33.0.5/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/demultiplexing/test_demux_results.py` & `cg-33.0.5/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/demultiplexing/test_flowcell_model.py` & `cg-33.0.5/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/demultiplexing/test_run_parameters.py` & `cg-33.0.5/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/mip/conftest.py` & `cg-33.0.5/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/mip/test_mip_analysis.py` & `cg-33.0.5/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/mip/test_mip_config.py` & `cg-33.0.5/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-33.0.5/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/mip/test_mip_sample_info.py` & `cg-33.0.5/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/nextflow/conftest.py` & `cg-33.0.5/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/nextflow/test_nextflow_deliver.py` & `cg-33.0.5/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/observations/conftest.py` & `cg-33.0.5/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/observations/test_observations_input_files.py` & `cg-33.0.5/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/report/test_validators.py` & `cg-33.0.5/tests/models/report/test_validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-"""Tests delivery report models validators"""
+"""Tests delivery report models validators."""
 from cgmodels.cg.constants import Pipeline
 
 from cg.constants import NA_FIELD, YES_FIELD, REPORT_GENDER
 from cg.constants.subject import Gender
 from cg.models.orders.constants import OrderType
 from cg.models.report.validators import (
     validate_empty_field,
     validate_boolean,
     validate_float,
     validate_list,
     validate_rml_sample,
     validate_supported_pipeline,
     validate_gender,
+    validate_percentage,
 )
 
 
 def test_validate_empty_field():
-    """Tests formatting an empty value"""
+    """Tests formatting an empty value."""
 
     # GIVEN a not valid empty field
     none_field = None
 
     # WHEN performing the validation
     output = validate_empty_field(none_field)
 
     # THEN check if the input value was formatted correctly
     assert output == NA_FIELD
 
 
 def test_validate_boolean():
-    """Tests boolean formatting for the delivery report"""
+    """Tests boolean formatting for the delivery report."""
 
     # GIVEN a not formatted inputs
     none_field = None
     true_field = True
     not_bool_field = "not a boolean"
 
     # WHEN performing the validation
@@ -44,15 +45,15 @@
     # THEN check if the input values were formatted correctly
     assert validated_none_field == NA_FIELD
     assert validated_true_field == YES_FIELD
     assert validated_not_bool_field == NA_FIELD
 
 
 def test_validate_float():
-    """Tests the validation of a float value"""
+    """Tests the validation of a float value."""
 
     # GIVEN a valid float input (float and string format)
     float_value = 12.3456789
     str_value = "12.3456789"
 
     # WHEN performing the validation
     validated_float_value = validate_float(float_value)
@@ -60,59 +61,72 @@
 
     # THEN check if the input values were formatted correctly
     assert validated_float_value == "12.35"
     assert validated_str_value == "12.35"
 
 
 def test_validate_float_zero_input():
-    """Tests the validation of a float value"""
+    """Tests the validation of a float value."""
 
     # GIVEN a valid float input (float and string format)
     float_value = 0.0
     str_value = "0.0"
 
     # WHEN performing the validation
     validated_float_value = validate_float(float_value)
     validated_str_value = validate_float(str_value)
 
     # THEN check if the input values were formatted correctly
     assert validated_float_value == "0.0"
     assert validated_str_value == "0.0"
 
 
+def test_validate_percentage():
+    """Tests the validation of a percentage value."""
+
+    # GIVEN a not formatted percentage
+    pct_value = 0.9876
+
+    # WHEN performing the validation
+    validated_pct_value = validate_percentage(pct_value)
+
+    # THEN check if the input values were formatted correctly
+    assert validated_pct_value == "98.76"
+
+
 def test_validate_list():
-    """Tests if a list is transformed into a string of comma separated values"""
+    """Tests if a list is transformed into a string of comma separated values."""
 
     # GIVEN a mock list
     mock_list = ["I'm", "a", "list"]
 
     # WHEN performing the validation
     validated_list = validate_list(mock_list)
 
     # THEN check if the input values were formatted correctly
     assert validated_list == "I'm, a, list"
 
 
 def test_validate_rml_sample(caplog):
-    """Performs validation on a preparation category"""
+    """Performs validation on a preparation category."""
 
     # GIVEN an invalid prep category
     prep_category = OrderType.RML
 
     # WHEN performing the validation
     try:
         validate_rml_sample(prep_category)
         assert False
     # THEN check if an exception was raised
     except ValueError:
         assert "The delivery report generation does not support RML samples" in caplog.text
 
 
 def test_validate_gender(caplog):
-    """Tests report gender parsing"""
+    """Tests report gender parsing."""
 
     # GIVEN an invalid gender category
     gender = Gender.FEMALE
     invalid_gender = "not_a_gender"
 
     # WHEN performing the validation
     validated_gender = validate_gender(gender)
@@ -120,15 +134,15 @@
 
     # THEN check if the gender has been correctly formatted
     assert validated_gender == REPORT_GENDER.get("female")
     assert validated_invalid_gender == NA_FIELD
 
 
 def test_validate_supported_pipeline_match_error(caplog):
-    """Tests if a customer requested pipeline matches the data analysis one"""
+    """Tests if a customer requested pipeline matches the data analysis one."""
 
     # GIVEN an input dictionary where the customers and executed pipeline are different
     dict_different_pipelines = {"customer_pipeline": Pipeline.MIP_DNA, "pipeline": Pipeline.FLUFFY}
 
     # WHEN performing the validation
     try:
         validate_supported_pipeline(None, dict_different_pipelines)
@@ -138,15 +152,15 @@
         assert (
             f"The analysis requested by the customer ({dict_different_pipelines.get('customer_pipeline')}) does not "
             f"match the one executed ({dict_different_pipelines.get('pipeline')})" in caplog.text
         )
 
 
 def test_validate_supported_pipeline(caplog):
-    """Tests that the analysis pipeline is supported by the delivery report workflow"""
+    """Tests that the analysis pipeline is supported by the delivery report workflow."""
 
     # GIVEN a dictionary with a not supported pipeline
     dict_invalid_pipeline = {"customer_pipeline": Pipeline.FLUFFY, "pipeline": Pipeline.FLUFFY}
 
     # WHEN performing the validation
     try:
         validate_supported_pipeline(None, dict_invalid_pipeline)
```

### Comparing `cg-33.0.4/tests/models/rnafusion/conftest.py` & `cg-33.0.5/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-33.0.5/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/test_cg_models.py` & `cg-33.0.5/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/test_compression_data.py` & `cg-33.0.5/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/test_file_data.py` & `cg-33.0.5/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/models/test_flowcell_class.py` & `cg-33.0.5/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/server/conftest.py` & `cg-33.0.5/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/add/test_store_add_application_version.py` & `cg-33.0.5/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/add/test_store_add_base.py` & `cg-33.0.5/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/add/test_store_add_customer.py` & `cg-33.0.5/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/add/test_store_add_flow_celll.py` & `cg-33.0.5/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/conftest.py` & `cg-33.0.5/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/delete/test_store_api_delete.py` & `cg-33.0.5/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/find/test_find_basic_data.py` & `cg-33.0.5/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-33.0.5/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/find/test_find_business_data.py` & `cg-33.0.5/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/find/test_find_business_data_analysis.py` & `cg-33.0.5/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/find/test_find_business_data_case.py` & `cg-33.0.5/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/find/test_find_business_data_sample.py` & `cg-33.0.5/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_analyses_to_clean.py` & `cg-33.0.5/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-33.0.5/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_store_api_status.py` & `cg-33.0.5/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_store_api_status_analysis.py` & `cg-33.0.5/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_store_api_status_cases.py` & `cg-33.0.5/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_store_api_status_customer.py` & `cg-33.0.5/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_store_api_status_pool.py` & `cg-33.0.5/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/status/test_store_api_status_sample.py` & `cg-33.0.5/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/api/test_base.py` & `cg-33.0.5/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/conftest.py` & `cg-33.0.5/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_analyses_filters.py` & `cg-33.0.5/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_application_filters.py` & `cg-33.0.5/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_application_version_filters.py` & `cg-33.0.5/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_bed_filters.py` & `cg-33.0.5/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_bed_version_filters.py` & `cg-33.0.5/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_case_sample_filters.py` & `cg-33.0.5/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_cases_filters.py` & `cg-33.0.5/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_collaboration_filters.py` & `cg-33.0.5/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_customer_filters.py` & `cg-33.0.5/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_flow_cell_filters.py` & `cg-33.0.5/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_invoice_filters.py` & `cg-33.0.5/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_organism_filters.py` & `cg-33.0.5/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_panel_filters.py` & `cg-33.0.5/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_pool_filters.py` & `cg-33.0.5/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_samples_filters.py` & `cg-33.0.5/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/filters/test_status_user_filters.py` & `cg-33.0.5/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/test_delivery.py` & `cg-33.0.5/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store/test_store_models.py` & `cg-33.0.5/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/store_helpers.py` & `cg-33.0.5/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/test_store_helpers.py` & `cg-33.0.5/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/utils/conftest.py` & `cg-33.0.5/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/utils/test_commands.py` & `cg-33.0.5/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/utils/test_date.py` & `cg-33.0.5/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/utils/test_dict.py` & `cg-33.0.5/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/utils/test_dispatcher.py` & `cg-33.0.5/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-33.0.4/tests/utils/test_utils.py` & `cg-33.0.5/tests/utils/test_utils.py`

 * *Files identical despite different names*

