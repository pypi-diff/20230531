# Comparing `tmp/qsiprep-0.8.0rc3.tar.gz` & `tmp/qsiprep-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qsiprep-0.8.0rc3.tar", last modified: Wed Feb 19 09:32:04 2020, max compression
+gzip compressed data, was "dist/qsiprep-0.9.0b1.tar", last modified: Thu Jun 18 15:10:24 2020, max compression
```

## Comparing `qsiprep-0.8.0rc3.tar` & `qsiprep-0.9.0b1.tar`

### file list

```diff
@@ -1,163 +1,165 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2301 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4058 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/CHANGES.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2219 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/README.rst
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      184 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1046 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/setup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2028 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/PKG-INFO
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/_version.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2462 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/cli/version.py
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)    40461 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/cli/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4084 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/cli/convertODFs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      160 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/cli/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18894 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/_version.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2030 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/due.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/func/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/func/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/anat/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3089 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/anat/skullstrip.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      332 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/anat/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23861 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/anat/ants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4564 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/utils/misc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7121 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/utils/bids.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/dwi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/dwi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2770 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/__about__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13853 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/reports.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18491 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/plots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25109 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1427 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/engine/workflows.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/engine/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/common/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1066 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/common/orient.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1059 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2148 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/fixes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16254 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/registration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6743 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/segmentation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15585 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/freesurfer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8761 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/surf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11477 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/cifti.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11416 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/bids.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11634 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/masks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1546 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2538 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/plotting.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5867 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/report_base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28161 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11872 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/itk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27188 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/images.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      794 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23234 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/mni.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9105 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/ants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/data/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4470 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/data/getters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14226 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/data/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      434 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/niworkflows/data/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      907 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/maths.pyx
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1312 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/misc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10404 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/bids.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7453 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/sentry.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21717 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/brainsuite_shore.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2081 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/sloppy_recon.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42130 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/grouping.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/atlases.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37601 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/shm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8529 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/bspline.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10530 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/utils/testing.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/workflows/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5036 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/fmap.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10090 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11206 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/unwarp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7603 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/syn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9051 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/pepolar.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1099 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/phdiff.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17749 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/mrtrix.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8197 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/dsi_studio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1014 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/interchange.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2110 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/converters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11409 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/build_workflow.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3769 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/anatomical.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14826 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/dipy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2572 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/recon/dynamics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    70456 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/anatomical.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5661 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/qc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4115 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/confounds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4602 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/registration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15757 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/intramodal_template.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19907 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/finalize.py
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)    15524 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8297 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31370 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/hmc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11888 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/fsl.py
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)    22475 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10204 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/pre_hmc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8020 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/hmc_sdc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      367 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10968 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/resampling.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9591 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/dwi/derivatives.py
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)    33682 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      160 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/workflows/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/__about__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/viz/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11869 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/viz/reports.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      270 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/viz/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1440 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/engine/workflows.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      728 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24281 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/nilearn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    44817 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/mrtrix.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7102 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/qc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20955 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/dsi_studio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9643 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/confounds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36925 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/gradients.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12275 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/converters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16424 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/freesurfer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9668 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/surf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26566 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/reports.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8480 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/anatomical.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20953 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/bids.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20862 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/shoreline.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23937 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/dipy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42267 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/fmap.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10363 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/eddy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10919 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/niworkflows.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/connectivity.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18168 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9790 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/itk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28277 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/images.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8338 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/dwi_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      973 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6424 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/interfaces/ants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep/data/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      189 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/qsiprep/data/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       94 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/requirements.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68817 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/versioneer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1494 2020-02-19 09:31:48.000000 qsiprep-0.8.0rc3/LICENSE
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4360 2020-02-19 09:32:04.000000 qsiprep-0.8.0rc3/qsiprep.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2020-02-19 09:32:03.000000 qsiprep-0.8.0rc3/qsiprep.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        8 2020-02-19 09:32:03.000000 qsiprep-0.8.0rc3/qsiprep.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2028 2020-02-19 09:32:03.000000 qsiprep-0.8.0rc3/qsiprep.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      696 2020-02-19 09:32:03.000000 qsiprep-0.8.0rc3/qsiprep.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2020-02-19 09:32:03.000000 qsiprep-0.8.0rc3/qsiprep.egg-info/dependency_links.txt
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.139059 qsiprep-0.9.0b1/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4231 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/CHANGES.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1494 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/LICENSE
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      184 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2027 2020-06-18 15:10:24.139059 qsiprep-0.9.0b1/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2219 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/README.rst
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/pyproject.toml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.143060 qsiprep-0.9.0b1/qsiprep/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/qsiprep/__about__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      728 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/qsiprep/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      408 2020-06-18 15:10:24.143060 qsiprep-0.9.0b1/qsiprep/_version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.119058 qsiprep-0.9.0b1/qsiprep/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      160 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/qsiprep/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4084 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/qsiprep/cli/convertODFs.py
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)    41180 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/qsiprep/cli/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2462 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/qsiprep/cli/version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.119058 qsiprep-0.9.0b1/qsiprep/data/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      189 2020-06-18 15:02:33.000000 qsiprep-0.9.0b1/qsiprep/data/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.119058 qsiprep-0.9.0b1/qsiprep/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1440 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/engine/workflows.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.123058 qsiprep-0.9.0b1/qsiprep/interfaces/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      973 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8480 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/anatomical.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6498 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/ants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21074 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/bids.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9643 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/confounds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/connectivity.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12992 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/converters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24562 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/dipy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22863 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/dsi_studio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19848 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/dwi_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10363 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/eddy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42587 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/fmap.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16424 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/freesurfer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36925 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/gradients.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24355 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/images.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9790 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/itk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46949 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/mrtrix.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24281 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/nilearn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10917 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/niworkflows.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7102 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/qc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33266 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/reports.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20862 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/shoreline.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9668 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/surf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18380 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/interfaces/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.127058 qsiprep-0.9.0b1/qsiprep/niworkflows/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2770 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/__about__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1059 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18894 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/_version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.127058 qsiprep-0.9.0b1/qsiprep/niworkflows/anat/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      332 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/anat/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23861 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/anat/ants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3089 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/anat/skullstrip.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.127058 qsiprep-0.9.0b1/qsiprep/niworkflows/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/common/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1066 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/common/orient.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.127058 qsiprep-0.9.0b1/qsiprep/niworkflows/data/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      434 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/data/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4470 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/data/getters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14226 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/data/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2030 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/due.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.127058 qsiprep-0.9.0b1/qsiprep/niworkflows/dwi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/dwi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.127058 qsiprep-0.9.0b1/qsiprep/niworkflows/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1427 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/engine/workflows.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.127058 qsiprep-0.9.0b1/qsiprep/niworkflows/func/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/func/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.131059 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      794 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9105 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/ants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11416 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/bids.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11477 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/cifti.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2148 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/fixes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15585 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/freesurfer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27188 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/images.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11872 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/itk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11634 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/masks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23234 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/mni.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1546 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2538 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/plotting.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16254 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/registration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5867 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/report_base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6743 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/segmentation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8761 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/surf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28161 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.131059 qsiprep-0.9.0b1/qsiprep/niworkflows/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7121 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/utils/bids.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4564 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/utils/misc.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.131059 qsiprep-0.9.0b1/qsiprep/niworkflows/viz/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/viz/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18491 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/viz/plots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13853 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/viz/reports.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37078 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/niworkflows/viz/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.135059 qsiprep-0.9.0b1/qsiprep/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/atlases.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10404 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/bids.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21717 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/brainsuite_shore.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8529 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/bspline.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46033 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/grouping.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      907 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/maths.pyx
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1312 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/misc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7453 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/sentry.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37601 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/shm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2159 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/sloppy_recon.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10530 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/utils/testing.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.135059 qsiprep-0.9.0b1/qsiprep/viz/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      270 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/viz/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12260 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/viz/reports.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.135059 qsiprep-0.9.0b1/qsiprep/workflows/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      160 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    70456 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/anatomical.py
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)    37762 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/base.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.135059 qsiprep-0.9.0b1/qsiprep/workflows/dwi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      367 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/__init__.py
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)    22768 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4115 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/confounds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9591 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/derivatives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11643 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/distortion_group_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16747 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/finalize.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11888 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/fsl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31370 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/hmc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8020 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/hmc_sdc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15823 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/intramodal_template.py
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)    16090 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12425 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/pre_hmc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4970 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/qc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4602 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/registration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10167 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/resampling.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8297 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/dwi/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.139059 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1099 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10090 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5011 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/fmap.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9053 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/pepolar.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6454 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/phdiff.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7603 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/syn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11206 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/unwarp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3790 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.139059 qsiprep-0.9.0b1/qsiprep/workflows/recon/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3769 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/anatomical.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9372 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13408 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/build_workflow.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2110 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/converters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17414 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/dipy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13940 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/dsi_studio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/dynamics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1014 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/interchange.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/mrtrix.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2572 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/qsiprep/workflows/recon/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2020-06-18 15:10:24.119058 qsiprep-0.9.0b1/qsiprep.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2027 2020-06-18 15:10:23.000000 qsiprep-0.9.0b1/qsiprep.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4444 2020-06-18 15:10:24.000000 qsiprep-0.9.0b1/qsiprep.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2020-06-18 15:10:23.000000 qsiprep-0.9.0b1/qsiprep.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2020-06-18 15:10:23.000000 qsiprep-0.9.0b1/qsiprep.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      710 2020-06-18 15:10:23.000000 qsiprep-0.9.0b1/qsiprep.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        8 2020-06-18 15:10:23.000000 qsiprep-0.9.0b1/qsiprep.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       94 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/requirements.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2319 2020-06-18 15:10:24.143060 qsiprep-0.9.0b1/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1046 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/setup.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68817 2020-06-18 15:02:34.000000 qsiprep-0.9.0b1/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qsiprep-0.8.0rc3/setup.cfg` & `qsiprep-0.9.0b1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -27,25 +27,27 @@
 
 [options]
 python_requires = >=3.5
 install_requires = 
 	nibabel >=3.0.0
 	indexed_gzip >=0.8.8
 	nilearn !=0.5.0, !=0.5.1
-	nipype <=1.1.9
+	nipype >=1.3.1
 	psutil >=5.4
 	pybids ~= 0.9.3
 	matplotlib <=2.2.3
 	svgutils
 	numpy
-	dipy<=0.15.0
+	dipy >= 1.0
+	fury
 	seaborn
 	pandas
 	pyyaml
 	jinja2
+	xvfbwrapper
 	scikit-learn >=0.20.2
 	scikit-image
 	statsmodels
 test_requires = 
 	coverage
 	codecov
 	pytest
```

### Comparing `qsiprep-0.8.0rc3/CHANGES.rst` & `qsiprep-0.9.0b1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+0.9.0beta1 (June 17, 2020)
+==========================
+
+ * Adds support for HCP lifespan sequences
+ * Introduces --distortion-group-merge option for combining paired scans
+
 0.8.0 (February 12, 2020)
 =========================
 
  * Removes oblique angles from T1w headers to fix N4 bug (#103)
 
 0.7.2 (February 4, 2020)
 ========================
+
  * Fixed a bug in b=0 masking when images have high signal intensity in ventricles (#99)
 
 0.7.1 (January 29, 2020)
 ========================
 
  * Image QC summary data is produced for each output (#95)
  * Update DSI Studio (#88)
```

### Comparing `qsiprep-0.8.0rc3/README.rst` & `qsiprep-0.9.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/setup.py` & `qsiprep-0.9.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/PKG-INFO` & `qsiprep-0.9.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsiprep
-Version: 0.8.0rc3
+Version: 0.9.0b1
 Summary: qsiprep builds workflows for preprocessing and reconstructing q-space images
 Home-page: https://github.com/pennbbl/qsiprep
 Author: The PennBBL developers
 Author-email: Matthew.Cieslak@pennmedicine.upenn.edu
 Maintainer: Matt Cieslak
 Maintainer-email: Matthew.Cieslak@pennmedicine.upenn.edu
 License: 3-clause BSD
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/cli/version.py` & `qsiprep-0.9.0b1/qsiprep/cli/version.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/cli/run.py` & `qsiprep-0.9.0b1/qsiprep/cli/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         '--dwi_denoise_window', '--dwi-denoise-window',
         action='store',
         type=int,
         default=5,
         help='window size in voxels for ``dwidenoise``. Must be odd (default: 5). '
              'If 0, ``dwidwenoise`` will not be run')
     g_conf.add_argument(
-        '--unringing-method', '--unringing-method',
+        '--unringing-method', '--unringing_method',
         action='store',
         choices=['none', 'mrdegibbs'],
         help='Method for Gibbs-ringing removal.\n - none: no action\n - mrdegibbs: '
              'use mrdegibbs from mrtrix3')
     g_conf.add_argument(
         '--dwi-no-biascorr', '--dwi_no_biascorr',
         action='store_true',
@@ -200,30 +200,40 @@
              '``--combine-all-dwis``')
     g_conf.add_argument(
         '--combine_all_dwis', '--combine-all-dwis',
         action='store_true',
         help='combine dwis from across multiple runs for motion correction '
         'and reconstruction.')
     g_conf.add_argument(
+        '--distortion-group-merge', '--distortion_group_merge',
+        action='store',
+        choices=['concat', 'average', 'none'],
+        default='none',
+        help='How to combine images across distorted groups.\n'
+        ' - concatenate: append images in the 4th dimension\n '
+        ' - average: if a whole sequence was duplicated in both PE\n'
+        '            directions, average the corrected images of the same\n'
+        '            q-space coordinate\n'
+        ' - none: Default. Keep distorted groups separate'
+    )
+    g_conf.add_argument(
         '--write-local-bvecs', '--write_local_bvecs',
         action='store_true',
         default=False,
         help='write a series of voxelwise bvecs, relevant if '
         'writing preprocessed dwis to template space')
     g_conf.add_argument(
         '--output-space', '--output_space',
         action='store',
         choices=['T1w', 'template'],
         nargs='+',
         default=['T1w'],
         help='volume and surface spaces to resample dwis into\n'
         ' - T1w: subject anatomical volume\n'
-        ' - template: normalization target specified by --template\n'
-        'this argument can be single value or a space delimited list,\n'
-        'for example: --output-space T1w template')
+        ' - template: deprecated. Will be ignored\n')
     g_conf.add_argument(
         '--template',
         required=False,
         action='store',
         choices=['MNI152NLin2009cAsym'],
         default='MNI152NLin2009cAsym',
         help='volume template space (default: MNI152NLin2009cAsym)')
@@ -501,16 +511,16 @@
     # Set logging
     logger.setLevel(log_level)
     nlogging.getLogger('nipype.workflow').setLevel(log_level)
     nlogging.getLogger('nipype.interface').setLevel(log_level)
     nlogging.getLogger('nipype.utils').setLevel(log_level)
 
     errno = 0
-    mode = "recon" if opts.recon_only else "prep"
-    if mode == "recon":
+    mode = "qsirecon" if opts.recon_only else "qsiprep"
+    if mode == "qsirecon":
         logger.info("running qsirecon")
         building_func = build_recon_workflow
     else:
         logger.info("running qsiprep")
         building_func = build_qsiprep_workflow
 
     # Call build_workflow(opts, retval)
@@ -544,15 +554,15 @@
 
     if opts.boilerplate:
         sys.exit(int(retcode > 0))
 
     # Check workflow for missing commands
     missing = check_deps(qsiprep_wf)
     if missing:
-        print("Cannot run qsiprep. Missing dependencies:")
+        print("Cannot run {}. Missing dependencies:".format(mode))
         for iface, cmd in missing:
             print("\t{} (Interface: {})".format(cmd, iface))
         sys.exit(2)
 
     # Clean up master process before running workflow, which may create forks
     gc.collect()
 
@@ -563,39 +573,37 @@
 
     errno = 1
     try:
         qsiprep_wf.run(**plugin_settings)
     except Exception as e:
         if not opts.notrack:
             from ..utils.sentry import process_crashfile
-            crashfolders = [Path(output_dir) / 'qsiprep' / 'sub-{}'.format(s) / 'log' / run_uuid
+            crashfolders = [Path(output_dir) / mode / 'sub-{}'.format(s) / 'log' / run_uuid
                             for s in subject_list]
             for crashfolder in crashfolders:
                 for crashfile in crashfolder.glob('crash*.*'):
                     process_crashfile(crashfile)
 
             if "Workflow did not execute cleanly" not in str(e):
                 sentry_sdk.capture_exception(e)
         logger.critical('QSIPrep failed: %s', e)
         raise
     else:
         errno = 0
-        logger.log(25, 'QSI{} finished without errors'.format(mode))
+        logger.log(25, 'QSI{} finished without errors'.format(mode[3:]))
         if not opts.notrack:
-            sentry_sdk.capture_message('QSI{} finished without errors'.format(mode),
+            sentry_sdk.capture_message('QSI{} finished without errors'.format(mode[3:]),
                                        level='info')
-
-    # No reports for recon mode yet
-    if mode == "recon":
-        sys.exit(int(errno > 0))
-
     # Generate reports phase
-    errno += generate_reports(subject_list, output_dir, work_dir, run_uuid)
-    write_derivative_description(bids_dir, str(Path(output_dir) / 'qsiprep'))
-    if opts.recon_spec is None:
+    errno += generate_reports(subject_list, output_dir, work_dir, run_uuid,
+                              pipeline_mode=mode)
+    write_derivative_description(bids_dir, str(Path(output_dir) / mode))
+
+    # If we were recon-only, then we're done
+    if mode == "qsirecon" or opts.recon_spec is None:
         logger.info("No additional workflows to run.")
         sys.exit(int(errno > 0))
 
     # Run an additional workflow if preproc + recon are requested
     opts.recon_input = output_dir + "/qsiprep"
     with Manager() as mgr:
         retval = mgr.dict()
@@ -639,30 +647,32 @@
     # Clean up master process before running workflow, which may create forks
     gc.collect()
     try:
         qsirecon_post_wf.run(**plugin_settings)
     except Exception as e:
         if not opts.notrack:
             from ..utils.sentry import process_crashfile
-            crashfolders = [output_dir / 'qsiprep' / 'sub-{}'.format(s) / 'log' / run_uuid
+            crashfolders = [Path(output_dir) / 'qsirecon' / 'sub-{}'.format(s) / 'log' / run_uuid
                             for s in subject_list]
             for crashfolder in crashfolders:
                 for crashfile in crashfolder.glob('crash*.*'):
                     process_crashfile(crashfile)
 
             if "Workflow did not execute cleanly" not in str(e):
                 sentry_sdk.capture_exception(e)
-        logger.critical('QSIPrep failed: %s', e)
+        logger.critical('QSIRecon failed: %s', e)
         raise
     else:
         errno += 0
         logger.log(25, 'QSIPrep finished without errors')
         if not opts.notrack:
             sentry_sdk.capture_message('QSIPostRecon finished without errors',
                                        level='info')
+    errno += generate_reports(subject_list, output_dir, work_dir, run_uuid,
+                              pipeline_mode='qsirecon')
     sys.exit(int(errno > 0))
 
 
 def build_qsiprep_workflow(opts, retval):
     """
     Create the Nipype Workflow that supports the whole execution
     graph, given the inputs.
@@ -718,22 +728,26 @@
     layout = BIDSLayout(str(bids_dir), validate=False)
     subject_list = collect_participants(
         layout, participant_label=opts.participant_label)
     retval['subject_list'] = subject_list
 
     output_spaces = opts.output_space or []
 
-    force_spatial_normalization = opts.force_spatial_normalization
+    force_spatial_normalization = opts.force_spatial_normalization or \
+        'template' in output_spaces
+
+    if 'template' in output_spaces:
+        logger.warning("Using 'template' as an output space is no longer supported.")
+        output_spaces = ["T1w"]
+
     # Check output_space
-    if ('template' not in output_spaces and not force_spatial_normalization) \
-            and (opts.use_syn_sdc or opts.force_syn):
+    if not force_spatial_normalization and (opts.use_syn_sdc or opts.force_syn):
         msg = [
-            'SyN SDC correction requires T1 to MNI registration, but '
-            '"template" is not specified in "--output-space" arguments.',
-            'Option --use-syn will be cowardly dismissed.'
+            'SyN SDC correction requires T1 to MNI registration.',
+            'Adding T1w-based normalization'
         ]
         force_spatial_normalization = True
         logger.warning(' '.join(msg))
 
     # Load base plugin_settings from file if --use-plugin
     if opts.use_plugin is not None:
         from yaml import load as loadyml
@@ -835,14 +849,15 @@
         freesurfer=opts.do_reconall,
         debug=opts.sloppy,
         low_mem=opts.low_mem,
         anat_only=opts.anat_only,
         longitudinal=opts.longitudinal,
         b0_threshold=opts.b0_threshold,
         combine_all_dwis=opts.combine_all_dwis,
+        distortion_group_merge=opts.distortion_group_merge,
         dwi_denoise_window=opts.dwi_denoise_window,
         unringing_method=opts.unringing_method,
         dwi_no_biascorr=opts.dwi_no_biascorr,
         no_b0_harmonization=opts.no_b0_harmonization,
         denoise_before_combining=opts.denoise_before_combining,
         write_local_bvecs=opts.write_local_bvecs,
         omp_nthreads=omp_nthreads,
@@ -980,15 +995,15 @@
     if 1 < nthreads < omp_nthreads:
         logger.warning(
             'Per-process threads (--omp-nthreads=%d) exceed total '
             'threads (--nthreads/--n_cpus=%d)', omp_nthreads, nthreads)
 
     # Set up directories
     output_dir = op.abspath(opts.output_dir)
-    log_dir = op.join(output_dir, 'qsiprep', 'logs')
+    log_dir = op.join(output_dir, 'qsirecon', 'logs')
     work_dir = op.abspath(opts.work_dir or 'work')  # Set work/ as default
 
     # Check and create output and working directories
     os.makedirs(output_dir, exist_ok=True)
     os.makedirs(log_dir, exist_ok=True)
     os.makedirs(work_dir, exist_ok=True)
 
@@ -1046,15 +1061,15 @@
         low_mem=opts.low_mem,
         omp_nthreads=omp_nthreads,
         bids_dir=bids_dir,
         sloppy=opts.sloppy
     )
     retval['return_code'] = 0
 
-    logs_path = Path(output_dir) / 'qsiprep' / 'logs'
+    logs_path = Path(output_dir) / 'qsirecon' / 'logs'
     boilerplate = retval['workflow'].visit_desc()
     (logs_path / 'CITATION.md').write_text(boilerplate)
     logger.log(
         25, 'Works derived from this qsiprep execution should '
         'include the following boilerplate:\n\n%s', boilerplate)
 
     # Generate HTML file resolving citations
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/cli/convertODFs.py` & `qsiprep-0.9.0b1/qsiprep/cli/convertODFs.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/_version.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/_version.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/due.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/due.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/anat/skullstrip.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/anat/skullstrip.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/anat/ants.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/anat/ants.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/utils/misc.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/utils/misc.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/utils/bids.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/utils/bids.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/__about__.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/__about__.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/reports.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/viz/reports.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/plots.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/viz/plots.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/viz/utils.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/viz/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 import re
 from sys import version_info
 from uuid import uuid4
 from io import open, StringIO
 
 import numpy as np
 import nibabel as nb
+import matplotlib.pyplot as plt
 
+from dipy.core.ndindex import ndindex
+from dipy.reconst.odf import gfa
+from dipy.direction import peak_directions
 from lxml import etree
 from nilearn import image as nlimage
 from nilearn.plotting import plot_anat
 from svgutils.transform import SVGFigure
 from seaborn import color_palette
+from PIL import Image
 
 from .. import NIWORKFLOWS_LOG
 from nipype.utils import filemanip
 
 try:
     from shutil import which
 except ImportError:
@@ -586,15 +591,14 @@
 def plot_melodic_components(melodic_dir, in_file, tr=None,
                             out_file='melodic_reportlet.svg',
                             compress='auto', report_mask=None,
                             noise_components_file=None):
     from nilearn.image import index_img, iter_img
     import nibabel as nb
     import numpy as np
-    import pylab as plt
     import seaborn as sns
     from matplotlib.gridspec import GridSpec
     import os
     import re
     from io import StringIO
     sns.set_style("white")
     current_palette = sns.color_palette()
@@ -722,7 +726,280 @@
     image_svg = re.sub(' width="[0-9]+[a-z]*"', '', image_svg, count=1)
     image_svg = re.sub(' viewBox',
                        ' preseveAspectRation="xMidYMid meet" viewBox',
                        image_svg, count=1)
 
     with open(out_file, 'w' if PY3 else 'wb') as f:
         f.write(image_svg)
+
+
+def slices_from_bbox(mask_data, cuts=3, padding=0):
+    """Finds equi-spaced cuts for presenting images"""
+    B = np.argwhere(mask_data > 0)
+    start_coords = B.min(0)
+    stop_coords = B.max(0) + 1
+
+    vox_coords = []
+    for start, stop in zip(start_coords, stop_coords):
+        inc = abs(stop - start) / (cuts + 2 * padding + 1)
+        slices = [start + (i + 1) * inc for i in range(cuts + 2 * padding)]
+        vox_coords.append(slices[padding:-padding])
+    return {k: [int(_v) for _v in v] for k, v in zip(['x', 'y', 'z'], vox_coords)}
+
+
+def plot_peak_slice(odf_4d, sphere, background_data, out_file, axis, slicenum, mask_data,
+                    tile_size=1200, normalize_peaks=True):
+    from fury import actor, window
+    view_up = [(0., 0., 1.), (0., 0., 1.), (0., -1., 0.)]
+
+    # Make a slice mask to reduce memory
+    new_shape = list(odf_4d.shape)
+    new_shape[axis] = 1
+    image_shape = new_shape[:3]
+    midpoint = (new_shape[0] / 2., new_shape[1] / 2., new_shape[2] / 2.)
+
+    if axis == 0:
+        odf_slice = odf_4d[slicenum, :, :, :].reshape(new_shape)
+        image_slice = background_data[slicenum, :, :].reshape(image_shape)
+        mask_slice = mask_data[slicenum, :, :].reshape(image_shape)
+        camera_dist = max(midpoint[1], midpoint[2]) * np.pi
+    elif axis == 1:
+        odf_slice = odf_4d[:, slicenum, :, :].reshape(new_shape)
+        image_slice = background_data[:, slicenum, :].reshape(image_shape)
+        mask_slice = mask_data[:, slicenum, :].reshape(image_shape)
+        camera_dist = max(midpoint[0], midpoint[2]) * np.pi
+    elif axis == 2:
+        odf_slice = odf_4d[:, :, slicenum, :].reshape(new_shape)
+        image_slice = background_data[:, :, slicenum].reshape(image_shape)
+        mask_slice = mask_data[:, :, slicenum].reshape(image_shape)
+        camera_dist = max(midpoint[0], midpoint[1]) * np.pi
+    position = list(midpoint)
+    position[axis] += camera_dist
+
+    # Find the actual peaks
+    peak_dirs, peak_values = peaks_from_odfs(odf_slice, sphere,
+                                             relative_peak_threshold=.1,
+                                             min_separation_angle=15,
+                                             mask=mask_slice,
+                                             normalize_peaks=normalize_peaks,
+                                             npeaks=3)
+    if normalize_peaks:
+        peak_values = peak_values / peak_values.max() * np.pi
+    peak_actor = actor.peak_slicer(peak_dirs, peak_values, colors=None)
+    image_actor = actor.slicer(image_slice, opacity=0.6, interpolation='nearest')
+    image_size = (tile_size, tile_size)
+    scene = window.Scene()
+    scene.add(image_actor)
+    scene.add(peak_actor)
+
+    xfov_min, xfov_max = 0, new_shape[0] - 1
+    yfov_min, yfov_max = 0, new_shape[1] - 1
+    zfov_min, zfov_max = 0, new_shape[2] - 1
+    peak_actor.display_extent(xfov_min, xfov_max, yfov_min, yfov_max, zfov_min, zfov_max)
+    image_actor.display_extent(xfov_min, xfov_max, yfov_min, yfov_max, zfov_min, zfov_max)
+    scene.set_camera(focal_point=tuple(midpoint),
+                     position=tuple(position),
+                     view_up=view_up[axis])
+    window.record(scene, out_path=out_file, reset_camera=False, size=image_size)
+    scene.clear()
+
+
+def peak_slice_series(odf_4d, sphere, background_data, out_file, mask_image=None,
+                      prefix='odf', tile_size=1200, n_cuts=3, padding=4,
+                      normalize_peaks=True):
+
+    # Make a slice mask to reduce memory
+    if mask_image is None:
+        image_mask = np.ones(background_data.shape)
+    else:
+        image_mask = nb.load(mask_image).get_fdata()
+
+    slice_indices = slices_from_bbox(background_data, cuts=n_cuts, padding=padding)
+    # Render the axial slices
+    z_image = Image.new('RGB', (tile_size, tile_size * n_cuts))
+    for slicenum, z_slice in enumerate(slice_indices['z']):
+        png_file = '{}_tra_{:03d}.png'.format(prefix, z_slice)
+        plot_peak_slice(odf_4d, sphere, background_data, png_file, 2, z_slice, image_mask,
+                        tile_size, normalize_peaks)
+        z_image.paste(Image.open(png_file), (0, slicenum * tile_size))
+
+    # Render the sagittal slices
+    x_image = Image.new('RGB', (tile_size, tile_size * n_cuts))
+    for slicenum, x_slice in enumerate(slice_indices['x']):
+        png_file = '{}_sag_{:03d}.png'.format(prefix, x_slice)
+        plot_peak_slice(odf_4d, sphere, background_data, png_file, 0, x_slice, image_mask,
+                        tile_size, normalize_peaks)
+        x_image.paste(Image.open(png_file), (0, slicenum * tile_size))
+
+    # Render the coronal slices
+    y_image = Image.new('RGB', (tile_size, tile_size * n_cuts))
+    for slicenum, y_slice in enumerate(slice_indices['y']):
+        png_file = '{}_cor_{:03d}.png'.format(prefix, y_slice)
+        plot_peak_slice(odf_4d, sphere, background_data, png_file, 1, y_slice, image_mask,
+                        tile_size, normalize_peaks)
+        y_image.paste(Image.open(png_file), (0, slicenum * tile_size))
+
+    final_image = Image.new('RGB', (tile_size * 3, tile_size * n_cuts))
+    final_image.paste(z_image, (0, 0))
+    final_image.paste(x_image, (tile_size, 0))
+    final_image.paste(y_image, (tile_size * 2, 0))
+    final_image.save(out_file)
+
+
+def peaks_from_odfs(odf4d, sphere, relative_peak_threshold,
+                    min_separation_angle, mask=None,
+                    gfa_thr=0, normalize_peaks=False,
+                    npeaks=5):
+
+    shape = odf4d.shape[:-1]
+    if mask is None:
+        mask = np.ones(shape, dtype='bool')
+    else:
+        if mask.shape != shape:
+            raise ValueError("Mask is not the same shape as data.")
+
+    gfa_array = np.zeros(shape)
+    qa_array = np.zeros((shape + (npeaks,)))
+
+    peak_dirs = np.zeros((shape + (npeaks, 3)))
+    peak_values = np.zeros((shape + (npeaks,)))
+    peak_indices = np.zeros((shape + (npeaks,)), dtype='int')
+    peak_indices.fill(-1)
+
+    global_max = -np.inf
+    for idx in ndindex(shape):
+        if not mask[idx]:
+            continue
+        odf = odf4d[idx]
+        gfa_array[idx] = gfa(odf)
+        if gfa_array[idx] < gfa_thr:
+            global_max = max(global_max, odf.max())
+            continue
+        # Get peaks of odf
+        direction, pk, ind = peak_directions(odf, sphere,
+                                             relative_peak_threshold,
+                                             min_separation_angle)
+        # Calculate peak metrics
+        if pk.shape[0] != 0:
+            global_max = max(global_max, pk[0])
+            n = min(npeaks, pk.shape[0])
+            qa_array[idx][:n] = pk[:n] - odf.min()
+            peak_dirs[idx][:n] = direction[:n]
+            peak_indices[idx][:n] = ind[:n]
+            peak_values[idx][:n] = pk[:n]
+
+            if normalize_peaks:
+                peak_values[idx][:n] /= pk[0]
+                peak_dirs[idx] *= peak_values[idx][:, None]
+
+    qa_array /= global_max
+
+    return peak_dirs, peak_values
+
+
+def get_camera_for_roi(roi_data, roi_id, view_axis):
+    voxel_coords = np.row_stack(np.nonzero(roi_data == roi_id))
+    centroid = voxel_coords.mean(1)
+    other_axes = [[1, 2], [0, 2], [0, 1]][view_axis]
+    projected_x = voxel_coords[other_axes[0]]
+    projected_y = voxel_coords[other_axes[1]]
+    xspan = projected_x.max() - projected_x.min()
+    yspan = projected_y.max() - projected_y.min()
+    camera_distance = max(xspan, yspan) * np.pi
+    return centroid, camera_distance
+
+
+def plot_an_odf_slice(odf_4d, full_sphere, background_data, tile_size, filename,
+                      centroid, axis, camera_distance, subtract_iso, mask_image):
+    from fury import actor, window
+    view_up = [(0., 0., 1.), (0., 0., 1.), (0., -1., 0.)]
+
+    # Adjust the centroid so it's only a single slice
+    slicenum = int(np.round(centroid)[axis])
+    centroid[axis] = 0
+    position = centroid.copy()
+    position[axis] = position[axis] + camera_distance
+
+    # Roll if viewing an axial slice
+    roll = 3 if axis == 2 else 0
+    position[1] = position[1] - roll
+
+    # Ensure the dimensions reflect that there is only one slice
+    new_shape = list(odf_4d.shape)
+    new_shape[axis] = 1
+    image_shape = new_shape[:3]
+    if axis == 0:
+        odf_slice = odf_4d[slicenum, :, :, :].reshape(new_shape)
+        image_slice = background_data[slicenum, :, :].reshape(image_shape)
+    elif axis == 1:
+        odf_slice = odf_4d[:, slicenum, :, :].reshape(new_shape)
+        image_slice = background_data[:, slicenum, :].reshape(image_shape)
+    elif axis == 2:
+        odf_slice = odf_4d[:, :, slicenum, :].reshape(new_shape)
+        image_slice = background_data[:, :, slicenum].reshape(image_shape)
+
+    # Tile to get the whole ODF
+    odf_slice = np.tile(odf_slice, (1, 1, 1, 2))
+    if subtract_iso:
+        odf_slice = odf_slice - odf_slice.min(3, keepdims=True)
+    # Make graphics objects
+    odf_actor = actor.odf_slicer(odf_slice, sphere=full_sphere,
+                                 colormap=None, scale=0.6, mask=image_slice)
+    image_actor = actor.slicer(image_slice, opacity=0.6, interpolation='nearest')
+    image_size = (tile_size, tile_size)
+    scene = window.Scene()
+    scene.add(image_actor)
+    scene.add(odf_actor)
+    xfov_min, xfov_max = 0, new_shape[0] - 1
+    yfov_min, yfov_max = 0, new_shape[1] - 1
+    zfov_min, zfov_max = 0, new_shape[2] - 1
+    odf_actor.display_extent(xfov_min, xfov_max, yfov_min, yfov_max, zfov_min, zfov_max)
+    image_actor.display_extent(xfov_min, xfov_max, yfov_min, yfov_max, zfov_min, zfov_max)
+    scene.set_camera(focal_point=tuple(centroid),
+                     position=tuple(position),
+                     view_up=view_up[axis])
+    window.record(scene, out_path=filename, reset_camera=False, size=image_size)
+    scene.clear()
+
+
+def odf_roi_plot(odf_4d, halfsphere, background_data, out_file, roi_file,
+                 prefix='odf', tile_size=1200, subtract_iso=False, mask=None):
+
+    roi_data = nb.load(roi_file).get_fdata()
+    roi_image = Image.new('RGB', (tile_size * 3, tile_size))
+    roi1_centroid, roi1_distance = get_camera_for_roi(roi_data, 1, 2)
+    roi2_centroid, roi2_distance = get_camera_for_roi(roi_data, 2, 1)
+    roi3_centroid, roi3_distance = get_camera_for_roi(roi_data, 3, 1)
+
+    camera_distance = max(roi1_distance, roi2_distance, roi3_distance)
+    # Make a slice mask to reduce memory
+    if mask is None:
+        image_mask = np.ones(roi_data.shape)
+    else:
+        image_mask = nb.load(mask).get_fdata()
+
+    # Fill out the other half of the sphere
+    odf_sphere = halfsphere.mirror()
+    semiovale_axial_file = '{}_semoivale_axial.png'.format(prefix)
+    plot_an_odf_slice(odf_4d, odf_sphere, background_data, tile_size,
+                      semiovale_axial_file, centroid=roi1_centroid, axis=2,
+                      camera_distance=camera_distance, subtract_iso=subtract_iso,
+                      mask_image=image_mask)
+    roi_image.paste(Image.open(semiovale_axial_file), (0, 0))
+
+    # Render the coronal slice with a double-crossing
+    cst_x_cc_file = '{}_CSTxCC.png'.format(prefix)
+    plot_an_odf_slice(odf_4d, odf_sphere, background_data, tile_size,
+                      cst_x_cc_file, centroid=roi2_centroid, axis=1,
+                      camera_distance=camera_distance, subtract_iso=subtract_iso,
+                      mask_image=image_mask)
+    roi_image.paste(Image.open(cst_x_cc_file), (tile_size, 0))
+
+    # Render the corpus callosum
+    cc_file = '{}_CC.png'.format(prefix)
+    plot_an_odf_slice(odf_4d, odf_sphere, background_data, tile_size,
+                      cc_file, centroid=roi3_centroid, axis=1,
+                      camera_distance=camera_distance, subtract_iso=subtract_iso,
+                      mask_image=image_mask)
+    roi_image.paste(Image.open(cc_file), (2 * tile_size, 0))
+
+    roi_image.save(out_file)
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/engine/workflows.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/engine/workflows.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/common/orient.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/common/orient.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/__init__.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/__init__.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/fixes.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/fixes.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/registration.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/registration.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/segmentation.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/segmentation.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/freesurfer.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/freesurfer.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/surf.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/surf.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/cifti.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/cifti.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/bids.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/bids.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/masks.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/masks.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/patches.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/patches.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/plotting.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/plotting.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/report_base.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/report_base.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/utils.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/itk.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/itk.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/images.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/images.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/__init__.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/mni.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/mni.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/interfaces/ants.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/interfaces/ants.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/data/getters.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/data/getters.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/niworkflows/data/utils.py` & `qsiprep-0.9.0b1/qsiprep/niworkflows/data/utils.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/maths.pyx` & `qsiprep-0.9.0b1/qsiprep/utils/maths.pyx`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/misc.py` & `qsiprep-0.9.0b1/qsiprep/utils/misc.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/bids.py` & `qsiprep-0.9.0b1/qsiprep/utils/bids.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/sentry.py` & `qsiprep-0.9.0b1/qsiprep/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/brainsuite_shore.py` & `qsiprep-0.9.0b1/qsiprep/utils/brainsuite_shore.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/sloppy_recon.py` & `qsiprep-0.9.0b1/qsiprep/utils/sloppy_recon.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,21 @@
         ("Dipy", "MAPMRI_reconstruction"): {
             "extrapolate_scheme": "ABCD",
             "anisotropic_scaling": False,
             "laplacian_weighting": 0.2},
 
         ("DSI Studio", "connectivity"): {
             "fiber_count": 5000},
+        ("DSI Studio", "tractography"): {
+            "fiber_count": 5000},
 
         ("MRTrix3", "tractography"): {
             "tckgen": {
-                "select": 100,
-                "seed": 500,
+                "select": 1000,
+                "seed": 5000,
                 "backtrack": "DELETE",
                 "n_samples": "DELETE",
                 "n_trials": "DELETE",
                 "algorithm": "SD_Stream"}},
 
         ("MRTrix3", "connectivity"): {
             "tck2connectome": {
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/grouping.py` & `qsiprep-0.9.0b1/qsiprep/utils/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,32 @@
     >>> import os
     >>> from qsiprep.utils.testing import get_grouping_test_data
     >>> data_root = get_grouping_test_data()
     >>> os.chdir(data_root)
 """
 from collections import defaultdict
 import logging
-import os
 from nipype.utils.filemanip import split_filename
-
+from ..interfaces.bids import get_bids_params
 LOGGER = logging.getLogger('nipype.workflow')
 
 
 def group_dwi_scans(bids_layout, subject_data, using_fsl=False, combine_scans=True,
-                    ignore_fieldmaps=False):
+                    ignore_fieldmaps=False, concatenate_distortion_groups=False):
     """Determine which scans can be concatenated based on their acquisition parameters.
 
     **Parameters**
         bids_layout : layout
             A PyBIDS layout
         group_for_eddy : bool
             Should a plus and minus series be grouped together for TOPUP/eddy?
         combine_scans : bool
             Should scan concatention happen?
+        concatenate_distortion_groups : bool
+            Will distortion groups get merged at the end of the pipeline?
 
     **Returns**
         scan_groups : list of dictionaries
             A dict where the keys are the BIDS derivatives name of the output file after
             concatenation. The values are lists of dwi files in that group
     """
 
@@ -49,15 +50,18 @@
     for dwi_session_group in dwi_session_groups:
         dwi_fmap_groups.extend(
             group_by_warpspace(dwi_session_group, bids_layout, ignore_fieldmaps))
 
     if using_fsl:
         return group_for_eddy(dwi_fmap_groups)
 
-    return dwi_fmap_groups
+    if concatenate_distortion_groups:
+        return dwi_fmap_groups, group_for_concatenation(dwi_fmap_groups)
+
+    return dwi_fmap_groups, {}
 
 
 def get_session_groups(layout, subject_data, combine_all_dwis):
     # Handle the grouping of multiple dwi files within a session
     sessions = layout.get_sessions() if layout is not None else []
     all_dwis = subject_data['dwi']
     dwi_session_groups = []
@@ -765,15 +769,15 @@
         "dwi_series_pedir": pe_dir,
         "fieldmap_info": fieldmap_info,
         "concatenated_bids_name": get_concatenated_bids_name(dwi_files + rpe_files)
     }
     return merged_group
 
 
-def group_for_eddy(dwi_fmap_groups):
+def group_for_eddy(all_dwi_fmap_groups):
     """Find matched pairs of phase encoding directions that can be combined for TOPUP/eddy.
 
     Any groups that don't have a phase encoding direction won't be correctable by eddy/TOPUP.
 
     Examples:
     ----------
 
@@ -859,35 +863,56 @@
        'suffix': 'phasediff'},
       'dwi_series_pedir': 'j',
       'concatenated_bids_name': 'sub-1_dir-AP'}]
 
     """
     eddy_dwi_groups = []
     eddy_compatible_suffixes = ('dwi', 'epi')
-    for pe_dir in 'ijk':
-        plus_series = [dwi_group for dwi_group in dwi_fmap_groups if
-                       dwi_group.get('dwi_series_pedir') == pe_dir
-                       and dwi_group['fieldmap_info'].get('suffix') in eddy_compatible_suffixes]
-        minus_series = [dwi_group for dwi_group in dwi_fmap_groups if
-                        dwi_group.get('dwi_series_pedir') == pe_dir + '-'
-                        and dwi_group['fieldmap_info'].get('suffix') in eddy_compatible_suffixes]
+    session_groups = _group_by_sessions(all_dwi_fmap_groups)
+    for _, dwi_fmap_groups in session_groups.items():
+        for pe_dir in 'ijk':
+            plus_series = [dwi_group for dwi_group in dwi_fmap_groups if
+                           dwi_group.get('dwi_series_pedir') == pe_dir
+                           and dwi_group['fieldmap_info'].get('suffix') in
+                           eddy_compatible_suffixes]
+            minus_series = [dwi_group for dwi_group in dwi_fmap_groups if
+                            dwi_group.get('dwi_series_pedir') == pe_dir + '-'
+                            and dwi_group['fieldmap_info'].get('suffix') in
+                            eddy_compatible_suffixes]
+
+            # Can these be grouped?
+            if plus_series and minus_series:
+                eddy_dwi_groups.append(merge_dwi_groups(plus_series, minus_series))
+            else:
+                eddy_dwi_groups.extend(plus_series + minus_series)
+
+        # Add separate groups for non-compatible fieldmaps
+        for dwi_group in dwi_fmap_groups:
+            if dwi_group['fieldmap_info'].get('suffix') not in eddy_compatible_suffixes:
+                eddy_dwi_groups.append(dwi_group)
 
-        # Can these be grouped?
+    return eddy_dwi_groups, {group['concatenated_bids_name']: group['concatenated_bids_name']
+                             for group in eddy_dwi_groups}
 
-        if plus_series and minus_series:
-            eddy_dwi_groups.append(merge_dwi_groups(plus_series, minus_series))
-        else:
-            eddy_dwi_groups.extend(plus_series + minus_series)
 
-    # Add separate groups for non-compatible fieldmaps
-    for dwi_group in dwi_fmap_groups:
-        if dwi_group['fieldmap_info'].get('suffix') not in eddy_compatible_suffixes:
-            eddy_dwi_groups.append(dwi_group)
+def group_for_concatenation(all_dwi_fmap_groups):
+    """Find matched pairs of phase encoding directions that can be combined after SHORELine.
+    """
+    concatenation_grouping = {}
+    session_groups = _group_by_sessions(all_dwi_fmap_groups)
+    for _, dwi_fmap_groups in session_groups.items():
+        all_images = []
+        for group in dwi_fmap_groups:
+            all_images.extend(group['dwi_series'])
+        group_name = get_concatenated_bids_name(all_images)
+        # Add separate groups for non-compatible fieldmaps
+        for group in dwi_fmap_groups:
+            concatenation_grouping[group['concatenated_bids_name']] = group_name
 
-    return eddy_dwi_groups
+    return concatenation_grouping
 
 
 def get_concatenated_bids_name(dwi_group):
     """Derive the output file name for a group of dwi files.
 
     Strip away non-shared key/values from the input list of files. This function
     assumes you have already split the dwi group into something meaningful and
@@ -918,25 +943,78 @@
     ...    '/data/sub-1/dwi/sub-1_acq-HCP_dir-PA_run-2_dwi.nii.gz'
     ... ])
     'sub-1_acq-HCP'
 
     """
     # If a single file, use its name, otherwise use the common prefix
     if len(dwi_group) > 1:
-        no_runs = []
-        for dwi in dwi_group:
-            no_runs.append(
-                "_".join([part for part in dwi.split("_")
-                          if not part.startswith("run")]))
-        input_fname = os.path.commonprefix(no_runs)
-        fname = split_filename(input_fname)[1]
+        fname = _get_common_bids_fields(dwi_group)
         parts = fname.split('_')
         full_parts = [part for part in parts if not part.endswith('-')]
         fname = '_'.join(full_parts)
     else:
         input_fname = dwi_group[0]
         fname = split_filename(input_fname)[1]
 
     if fname.endswith("_dwi"):
         fname = fname[:-4]
 
     return fname.replace(".", "").replace(" ", "")
+
+
+def _get_common_bids_fields(fnames):
+    bids_keys = defaultdict(set)
+    for fname in fnames:
+        basename = split_filename(fname)[1]
+        for token in basename.split("_"):
+            parts = token.split("-")
+            if len(parts) == 2:
+                key, value = parts
+                bids_keys[key].update((value,))
+
+    # Find all the keys with a single unique value
+    common_bids = []
+    for key in ['sub', 'ses', 'acq', 'dir', 'run']:
+        if len(bids_keys[key]) == 1:
+            common_bids.append(key + "-" + bids_keys[key].pop())
+    return "_".join(common_bids)
+
+
+def _group_by_sessions(dwi_fmap_groups):
+    """Create a lookup of distortion groups by session
+
+    Paired DWI series to correct each other:
+    >>> dwi_groups = [
+    ...  {'dwi_series': ['.../mixed_fmaps/sub-1/ses-1/dwi/sub-1_ses-1_dir-AP_run-1_dwi.nii.gz'],
+    ...      'fieldmap_info': {'suffix': 'dwi',
+    ...      'dwi': ['.../mixed_fmaps/sub-1/ses-1/dwi/sub-1_ses-1_dir-PA_run-2_dwi.nii.gz']},
+    ...   'dwi_series_pedir': 'j',
+    ...      'concatenated_bids_name': 'sub-1_ses-1_dir-AP_run-1'},
+    ...  {'dwi_series': ['.../mixed_fmaps/sub-1/ses-1/dwi/sub-1_ses-1_dir-PA_run-2_dwi.nii.gz'],
+    ...      'fieldmap_info': {'suffix': 'dwi',
+    ...      'dwi': ['.../mixed_fmaps/sub-1/ses-1/dwi/sub-1_ses-1_dir-AP_run-1_dwi.nii.gz']},
+    ...      'dwi_series_pedir': 'j-',
+    ...   'concatenated_bids_name': 'sub-1_ses-1_dir-PA_run-2'},
+    ...  {'dwi_series': [
+    ...          '.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2/dir-AP_run-1_dwi.nii.gz',
+    ...          '.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2/dir-AP_run-2_dwi.nii.gz'],
+    ...      'fieldmap_info': {'suffix': 'dwi',
+    ...       'dwi': ['.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2_dir-PA_run-1_dwi.nii.gz',
+    ...               '.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2_dir-PA_run-2_dwi.nii.gz']},
+    ...      'dwi_series_pedir': 'j',
+    ...      'concatenated_bids_name': 'sub-1_ses-2_dir-AP'},
+    ...     {'dwi_series': [
+    ...           '.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2_dir-PA_run-1_dwi.nii.gz',
+    ...           '.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2_dir-PA_run-2_dwi.nii.gz'],
+    ...      'fieldmap_info': {'suffix': 'dwi',
+    ...       'dwi': ['.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2_dir-AP_run-1_dwi.nii.gz',
+    ...               '.../opposite_concat/sub-1/ses-2/dwi/sub-1_ses-2_dir-AP_run-2_dwi.nii.gz']},
+    ...      'dwi_series_pedir': 'j-',
+    ...      'concatenated_bids_name': 'sub-1_ses-2_dir-PA'}]
+
+
+    """
+    ses_lookup = defaultdict(list)
+    for group in dwi_fmap_groups:
+        bids_info = get_bids_params(group['concatenated_bids_name'])
+        ses_lookup[bids_info['session_id']].append(group)
+    return ses_lookup
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/atlases.py` & `qsiprep-0.9.0b1/qsiprep/utils/atlases.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/shm.py` & `qsiprep-0.9.0b1/qsiprep/utils/shm.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/bspline.py` & `qsiprep-0.9.0b1/qsiprep/utils/bspline.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/utils/testing.py` & `qsiprep-0.9.0b1/qsiprep/utils/testing.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/fmap.py` & `qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/fmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 This corresponds to the section 8.9.3 --fieldmap image (and one magnitude image)--
 of the BIDS specification.
 
 """
 
 from nipype.pipeline import engine as pe
 from nipype.interfaces import utility as niu, fsl, ants
-from nipype.workflows.dmri.fsl.utils import demean_image, cleanup_edge_pipeline
+from .utils import demean_image, cleanup_edge_pipeline
 from ...niworkflows.engine.workflows import LiterateWorkflow as Workflow
 from ...niworkflows.interfaces.images import IntraModalMerge
 from ...niworkflows.interfaces.masks import BETRPT
 
 from ...interfaces import (
     FieldEnhance, FieldToRadS, FieldToHz, DerivativesDataSink
 )
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/base.py` & `qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/base.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/unwarp.py` & `qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/unwarp.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/syn.py` & `qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/syn.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/pepolar.py` & `qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/pepolar.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,28 +179,28 @@
     fmap2ref_reg = pe.Node(ants.Registration(from_file=ants_settings,
                                              output_warped_image=True),
                            name='fmap2ref_reg', n_procs=omp_nthreads)
     resample_epi_fmap = pe.Node(ANTSApplyTransformsRPT(dimension=3,
                                                        generate_report=False,
                                                        float=True,
                                                        interpolation='LanczosWindowedSinc'),
-                                name='unwarp_reference')
+                                name='resample_epi_fmap')
     workflow = Workflow(name=name)
 
     def _flatten(l):
         from nipype.utils.filemanip import filename_to_list
         return [item for sublist in l for item in filename_to_list(sublist)]
 
     workflow.connect([
         (inputnode, prepare_b0s, [('fmaps', 'b0_file')]),
         (prepare_b0s, merge, [(('fmap_file', _flatten), 'in_files')]),
         (merge, enhance_b0, [('out_file', 'b0_file')]),
         (enhance_b0, fmap2ref_reg, [('enhanced_file', 'moving_image')]),
         (inputnode, fmap2ref_reg, [('ref_brain', 'fixed_image')]),
-        (fmap2ref_reg, resample_epi_fmap, [('forward_transforms', 'transforms')]),
+        (fmap2ref_reg, resample_epi_fmap, [('composite_transform', 'transforms')]),
         (enhance_b0, resample_epi_fmap, [('enhanced_file', 'input_image')]),
         (inputnode, resample_epi_fmap, [('ref_brain', 'reference_image')]),
         (resample_epi_fmap, outputnode, [('output_image', 'out_file')])
     ])
 
     return workflow
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/__init__.py` & `qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/__init__.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/fieldmap/phdiff.py` & `qsiprep-0.9.0b1/qsiprep/workflows/fieldmap/phdiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 8.9.1 in BIDS 1.0.0: one phase diff and at least one magnitude image
 8.9.2 in BIDS 1.0.0: two phases and at least one magnitude image
 
 """
 
 from nipype.interfaces import ants, fsl, utility as niu
 from nipype.pipeline import engine as pe
-from nipype.workflows.dmri.fsl.utils import siemens2rads, demean_image, \
-    cleanup_edge_pipeline
+from .utils import cleanup_edge_pipeline, siemens2rads, demean_image
 from ...niworkflows.engine.workflows import LiterateWorkflow as Workflow
 from ...niworkflows.interfaces.bids import ReadSidecarJSON
 from ...niworkflows.interfaces.images import IntraModalMerge
 from ...niworkflows.interfaces.masks import BETRPT
 
 from ...interfaces import Phasediff2Fieldmap, Phases2Fieldmap, DerivativesDataSink
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/mrtrix.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/mrtrix.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,35 @@
 .. autofunction:: init_mrtrix_csd_recon_wf
 
 """
 import logging
 import nipype.pipeline.engine as pe
 import nipype.interfaces.utility as niu
 from nipype.interfaces import afni
-from qsiprep.interfaces.bids import ReconDerivativesDataSink
+from ...interfaces.bids import ReconDerivativesDataSink
+from ...interfaces.reports import ReconPeaksReport, ConnectivityReport
 from qsiprep.interfaces.mrtrix import (
     EstimateFOD, SS3TEstimateFOD, MRTrixIngress, SS3TDwi2Response, GlobalTractography,
     MRTrixAtlasGraph, SIFT2, TckGen, MTNormalize)
 from .interchange import input_fields
+from ...engine import Workflow
 
 LOGGER = logging.getLogger('nipype.interface')
 MULTI_RESPONSE_ALGORITHMS = ('dhollander', 'msmt_5tt')
 
+CITATIONS = {
+    "dhollander": "(@dhollander2019response, @dhollander2016unsupervised)",
+    "msmt_5tt": "(@msmt5tt)",
+    "csd": "(@originalcsd, @tournier2007robust)",
+    "msmt_csd": "(@originalcsd, @msmt5tt)"
+}
 
-def init_mrtrix_csd_recon_wf(name="mrtrix_recon", output_suffix="", params={}):
+
+def init_mrtrix_csd_recon_wf(omp_nthreads, has_transform, name="mrtrix_recon",
+                             output_suffix="", params={}):
     """Create FOD images for WM, GM and CSF.
 
     This workflow uses mrtrix tools to run csd on multishell data. At the end,
     mtnormalise is run.
 
     Inputs
 
@@ -56,93 +66,142 @@
             parameters for dwi2fod. A minimal example would be
             ``{"algorithm": "msmt_csd", "max_sh": [6, 8, 8]}``.
         mtnormalize: bool
             Should the FODs be mtnormalized?
 
 
     """
-    inputnode = pe.Node(niu.IdentityInterface(fields=input_fields),
+    inputnode = pe.Node(niu.IdentityInterface(fields=input_fields + ['odf_rois']),
                         name="inputnode")
     outputnode = pe.Node(
         niu.IdentityInterface(
             fields=['fod_sh_mif', 'wm_odf', 'wm_txt', 'gm_odf', 'gm_txt', 'csf_odf',
                     'csf_txt']),
         name="outputnode")
+    workflow = Workflow(name=name)
+    desc = """MRtrix3 Reconstruction
+
+: """
 
     # Resample anat mask
     resample_mask = pe.Node(
         afni.Resample(outputtype='NIFTI_GZ', resample_mode="NN"), name='resample_mask')
 
     # Response estimation
     response = params.get('response', {})
     response_algorithm = response.get('algorithm', 'dhollander')
     response['algorithm'] = response_algorithm
+    response['nthreads'] = omp_nthreads
+    if response_algorithm == 'csd':
+        desc += 'Single-tissue '
+    else:
+        desc += 'Multi-tissue '
+
+    desc += """\
+fiber response functions were estimated using the {} algorithm.
+FODs were estimated via constrained spherical deconvolution
+(CSD, @originalcsd, @tournier2008csd) \
+""".format(response_algorithm)
+    if response_algorithm == 'msmt_5tt':
+        desc += 'using a T1w-based segmentation {}.'.format(CITATIONS[response_algorithm])
+    else:
+        desc += 'using an unsupervised multi-tissue method {}.'.format(
+            CITATIONS[response_algorithm])
 
     # FOD estimation
     fod = params.get('fod', {})
     fod_algorithm = fod.get('algorithm', 'msmt_csd')
     fod['algorithm'] = fod_algorithm
+    fod['nthreads'] = omp_nthreads
     using_multitissue = fod_algorithm in ('ss3t', 'msmt_csd')
 
     # Intensity normalize?
     run_mtnormalize = params.get('mtnormalize', True) and using_multitissue
 
-    workflow = pe.Workflow(name=name)
     create_mif = pe.Node(MRTrixIngress(), name='create_mif')
     # Use dwi2response from 3Tissue for updated dhollander
     estimate_response = pe.Node(SS3TDwi2Response(**response), 'estimate_response')
 
     if response_algorithm == 'msmt_5tt':
         workflow.connect([
             (inputnode, estimate_response, [('mrtrix_5tt', 'mtt_file')])])
 
-    if fod_algorithm == 'msmt_csd':
+    if fod_algorithm in ('msmt_csd', 'csd'):
         estimate_fod = pe.Node(EstimateFOD(**fod), 'estimate_fod')
+        desc += ' Reconstruction was done using MRtrix3 (@mrtrix3).'
     elif fod_algorithm == 'ss3t':
         estimate_fod = pe.Node(SS3TEstimateFOD(**fod), 'estimate_fod')
+        desc += """ \
+A single-shell-optimized multi-tissue CSD was performed using MRtrix3Tissue
+(https://3Tissue.github.io), a fork of MRtrix3 (@mrtrix3)"""
+
+    # Make a visual report of the model
+    plot_peaks = pe.Node(ReconPeaksReport(), name='plot_peaks')
+    ds_report_peaks = pe.Node(
+        ReconDerivativesDataSink(extension='.png',
+                                 desc="wmFOD",
+                                 suffix='peaks'),
+        name='ds_report_peaks',
+        run_without_submitting=True)
+
+    # Plot targeted regions
+    if has_transform:
+        ds_report_odfs = pe.Node(
+            ReconDerivativesDataSink(extension='.png',
+                                     desc="wmFOD",
+                                     suffix='odfs'),
+            name='ds_report_odfs',
+            run_without_submitting=True)
+        workflow.connect(plot_peaks, 'odf_report', ds_report_odfs, 'in_file')
 
     workflow.connect([
         (estimate_response, estimate_fod, [('wm_file', 'wm_txt'),
                                            ('gm_file', 'gm_txt'),
                                            ('csf_file', 'csf_txt')]),
         (inputnode, resample_mask, [('t1_brain_mask', 'in_file'),
                                     ('dwi_file', 'master')]),
         (inputnode, create_mif, [('dwi_file', 'dwi_file'),
                                  ('bval_file', 'bval_file'),
                                  ('bvec_file', 'bvec_file'),
                                  ('b_file', 'b_file')]),
+        (inputnode, plot_peaks, [('dwi_ref', 'background_image'),
+                                 ('odf_rois', 'odf_rois')]),
+        (resample_mask, plot_peaks, [('out_file', 'mask_file')]),
+        (plot_peaks, ds_report_peaks, [('out_report', 'in_file')]),
         (create_mif, estimate_response, [('mif_file', 'in_file')]),
         (estimate_response, outputnode, [('wm_file', 'wm_txt'),
                                          ('gm_file', 'gm_txt'),
                                          ('csf_file', 'csf_txt')]),
 
         (create_mif, estimate_fod, [('mif_file', 'in_file')]),
         (resample_mask, estimate_fod, [('out_file', 'mask_file')]),
         (resample_mask, estimate_response, [('out_file', 'in_mask')])])
 
     if not run_mtnormalize:
         workflow.connect([
+            (estimate_fod, plot_peaks, [('wm_odf', 'mif_file')]),
             (estimate_fod, outputnode, [('wm_odf', 'fod_sh_mif'),
                                         ('wm_odf', 'wm_odf'),
                                         ('gm_odf', 'gm_odf'),
                                         ('csf_odf', 'csf_odf')])])
     else:
         intensity_norm = pe.Node(
             MTNormalize(inlier_mask='inliers.nii.gz', norm_image='norm.nii.gz'),
             name='intensity_norm')
         workflow.connect([
             (resample_mask, intensity_norm, [('out_file', 'mask_file')]),
             (estimate_fod, intensity_norm, [('wm_odf', 'wm_odf'),
                                             ('gm_odf', 'gm_odf'),
                                             ('csf_odf', 'csf_odf')]),
+            (intensity_norm, plot_peaks, [('wm_normed_odf', 'mif_file')]),
             (intensity_norm, outputnode, [('wm_normed_odf', 'fod_sh_mif'),
                                           ('wm_normed_odf', 'wm_odf'),
                                           ('gm_normed_odf', 'gm_odf'),
-                                          ('csf_normed_odf', 'csf_odf')])
-        ])
+                                          ('csf_normed_odf', 'csf_odf')])])
+        desc += " FODs were intensity-normalized using mtnormalize (@mtnormalize)."
 
     if output_suffix:
         normed = '' if not run_mtnormalize else 'mtnormed'
         ds_wm_odf = pe.Node(
             ReconDerivativesDataSink(extension='.mif.gz',
                                      desc="wmFOD" + normed,
                                      suffix=output_suffix,
@@ -206,18 +265,20 @@
                                              desc="mtinliermask",
                                              suffix=output_suffix,
                                              compress=True),
                     name='ds_inlier_mask',
                     run_without_submitting=True)
                 workflow.connect(intensity_norm, 'inlier_mask', ds_inlier_mask, 'in_file')
 
+    workflow.__desc__ = desc
     return workflow
 
 
-def init_global_tractography_wf(name="mrtrix_recon", output_suffix="", params={}):
+def init_global_tractography_wf(omp_nthreads, has_transform, name="mrtrix_recon",
+                                output_suffix="", params={}):
     """Run multi-shell, multi-tissue global tractography
 
     This workflow uses mrtrix tools to run csd on multishell data.
 
     Inputs
 
         dwi_file
@@ -310,15 +371,16 @@
             name='ds_residual_energy',
             run_without_submitting=True)
         workflow.connect(outputnode, 'residual_energy', ds_residual_energy, 'in_file')
 
     return workflow
 
 
-def init_mrtrix_tractography_wf(name="mrtrix_tracking", output_suffix="", params={}):
+def init_mrtrix_tractography_wf(omp_nthreads, has_transform, name="mrtrix_tracking",
+                                output_suffix="", params={}):
     """Run tractography
 
     This workflow uses mrtrix tools to run csd on multishell data.
 
     Inputs
 
         fod_sh_mif
@@ -344,17 +406,19 @@
         name="outputnode")
 
     workflow = pe.Workflow(name=name)
     # Resample anat mask
     resample_mask = pe.Node(
         afni.Resample(outputtype='NIFTI_GZ', resample_mode="NN"), name='resample_mask')
     tracking_params = params.get("tckgen", {})
+    tracking_params['nthreads'] = omp_nthreads
     use_sift2 = params.get("use_sift2", True)
     use_5tt = params.get("use_5tt", False)
     sift_params = params.get("sift2", {})
+    sift_params['nthreads'] = omp_nthreads
     tracking = pe.Node(TckGen(**tracking_params), name='tractography')
     workflow.connect([
         (inputnode, resample_mask, [('t1_brain_mask', 'in_file'),
                                     ('dwi_file', 'master')]),
         (inputnode, tracking, [
             ('fod_sh_mif', 'in_file'),
             ('fod_sh_mif', 'seed_dynamic')]),
@@ -391,17 +455,17 @@
             name='ds_tck_file',
             run_without_submitting=True)
         workflow.connect(outputnode, 'tck_file', ds_tck_file, 'in_file')
 
     return workflow
 
 
-def init_mrtrix_connectivity_wf(name="mrtrix_connectiity", params={},
-                                output_suffix="", n_procs=1):
-    """Runs ``tck2connectome`` on a ``tck`` file.abs
+def init_mrtrix_connectivity_wf(omp_nthreads, has_transform, name="mrtrix_connectiity",
+                                params={}, output_suffix=""):
+    """Runs ``tck2connectome`` on a ``tck`` file.
 
     Inputs
 
         tck_file
             mrtrix3 tck file.
 
     Outputs
@@ -414,28 +478,33 @@
         niu.IdentityInterface(
             fields=input_fields + ['tck_file', 'sift_weights', 'atlas_configs']),
         name="inputnode")
     outputnode = pe.Node(niu.IdentityInterface(fields=['matfile']),
                          name="outputnode")
     workflow = pe.Workflow(name=name)
     conmat_params = params.get("tck2connectome", {})
-    use_sift_weights = params.get("use_sift_weights", False)
-    calc_connectivity = pe.Node(MRTrixAtlasGraph(**conmat_params),
+    calc_connectivity = pe.Node(MRTrixAtlasGraph(tracking_params=conmat_params),
                                 name='calc_connectivity')
+    plot_connectivity = pe.Node(ConnectivityReport(), name='plot_connectivity')
+    ds_report_connectivity = pe.Node(
+        ReconDerivativesDataSink(extension='.svg',
+                                 desc="MRtrix3Connectivity",
+                                 suffix='matrices'),
+        name='ds_report_connectivity',
+        run_without_submitting=True)
     workflow.connect([
         (inputnode, calc_connectivity, [('atlas_configs', 'atlas_configs'),
-                                        ('tck_file', 'in_file')]),
+                                        ('tck_file', 'in_file'),
+                                        ('sift_weights', 'in_weights')]),
+        (calc_connectivity, plot_connectivity, [
+            ('connectivity_matfile', 'connectivity_matfile')]),
+        (plot_connectivity, ds_report_connectivity, [('out_report', 'in_file')]),
         (calc_connectivity, outputnode, [('connectivity_matfile', 'matfile')])
     ])
 
-    if use_sift_weights:
-        workflow.connect([
-            (inputnode, calc_connectivity, [('sift_weights', 'in_weights')])
-        ])
-
     if output_suffix:
         # Save the output in the outputs directory
         ds_connectivity = pe.Node(ReconDerivativesDataSink(suffix=output_suffix),
                                   name='ds_' + name,
                                   run_without_submitting=True)
         workflow.connect(calc_connectivity, 'connectivity_matfile', ds_connectivity, 'in_file')
     return workflow
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/interchange.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/interchange.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/converters.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/converters.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/build_workflow.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/build_workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import nipype.pipeline.engine as pe
-import nipype.interfaces.utility as niu
+from pkg_resources import resource_filename as pkgr
+from nipype.interfaces import ants, utility as niu
 from nipype.utils.filemanip import split_filename
 from qsiprep.interfaces.bids import QsiReconIngress, ReconDerivativesDataSink
 from qsiprep.interfaces.utils import GetConnectivityAtlases
 from .dsi_studio import (init_dsi_studio_recon_wf, init_dsi_studio_export_wf,
-                         init_dsi_studio_connectivity_wf)
+                         init_dsi_studio_connectivity_wf, init_dsi_studio_tractography_wf)
 from .dipy import init_dipy_brainsuite_shore_recon_wf, init_dipy_mapmri_recon_wf
 from .mrtrix import (init_mrtrix_csd_recon_wf, init_global_tractography_wf,
                      init_mrtrix_tractography_wf, init_mrtrix_connectivity_wf)
 from .converters import init_mif_to_fibgz_wf
 from .dynamics import init_controllability_wf
 from .utils import init_conform_dwi_wf, init_discard_repeated_samples_wf
 from ...engine import Workflow
@@ -25,16 +26,19 @@
 def _check_repeats(nodelist):
     total_len = len(nodelist)
     unique_len = len(set(nodelist))
     if not total_len == unique_len:
         raise Exception
 
 
-def init_dwi_recon_workflow(dwi_files, workflow_spec, output_dir, reportlets_dir,
+def init_dwi_recon_workflow(dwi_files, workflow_spec, output_dir, reportlets_dir, has_transform,
                             omp_nthreads, name="recon_wf"):
+    """Convert a workflow spec into a nipype workflow.
+
+    """
     atlas_names = workflow_spec.get('atlases', [])
     space = workflow_spec['space']
     workflow = Workflow(name=name)
     scans_iter = pe.Node(niu.IdentityInterface(fields=['dwi_file']), name='scans_iter')
     scans_iter.iterables = ("dwi_file", dwi_files)
     inputnode = pe.Node(niu.IdentityInterface(fields=input_fields + ['dwi_file']),
                         name='inputnode')
@@ -45,25 +49,44 @@
     if not workflow_spec['name'] == 'fake':
         scans_iter.inputs.dwi_file = dwi_files
 
     # Connect the collected diffusion data (gradients, etc) to the inputnode
     workflow.connect([
         (scans_iter, qsiprep_preprocessed_dwi_data, ([('dwi_file', 'dwi_file')])),
         (qsiprep_preprocessed_dwi_data, inputnode, [
-            (trait, trait) for trait in qsiprep_output_names])
-    ])
+            (trait, trait) for trait in qsiprep_output_names])])
+
     # Resample all atlases to dwi_file's resolution
     get_atlases = pe.Node(
         GetConnectivityAtlases(atlas_names=atlas_names, space=space),
         name='get_atlases',
         run_without_submitting=True)
 
+    # Resample ROI targets to DWI resolution for ODF plotting
+    crossing_rois_file = pkgr('qsiprep', 'data/crossing_rois.nii.gz')
+    odf_rois = pe.Node(
+        ants.ApplyTransforms(interpolation="MultiLabel", dimension=3),
+        name="odf_rois")
+    odf_rois.inputs.input_image = crossing_rois_file
+    if has_transform and space == "T1w":
+        workflow.connect(inputnode, 't1_2_mni_reverse_transform', odf_rois, 'transforms')
+    elif space == 'template':
+        odf_rois.inputs.transforms = ['identity']
+    else:
+        LOGGER.warning("Unable to transform ODF ROIs to dwi data. "
+                       "No ODF reports will be created.")
+        odf_rois = pe.Node(niu.IdentityInterface(fields=['output_image']), name='odf_rois')
+    workflow.connect(scans_iter, 'dwi_file', odf_rois, 'reference_image')
+
     # Save the atlases
     if len(atlas_names) > 0:
         if space == "T1w":
+            if not has_transform:
+                LOGGER.critical("No reverse transform found, unable to move atlases"
+                                " into DWI space")
             workflow.connect([
                 (inputnode, get_atlases,
                  [('t1_2_mni_reverse_transform', 'forward_transform')])])
         for atlas in workflow_spec['atlases']:
             workflow.connect([
                 (get_atlases,
                  pe.Node(ReconDerivativesDataSink(space=space,
@@ -101,15 +124,16 @@
             ])
         workflow.connect(inputnode, "dwi_file", get_atlases, "reference_image")
     # Read nodes from workflow spec, make sure we can implement them
     nodes_to_add = []
     for node_spec in workflow_spec['nodes']:
         if not node_spec['name']:
             raise Exception("Node has no name [{}]".format(node_spec))
-        new_node = workflow_from_spec(node_spec)
+        new_node = workflow_from_spec(omp_nthreads, has_transform or space == 'template',
+                                      node_spec)
         if new_node is None:
             raise Exception("Unable to create a node for %s" % node_spec)
         nodes_to_add.append(new_node)
     workflow.add_nodes(nodes_to_add)
     _check_repeats(workflow.list_node_names())
     # Now that all nodes are in the workflow, connect them
     for node_spec in workflow_spec['nodes']:
@@ -136,25 +160,25 @@
             downstream_inputnode_name = node_name + ".inputnode"
             downstream_inputnode = workflow.get_node(downstream_inputnode_name)
             downstream_inputs = set(downstream_inputnode.outputs.get().keys())
 
             connect_from_upstream = upstream_outputs.intersection(downstream_inputs)
             connect_from_qsiprep = default_input_set - connect_from_upstream
 
-            LOGGER.info("connecting %s from %s to %s", connect_from_qsiprep,
-                        inputnode, node)
+            # LOGGER.info("connecting %s from %s to %s", connect_from_qsiprep,
+            #             inputnode, node)
             workflow.connect([
                 (inputnode, node,
                  _as_connections(connect_from_qsiprep, dest_prefix='inputnode.'))])
             # for qp_connection in connect_from_qsiprep:
             #    workflow.connect(inputnode, qp_connection, node, 'inputnode.' + qp_connection)
             _check_repeats(workflow.list_node_names())
 
-            LOGGER.info("connecting %s from %s to %s", connect_from_upstream,
-                        upstream_outputnode_name, downstream_inputnode_name)
+            # LOGGER.info("connecting %s from %s to %s", connect_from_upstream,
+            #             upstream_outputnode_name, downstream_inputnode_name)
             workflow.connect([
                 (upstream_node, node,
                  _as_connections(
                     connect_from_upstream, src_prefix='outputnode.', dest_prefix='inputnode.'))])
             # for upstream_connection in connect_from_upstream:
             #     workflow.connect(upstream_node, "outputnode." + upstream_connection,
             #                      node, 'inputnode.' + upstream_connection)
@@ -162,29 +186,35 @@
 
         # If it's a connectivity calculation, send it the atlas configs
         if node_spec['action'] == 'connectivity':
             workflow.connect([(get_atlases, node,
                                [('atlas_configs', 'inputnode.atlas_configs')])])
         _check_repeats(workflow.list_node_names())
 
+        # Send the ODF rois to reconstruction nodes
+        if node_spec['action'] == 'csd' or 'reconstruction' in node_spec['action']:
+            workflow.connect([(odf_rois, node,
+                               [('output_image', 'inputnode.odf_rois')])])
+        _check_repeats(workflow.list_node_names())
+
     # Fill-in datasinks and reportlet datasinks seen so far
     for node in workflow.list_node_names():
         node_suffix = node.split('.')[-1]
         if node_suffix.startswith('ds_'):
             workflow.connect(scans_iter, 'dwi_file', workflow.get_node(node), 'source_file')
             workflow.get_node(node).inputs.space = space
             if "report" in node_suffix:
                 workflow.get_node(node).inputs.base_directory = reportlets_dir
             else:
                 workflow.get_node(node).inputs.base_directory = output_dir
 
     return workflow
 
 
-def workflow_from_spec(node_spec):
+def workflow_from_spec(omp_nthreads, has_transform, node_spec):
     """Build a nipype workflow based on a json file."""
     software = node_spec.get("software", "qsiprep")
     output_suffix = node_spec.get("output_suffix", "")
     node_name = node_spec.get("name", None)
     parameters = node_spec.get("parameters", {})
 
     if node_name is None:
@@ -192,49 +222,51 @@
     kwargs = {"name": node_name,
               "output_suffix": output_suffix,
               "params": parameters}
 
     # DSI Studio operations
     if software == "DSI Studio":
         if node_spec["action"] == "reconstruction":
-            return init_dsi_studio_recon_wf(**kwargs)
+            return init_dsi_studio_recon_wf(omp_nthreads, has_transform, **kwargs)
         if node_spec["action"] == "export":
-            return init_dsi_studio_export_wf(**kwargs)
+            return init_dsi_studio_export_wf(omp_nthreads, has_transform, **kwargs)
+        if node_spec["action"] == "tractography":
+            return init_dsi_studio_tractography_wf(omp_nthreads, has_transform, **kwargs)
         if node_spec["action"] == "connectivity":
-            return init_dsi_studio_connectivity_wf(**kwargs)
+            return init_dsi_studio_connectivity_wf(omp_nthreads, has_transform, **kwargs)
 
     # MRTrix3 operations
     elif software == "MRTrix3":
         if node_spec["action"] == "csd":
-            return init_mrtrix_csd_recon_wf(**kwargs)
+            return init_mrtrix_csd_recon_wf(omp_nthreads, has_transform, **kwargs)
         if node_spec["action"] == "global_tractography":
-            return init_global_tractography_wf(**kwargs)
+            return init_global_tractography_wf(omp_nthreads, has_transform, **kwargs)
         if node_spec["action"] == "tractography":
-            return init_mrtrix_tractography_wf(**kwargs)
+            return init_mrtrix_tractography_wf(omp_nthreads, has_transform, **kwargs)
         if node_spec["action"] == "connectivity":
-            return init_mrtrix_connectivity_wf(**kwargs)
+            return init_mrtrix_connectivity_wf(omp_nthreads, has_transform, **kwargs)
 
     # Dipy operations
     elif software == "Dipy":
         if node_spec["action"] == "3dSHORE_reconstruction":
-            return init_dipy_brainsuite_shore_recon_wf(**kwargs)
+            return init_dipy_brainsuite_shore_recon_wf(omp_nthreads, has_transform, **kwargs)
         if node_spec["action"] == "MAPMRI_reconstruction":
-            return init_dipy_mapmri_recon_wf(**kwargs)
+            return init_dipy_mapmri_recon_wf(omp_nthreads, has_transform, **kwargs)
 
     # qsiprep operations
     else:
         if node_spec['action'] == "controllability":
             return init_controllability_wf(**kwargs)
         if node_spec['action'] == 'discard_repeated_samples':
             return init_discard_repeated_samples_wf(**kwargs)
         if node_spec['action'] == 'conform':
             return init_conform_dwi_wf(**kwargs)
         if node_spec['action'] == 'mif_to_fib':
             return init_mif_to_fibgz_wf(**kwargs)
-    raise Exception("Unknown node %s", node_spec)
+    raise Exception("Unknown node %s" % node_spec)
 
 
 def _as_connections(attr_list, src_prefix='', dest_prefix=''):
     return [(src_prefix + item, dest_prefix + item) for item in attr_list]
 
 
 def _get_wf_name(dwi_file):
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/anatomical.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/anatomical.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/dipy.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/dipy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 Dipy Reconstruction workflows
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. autofunction:: init_dipy_brainsuite_shore_recon_wf
 
 """
+import logging
 import nipype.pipeline.engine as pe
 from nipype.interfaces import afni, utility as niu
-import logging
 from qsiprep.interfaces.bids import ReconDerivativesDataSink
 from ...interfaces.dipy import BrainSuiteShoreReconstruction, MAPMRIReconstruction
 from .interchange import input_fields
 from ...engine import Workflow
+from ...interfaces.reports import ReconPeaksReport
 
 LOGGER = logging.getLogger('nipype.interface')
 
 
 def external_format_datasinks(output_suffix, params, wf):
     """Add datasinks for Dipy Reconstructions in other formats."""
     outputnode = wf.get_node("outputnode")
@@ -33,15 +34,16 @@
                                      suffix=output_suffix,
                                      compress=False),
             name='ds_{}_mif'.format(output_suffix),
             run_without_submitting=True)
         wf.connect(outputnode, 'fod_sh_mif', ds_mif, 'in_file')
 
 
-def init_dipy_brainsuite_shore_recon_wf(name="dipy_3dshore_recon", output_suffix="", params={}):
+def init_dipy_brainsuite_shore_recon_wf(omp_nthreads, has_transform, name="dipy_3dshore_recon",
+                                        output_suffix="", params={}):
     """Reconstruct EAPs, ODFs, using 3dSHORE (brainsuite-style basis set).
 
     Inputs
 
         *qsiprep outputs*
 
     Outputs
@@ -88,29 +90,40 @@
         pos_grid: int
             Grid points for estimating EAP(default=11)
         pos_radius
             Radius for EAP estimation (default=20e-03)
 
     """
 
-    inputnode = pe.Node(niu.IdentityInterface(fields=input_fields),
+    inputnode = pe.Node(niu.IdentityInterface(fields=input_fields + ['odf_rois']),
                         name="inputnode")
     outputnode = pe.Node(
         niu.IdentityInterface(
             fields=['shore_coeffs_image', 'rtop_image', 'alpha_image', 'r2_image',
                     'cnr_image', 'regularization_image', 'fibgz', 'fod_sh_mif',
                     'dwi_file', 'bval_file', 'bvec_file', 'b_file']),
         name="outputnode")
 
     workflow = Workflow(name=name)
+    desc = """Dipy Reconstruction
+
+: """
     resample_mask = pe.Node(
         afni.Resample(outputtype='NIFTI_GZ', resample_mode="NN"), name='resample_mask')
     recon_shore = pe.Node(BrainSuiteShoreReconstruction(**params), name="recon_shore")
     doing_extrapolation = params.get("extrapolate_scheme") in ("HCP", "ABCD")
 
+    plot_peaks = pe.Node(ReconPeaksReport(), name='plot_peaks')
+    ds_report_peaks = pe.Node(
+        ReconDerivativesDataSink(extension='.png',
+                                 desc="3dSHOREODF",
+                                 suffix='peaks'),
+        name='ds_report_peaks',
+        run_without_submitting=True)
+
     workflow.connect([
         (inputnode, recon_shore, [('dwi_file', 'dwi_file'),
                                   ('bval_file', 'bval_file'),
                                   ('bvec_file', 'bvec_file')]),
         (inputnode, resample_mask, [('t1_brain_mask', 'in_file'),
                                     ('dwi_file', 'master')]),
         (resample_mask, recon_shore, [('out_file', 'mask_file')]),
@@ -121,15 +134,31 @@
                                    ('cnr_image', 'cnr_image'),
                                    ('regularization_image', 'regularization_image'),
                                    ('fibgz', 'fibgz'),
                                    ('fod_sh_mif', 'fod_sh_mif'),
                                    ('extrapolated_dwi', 'dwi_file'),
                                    ('extrapolated_bvals', 'bval_file'),
                                    ('extrapolated_bvecs', 'bvec_file'),
-                                   ('extrapolated_b', 'b_file')])])
+                                   ('extrapolated_b', 'b_file')]),
+        (inputnode, plot_peaks, [('dwi_ref', 'background_image'),
+                                 ('odf_rois', 'odf_rois')]),
+        (resample_mask, plot_peaks, [('out_file', 'mask_file')]),
+        (recon_shore, plot_peaks, [('odf_directions', 'directions_file'),
+                                   ('odf_amplitudes', 'odf_file')]),
+        (plot_peaks, ds_report_peaks, [('out_report', 'in_file')])])
+
+    # Plot targeted regions
+    if has_transform:
+        ds_report_odfs = pe.Node(
+            ReconDerivativesDataSink(extension='.png',
+                                     desc="3dSHOREODF",
+                                     suffix='odfs'),
+            name='ds_report_odfs',
+            run_without_submitting=True)
+        workflow.connect(plot_peaks, 'odf_report', ds_report_odfs, 'in_file')
 
     if output_suffix:
         external_format_datasinks(output_suffix, params, workflow)
 
         ds_rtop = pe.Node(
             ReconDerivativesDataSink(extension='.nii.gz',
                                      desc="rtop",
@@ -209,18 +238,20 @@
             ds_extrap_b = pe.Node(
                 ReconDerivativesDataSink(extension='.b',
                                          desc="extrapolated",
                                          suffix=output_suffix),
                 name='ds_extrap_b',
                 run_without_submitting=True)
             workflow.connect(outputnode, 'b_file', ds_extrap_b, 'in_file')
+    workflow.__desc__ = desc
     return workflow
 
 
-def init_dipy_mapmri_recon_wf(name="dipy_mapmri_recon", output_suffix="", params={}):
+def init_dipy_mapmri_recon_wf(omp_nthreads, has_transform, name="dipy_mapmri_recon",
+                              output_suffix="", params={}):
     """Reconstruct EAPs, ODFs, using 3dSHORE (brainsuite-style basis set).
 
     Inputs
 
         *qsiprep outputs*
 
     Outputs
@@ -287,26 +318,36 @@
         cvxpy_solver : str, optional
             cvxpy solver name. Optionally optimize the positivity constraint
             with a particular cvxpy solver. See http://www.cvxpy.org/ for
             details.
             Default: None (cvxpy chooses its own solver)
     """
 
-    inputnode = pe.Node(niu.IdentityInterface(fields=input_fields),
+    inputnode = pe.Node(niu.IdentityInterface(fields=input_fields + ['odf_rois']),
                         name="inputnode")
     outputnode = pe.Node(
         niu.IdentityInterface(
             fields=['mapmri_coeffs', 'rtop', 'rtap', 'rtpp', 'fibgz', 'fod_sh_mif',
                     'parng', 'perng', 'ng', 'qiv', 'lapnorm', 'msd']),
         name="outputnode")
 
     workflow = Workflow(name=name)
+    desc = """Dipy Reconstruction
+
+: """
     recon_map = pe.Node(MAPMRIReconstruction(**params), name="recon_map")
     resample_mask = pe.Node(
         afni.Resample(outputtype='NIFTI_GZ', resample_mode="NN"), name='resample_mask')
+    plot_peaks = pe.Node(ReconPeaksReport(), name='plot_peaks')
+    ds_report_peaks = pe.Node(
+        ReconDerivativesDataSink(extension='.png',
+                                 desc="MAPLMRIODF",
+                                 suffix='peaks'),
+        name='ds_report_peaks',
+        run_without_submitting=True)
 
     workflow.connect([
         (inputnode, recon_map, [('dwi_file', 'dwi_file'),
                                 ('bval_file', 'bval_file'),
                                 ('bvec_file', 'bvec_file')]),
         (inputnode, resample_mask, [('t1_brain_mask', 'in_file'),
                                     ('dwi_file', 'master')]),
@@ -318,23 +359,38 @@
                                  ('parng', 'parng'),
                                  ('perng', 'perng'),
                                  ('msd', 'msd'),
                                  ('ng', 'ng'),
                                  ('qiv', 'qiv'),
                                  ('lapnorm', 'lapnorm'),
                                  ('fibgz', 'fibgz'),
-                                 ('fod_sh_mif', 'fod_sh_mif')])
+                                 ('fod_sh_mif', 'fod_sh_mif')]),
+        (resample_mask, plot_peaks, [('out_file', 'mask_file')]),
+        (inputnode, plot_peaks, [('dwi_ref', 'background_image'),
+                                 ('odf_rois', 'odf_rois')]),
+        (recon_map, plot_peaks, [('odf_directions', 'directions_file'),
+                                 ('odf_amplitudes', 'odf_file')]),
+        (plot_peaks, ds_report_peaks, [('out_report', 'in_file')])])
+
+    # Plot targeted regions
+    if has_transform:
+        ds_report_odfs = pe.Node(
+            ReconDerivativesDataSink(extension='.png',
+                                     desc="MAPLMRIODF",
+                                     suffix='odfs'),
+            name='ds_report_odfs',
+            run_without_submitting=True)
+        workflow.connect(plot_peaks, 'odf_report', ds_report_odfs, 'in_file')
 
-    ])
     if output_suffix:
         external_format_datasinks(output_suffix, params, workflow)
         connections = []
         for scalar_name in ['rtop', 'rtap', 'rtpp', 'qiv', 'msd', 'lapnorm']:
             connections += [(outputnode,
                              pe.Node(
                                  ReconDerivativesDataSink(desc=scalar_name,
                                                           suffix=output_suffix),
                                  name='ds_%s_%s' % (name, scalar_name)),
                              [(scalar_name, 'in_file')])]
         workflow.connect(connections)
-
+    workflow.__desc__ = desc
     return workflow
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/utils.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/utils.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/base.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 
 """
 
 import os
 import os.path as op
 from glob import glob
 from copy import deepcopy
+from nipype import __version__ as nipype_ver
+from nilearn import __version__ as nilearn_ver
+from dipy import __version__ as dipy_ver
 from pkg_resources import resource_filename as pkgrf
 from ...engine import Workflow
 from ...utils.sloppy_recon import make_sloppy
+from ...__about__ import __version__
 
 import logging
 import json
 from bids.layout import BIDSLayout
 from .build_workflow import init_dwi_recon_workflow
 from .anatomical import init_recon_anatomical_wf
 from .interchange import anatomical_input_fields
@@ -156,34 +160,68 @@
 
         spec = _load_recon_spec(recon_spec, sloppy=sloppy)
         space = spec['space']
         layout = BIDSLayout(recon_input, validate=False, absolute_paths=True)
         # Get all the output files that are in this space
         dwi_files = [f.path for f in
                      layout.get(suffix="dwi", subject=subject_id, absolute_paths=True,
-                                extensions=['nii', 'nii.gz'])
+                                extension=['nii', 'nii.gz'])
                      if 'space-' + space in f.filename]
         LOGGER.info("found %s in %s", dwi_files, recon_input)
 
     workflow = Workflow('sub-{}_{}'.format(subject_id, spec['name']))
+    workflow.__desc__ = """
+Results included in this manuscript come from reconstructions
+performed using *QSIprep* {qsiprep_ver},
+which is based on *Nipype* {nipype_ver}
+(@nipype1; @nipype2; RRID:SCR_002502).
+
+""".format(
+        qsiprep_ver=__version__, nipype_ver=nipype_ver)
+    workflow.__postdesc__ = """
+
+Many internal operations of *qsiprep* use
+*Nilearn* {nilearn_ver} [@nilearn, RRID:SCR_001362] and
+*Dipy* {dipy_ver}[@dipy].
+For more details of the pipeline, see [the section corresponding
+to workflows in *qsiprep*'s documentation]\
+(https://qsiprep.readthedocs.io/en/latest/workflows.html \
+"qsiprep's documentation").
+
+
+### References
+
+    """.format(nilearn_ver=nilearn_ver, dipy_ver=dipy_ver)
+
     if len(dwi_files) == 0:
         LOGGER.info("No dwi files found for %s", subject_id)
         return workflow
 
+    # Was there a forced normalization during preprocessing?
+    template_transform = [f.path for f in
+                          layout.get(subject_id=subject_id, suffix='xfm', extension=['.h5'])
+                          if 'to-T1w' in f.path and 'from-MNI152NLin2009cAsym' in f.path]
+    if template_transform:
+        template_transform = template_transform[0]
+        has_transform = True
+    else:
+        has_transform = False
+
     anat_ingress_wf = init_recon_anatomical_wf(subject_id=subject_id,
                                                recon_input_dir=recon_input,
                                                extras_to_make=spec.get('anatomical', []),
                                                name='anat_ingress_wf')
 
     to_connect = [('outputnode.' + name, 'inputnode.' + name) for name in anatomical_input_fields]
     # create a processing pipeline for the dwis in each session
     dwi_recon_wf = init_dwi_recon_workflow(dwi_files=dwi_files,
                                            workflow_spec=spec,
                                            reportlets_dir=reportlets_dir,
                                            output_dir=output_dir,
+                                           has_transform=has_transform,
                                            omp_nthreads=omp_nthreads)
     workflow.connect([(anat_ingress_wf, dwi_recon_wf, to_connect)])
 
     return workflow
 
 
 def _load_recon_spec(spec_name, sloppy=False):
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/recon/dynamics.py` & `qsiprep-0.9.0b1/qsiprep/workflows/recon/dynamics.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/anatomical.py` & `qsiprep-0.9.0b1/qsiprep/workflows/anatomical.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/qc.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/qc.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 
 .. autofunction:: init_dwi_reference_wf
 
 """
 from nipype.pipeline import engine as pe
 from nipype.interfaces import utility as niu, afni
 from ...engine import Workflow
-from ...interfaces.nilearn import Merge
 from ...interfaces.dsi_studio import DSIStudioSrcQC, DSIStudioCreateSrc
 from ...interfaces.reports import InteractiveReport
 from ...interfaces.dipy import TensorReconstruction
 from ...interfaces.anatomical import DiceOverlap
 
-
 DEFAULT_MEMORY_MIN_GB = 0.01
 
 
 def init_modelfree_qc_wf(dwi_files=None, name='dwi_qc_wf'):
     """
     This workflow runs DSI Studio's QC metrics
 
@@ -40,46 +38,32 @@
         bvec_file
             bvec file corresponding to the concatenated dwi_files inputs or dwi_file
 
     **Outputs**
 
         qc file
             DSI Studio's src QC metrics for the input data
-        concatenated_data
-            The concatenated images used to calculate QC
 
 
     """
     workflow = Workflow(name=name)
     workflow.__desc__ = """\
 """
     inputnode = pe.Node(
         niu.IdentityInterface(fields=['dwi_file', 'bval_file', 'bvec_file']),
         name='inputnode')
     outputnode = pe.Node(
-        niu.IdentityInterface(fields=['qc_summary', 'concatenated_data']),
+        niu.IdentityInterface(fields=['qc_summary']),
         name='outputnode')
 
     raw_src = pe.Node(DSIStudioCreateSrc(), name='raw_src')
     raw_qc = pe.Node(DSIStudioSrcQC(), name='raw_qc')
-
-    if dwi_files:
-        if len(dwi_files) > 1:
-            concat_raw_dwis = pe.Node(Merge(in_files=dwi_files, is_dwi=True),
-                                      name='concat_raw_dwis')
-            workflow.connect(concat_raw_dwis, "out_file", raw_src, "input_nifti_file")
-            workflow.connect(concat_raw_dwis, "out_file", outputnode, "concatenated_data")
-        else:
-            raw_src.inputs.input_nifti_file = dwi_files[0]
-            outputnode.inputs.concatenated_data = dwi_files[0]
-    else:
-        workflow.connect(inputnode, 'dwi_file', raw_src, 'input_nifti_file')
-
     workflow.connect([
         (inputnode, raw_src, [
+            ('dwi_file', 'input_nifti_file'),
             ('bval_file', 'input_bvals_file'),
             ('bvec_file', 'input_bvecs_file')]),
         (raw_src, raw_qc, [('output_src', 'src_file')]),
         (raw_qc, outputnode, [('qc_txt', 'qc_summary')]),
     ])
 
     return workflow
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/confounds.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/confounds.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/registration.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/registration.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/intramodal_template.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/intramodal_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,18 @@
                             name='split_outputs')
     for output_num, output_name in enumerate(output_names):
         workflow.connect(split_outputs, 'out%d' % (output_num + 1), outputnode, output_name)
 
     runtime_opts = {'num_cores': 1, 'parallel_control': 0}
     if omp_nthreads > 1:
         runtime_opts = {'num_cores': omp_nthreads, 'parallel_control': 2}
-    ants_mvtc2 = pe.Node(MultivariateTemplateConstruction2(dimension=3, **runtime_opts),
-                         name='ants_mvtc2')
+    ants_mvtc2 = pe.Node(
+        MultivariateTemplateConstruction2(dimension=3, iteration_limit=num_iterations,
+                                          **runtime_opts),
+        name='ants_mvtc2')
 
     workflow.connect([
         (merge_inputs, rename_inputs, [('out', 'in_file')]),
         (rename_inputs, ants_mvtc2, [('out_file', 'input_images')]),
         (ants_mvtc2, split_outputs, [
             ('forward_transforms', 'inlist')]),
         (ants_mvtc2, outputnode, [
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/merge.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/merge.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from nipype.utils.filemanip import split_filename
 from nipype.interfaces import utility as niu
 from .util import _get_wf_name
 from .qc import init_modelfree_qc_wf
 from ...interfaces import ConformDwi, DerivativesDataSink
 from ...interfaces.mrtrix import DWIDenoise, DWIBiasCorrect, MRDeGibbs
 from ...interfaces.gradients import ExtractB0s
-from ...interfaces.nilearn import MaskEPI
+from ...interfaces.nilearn import MaskEPI, Merge
 from ...interfaces.dwi_merge import MergeDWIs, StackConfounds
 from ...engine import Workflow
 
 DEFAULT_MEMORY_MIN_GB = 0.01
 LOGGER = logging.getLogger('nipype.workflow')
 
 
@@ -77,15 +77,17 @@
             is run on the merged dwi series.
         calculate_qc : bool
             Should DSI Studio's QC be calculated on the merged raw data?
 
     **Outputs**
 
         merged_image
-            dwi series, resampled to T1w space
+            dwi series, conformed, denoised if requested
+        merged_raw_image
+            dwi series, conformed, raw
         merged_bval
             bvals from merged images
         merged_bvec
             bvecs from merged images
         noise_image
             image(s) created by ``dwidenoise``
         original_files
@@ -94,29 +96,31 @@
             DSI Studio QC text file
 
     """
 
     workflow = Workflow(name=name)
     outputnode = pe.Node(
         niu.IdentityInterface(fields=[
-            'merged_image', 'merged_bval', 'merged_bvec', 'noise_images', 'bias_images',
-            'denoising_confounds', 'original_files', 'qc_summary', 'validation_reports']),
+            'merged_image', 'merged_raw_image', 'merged_bval', 'merged_bvec', 'noise_images',
+            'bias_images', 'denoising_confounds', 'original_files', 'qc_summary',
+            'validation_reports']),
         name='outputnode')
 
     # DWIs will be merged at some point.
     merge_dwis = pe.Node(
         MergeDWIs(bids_dwi_files=raw_dwi_files,
                   b0_threshold=b0_threshold,
                   harmonize_b0_intensities=not no_b0_harmonization),
         name='merge_dwis')
     # Create a denoising workflow for each input image
     num_dwis = len(raw_dwi_files)
     conformed_bvals = pe.Node(niu.Merge(num_dwis), name='conformed_bvals')
     conformed_bvecs = pe.Node(niu.Merge(num_dwis), name='conformed_bvecs')
     conformed_images = pe.Node(niu.Merge(num_dwis), name='conformed_images')
+    conformed_raw_images = pe.Node(niu.Merge(num_dwis), name='conformed_raw_images')
     conformation_reports = pe.Node(niu.Merge(num_dwis), name='conformation_reports')
     # derivatives from denoising
     denoising_confounds = pe.Node(niu.Merge(num_dwis), name='denoising_confounds')
     noise_images = pe.Node(niu.Merge(num_dwis), name='noise_images')
     bias_images = pe.Node(niu.Merge(num_dwis), name='bias_images')
     # Collect conformers and denoisers
     conformers = []
@@ -155,41 +159,47 @@
                     ('outputnode.bias_image', 'in%d' % dwi_num)])])
             dwi_source = denoising_wfs[-1]
             edge_prefix = 'outputnode.'
         else:
             dwi_source = conformers[-1]
             edge_prefix = ''
 
-        print("merging source", dwi_source)
         workflow.connect([
             (dwi_source, conformed_images, [(edge_prefix + 'dwi_file', 'in%d' % dwi_num)]),
+            (conformers[-1], conformed_raw_images, [('dwi_file', 'in%d' % dwi_num)]),
             (dwi_source, conformed_bvals, [(edge_prefix + 'bval_file', 'in%d' % dwi_num)]),
             (dwi_source, conformed_bvecs, [(edge_prefix + 'bvec_file', 'in%d' % dwi_num)]),
             (conformers[-1], conformation_reports, [('out_report', 'in%d' % dwi_num)])
         ])
 
-    # Get a QC score for the raw data
-    if calculate_qc:
-        qc_wf = init_modelfree_qc_wf(dwi_files=raw_dwi_files)
-        workflow.connect([
-            (qc_wf, outputnode, [('outputnode.qc_summary', 'qc_summary')]),
-            (merge_dwis, qc_wf, [('out_bval', 'inputnode.bval_file'),
-                                 ('out_bvec', 'inputnode.bvec_file')])])
+    # Get an orientation-conformed version of the raw inputs and their gradients
+    raw_merge = pe.Node(Merge(is_dwi=True), name='raw_merge')
 
     # Merge the either conformed-only or conformed-and-denoised data
     workflow.connect([
         (conformed_images, merge_dwis, [('out', 'dwi_files')]),
+        (conformed_raw_images, raw_merge, [('out', 'in_files')]),
+        (raw_merge, outputnode, [('out_file', 'merged_raw_image')]),
         (conformed_bvals, merge_dwis, [('out', 'bval_files')]),
         (conformed_bvecs, merge_dwis, [('out', 'bvec_files')]),
         (conformation_reports, outputnode, [('out', 'validation_reports')]),
         (merge_dwis, outputnode, [
             ('original_images', 'original_files'),
             ('out_bval', 'merged_bval'),
             ('out_bvec', 'merged_bvec')])])
 
+    # Get a QC score for the raw data
+    if calculate_qc:
+        qc_wf = init_modelfree_qc_wf()
+        workflow.connect([
+            (qc_wf, outputnode, [('outputnode.qc_summary', 'qc_summary')]),
+            (raw_merge, qc_wf, [('out_file', 'inputnode.dwi_file')]),
+            (merge_dwis, qc_wf, [('out_bval', 'inputnode.bval_file'),
+                                 ('out_bvec', 'inputnode.bvec_file')])])
+
     # We have denoised and combined, therefore we are done
     if denoise_before_combining:
         workflow.connect([
             (denoising_confounds, merge_dwis, [('out', 'denoising_confounds')]),
             (merge_dwis, outputnode, [
                 ('out_dwi', 'merged_image'),
                 ('merged_denoising_confounds', 'denoising_confounds')]),
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/util.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/util.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/hmc.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/hmc.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/fsl.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/fsl.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/base.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from nipype.pipeline import engine as pe
 from nipype.interfaces import utility as niu
 from nipype.interfaces.base import isdefined
 from ...interfaces import DerivativesDataSink
 
 from ...interfaces.reports import DiffusionSummary
 from ...interfaces.confounds import DMRISummary
+from ...interfaces.utils import TestInput
 from ...engine import Workflow
 
 # dwi workflows
 from ..fieldmap.unwarp import init_fmap_unwarp_report_wf
 from .hmc_sdc import init_qsiprep_hmcsdc_wf
 from .fsl import init_fsl_hmc_wf
 from .pre_hmc import init_dwi_pre_hmc_wf
@@ -306,15 +307,16 @@
             't1_2_fsnative_reverse_transform', 'dwi_sampling_grid']),
         name='inputnode')
     outputnode = pe.Node(
         niu.IdentityInterface(fields=[
             'confounds', 'hmc_optimization_data', 'itk_b0_to_t1', 'noise_images', 'bias_images',
             'dwi_files', 'cnr_map', 'bval_files', 'bvec_files', 'b0_ref_image', 'b0_indices',
             'dwi_mask', 'hmc_xforms', 'fieldwarps', 'sbref_file', 'original_files',
-            'raw_qc_file', 'coreg_score', 'raw_concatenated', 'carpetplot_data']),
+            'original_bvecs', 'raw_qc_file', 'coreg_score', 'raw_concatenated',
+            'carpetplot_data']),
         name='outputnode')
     workflow.__desc__ = """
 
 Diffusion data preprocessing
 
 : """
 
@@ -326,14 +328,15 @@
                                      dwi_no_biascorr=dwi_no_biascorr,
                                      no_b0_harmonization=no_b0_harmonization,
                                      orientation='LAS' if hmc_model == 'eddy' else 'LPS',
                                      source_file=source_file,
                                      low_mem=low_mem,
                                      denoise_before_combining=denoise_before_combining,
                                      omp_nthreads=omp_nthreads)
+    test_pre_hmc_connect = pe.Node(TestInput(), name='test_pre_hmc_connect')
 
     if hmc_model in ('none', '3dSHORE'):
         if not hmc_model == 'none' and shoreline_iters < 1:
             raise Exception("--shoreline-iters must be > 0 when --hmc-model is " + hmc_model)
         hmc_wf = init_qsiprep_hmcsdc_wf(
             scan_groups=scan_groups,
             source_file=source_file,
@@ -377,17 +380,19 @@
         (inputnode, hmc_wf, [
             ('t1_brain', 'inputnode.t1_brain'),
             ('t1_mask', 'inputnode.t1_mask'),
             ('t1_2_mni_reverse_transform', 'inputnode.t1_2_mni_reverse_transform')]),
         (pre_hmc_wf, outputnode, [
             ('outputnode.qc_file', 'raw_qc_file'),
             ('outputnode.original_files', 'original_files'),
+            ('outputnode.bvec_file', 'original_bvecs'),
             ('outputnode.bias_images', 'bias_images'),
             ('outputnode.noise_images', 'noise_images'),
-            ('outputnode.raw_concatenated', 'raw_concatenated')])
+            ('outputnode.raw_concatenated', 'raw_concatenated')]),
+        (pre_hmc_wf, test_pre_hmc_connect, [('outputnode.raw_concatenated', 'test1')])
     ])
 
     # calculate dwi registration to T1w
     b0_coreg_wf = init_b0_to_anat_registration_wf(omp_nthreads=omp_nthreads,
                                                   mem_gb=mem_gb['resampled'],
                                                   write_report=True)
     ds_report_coreg = pe.Node(
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/pre_hmc.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/pre_hmc.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 """
 
 from nipype import logging
 
 from nipype.pipeline import engine as pe
 from nipype.interfaces import utility as niu
 
-from ...interfaces.images import ConcatRPESplits
+from ...interfaces.dwi_merge import MergeDWIs
+from ...interfaces.nilearn import Merge
 from ...engine import Workflow
 
 # dwi workflows
 from .merge import init_merge_and_denoise_wf
 from .util import get_source_file
 from .qc import init_modelfree_qc_wf
 
@@ -31,14 +32,15 @@
                         dwi_no_biascorr,
                         no_b0_harmonization,
                         denoise_before_combining,
                         orientation,
                         omp_nthreads,
                         source_file,
                         low_mem,
+                        calculate_qc=True,
                         name="pre_hmc_wf"):
     """
     This workflow merges and denoises dwi scans. The outputs from this workflow is
     a single dwi file (optionally denoised) and corresponding bvals, bvecs.
 
     In the general case, a single warped group will be sent to this workflow. However,
     since eddy expects a single 4D input file, two warped groups can be processed
@@ -141,47 +143,93 @@
                                                 orientation=orientation,
                                                 omp_nthreads=omp_nthreads,
                                                 source_file=minus_source_file,
                                                 calculate_qc=False,
                                                 name="merge_minus")
 
         # Combine the original images from the splits into one 4D series + bvals/bvecs
-        concat_rpe_splits = pe.Node(ConcatRPESplits(), name="concat_rpe_splits")
+        pm_validation = pe.Node(niu.Merge(2), name='pm_validation')
+        pm_dwis = pe.Node(niu.Merge(2), name='pm_dwis')
+        pm_bids_dwis = pe.Node(niu.Merge(2), name='pm_bids_dwis')
+        pm_bvals = pe.Node(niu.Merge(2), name='pm_bvals')
+        pm_bvecs = pe.Node(niu.Merge(2), name='pm_bvecs')
+        pm_bias = pe.Node(niu.Merge(2), name='pm_bias')
+        pm_noise_images = pe.Node(niu.Merge(2), name='pm_noise')
+        pm_denoising_confounds = pe.Node(niu.Merge(2), name='pm_denoising_confounds')
+        pm_raw_images = pe.Node(niu.Merge(2), name='pm_raw_images')
+        rpe_concat = pe.Node(
+            MergeDWIs(harmonize_b0_intensities=not no_b0_harmonization,
+                      b0_threshold=b0_threshold),
+            name='rpe_concat')
+        raw_rpe_concat = pe.Node(Merge(is_dwi=True), name='raw_rpe_concat')
         qc_wf = init_modelfree_qc_wf(dwi_files=plus_files + minus_files)
 
         workflow.connect([
-            # Merge, denoise, combine
-            (merge_plus, concat_rpe_splits, [
-                ('outputnode.merged_image', 'dwi_plus'),
-                ('outputnode.merged_bval', 'bval_plus'),
-                ('outputnode.merged_bvec', 'bvec_plus'),
-                ('outputnode.bias_images', 'bias_images_plus'),
-                ('outputnode.noise_images', 'noise_images_plus'),
-                ('outputnode.denoising_confounds', 'denoising_confounds_plus')]),
-            (merge_minus, concat_rpe_splits, [
-                ('outputnode.merged_image', 'dwi_minus'),
-                ('outputnode.merged_bval', 'bval_minus'),
-                ('outputnode.merged_bvec', 'bvec_minus'),
-                ('outputnode.bias_images', 'bias_images_minus'),
-                ('outputnode.noise_images', 'noise_images_minus'),
-                ('outputnode.denoising_confounds', 'denoising_confounds_minus')]),
+            # combine PE+
+            (merge_plus, pm_dwis, [
+                ('outputnode.merged_image', 'in1')]),
+            (merge_plus, pm_bids_dwis, [
+                ('outputnode.original_files', 'in1')]),
+            (merge_plus, pm_bvals, [
+                ('outputnode.merged_bval', 'in1')]),
+            (merge_plus, pm_bvecs, [
+                ('outputnode.merged_bvec', 'in1')]),
+            (merge_plus, pm_bias, [
+                ('outputnode.bias_images', 'in1')]),
+            (merge_plus, pm_noise_images, [
+                ('outputnode.noise_images', 'in1')]),
+            (merge_plus, pm_raw_images, [
+                ('outputnode.merged_raw_image', 'in1')]),
+            (merge_plus, pm_denoising_confounds, [
+                ('outputnode.denoising_confounds', 'in1')]),
+            (merge_plus, pm_validation, [
+                ('outputnode.validation_reports', 'in1')]),
+
+            # combine PE-
+            (merge_minus, pm_dwis, [
+                ('outputnode.merged_image', 'in2')]),
+            (merge_minus, pm_bids_dwis, [
+                ('outputnode.original_files', 'in2')]),
+            (merge_minus, pm_bvals, [
+                ('outputnode.merged_bval', 'in2')]),
+            (merge_minus, pm_bvecs, [
+                ('outputnode.merged_bvec', 'in2')]),
+            (merge_minus, pm_bias, [
+                ('outputnode.bias_images', 'in2')]),
+            (merge_minus, pm_noise_images, [
+                ('outputnode.noise_images', 'in2')]),
+            (merge_minus, pm_raw_images, [
+                ('outputnode.merged_raw_image', 'in2')]),
+            (merge_minus, pm_denoising_confounds, [
+                ('outputnode.denoising_confounds', 'in2')]),
+            (merge_minus, pm_validation, [
+                ('outputnode.validation_reports', 'in2')]),
+
+            (pm_dwis, rpe_concat, [('out', 'dwi_files')]),
+            (pm_bids_dwis, rpe_concat, [('out', 'bids_dwi_files')]),
+            (pm_bvals, rpe_concat, [('out', 'bval_files')]),
+            (pm_bvecs, rpe_concat, [('out', 'bvec_files')]),
+            (pm_denoising_confounds, rpe_concat, [('out', 'denoising_confounds')]),
+
             # Connect to the outputnode
-            (concat_rpe_splits, outputnode, [
-                ('dwi_file', 'dwi_file'),
-                ('bval_file', 'bval_file'),
-                ('bvec_file', 'bvec_file'),
-                ('original_files', 'original_files'),
-                ('denoising_confounds', 'denoising_confounds'),
-                ('validation_reports', 'validation_reports'),
-                ('noise_images', 'noise_images'),
-                ('bias_images', 'bias_images')]),
-            (concat_rpe_splits, qc_wf, [
-                ('bval_file', 'inputnode.bval_file'),
-                ('bvec_file', 'inputnode.bvec_file')]),
-            (qc_wf, outputnode, [('outputnode.qc_summary', 'qc_file')])])
+            (rpe_concat, outputnode, [
+                ('out_dwi', 'dwi_file'),
+                ('out_bval', 'bval_file'),
+                ('out_bvec', 'bvec_file'),
+                ('original_images', 'original_files'),
+                ('merged_denoising_confounds', 'denoising_confounds')]),
+            (pm_validation, outputnode, [
+                ('out', 'validation_reports')]),
+            (pm_noise_images, outputnode, [
+                ('out', 'noise_images')]),
+            (pm_bias, outputnode, [
+                ('out', 'bias_images')]),
+            (pm_raw_images, raw_rpe_concat, [('out', 'in_files')]),
+            (raw_rpe_concat, outputnode, [('out_file', 'raw_concatenated')])
+        ])
         workflow.__postdesc__ = "Both groups were then merged into a single file, as required " \
                                 "for the FSL workflows. "
         return workflow
 
     merge_dwis = init_merge_and_denoise_wf(
         raw_dwi_files=dwi_series,
         b0_threshold=b0_threshold,
@@ -190,28 +238,30 @@
         dwi_no_biascorr=dwi_no_biascorr,
         no_b0_harmonization=no_b0_harmonization,
         denoise_before_combining=denoise_before_combining,
         orientation=orientation,
         calculate_qc=True,
         source_file=source_file)
 
-    qc_wf = init_modelfree_qc_wf(dwi_files=dwi_series)
-
     workflow.connect([
         (merge_dwis, outputnode, [
             ('outputnode.merged_image', 'dwi_file'),
             ('outputnode.merged_bval', 'bval_file'),
             ('outputnode.merged_bvec', 'bvec_file'),
             ('outputnode.bias_images', 'bias_images'),
             ('outputnode.noise_images', 'noise_images'),
             ('outputnode.validation_reports', 'validation_reports'),
             ('outputnode.denoising_confounds', 'denoising_confounds'),
-            ('outputnode.original_files', 'original_files')]),
-        (merge_dwis, qc_wf, [
-            ('outputnode.merged_bval', 'inputnode.bval_file'),
-            ('outputnode.merged_bvec', 'inputnode.bvec_file')]),
-        (qc_wf, outputnode, [
-            ('outputnode.qc_summary', 'qc_file'),
-            ('outputnode.concatenated_data', 'raw_concatenated')])
+            ('outputnode.original_files', 'original_files'),
+            ('outputnode.merged_raw_image', 'raw_concatenated')])
     ])
 
+    if calculate_qc:
+        qc_wf = init_modelfree_qc_wf(dwi_files=dwi_series)
+        workflow.connect([
+            (merge_dwis, qc_wf, [
+                ('outputnode.merged_raw_image', 'inputnode.dwi_file'),
+                ('outputnode.merged_bval', 'inputnode.bval_file'),
+                ('outputnode.merged_bvec', 'inputnode.bvec_file')]),
+            (qc_wf, outputnode, [('outputnode.qc_summary', 'qc_file')])])
+
     return workflow
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/hmc_sdc.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/hmc_sdc.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/resampling.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/resampling.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 from nipype.interfaces import utility as niu, ants
 
 from .util import init_dwi_reference_wf
 from ...engine import Workflow
 from ...interfaces.nilearn import Merge
 from ...interfaces.gradients import (ComposeTransforms, ExtractB0s, GradientRotation,
                                      LocalGradientRotation)
-from ...interfaces.itk import DisassembleTransform
 from ...interfaces.images import ChooseInterpolator
 from .qc import init_modelfree_qc_wf
 
 DEFAULT_MEMORY_MIN_GB = 0.01
 
 
 def init_dwi_trans_wf(source_file,
                       template,
                       mem_gb,
                       omp_nthreads,
                       output_resolution,
                       name='dwi_trans_wf',
                       use_compression=True,
                       to_mni=False,
-                      write_local_bvecs=False):
+                      write_local_bvecs=False,
+                      write_reports=True,
+                      concatenate=True):
     """
     This workflow samples dwi images to the ``output_grid`` in a "single shot"
     from the original DWI series.
 
     .. workflow::
         :graph2use: colored
         :simple_form: yes
@@ -99,15 +100,16 @@
             File defining the output space
         t1_mask
             Brain mask from the t1w
 
     **Outputs**
 
         dwi_resampled
-            DWI series, resampled to template space
+            DWI series, resampled to template space. One file if ``concatenate``, otherwise a
+            list of files
         dwi_ref_resampled
             Reference, contrast-enhanced summary of the DWI series, resampled to template space
         dwi_mask_resampled
             DWI series mask in template space
         cnr_map_resampled
             Contrast to noise map resampled
         bvals
@@ -159,103 +161,69 @@
             'resampled_dwi_mask',
             'rotated_bvecs',
             'local_bvecs',
             'b0_series',
             'resampled_qc']),
         name='outputnode')
 
-    def _aslist(in_value):
-        if isinstance(in_value, list):
-            return in_value
-        return [in_value]
-
     # get composite warps and composed affines for warping and rotating
     compose_transforms = pe.Node(ComposeTransforms(), name='compose_transforms')
-
-    def _get_first(lll):
-        from nipype.interfaces.base import isdefined
-        if isdefined(lll):
-            return lll[0]
-        return lll
+    get_interpolation = pe.Node(
+        ChooseInterpolator(output_resolution=output_resolution), name='get_interpolation')
+    dwi_transform = pe.MapNode(
+        ants.ApplyTransforms(float=True),
+        name='dwi_transform', iterfield=['input_image', 'transforms'])
+    rotate_gradients = pe.Node(GradientRotation(), name='rotate_gradients')
+    cnr_tfm = pe.Node(
+        ants.ApplyTransforms(interpolation='LanczosWindowedSinc', float=True),
+        name='cnr_tfm',
+        mem_gb=1)
 
     workflow.connect([
         (inputnode, compose_transforms, [
             ('output_grid', 'reference_image'),
             ('dwi_files', 'dwi_files'),
             ('hmc_xforms', 'hmc_affines'),
             ('itk_b0_to_t1', 'hmcsdc_dwi_ref_to_t1w_affine'),
             ('fieldwarps', 'fieldwarps'),
             ('b0_to_intramodal_template_transforms', 'b0_to_intramodal_template_transforms'),
-            (('intramodal_template_to_t1_affine', _get_first), 'intramodal_template_to_t1_affine'),
-            ('intramodal_template_to_t1_warp', 'intramodal_template_to_t1_warp'),
-            ])
-    ])
-
-    # Rotate the bvecs
-    rotate_gradients = pe.Node(GradientRotation(), name='rotate_gradients')
-
-    cnr_tfm = pe.Node(
-        ants.ApplyTransforms(interpolation='LanczosWindowedSinc', float=True),
-        name='cnr_tfm',
-        mem_gb=1)
-
-    if to_mni:
-        # Disassemble the to-mni transform if it's a h5 (it should be!)
-        disassemble_mni_xform = pe.Node(DisassembleTransform(), name='disassemble_mni_xform')
-
-        # Write corrected file in the designated output dir
-        mask_merge_tfms = pe.Node(niu.Merge(2), name='mask_merge_tfms',
-                                  run_without_submitting=True,
-                                  mem_gb=DEFAULT_MEMORY_MIN_GB)
-        workflow.connect([
-            (inputnode, disassemble_mni_xform, [('t1_2_mni_forward_transform',
-                                                 'in_file')]),
-            (disassemble_mni_xform, compose_transforms, [('out_transforms',
-                                                          't1_2_mni_forward_transform')]),
-            (inputnode, mask_merge_tfms, [('t1_2_mni_forward_transform', 'in1'),
-                                          (('itk_b0_to_t1', _aslist), 'in2')]),
-            (mask_merge_tfms, cnr_tfm, [('out', 'transforms')])
-        ])
-    else:
-        workflow.connect([
-            (compose_transforms, cnr_tfm, [(('out_warps', _get_first), 'transforms')])
-        ])
-
-    def _get_first(items):
-        return items[0]
-
-    get_interpolation = pe.Node(
-        ChooseInterpolator(output_resolution=output_resolution), name='get_interpolation')
-
-    dwi_transform = pe.MapNode(
-        ants.ApplyTransforms(float=True),
-        name='dwi_transform', iterfield=['input_image', 'transforms'])
-
-    merge = pe.Node(Merge(compress=use_compression), name='merge',
-                    mem_gb=mem_gb * 3)
-
-    extract_b0_series = pe.Node(ExtractB0s(), name="extract_b0_series")
-    final_b0_ref = init_dwi_reference_wf(register_t1=False, gen_report=True, desc='resampled',
-                                         name='final_b0_ref', source_file=source_file)
-
-    workflow.connect([
+            (('intramodal_template_to_t1_affine', _get_first),
+             'intramodal_template_to_t1_affine'),
+            ('intramodal_template_to_t1_warp', 'intramodal_template_to_t1_warp')]),
+        (compose_transforms, cnr_tfm, [(('out_warps', _get_first), 'transforms')]),
         (inputnode, rotate_gradients, [('bvec_files', 'bvec_files'),
                                        ('bval_files', 'bval_files')]),
         (compose_transforms, rotate_gradients, [('out_affines', 'affine_transforms')]),
         (rotate_gradients, outputnode, [('bvals', 'bvals'),
                                         ('bvecs', 'rotated_bvecs')]),
         (inputnode, cnr_tfm, [('cnr_map', 'input_image'),
                               ('output_grid', 'reference_image')]),
         (cnr_tfm, outputnode, [('output_image', 'cnr_map_resampled')]),
         (compose_transforms, dwi_transform, [('out_warps', 'transforms')]),
-        (inputnode, merge, [('name_source', 'header_source')]),
         (inputnode, dwi_transform, [('dwi_files', 'input_image'),
                                     ('output_grid', 'reference_image')]),
         (inputnode, get_interpolation, [('dwi_files', 'dwi_files')]),
         (get_interpolation, dwi_transform, [('interpolation_method', 'interpolation')]),
+    ])
+
+    # If concatenation is not happening here, send the still-split images to outputs
+    if not concatenate:
+        workflow.connect([
+            (dwi_transform, outputnode, [('output_image', 'dwi_resampled')])
+        ])
+        return workflow
+
+    merge = pe.Node(Merge(compress=use_compression), name='merge', mem_gb=mem_gb * 3)
+    extract_b0_series = pe.Node(ExtractB0s(), name="extract_b0_series")
+    final_b0_ref = init_dwi_reference_wf(register_t1=False, gen_report=write_reports,
+                                         desc='resampled', name='final_b0_ref',
+                                         source_file=source_file)
+
+    workflow.connect([
+        (inputnode, merge, [('name_source', 'header_source')]),
         (dwi_transform, merge, [('output_image', 'in_files')]),
         (merge, outputnode, [('out_file', 'dwi_resampled')]),
         (merge, extract_b0_series, [('out_file', 'dwi_series')]),
         (inputnode, extract_b0_series, [('b0_indices', 'b0_indices')]),
         (extract_b0_series, final_b0_ref, [('b0_average', 'inputnode.b0_template')]),
         (inputnode, final_b0_ref, [('t1_mask', 'inputnode.t1_mask')]),
         (final_b0_ref, outputnode, [
@@ -280,7 +248,20 @@
         ])
 
     return workflow
 
 
 def _first(inlist):
     return inlist[0]
+
+
+def _get_first(lll):
+    from nipype.interfaces.base import isdefined
+    if isdefined(lll):
+        return lll[0]
+    return lll
+
+
+def _aslist(in_value):
+    if isinstance(in_value, list):
+        return in_value
+    return [in_value]
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/dwi/derivatives.py` & `qsiprep-0.9.0b1/qsiprep/workflows/dwi/derivatives.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/workflows/base.py` & `qsiprep-0.9.0b1/qsiprep/workflows/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .. autofunction:: init_single_subject_wf
 
 """
 import logging
 import sys
 import os
 from copy import deepcopy
+from collections import defaultdict
 
 from nipype import __version__ as nipype_ver
 from nipype.pipeline import engine as pe
 from nipype.interfaces import utility as niu
 
 from nilearn import __version__ as nilearn_ver
 
@@ -29,29 +30,31 @@
 from ..utils.grouping import group_dwi_scans
 from ..__about__ import __version__
 
 from .anatomical import init_anat_preproc_wf
 from .dwi.base import init_dwi_preproc_wf
 from .dwi.finalize import init_dwi_finalize_wf
 from .dwi.intramodal_template import init_intramodal_template_wf
+from .dwi.distortion_group_merge import init_distortion_group_merge_wf
 from .dwi.util import get_source_file
 
 
 LOGGER = logging.getLogger('nipype.workflow')
 
 
 def init_qsiprep_wf(
         subject_list, run_uuid, work_dir, output_dir, bids_dir, ignore, debug, low_mem, anat_only,
         longitudinal, b0_threshold, hires, denoise_before_combining, dwi_denoise_window,
         unringing_method, dwi_no_biascorr, no_b0_harmonization, output_resolution,
-        combine_all_dwis, omp_nthreads, force_spatial_normalization, skull_strip_template,
-        skull_strip_fixed_seed, freesurfer, hmc_model, impute_slice_threshold, hmc_transform,
-        shoreline_iters, eddy_config, write_local_bvecs, output_spaces, template, motion_corr_to,
-        b0_to_t1w_transform, intramodal_template_iters, intramodal_template_transform,
-        prefer_dedicated_fmaps, fmap_bspline, fmap_demean, use_syn, force_syn):
+        combine_all_dwis, distortion_group_merge, omp_nthreads, force_spatial_normalization,
+        skull_strip_template, skull_strip_fixed_seed, freesurfer, hmc_model,
+        impute_slice_threshold, hmc_transform, shoreline_iters, eddy_config, write_local_bvecs,
+        output_spaces, template, motion_corr_to, b0_to_t1w_transform, intramodal_template_iters,
+        intramodal_template_transform, prefer_dedicated_fmaps, fmap_bspline, fmap_demean, use_syn,
+        force_syn):
     """
     This workflow organizes the execution of qsiprep, with a sub-workflow for
     each subject.
 
     .. workflow::
         :graph2use: orig
         :simple_form: yes
@@ -74,14 +77,15 @@
                               hires=False,
                               denoise_before_combining=True,
                               dwi_denoise_window=7,
                               unringing_method='mrdegibbs',
                               dwi_no_biascorr=False,
                               no_b0_harmonization=False,
                               combine_all_dwis=True,
+                              distortion_group_merge='concat',
                               omp_nthreads=1,
                               output_resolution=2.0,
                               hmc_model='3dSHORE',
                               skull_strip_template='OASIS',
                               skull_strip_fixed_seed=False,
                               output_spaces=['T1w', 'template'],
                               template='MNI152NLin2009cAsym',
@@ -136,14 +140,17 @@
             run spatial bias correction (N4) on dwi series
         no_b0_harmonization : bool
             skip rescaling dwi scans to have matching b=0 intensities across scans
         denoise_before_combining : bool
             'run ``dwidenoise`` before combining dwis. Requires ``combine_all_dwis``'
         combine_all_dwis : bool
             Combine all dwi sequences within a session into a single data set
+        distortion_group_merge : str
+            How to combine multiple distortion groups after correction. 'concat', 'average' or
+            'none'
         omp_nthreads : int
             Maximum number of threads an individual process may use
         skull_strip_template : str
             Name of ANTs skull-stripping template ('OASIS' or 'NKI')
         skull_strip_fixed_seed : bool
             Do not use a random seed for skull-stripping - will ensure
             run-to-run replicability when used with --omp-nthreads 1
@@ -227,14 +234,15 @@
             no_b0_harmonization=no_b0_harmonization,
             anat_only=anat_only,
             longitudinal=longitudinal,
             b0_threshold=b0_threshold,
             freesurfer=freesurfer,
             hires=hires,
             combine_all_dwis=combine_all_dwis,
+            distortion_group_merge=distortion_group_merge,
             omp_nthreads=omp_nthreads,
             skull_strip_template=skull_strip_template,
             skull_strip_fixed_seed=skull_strip_fixed_seed,
             output_spaces=output_spaces,
             template=template,
             prefer_dedicated_fmaps=prefer_dedicated_fmaps,
             motion_corr_to=motion_corr_to,
@@ -265,19 +273,20 @@
     return qsiprep_wf
 
 
 def init_single_subject_wf(
         subject_id, name, reportlets_dir, output_dir, bids_dir, ignore, debug, write_local_bvecs,
         low_mem, anat_only, longitudinal, b0_threshold, denoise_before_combining,
         dwi_denoise_window, unringing_method, dwi_no_biascorr, no_b0_harmonization,
-        combine_all_dwis, omp_nthreads, skull_strip_template, force_spatial_normalization,
-        skull_strip_fixed_seed, freesurfer, hires, output_spaces, template, output_resolution,
-        prefer_dedicated_fmaps, motion_corr_to, b0_to_t1w_transform, intramodal_template_iters,
-        intramodal_template_transform, hmc_model, hmc_transform, shoreline_iters, eddy_config,
-        impute_slice_threshold, fmap_bspline, fmap_demean, use_syn, force_syn):
+        combine_all_dwis, distortion_group_merge, omp_nthreads, skull_strip_template,
+        force_spatial_normalization, skull_strip_fixed_seed, freesurfer, hires, output_spaces,
+        template, output_resolution, prefer_dedicated_fmaps, motion_corr_to, b0_to_t1w_transform,
+        intramodal_template_iters, intramodal_template_transform, hmc_model, hmc_transform,
+        shoreline_iters, eddy_config, impute_slice_threshold, fmap_bspline, fmap_demean, use_syn,
+        force_syn):
     """
     This workflow organizes the preprocessing pipeline for a single subject.
     It collects and reports information about the subject, and prepares
     sub-workflows to perform anatomical and diffusion preprocessing.
 
     Anatomical preprocessing is performed in a single workflow, regardless of
     the number of sessions.
@@ -308,18 +317,19 @@
             anat_only=False,
             longitudinal=False,
             b0_threshold=100,
             freesurfer=False,
             hires=False,
             force_spatial_normalization=True,
             combine_all_dwis=True,
+            distortion_group_merge='none',
             omp_nthreads=1,
             skull_strip_template='OASIS',
             skull_strip_fixed_seed=False,
-            output_spaces=['T1w', 'template'],
+            output_spaces=['T1w'],
             template='MNI152NLin2009cAsym',
             prefer_dedicated_fmaps=False,
             motion_corr_to='iterative',
             b0_to_t1w_transform='Rigid',
             intramodal_template_iters=0,
             intramodal_template_transform="Rigid",
             hmc_model='3dSHORE',
@@ -361,14 +371,17 @@
             run spatial bias correction (N4) on dwi series
         no_b0_harmonization : bool
             skip rescaling dwi scans to have matching b=0 intensities across scans
         denoise_before_combining : bool
             'run ``dwidenoise`` before combining dwis. Requires ``combine_all_dwis``'
         combine_all_dwis : Bool
             Combine all dwi sequences within a session into a single data set
+        distortion_group_merge: str
+            How to combine preprocessed scans from different distortion groups. 'concat',
+            'average' or 'none'
         omp_nthreads : int
             Maximum number of threads an individual process may use
         skull_strip_template : str
             Name of ANTs skull-stripping template ('OASIS' or 'NKI')
         skull_strip_fixed_seed : bool
             Do not use a random seed for skull-stripping - will ensure
             run-to-run replicability when used with --omp-nthreads 1
@@ -386,15 +399,14 @@
             List of output spaces functional images are to be resampled to.
             Some parts of pipeline will only be instantiated for some output
             spaces.
 
             Valid spaces:
 
              - T1w
-             - template
 
         template : str
             Name of template targeted by ``template`` output space
         hmc_model : 'none', '3dSHORE' or 'MAPMRI'
             Model used to generate target images for head motion correction. If 'none'
             the transform from the nearest b0 will be used.
         hmc_transform : "Rigid" or "Affine"
@@ -475,14 +487,16 @@
 "qsiprep's documentation").
 
 
 ### References
 
 """.format(nilearn_ver=nilearn_ver)
 
+    merging_distortion_groups = not distortion_group_merge.lower() == 'none'
+
     inputnode = pe.Node(
         niu.IdentityInterface(fields=['subjects_dir']), name='inputnode')
 
     bidssrc = pe.Node(
         BIDSDataGrabber(subject_data=subject_data, anat_only=anat_only),
         name='bidssrc')
 
@@ -553,20 +567,54 @@
 
     if impute_slice_threshold > 0 and hmc_model == "none":
         LOGGER.warning("hmc_model must not be 'none' if slices are to be imputed. "
                        "setting `impute_slice_threshold=0`")
         impute_slice_threshold = 0
 
     # Handle the grouping of multiple dwi files within a session
-    dwi_fmap_groups = group_dwi_scans(layout, subject_data,
-                                      using_fsl=hmc_model == 'eddy',
-                                      combine_scans=combine_all_dwis,
-                                      ignore_fieldmaps="fieldmaps" in ignore)
+    # concatenation_scheme maps the outputs to their final concatenation group
+    dwi_fmap_groups, concatenation_scheme = group_dwi_scans(
+        layout, subject_data,
+        using_fsl=hmc_model == 'eddy',
+        combine_scans=combine_all_dwis,
+        ignore_fieldmaps="fieldmaps" in ignore,
+        concatenate_distortion_groups=merging_distortion_groups)
     LOGGER.info(dwi_fmap_groups)
 
+    # If a merge is happening at the end, make sure
+    if merging_distortion_groups:
+        # create a mapping of which across-distortion-groups are contained in each merge
+        merged_group_names = sorted(set(concatenation_scheme.values()))
+        merged_to_subgroups = defaultdict(list)
+        for subgroup_name, destination_name in concatenation_scheme.items():
+            merged_to_subgroups[destination_name].append(subgroup_name)
+
+        merging_group_workflows = {}
+        for merged_group in merged_group_names:
+            merging_group_workflows[merged_group] = init_distortion_group_merge_wf(
+                merging_strategy=distortion_group_merge,
+                harmonize_b0_intensities=not no_b0_harmonization,
+                b0_threshold=b0_threshold,
+                template=template,
+                output_dir=output_dir,
+                output_prefix=merged_group,
+                source_file=merged_group + '_dwi.nii.gz',
+                shoreline_iters=shoreline_iters,
+                hmc_model=hmc_model,
+                inputs_list=merged_to_subgroups[merged_group],
+                omp_nthreads=omp_nthreads,
+                reportlets_dir=reportlets_dir,
+                name=merged_group.replace('-', '_') + "_final_merge_wf")
+            workflow.connect([
+                (anat_preproc_wf, merging_group_workflows[merged_group], [
+                    ('outputnode.t1_brain', 'inputnode.t1_brain'),
+                    ('outputnode.t1_mask', 'inputnode.t1_mask'),
+                    ('outputnode.t1_seg', 'inputnode.t1_seg')])
+            ])
+
     outputs_to_files = {dwi_group['concatenated_bids_name']: dwi_group
                         for dwi_group in dwi_fmap_groups}
     if force_syn:
         for group_name in outputs_to_files:
             outputs_to_files[group_name]['fieldmap_info'] = {"suffix": "syn"}
     summary.inputs.dwi_groupings = outputs_to_files
 
@@ -608,14 +656,15 @@
                  'inputnode.t1_2_fsnative_forward_transform'),
                 ('outputnode.t1_2_fsnative_reverse_transform',
                  'inputnode.t1_2_fsnative_reverse_transform')])])
 
     # create a processing pipeline for the dwis in each session
     for output_fname, dwi_info in outputs_to_files.items():
         source_file = get_source_file(dwi_info['dwi_series'], output_fname, suffix="_dwi")
+        output_wfname = output_fname.replace('-', '_')
         dwi_preproc_wf = init_dwi_preproc_wf(
             scan_groups=dwi_info,
             output_prefix=output_fname,
             layout=layout,
             ignore=ignore,
             b0_threshold=b0_threshold,
             dwi_denoise_window=dwi_denoise_window,
@@ -657,16 +706,16 @@
             template=template,
             output_resolution=output_resolution,
             output_dir=output_dir,
             omp_nthreads=omp_nthreads,
             use_syn=use_syn,
             low_mem=low_mem,
             make_intramodal_template=make_intramodal_template,
-            source_file=source_file
-        )
+            source_file=source_file,
+            write_derivatives=not merging_distortion_groups)
 
         workflow.connect([
             (
                 anat_preproc_wf,
                 dwi_preproc_wf,
                 [
                     ('outputnode.t1_preproc', 'inputnode.t1_preproc'),
@@ -735,25 +784,52 @@
                     ('outputnode.raw_concatenated', 'inputnode.raw_concatenated'),
                     ('outputnode.confounds', 'inputnode.confounds'),
                     ('outputnode.carpetplot_data', 'inputnode.carpetplot_data')
                     ])
         ])
 
         if make_intramodal_template:
-            input_name = 'inputnode.{name}_b0_template'.format(
-                name=output_fname.replace('-', '_'))
-            output_name = 'outputnode.{name}_transform'.format(
-                name=output_fname.replace('-', '_'))
+            input_name = 'inputnode.{name}_b0_template'.format(name=output_wfname)
+            output_name = 'outputnode.{name}_transform'.format(name=output_wfname)
             workflow.connect([
                 (dwi_preproc_wf, intramodal_template_wf, [
                     ('outputnode.b0_ref_image', input_name)]),
                 (intramodal_template_wf, dwi_finalize_wf, [
                     (output_name, 'inputnode.b0_to_intramodal_template_transforms'),
                     ('outputnode.intramodal_template_to_t1_affine',
                      'inputnode.intramodal_template_to_t1_affine'),
                     ('outputnode.intramodal_template_to_t1_warp',
                      'inputnode.intramodal_template_to_t1_warp'),
                     ('outputnode.intramodal_template',
                      'inputnode.intramodal_template')])
             ])
 
+        if merging_distortion_groups:
+            image_name = 'inputnode.{name}_image'.format(name=output_wfname)
+            bval_name = 'inputnode.{name}_bval'.format(name=output_wfname)
+            bvec_name = 'inputnode.{name}_bvec'.format(name=output_wfname)
+            original_bvec_name = 'inputnode.{name}_original_bvec'.format(
+                name=output_wfname)
+            original_bids_name = 'inputnode.{name}_original_image'.format(
+                name=output_wfname)
+            raw_concatenated_image_name = 'inputnode.{name}_raw_concatenated_image'.format(
+                name=output_wfname)
+            confounds_name = 'inputnode.{name}_confounds'.format(name=output_wfname)
+            b0_ref_name = 'inputnode.{name}_b0_ref'.format(name=output_wfname)
+            cnr_name = 'inputnode.{name}_cnr'.format(name=output_wfname)
+            final_merge_wf = merging_group_workflows[concatenation_scheme[output_fname]]
+            workflow.connect([
+                (dwi_finalize_wf, final_merge_wf, [
+                    ('outputnode.bvals_t1', bval_name),
+                    ('outputnode.bvecs_t1', bvec_name),
+                    ('outputnode.dwi_t1', image_name),
+                    ('outputnode.t1_b0_ref', b0_ref_name),
+                    ('outputnode.cnr_map_t1', cnr_name)
+                    ]),
+                (dwi_preproc_wf, final_merge_wf, [
+                    ('outputnode.raw_concatenated', raw_concatenated_image_name),
+                    ('outputnode.original_bvecs', original_bvec_name),
+                    ('outputnode.original_files', original_bids_name),
+                    ('outputnode.confounds', confounds_name)])
+            ])
+
     return workflow
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/__about__.py` & `qsiprep-0.9.0b1/qsiprep/__about__.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/viz/reports.py` & `qsiprep-0.9.0b1/qsiprep/viz/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,50 +57,52 @@
         self.isnested = False
 
 
 class Report(object):
     """
     The full report object
     """
-    def __init__(self, path, config, out_dir, run_uuid, out_filename='report.html'):
+    def __init__(self, path, config, out_dir, run_uuid, out_filename='report.html',
+                 pipeline_type='qsiprep'):
         self.root = path
         self.sections = []
         self.errors = []
         self.out_dir = Path(out_dir)
         self.out_filename = out_filename
         self.run_uuid = run_uuid
+        self.pipeline_type = pipeline_type
 
         self._load_config(config)
 
     def _load_config(self, config):
         with open(config, 'r') as configfh:
             config = json.load(configfh)
 
         self.index(config['sections'])
 
     def index(self, config):
         fig_dir = 'figures'
         subject_dir = self.root.split('/')[-1]
         subject = re.search('^(?P<subject_id>sub-[a-zA-Z0-9]+)$', subject_dir).group()
-        svg_dir = self.out_dir / 'qsiprep' / subject / fig_dir
+        svg_dir = self.out_dir / self.pipeline_type / subject / fig_dir
         svg_dir.mkdir(parents=True, exist_ok=True)
         reportlet_list = list(sorted([str(f) for f in Path(self.root).glob('**/*.*')]))
 
         for subrep_cfg in config:
             reportlets = []
             for reportlet_cfg in subrep_cfg['reportlets']:
                 rlet = Reportlet(**reportlet_cfg)
                 for src in reportlet_list:
                     ext = src.split('.')[-1]
                     if rlet.file_pattern.search(src):
                         contents = None
                         if ext == 'html':
                             with open(src) as fp:
                                 contents = fp.read().strip()
-                        elif ext in ('svg', 'gif'):
+                        elif ext in ('svg', 'gif', 'png'):
                             fbase = Path(src).name
                             copyfile(src, str(svg_dir / fbase),
                                      copy=True, use_hardlink=True)
                             contents = str(Path(subject) / fig_dir / fbase)
                         if contents:
                             rlet.source_files.append(src)
                             rlet.contents.append(contents)
@@ -110,15 +112,15 @@
 
             if reportlets:
                 sub_report = SubReport(
                     subrep_cfg['name'], reportlets=reportlets,
                     title=subrep_cfg.get('title'))
                 self.sections.append(order_by_run(sub_report))
 
-        error_dir = self.out_dir / "qsiprep" / subject / 'log' / self.run_uuid
+        error_dir = self.out_dir / self.pipeline_type / subject / 'log' / self.run_uuid
         if error_dir.is_dir():
             self.index_error_dir(error_dir)
 
     def index_error_dir(self, error_dir):
         """
         Crawl subjects crash directory for the corresponding run and return text for
         .pklz crash file found.
@@ -161,15 +163,15 @@
             data['inputs'] = sorted(inputs)
         else:
             data['node_dir'] = "Node crashed before execution"
         data['traceback'] = '\n'.join(lines[traceback_start:])
         return data
 
     def generate_report(self):
-        logs_path = self.out_dir / 'qsiprep' / 'logs'
+        logs_path = self.out_dir / self.pipeline_type / 'logs'
 
         boilerplate = []
         boiler_idx = 0
 
         if (logs_path / 'CITATION.html').exists():
             text = (logs_path / 'CITATION.html').read_text(encoding='UTF-8')
             text = '<div class="boiler-html">%s</div>' % re.compile(
@@ -201,15 +203,16 @@
             trim_blocks=True, lstrip_blocks=True
         )
         report_tpl = env.get_template('viz/report.tpl')
         report_render = report_tpl.render(sections=self.sections, errors=self.errors,
                                           boilerplate=boilerplate)
 
         # Write out report
-        (self.out_dir / 'qsiprep' / self.out_filename).write_text(report_render, encoding='UTF-8')
+        (self.out_dir / self.pipeline_type / self.out_filename).write_text(
+            report_render, encoding='UTF-8')
         return len(self.errors)
 
 
 def order_by_run(subreport):
     ordered = []
     run_reps = {}
     for element in subreport.reportlets:
@@ -267,15 +270,15 @@
         acq=" Acquisition: " + outputs['acq_id'] if outputs['acq_id'] else '',
         rec=" Reconstruction: " + outputs['rec_id'] if outputs['rec_id'] else '',
         run=" Run: " + outputs['run_id'] if outputs['run_id'] else ''
     )
     return name.strip('_'), title
 
 
-def run_reports(reportlets_dir, out_dir, subject_label, run_uuid):
+def run_reports(reportlets_dir, out_dir, subject_label, run_uuid, report_type='qsiprep'):
     """
     Runs the reports
 
     >>> import os
     >>> from shutil import copytree
     >>> from tempfile import TemporaryDirectory
     >>> filepath = os.path.dirname(os.path.realpath(__file__))
@@ -290,29 +293,34 @@
     ...             os.path.abspath('out'),
     ...             '01', 'madeoutuuid')
     0
     >>> os.chdir(curdir)
     >>> tmpdir.cleanup()
 
     """
-    reportlet_path = str(Path(reportlets_dir) / 'qsiprep' / ("sub-%s" % subject_label))
-    config = pkgrf('qsiprep', 'viz/config.json')
+    reportlet_path = str(Path(reportlets_dir) / report_type / ("sub-%s" % subject_label))
+    if report_type == 'qsiprep':
+        config = pkgrf('qsiprep', 'viz/config.json')
+    else:
+        config = pkgrf('qsiprep', 'viz/recon_config.json')
 
     out_filename = 'sub-{}.html'.format(subject_label)
-    report = Report(reportlet_path, config, out_dir, run_uuid, out_filename)
+    report = Report(reportlet_path, config, out_dir, run_uuid, out_filename,
+                    pipeline_type=report_type)
     return report.generate_report()
 
 
-def generate_reports(subject_list, output_dir, work_dir, run_uuid):
+def generate_reports(subject_list, output_dir, work_dir, run_uuid, pipeline_mode='qsiprep'):
     """
     A wrapper to run_reports on a given ``subject_list``
     """
     reports_dir = str(Path(work_dir) / 'reportlets')
     report_errors = [
-        run_reports(reports_dir, output_dir, subject_label, run_uuid=run_uuid)
+        run_reports(reports_dir, output_dir, subject_label, run_uuid=run_uuid,
+                    report_type=pipeline_mode)
         for subject_label in subject_list
     ]
 
     errno = sum(report_errors)
     if errno:
         import logging
         logger = logging.getLogger('cli')
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/engine/workflows.py` & `qsiprep-0.9.0b1/qsiprep/engine/workflows.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/__init__.py` & `qsiprep-0.9.0b1/qsiprep/__init__.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/nilearn.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/nilearn.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/mrtrix.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/mrtrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 """
 import os
 import os.path as op
 from copy import deepcopy
 import numpy as np
 import nibabel as nb
 import pandas as pd
-from scipy.io.matlab import savemat
+from scipy.io.matlab import savemat, loadmat
 from nilearn.image import load_img, threshold_img, iter_img
+import nipype.pipeline.engine as pe
+import nipype.interfaces.utility as niu
 from nipype import logging
 from nipype.utils.filemanip import fname_presuffix, split_filename, which
 from nipype.interfaces.base import (
     traits, TraitedSpec, BaseInterfaceInputSpec, File, SimpleInterface, InputMultiObject,
     isdefined, CommandLineInputSpec)
 from nipype.interfaces.mrtrix3 import Generate5tt, ResponseSD, MRConvert
 from nipype.interfaces.mrtrix3.utils import Generate5ttInputSpec
@@ -759,14 +761,17 @@
             if not isdefined(output):
                 output = fname + "_residualEnergy.mif"
             return output
         return None
 
 
 class BuildConnectomeInputSpec(CommandLineInputSpec):
+    atlas_name = traits.Str(desc='name of atlas (for variables in matfile)')
+    atlas_config = traits.Dict(desc='atlas configs for atlases to run connectivity for')
+    measure = traits.Str(desc='Name of the connectivity measure')
     in_file = File(
         exists=True,
         argstr='%s',
         mandatory=True,
         position=-3,
         desc='input tractography')
     in_parc = File(
@@ -810,14 +815,15 @@
     length_scale = traits.Enum("None", "length", "invlength", argstr='%s')
     scale_invnodevol = traits.Bool(False, argstr="-scale_invnodevol")
     in_scalar = File(
         exists=True,
         argstr='-scale_file %s',
         desc='provide the associated image '
         'for the mean_scalar metric')
+    use_sift_weights = traits.Bool(default=False, usedefault=True)
     in_weights = File(
         exists=True,
         argstr='-tck_weights_in %s',
         desc='specify a text scalar '
         'file containing the streamline weights')
     keep_unassigned = traits.Bool(
         argstr='-keep_unassigned',
@@ -832,15 +838,16 @@
         ' both ends)')
     symmetric = traits.Bool(
         argstr='-symmetric',
         desc='Make matrices symmetric on output')
 
 
 class BuildConnectomeOutputSpec(TraitedSpec):
-    out_file = File(exists=True, desc='the output response file')
+    out_file = File(exists=True, desc='the output connectivity csv')
+    connectivity_matfile = File(exists=True, desc='the matfile containing connectivity data')
     out_assignments = File(exists=True, desc='streamline assignment csv')
 
 
 class BuildConnectome(MRTrix3Base):
     """
     Generate a connectome matrix from a streamlines file and a node
     parcellation image
@@ -858,31 +865,55 @@
     _cmd = 'tck2connectome'
     input_spec = BuildConnectomeInputSpec
     output_spec = BuildConnectomeOutputSpec
 
     def _list_outputs(self):
         outputs = self.output_spec().get()
         outputs['out_file'] = op.abspath(self.inputs.out_file)
+        prefix = self.inputs.atlas_name + "_" + self.inputs.measure
+        outputs['connectivity_matfile'] = op.abspath(prefix + "_connectivity.mat")
         if isdefined(self.inputs.out_assignments):
             outputs['out_assignments'] = op.abspath(self.inputs.out_assignments)
         return outputs
 
+    def _post_run_hook(self, runtime):
+        atlas_config = self.inputs.atlas_config
+        atlas_name = self.inputs.atlas_name
+
+        # Aggregate the connectivity/network data from DSI Studio
+        official_labels = np.array(atlas_config['node_ids']).astype(np.int)
+        connectivity_data = {
+            atlas_name + "_region_ids": official_labels,
+            atlas_name + "_region_labels": np.array(atlas_config['node_names'])
+        }
+
+        # get the connectivity matrix
+        prefix = atlas_name + "_" + self.inputs.measure
+        connectivity_data[prefix + "_connectivity"] = np.loadtxt(self.inputs.out_file)
+        merged_matfile = op.join(runtime.cwd, prefix + "_connectivity.mat")
+        savemat(merged_matfile, connectivity_data, long_field_names=True)
+        return runtime
+
     def _format_arg(self, name, spec, val):
         if name == 'length_scale':
             if val == 'length':
                 return '-scale_length'
             if val == 'invlength':
                 return '-scale_invlength'
             return ''
+        if name == 'in_weights':
+            if self.inputs.use_sift_weights:
+                return spec.argstr % val
         return super(BuildConnectome, self)._format_arg(name, spec, val)
 
 
 class MRTrixAtlasGraphInputSpec(BuildConnectomeInputSpec):
     atlas_configs = traits.Dict(desc='atlas configs for atlases to run connectivity for',
                                 mandatory=True)
+    tracking_params = traits.List(desc='list of sets of parameters for tck2connectome')
 
 
 class MRTrixAtlasGraphOutputSpec(TraitedSpec):
     connectivity_matfile = File(exists=True)
     commands = File()
 
 
@@ -895,58 +926,69 @@
         # Get all inputs from the ApplyTransforms object
         ifargs = self.inputs.get()
         ifargs['nthreads'] = 1
 
         # Get number of parallel jobs
         num_threads = ifargs.pop('nthreads')
         atlas_configs = ifargs.pop('atlas_configs')
+        tracking_params = self.inputs.tracking_params
         del ifargs['in_parc']
 
-        # flatten the atlas_configs
-        args = [(atlas_name, atlas_config, self.inputs.in_file, ifargs) for atlas_name,
-                atlas_config in atlas_configs.items()]
-
-        if num_threads == 1:
-            outputs = [_mrtrix_connectivity(arg) for arg in args]
+        # Make a workflow for each atlas and tracking parameter set
+        workflow = pe.Workflow(name='dsistudio_atlasgraph')
+        nodes = []
+        merge_mats = pe.Node(niu.Merge(len(tracking_params) * len(atlas_configs)),
+                             name='merge_mats')
+        outputnode = pe.Node(niu.IdentityInterface(fields=['matfiles']), name='outputnode')
+        workflow.connect(merge_mats, 'out', outputnode, 'matfiles')
+        in_num = 1
+        for atlas_name, atlas_config in atlas_configs.items():
+            for tracking_param_set in self.inputs.tracking_params:
+                node_args = deepcopy(ifargs)
+                # Symlink in the fib file
+                node_args.pop('atlas_config')
+                node_args.pop('atlas_name')
+                node_args.pop('tracking_params')
+                measure_name = tracking_param_set['measure']
+                node_args.update(tracking_param_set)
+                nodes.append(
+                    pe.Node(
+                        BuildConnectome(
+                            atlas_config=atlas_config,
+                            atlas_name=atlas_name,
+                            in_parc=atlas_config['dwi_resolution_mif'],
+                            **node_args),
+                        name=atlas_name + "_" + measure_name)
+                )
+                workflow.connect(nodes[-1], 'connectivity_matfile',
+                                 merge_mats, 'in%d' % in_num)
+                in_num += 1
+
+        workflow.config['execution']['stop_on_first_crash'] = 'true'
+        workflow.config['execution']['remove_unnecessary_outputs'] = 'false'
+        workflow.base_dir = runtime.cwd
+        if num_threads > 1:
+            wf_result = workflow.run(plugin='MultiProc', plugin_args={'n_procs': num_threads})
         else:
-            from concurrent.futures import ThreadPoolExecutor
-            with ThreadPoolExecutor(max_workers=num_threads) as pool:
-                outputs = list(pool.map(_mrtrix_connectivity, args))
-
-        commands = [out[0] for out in outputs]
-        commands_file = op.join(runtime.cwd, "mrtrix_commands.txt")
-        with open(commands_file, "w") as f:
-            f.write("\n----------\n".join(commands))
-        self._results['commands'] = commands_file
-
-        matfile_list = [out[1] for out in outputs]
+            wf_result = workflow.run()
+        merge_node, = [node for node in list(wf_result.nodes) if node.name.endswith('merge_mats')]
         merged_connectivity_file = op.join(runtime.cwd, "combined_connectivity.mat")
-        _merge_conmats(matfile_list, args, merged_connectivity_file)
+        _merge_conmats(merge_node.result.outputs.out, merged_connectivity_file)
         self._results['connectivity_matfile'] = merged_connectivity_file
 
         return runtime
 
 
-def _merge_conmats(matfile_list, recon_args, outfile):
+def _merge_conmats(matfile_list, outfile):
     """Merge the many matfiles output by dsi studio and ensure they conform"""
     connectivity_values = {}
 
-    for matfile, (atlas_name, atlas_config, tck_file, ifargs) in zip(matfile_list, recon_args):
-        labels = np.array(atlas_config['node_ids']).astype(np.int)
-        connectivity_values[atlas_name + "_region_ids"] = labels
-        connectivity_values[atlas_name + "_region_labels"] = np.array(atlas_config['node_names'])
-        measure_name = atlas_name + '_' + ifargs['stat_edge']
-        if isdefined(ifargs['length_scale']):
-            measure_name += "_" + ifargs['length_scale']
-        if isdefined(ifargs['scale_invnodevol']):
-            measure_name += "_invroiscale"
-        connectivity_values[measure_name + "_connectivity"] = np.loadtxt(matfile)
-        connectivity_values[measure_name + "_tck"] = tck_file
-        connectivity_values[measure_name + "_image"] = atlas_config['dwi_resolution_mif']
-    savemat(outfile, connectivity_values, do_compression=True)
+    for matfile in matfile_list:
+        connectivity_values.update(loadmat(matfile))
+    savemat(outfile, connectivity_values, long_field_names=True, do_compression=True)
 
 
 def _mrtrix_connectivity(args):
     atlas_name, atlas_config, _, ifargs = args
     csv_name = 'atlas_{}_length_{}_roiscale_{}_stat_{}.csv'.format(
         atlas_name, ifargs['length_scale'], ifargs['scale_invnodevol'],
         ifargs['stat_edge']).replace("<undefined>", "None")
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/qc.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/qc.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/dsi_studio.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/dsi_studio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 #!python
-from __future__ import print_function
-
-from nipype.interfaces.base import (TraitedSpec, CommandLineInputSpec, BaseInterfaceInputSpec,
-                                    CommandLine, File, traits, isdefined, SimpleInterface)
-
 import os
 import os.path as op
-from glob import glob
-from nipype.utils.filemanip import fname_presuffix
 import logging
+from glob import glob
 from copy import deepcopy
 import numpy as np
+from nipype.interfaces.base import (TraitedSpec, CommandLineInputSpec, BaseInterfaceInputSpec,
+                                    CommandLine, File, traits, isdefined, SimpleInterface)
+import nipype.pipeline.engine as pe
+import nipype.interfaces.utility as niu
+from nipype.utils.filemanip import fname_presuffix, split_filename
 from scipy.io.matlab import loadmat, savemat
 import nibabel as nb
 LOGGER = logging.getLogger('nipype.interface')
 
 
-class DSIStudioCreateSrcInputSpec(CommandLineInputSpec):
+class DSIStudioCommandLineInputSpec(CommandLineInputSpec):
+    nthreads = traits.Int(1, usedefault=True, argstr="--threads=%d")
+
+
+class DSIStudioCreateSrcInputSpec(DSIStudioCommandLineInputSpec):
     test_trait = traits.Bool()
     input_nifti_file = File(
         desc="DWI Nifti file",
-        argstr="--source=%s",
-        copyfile=False)
+        argstr="--source=%s")
     input_dicom_dir = File(
         desc="Directory with DICOM data from only the dwi",
         exists=True,
         argstr="--source=%s")
     input_bvals_file = File(
         desc="Text file containing b values", exists=True, argstr="--bval=%s")
     input_bvecs_file = File(
@@ -38,69 +40,61 @@
         argstr="--b_table=%s")
     recursive = traits.Bool(
         False,
         desc="Search for DICOM files recursively",
         argstr="--recursive=1")
     subject_id = traits.Str("data")
     output_src = File(
-        name_template="%s.src.gz",
-        default='',
-        usedefault=True,
         desc="Output file (.src.gz)",
         argstr="--output=%s",
-        name_source="subject_id",
         genfile=True)
     grad_dev = File(
         desc="Gradient deviation file",
         exists=True,
         copyfile=True,
         position=-1,
         argstr="#%s")
 
 
 class DSIStudioCreateSrcOutputSpec(TraitedSpec):
     output_src = File(
-        name_template="%s.src.gz",
         desc="Output file (.src.gz)",
-        argstr="--output=%s",
         name_source="subject_id")
 
 
 class DSIStudioCreateSrc(CommandLine):
     input_spec = DSIStudioCreateSrcInputSpec
     output_spec = DSIStudioCreateSrcOutputSpec
     _cmd = "dsi_studio --action=src "
 
-    def _format_arg(self, name, spec, value):
-        if name == "output_src":
-            if not self.inputs.output_src:
-                return '--output=' + self._gen_filename()
-            return '--output=' + self.inputs.output_src
-        return super(DSIStudioCreateSrc, self)._format_arg(name, spec, value)
-
-    def _gen_filename(self):
-        cwd = os.getcwd()
-        input_fname = self.inputs.input_dicom_dir if isdefined(self.inputs.input_dicom_dir) \
-            else self.inputs.input_nifti_file
-        if not isdefined(input_fname):
-            raise Exception()
-        return fname_presuffix(input_fname, newpath=cwd, suffix=".src.gz", use_ext=False)
+    def _gen_filename(self, name):
+        if not name == 'output_src':
+            return None
+        if isdefined(self.inputs.input_nifti_file):
+            _, fname, ext = split_filename(self.inputs.input_nifti_file)
+        elif isdefined(self.inputs.input_dicom_dir):
+            fname = op.split(self.inputs.dicom_dir)[1]
+        else:
+            raise Exception('Need either an input dicom director or nifti')
+
+        output = op.abspath(fname) + ".src.gz"
+        return output
 
     def _list_outputs(self):
         outputs = self.output_spec().get()
-        outputs["output_src"] = self._gen_filename()
+        outputs['output_src'] = self._gen_filename('output_src')
         return outputs
 
 
-class _DSIStudioSrcQCInputSpec(CommandLineInputSpec):
+class _DSIStudioSrcQCInputSpec(DSIStudioCommandLineInputSpec):
     src_file = File(exists=True, copyfile=True, argstr="%s",
                     desc='DSI Studio src[.gz] file')
 
 
-class _DSIStudioSrcQCOutputSpec(CommandLineInputSpec):
+class _DSIStudioSrcQCOutputSpec(DSIStudioCommandLineInputSpec):
     qc_txt = File(exists=True, desc="Text file with QC measures")
 
 
 class DSIStudioSrcQC(CommandLine):
     _cmd = 'dsi_studio --action=qc'
     input_spec = _DSIStudioSrcQCInputSpec
     output_spec = _DSIStudioSrcQCOutputSpec
@@ -113,15 +107,15 @@
     def _list_outputs(self):
         outputs = self.output_spec().get()
         outputs['qc_txt'] = op.abspath("src_report.txt")
         return outputs
 
 
 # Step 2 reonstruct ODFs
-class DSIStudioReconstructionInputSpec(CommandLineInputSpec):
+class DSIStudioReconstructionInputSpec(DSIStudioCommandLineInputSpec):
     input_src_file = File(
         desc="DSI Studio src file",
         mandatory=True,
         exists=True,
         copyfile=False,
         argstr="--source=%s")
     mask = File(
@@ -235,21 +229,21 @@
         results = glob(target)
         assert len(results) == 1
         outputs["output_fib"] = results[0]
 
         return outputs
 
 
-class DSIStudioExportInputSpec(CommandLineInputSpec):
+class DSIStudioExportInputSpec(DSIStudioCommandLineInputSpec):
     input_file = File(
         exists=True, argstr="--source=%s", mandatory=True, copyfile=False)
     to_export = traits.Str(mandatory=True, argstr="--export=%s")
 
 
-class DSIStudioExportOutputSpec(CommandLineInputSpec):
+class DSIStudioExportOutputSpec(DSIStudioCommandLineInputSpec):
     gfa_file = File(desc="Exported files")
     fa0_file = File(desc="Exported files")
     fa1_file = File(desc="Exported files")
     fa2_file = File(desc="Exported files")
     fa3_file = File(desc="Exported files")
     fa4_file = File(desc="Exported files")
     iso_file = File(desc="Exported files")
@@ -267,16 +261,18 @@
         for expected in to_expect:
             matches = glob("*" + expected + "*.nii.gz")
             if len(matches) == 1:
                 outputs[expected + "_file"] = os.path.abspath(matches[0])
         return outputs
 
 
-class DSIStudioConnectivityMatrixInputSpec(CommandLineInputSpec):
-    tract_file = File(exists=True, argstr="--tract=%s")
+class DSIStudioConnectivityMatrixInputSpec(DSIStudioCommandLineInputSpec):
+    trk_file = File(exists=True, argstr="--tract=%s")
+    atlas_config = traits.Dict(desc='atlas configs for atlases to run connectivity for')
+    atlas_name = traits.Str()
     input_fib = File(
         exists=True, argstr="--source=%s", mandatory=True, copyfile=False)
     fiber_count = traits.Int(xor=["seed_count"], argstr="--fiber_count=%d")
     seed_count = traits.Int(xor=["fiber_count"], argstr="--seed_count=%d")
     method = traits.Enum((0, 4), argstr="--method=%d", usedefault=True)
     seed_plan = traits.Enum((0, 1), argstr="--seed_plan=%d")
     initial_dir = traits.Enum((0, 1, 2), argstr="--initial_dir=%d")
@@ -298,45 +294,64 @@
     step_size = traits.CFloat(argstr="--step_size=%.2f")
     turning_angle = traits.CFloat(argstr="--turning_angle=%.2f")
     interpo_angle = traits.CFloat(argstr="--interpo_angle=%.2f")
     smoothing = traits.CFloat(argstr="--smoothing=%.2f")
     min_length = traits.CInt(argstr="--min_length=%d")
     max_length = traits.CInt(argstr="--max_length=%d")
     thread_count = traits.Int(1, argstr="--thread_count=%d", usedefault=True)
-    output_trk = traits.Str(
-        name_template="%s.trk.gz",
-        desc="Output file (trk.gz)",
-        argstr="--output=%s",
-        name_source="input_fib")
 
 
 class DSIStudioConnectivityMatrixOutputSpec(TraitedSpec):
     # What to write out
-    connectivity_matrices = traits.List()
+    connectivity_matfile = traits.File(exists=True)
 
 
 class DSIStudioConnectivityMatrix(CommandLine):
     input_spec = DSIStudioConnectivityMatrixInputSpec
     output_spec = DSIStudioConnectivityMatrixOutputSpec
     _cmd = "dsi_studio --action=ana "
 
+    def _post_run_hook(self, runtime):
+        atlas_config = self.inputs.atlas_config
+        atlas_name = self.inputs.atlas_name
+
+        # Aggregate the connectivity/network data from DSI Studio
+        official_labels = np.array(atlas_config['node_ids']).astype(np.int)
+        connectivity_data = {
+            atlas_name + "_region_ids": official_labels,
+            atlas_name + "_region_labels": np.array(atlas_config['node_names'])
+        }
+
+        # Gather the connectivity matrices
+        matfiles = glob(runtime.cwd + "/*.connectivity.mat")
+        for matfile in matfiles:
+            measure = "_".join(matfile.split(".")[-4:-2])
+            connectivity_data[atlas_name + "_" + measure + "_connectivity"] = \
+                _sanitized_connectivity_matrix(matfile, official_labels)
+
+        # Gather the network measure files
+        network_results = glob(runtime.cwd + "/*network*txt")
+        for network_result in network_results:
+            measure = "_".join(network_result.split(".")[-4:-2])
+            connectivity_data.update(
+                _sanitized_network_measures(network_result, official_labels,
+                                            atlas_name, measure))
+        merged_matfile = op.join(runtime.cwd, atlas_name + "_connectivity.mat")
+        savemat(merged_matfile, connectivity_data, long_field_names=True)
+        return runtime
+
     def _list_outputs(self):
         outputs = self.output_spec().get()
-        results = glob("*.connectivity.mat")
-        outputs["connectivity_matrices"] = [
-            os.path.abspath(c) for c in results
-        ]
-        network_results = glob("*network*txt")
-        outputs["connectivity_matrices"] += [op.abspath(c) for c in network_results]
+        outputs['connectivity_matfile'] = op.abspath(
+            self.inputs.atlas_name + "_connectivity.mat")
         return outputs
 
 
 class DSIStudioAtlasGraphInputSpec(DSIStudioConnectivityMatrixInputSpec):
     atlas_configs = traits.Dict(desc='atlas configs for atlases to run connectivity for')
-    n_procs = traits.Int(1, usedefault=True)
 
 
 class DSIStudioAtlasGraphOutputSpec(TraitedSpec):
     connectivity_matfile = File(exists=True)
     commands = File()
 
 
@@ -348,148 +363,179 @@
     def _run_interface(self, runtime):
         # Get all inputs from the ApplyTransforms object
         ifargs = self.inputs.get()
         ifargs.pop('connectivity')
         ifargs['thread_count'] = 1
 
         # Get number of parallel jobs
-        num_threads = ifargs.pop('n_procs')
+        num_threads = ifargs.pop('nthreads')
         atlas_configs = ifargs.pop('atlas_configs')
-
-        # flatten the atlas_configs
-        args = [(atlas_name, atlas_config, ifargs) for atlas_name, atlas_config
-                in atlas_configs.items()]
-
-        if num_threads == 1:
-            outputs = [_dsi_studio_connectivity(arg) for arg in args]
+        workflow = pe.Workflow(name='dsistudio_atlasgraph')
+        nodes = []
+        merge_mats = pe.Node(niu.Merge(len(atlas_configs)), name='merge_mats')
+        outputnode = pe.Node(niu.IdentityInterface(fields=['matfiles']), name='outputnode')
+        workflow.connect(merge_mats, 'out', outputnode, 'matfiles')
+        for atlasnum, (atlas_name, atlas_config) in enumerate(atlas_configs.items(), start=1):
+            node_args = deepcopy(ifargs)
+            # Symlink in the fib file
+            node_args.pop('atlas_config')
+            node_args.pop('atlas_name')
+            nodes.append(
+                pe.Node(
+                    DSIStudioConnectivityMatrix(
+                        atlas_config=atlas_config,
+                        atlas_name=atlas_name,
+                        connectivity=atlas_config['dwi_resolution_file'],
+                        **node_args),
+                    name=atlas_name)
+            )
+            workflow.connect(nodes[-1], 'connectivity_matfile',
+                             merge_mats, 'in%d' % atlasnum)
+
+        workflow.config['execution']['stop_on_first_crash'] = 'true'
+        workflow.config['execution']['remove_unnecessary_outputs'] = 'false'
+        workflow.base_dir = runtime.cwd
+        if num_threads > 1:
+            wf_result = workflow.run(plugin='MultiProc', plugin_args={'n_procs': num_threads})
         else:
-            from concurrent.futures import ThreadPoolExecutor
-            with ThreadPoolExecutor(max_workers=num_threads) as pool:
-                outputs = list(pool.map(_dsi_studio_connectivity, args))
-
-        commands = [out[0] for out in outputs]
-        commands_file = op.join(runtime.cwd, "dsi_studio_commands.txt")
-        with open(commands_file, "w") as f:
-            f.write("\n----------\n".join(commands))
-        self._results['commands'] = commands_file
-
-        matfile_lists = [out[1] for out in outputs]
+            wf_result = workflow.run()
+        merge_node, = [node for node in list(wf_result.nodes) if node.name.endswith('merge_mats')]
         merged_connectivity_file = op.join(runtime.cwd, "combined_connectivity.mat")
-        _merge_conmats(matfile_lists, args, merged_connectivity_file)
+        _merge_conmats(merge_node.result.outputs.out, merged_connectivity_file)
         self._results['connectivity_matfile'] = merged_connectivity_file
 
         return runtime
 
 
 def _parse_network_file(txtfile):
     with open(txtfile, "r") as f:
         lines = f.readlines()
     network_data = {}
     for line in lines:
         sanitized_line = line.strip().replace("(", "_").replace(")", "")
         tokens = sanitized_line.split("\t")
         measure_name = tokens[0]
         if measure_name == 'network_measures':
-            network_data['region_ids'] = tokens[1:]
+            network_data['region_ids'] = [token.lstrip('region') for token in tokens[1:]]
             continue
 
         values = list(map(float, tokens[1:]))
         if len(values) == 1:
             network_data[measure_name] = values[0]
         else:
             network_data[measure_name] = np.array(values)
 
     return network_data
 
 
-def _merge_conmats(matfile_lists, recon_args, outfile):
+def _merge_conmats(matfile_lists, outfile):
     """Merge the many matfiles output by dsi studio and ensure they conform"""
     connectivity_values = {}
+    for matfile in matfile_lists:
+        connectivity_values.update(loadmat(matfile))
+    savemat(outfile, connectivity_values, long_field_names=True)
+
+
+def _sanitized_connectivity_matrix(conmat, official_labels):
+    """Load a matfile from DSI studio and re-format the connectivity matrix.
+
+    Parameters:
+    -----------
+
+        conmat : str
+            Path to a connectivity matfile from DSI Studio
+        official_labels : ndarray (M,)
+            Array of official ROI labels. The matrix in conmat will be reordered to
+            match the ROI labels in this array
+
+    Returns:
+    --------
+        connectivity_matrix : ndarray (M, M)
+            The DSI Studio data reordered to match official_labels
+    """
+    m = loadmat(conmat)
+    n_atlas_labels = len(official_labels)
+    # Column names are binary strings. Very confusing.
+    column_names = "".join(
+        [s.decode('UTF-8') for s in m["name"].squeeze().view("S1")]).split("\n")[:-1]
+    matfile_region_ids = np.array([int(name[6:]) for name in column_names])
+
+    # Where does each column go? Make an index array
+    connectivity = m['connectivity']
+    in_this_mask = np.isin(official_labels, matfile_region_ids)
+    truncated_labels = official_labels[in_this_mask]
+    assert np.all(truncated_labels == matfile_region_ids)
+    output = np.zeros((n_atlas_labels, n_atlas_labels))
+    new_row = np.searchsorted(official_labels, matfile_region_ids)
+
+    for row_index, conn in zip(new_row, connectivity):
+        tmp = np.zeros(n_atlas_labels)
+        tmp[in_this_mask] = conn
+        output[row_index] = tmp
+
+    return output
+
+
+def _sanitized_network_measures(network_txt, official_labels, atlas_name, measure):
+    """Load a network text file from DSI studio and re-format it.
+
+    Parameters:
+    -----------
+
+        network_txt : str
+            Path to a network text file from DSI Studio
+        official_labels : ndarray (M,)
+            Array of official ROI labels. The matrix in conmat will be reordered to
+            match the ROI labels in this array
+        atlas_name : str
+            Name of the atlas used
+        measure : the name of the connectivity measure
+
+    Returns:
+    --------
+        connectivity_matrix : ndarray (M, M)
+            The DSI Studio data reordered to match official_labels
+    """
+    network_values = {}
+    n_atlas_labels = len(official_labels)
+    network_data = _parse_network_file(network_txt)
+    # Make sure to get the full atlas
+    network_region_ids = np.array(network_data['region_ids']).astype(np.int)
+    # If all the regions are found
+    in_this_mask = np.isin(official_labels, network_region_ids)
+    if np.all(in_this_mask):
+        truncated_labels = official_labels
+    else:
+        truncated_labels = official_labels[in_this_mask]
+    assert np.all(truncated_labels == network_region_ids)
+
+    for net_measure_name, net_measure_data in network_data.items():
+        variable_name = atlas_name + "_" + measure + "_" + net_measure_name
+        if type(net_measure_data) is np.ndarray:
+            tmp = np.zeros(n_atlas_labels)
+            tmp[in_this_mask] = net_measure_data
+            network_values[variable_name] = tmp
+        else:
+            network_values[variable_name] = net_measure_data
 
-    for matfile_list, (atlas_name, atlas_config, ifargs) in zip(matfile_lists, recon_args):
-        matfiles = [f for f in matfile_list if f.endswith('.mat')]
-        txtfiles = [f for f in matfile_list if f.endswith('.txt')]
-
-        labels = np.array(atlas_config['node_ids']).astype(np.int)
-        connectivity_values[atlas_name + "_region_ids"] = labels
-        connectivity_values[atlas_name + "_region_labels"] = np.array(atlas_config['node_names'])
-        n_atlas_labels = len(labels)
-
-        for conmat in matfiles:
-            m = loadmat(conmat)
-            measure = "_".join(conmat.split(".")[-4:-2])
-            # Column names are binary strings. Very confusing.
-            column_names = "".join(
-                [s.decode('UTF-8') for s in m["name"].squeeze().view("S1")]).split("\n")[:-1]
-            region_ids = np.array([int(name[6:]) for name in column_names])
-
-            # Where does each column go? Make an index array
-            connectivity = m['connectivity']
-            in_this_mask = np.in1d(labels, region_ids)
-            truncated_labels = labels[in_this_mask]
-            assert np.all(truncated_labels == region_ids)
-            output = np.zeros((n_atlas_labels, n_atlas_labels))
-            new_row = np.searchsorted(labels, region_ids)
-
-            for row_index, conn in zip(new_row, connectivity):
-                tmp = np.zeros(n_atlas_labels)
-                tmp[in_this_mask] = conn
-                output[row_index] = tmp
-            connectivity_values[atlas_name + "_" + measure + "_connectivity"] = output
-
-        for network_txt in txtfiles:
-            measure = "_".join(network_txt.split(".")[-4:-2])
-            network_data = _parse_network_file(network_txt)
-
-            # Make sure to get the full atlas
-            region_ids = np.array(network_data.pop('region_ids')).astype(np.int)
-            in_this_mask = np.in1d(labels, region_ids)
-            truncated_labels = labels[in_this_mask]
-            assert np.all(truncated_labels == region_ids)
-            new_row = np.searchsorted(labels, region_ids)
-
-            for net_measure_name, net_measure_data in network_data.items():
-                variable_name = atlas_name + "_" + measure + "_" + net_measure_name
-                if type(net_measure_data) is np.ndarray:
-                    tmp = np.zeros_like(net_measure_data)
-                    tmp[in_this_mask] = net_measure_data
-                    connectivity_values[variable_name] = tmp
-                else:
-                    connectivity_values[variable_name] = net_measure_data
-
-    savemat(outfile, connectivity_values)
-
-
-def _dsi_studio_connectivity(args):
-    atlas_name, atlas_config, ifargs = args
-    rundir = op.abspath(atlas_name)
-    # Make a temporary directory for this node
-    os.makedirs(rundir, exist_ok=True)
-    ifargs = deepcopy(ifargs)
-    input_fib = ifargs.pop('input_fib')
-    new_fib = op.join(rundir, op.split(input_fib)[1])
-    os.symlink(input_fib, new_fib)
-    con = DSIStudioTracking(input_fib=new_fib, connectivity=atlas_config['dwi_resolution_file'],
-                            **ifargs)
-    con.terminal_output = 'allatonce'
-    con.resource_monitor = False
-    LOGGER.info(con.cmdline)
-    run = con.run(cwd=rundir)
-    runtime = run.runtime
-
-    return runtime.cmdline, run.outputs.connectivity_matrices
+    return network_values
 
 
 class DSIStudioTrackingInputSpec(DSIStudioConnectivityMatrixInputSpec):
     roi = File(exists=True, argstr="--roi=%s")
     roi2 = File(exists=True, argstr="--roi2=%s")
     roa = File(exists=True, argstr="--roa=%s")
     end = File(exists=True, argstr="--end=%s")
     end2 = File(exists=True, argstr="--end2=%s")
     ter = File(exists=True, argstr="--ter=%s")
+    output_trk = traits.Str(
+        name_template="%s.trk.gz",
+        desc="Output file (trk.gz)",
+        argstr="--output=%s",
+        name_source="input_fib")
 
 
 class DSIStudioTrackingOutputSpec(TraitedSpec):
     output_trk = traits.Str(
         name_template="%s.trk.gz",
         desc="Output file (trk.gz)",
         argstr="--output=%s",
@@ -502,18 +548,20 @@
 class DSIStudioTracking(CommandLine):
     input_spec = DSIStudioTrackingInputSpec
     output_spec = DSIStudioTrackingOutputSpec
     _cmd = "dsi_studio --action=trk"
 
     def _list_outputs(self):
         outputs = self.output_spec().get()
-        results = glob(self.inputs.output_trk + "*src*fib*trk.gz")
+        results = glob("*trk.gz")
         if len(results) == 1:
             trk_out = os.path.abspath(results[0])
             outputs["output_trk"] = trk_out
+        else:
+            raise Exception("DSI Studio did not produce a trk.gz file")
         conmat_results = glob("*.connectivity.mat")
         outputs["connectivity_matrices"] = [
             os.path.abspath(c) for c in conmat_results
         ]
         if isdefined(self.inputs.to_export):
             if "gfa" in self.inputs.to_export:
                 outputs["output_gfa"] = trk_out + ".gfa.txt"
@@ -539,22 +587,25 @@
         dsi_studio_file = self.inputs.dsi_studio_nifti
         new_file = fname_presuffix(dsi_studio_file, suffix="fixhdr", newpath=runtime.cwd)
         dsi_img = nb.load(dsi_studio_file)
         correct_img = nb.load(self.inputs.correct_header_nifti)
 
         new_axcodes = nb.aff2axcodes(correct_img.affine)
         input_axcodes = nb.aff2axcodes(dsi_img.affine)
+
         # Is the input image oriented how we want?
         if not input_axcodes == new_axcodes:
             # Re-orient
             input_orientation = nb.orientations.axcodes2ornt(input_axcodes)
             desired_orientation = nb.orientations.axcodes2ornt(new_axcodes)
             transform_orientation = nb.orientations.ornt_transform(input_orientation,
                                                                    desired_orientation)
             reoriented_img = dsi_img.as_reoriented(transform_orientation)
-            nb.Nifti1Image(reoriented_img.get_data(), correct_img.affine, correct_img.header
-                           ).to_filename(new_file)
-            self._results['out_file'] = new_file
+
         else:
-            self._results['out_file'] = dsi_studio_file
+            reoriented_img = dsi_img
+
+        # No matter what, still use the correct affine
+        nb.Nifti1Image(reoriented_img.get_data(), correct_img.affine).to_filename(new_file)
+        self._results['out_file'] = new_file
 
         return runtime
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/confounds.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/confounds.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/gradients.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/gradients.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/converters.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/converters.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,56 +103,20 @@
     def _run_interface(self, runtime):
         fib_file = self.inputs.fib_file
         if isdefined(self.inputs.mif_file):
             output_mif_file = self.inputs.mif_file
         else:
             output_mif_file = fname_presuffix(fib_file, newpath=runtime.cwd, suffix=".mif",
                                               use_ext=False)
-        fibmat = fast_load_fibgz(fib_file)
-        dims = tuple(fibmat['dimension'].squeeze().astype(np.int))
-        directions = fibmat['odf_vertices'].T
-
-        odf_vars = [k for k in fibmat.keys() if re.match("odf\\d+", k)]
-        valid_odfs = []
-        flat_mask = fibmat["fa0"].squeeze() > 0
-        n_voxels = np.prod(dims)
-        for n in range(len(odf_vars)):
-            varname = "odf%d" % n
-            odfs = fibmat[varname]
-            odf_sum = odfs.sum(0)
-            odf_sum_mask = odf_sum > 0
-            valid_odfs.append(odfs[:, odf_sum_mask].T)
-        odf_array = np.row_stack(valid_odfs)
-        if self.inputs.subtract_iso:
-            odf_array = odf_array - odf_array.min(0)
-
-        # Convert each column to a 3d file, then concatenate them
-        odfs_3d = []
-        for odf_vals in odf_array.T:
-            new_data = np.zeros(n_voxels, dtype=np.float32)
-            new_data[flat_mask] = odf_vals
-            odfs_3d.append(new_data.reshape(dims, order="F"))
-
-        real_img = nb.load(self.inputs.ref_image)
-        odf4d = np.stack(odfs_3d, -1)
-        odf4d_img = nb.Nifti1Image(odf4d, real_img.affine, real_img.header)
-        odf_values_file = op.join(runtime.cwd, "odf_values.nii")
-        odf4d_img.to_filename(odf_values_file)
-
-        num_dirs, _ = directions.shape
-        hemisphere = num_dirs // 2
-        x, y, z = directions[:hemisphere].T
-        _, theta, phi = cart2sphere(-x, -y, z)
-        dirs_txt = op.join(runtime.cwd, "ras+directions.txt")
-        np.savetxt(dirs_txt, np.column_stack([phi, theta]))
-
-        popen_run(["amp2sh", "-quiet", "-force", "-directions", dirs_txt, "odf_values.nii",
-                   output_mif_file])
-        os.remove(odf_values_file)
-        os.remove(dirs_txt)
+        # Get the amplitudes as a Nifti1Image and sphere directions
+        amplitudes, directions = fib2amps(fib_file,
+                                          self.inputs.ref_image,
+                                          self.inputs.subtract_iso)
+        # convert them to MRTrix mif format
+        amplitudes_to_sh_mif(amplitudes, directions, output_mif_file, runtime.cwd)
         self._results['mif_file'] = output_mif_file
         return runtime
 
 
 def get_dsi_studio_ODF_geometry(odf_key):
     mat_path = pkgr('qsiprep', 'data/odfs.mat')
     m = loadmat(mat_path)
@@ -307,14 +271,42 @@
 
     popen_run(["amp2sh", "-quiet", "-force", "-directions", dirs_txt, "odf_values.nii",
                output_file])
     os.remove(temp_nii)
     os.remove(dirs_txt)
 
 
+def mif2amps(sh_mif_file, working_dir, dsi_studio_odf="odf8"):
+    """Convert a MRTrix SH mif file to a NiBabel amplitudes image.
+
+    Parameters:
+    ===========
+
+    sh_mif_file : str
+        path to the mif file with SH coefficients
+
+    """
+    verts, _ = get_dsi_studio_ODF_geometry(dsi_studio_odf)
+    num_dirs, _ = verts.shape
+    hemisphere = num_dirs // 2
+    directions = verts[:hemisphere]
+    x, y, z = directions.T
+    _, theta, phi = cart2sphere(x, y, -z)
+    dirs_txt = op.join(working_dir, "directions.txt")
+    np.savetxt(dirs_txt, np.column_stack([phi, theta]))
+
+    odf_amplitudes_nii = op.join(working_dir, "amplitudes.nii")
+    popen_run(["sh2amp", "-quiet", "-nonnegative", sh_mif_file, dirs_txt, odf_amplitudes_nii])
+
+    if not op.exists(odf_amplitudes_nii):
+        raise FileNotFoundError("Unable to create %s", odf_amplitudes_nii)
+    amplitudes_img = nb.load(odf_amplitudes_nii)
+    return amplitudes_img, directions
+
+
 def fast_load_fibgz(fib_file):
     """Load a potentially gzipped fibgz file more quickly than using built-in gzip.
     """
     # Try to load a non-zipped file
     if not fib_file.endswith("gz"):
         return loadmat(fib_file)
 
@@ -337,7 +329,40 @@
         fh = StringIO(p.communicate()[0])
         assert p.returncode == 0
         return loadmat(fh)
 
     with gzip.open(fib_file, "r") as f:
         LOGGER.info("Loading with python gzip. To load faster install zcat or gzcat.")
         return loadmat(f)
+
+
+def fib2amps(fib_file, ref_image, subtract_iso=True):
+    fibmat = fast_load_fibgz(fib_file)
+    dims = tuple(fibmat['dimension'].squeeze().astype(np.int))
+    directions = fibmat['odf_vertices'].T
+
+    odf_vars = [k for k in fibmat.keys() if re.match("odf\\d+", k)]
+    valid_odfs = []
+    flat_mask = fibmat["fa0"].squeeze().ravel(order='F') > 0
+    n_voxels = np.prod(dims)
+    for n in range(len(odf_vars)):
+        varname = "odf%d" % n
+        odfs = fibmat[varname]
+        odf_sum = odfs.sum(0)
+        odf_sum_mask = odf_sum > 0
+        valid_odfs.append(odfs[:, odf_sum_mask].T)
+    odf_array = np.row_stack(valid_odfs)
+    if subtract_iso:
+        odf_array = odf_array - odf_array.min(0)
+
+    # Convert each column to a 3d file, then concatenate them
+    odfs_3d = []
+    for odf_vals in odf_array.T:
+        new_data = np.zeros(n_voxels, dtype=np.float32)
+        new_data[flat_mask] = odf_vals
+        odfs_3d.append(new_data.reshape(dims, order="F"))
+
+    real_img = nb.load(ref_image)
+    odf4d = np.stack(odfs_3d, -1)
+    odf4d_img = nb.Nifti1Image(odf4d, real_img.affine, real_img.header)
+
+    return odf4d_img, directions
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/freesurfer.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/freesurfer.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/surf.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/surf.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/reports.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/reports.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,24 +16,30 @@
 import re
 from collections import defaultdict
 from mpl_toolkits.mplot3d import Axes3D  # noqa: F401
 import seaborn as sns
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import animation
+from scipy.io.matlab import loadmat
 import pandas as pd
 import numpy as np
 from nipype.interfaces.base import (
     traits, TraitedSpec, BaseInterfaceInputSpec,
     File, Directory, InputMultiPath, InputMultiObject, Str, isdefined,
     SimpleInterface)
 from nipype.interfaces import freesurfer as fs
+from nipype.interfaces.mixins import reporting
+import nibabel as nb
+from dipy.core.sphere import HemiSphere
 from .gradients import concatenate_bvals, concatenate_bvecs
 from .qc import createB0_ColorFA_Mask_Sprites, createSprite4D
 from .bids import get_bids_params
+from ..niworkflows.viz.utils import peak_slice_series, odf_roi_plot
+from .converters import fib2amps, mif2amps
 
 SUBJECT_TEMPLATE = """\t<ul class="elem-desc">
 \t\t<li>Subject ID: {subject_id}</li>
 \t\t<li>Structural images: {n_t1s:d} T1-weighted {t2w}</li>
 \t\t<li>Diffusion-weighted series: inputs {n_dwis:d}, outputs {n_outputs:d}</li>
 {groupings}
 \t\t<li>Resampling targets: {output_spaces}
@@ -304,14 +310,18 @@
         bvals = concatenate_bvals(self.inputs.orig_bval_files, None)
         if isdefined(self.inputs.source_files):
             file_array = np.array(self.inputs.source_files)
             unique_files, filenums = np.unique(file_array, return_inverse=True)
         else:
             filenums = np.ones_like(bvals)
 
+        # Account for the possibility that this is a PE Pair average
+        if len(filenums) == len(bvals) * 2:
+            filenums = filenums[:len(bvals)]
+
         # Plot the final bvecs if provided
         final_bvecs = None
         if isdefined(self.inputs.final_bvec_file):
             final_bvecs = np.loadtxt(self.inputs.final_bvec_file).T
 
         plot_gradients(bvals, orig_bvecs, filenums, outfile, final_bvecs)
         self._results['plot_file'] = outfile
@@ -336,14 +346,16 @@
             x, y, z = np.column_stack([minvec, maxvec])
             ax.plot(x, y, z, color="k")
             txt_pos = maxvec + 5
             ax.text(txt_pos[0], txt_pos[1], txt_pos[2], labels[axnum], size=8,
                     zorder=1, color='k')
 
     if final_bvecs is not None:
+        if final_bvecs.shape[0] == 3:
+            final_bvecs = final_bvecs.T
         fqx, fqy, fqz = (qrads[:, np.newaxis] * final_bvecs).T
         fig, axes = plt.subplots(nrows=1, ncols=2, figsize=(10, 5),
                                  subplot_kw={"aspect": "equal", "projection": "3d"})
         orig_ax = axes[0]
         final_ax = axes[1]
         axes_list = [orig_ax, final_ax]
         final_ax.scatter(fqx, fqy, fqz, c=source_filenums, marker="+")
@@ -543,56 +555,92 @@
         prefix + 'neighbor_corr': [dwi_corr],
         prefix + 'num_bad_slices': [n_bad_slices],
         prefix + 'num_directions': [n_dirs]
     }
     return data
 
 
-def calculate_motion_summary(confounds_tsv):
-    if not isdefined(confounds_tsv) or confounds_tsv is None:
-        return {
-            "mean_fd": [np.nan],
-            "max_fd": [np.nan],
-            "max_rotation": [np.nan],
-            "max_translation": [np.nan],
-            "max_rel_rotation": [np.nan],
-            "max_rel_translation": [np.nan]
-        }
-    df = pd.read_csv(confounds_tsv, delimiter="\t")
-    translations = df[['trans_x', 'trans_y', 'trans_z']].to_numpy()
-    rotations = df[['rot_x', 'rot_y', 'rot_z']].to_numpy()
+def motion_derivatives(translations, rotations, framewise_disp,
+                       original_files):
 
     def padded_diff(data):
         out = np.zeros_like(data)
         out[1:] = np.diff(data, axis=0)
         return out
 
     drotations = padded_diff(rotations)
     dtranslations = padded_diff(translations)
 
     # We don't want the relative values across the boundaries of runs.
     # Determine which values should be ignored
-    file_labels, _ = pd.factorize(df['original_file'])
+    file_labels, _ = pd.factorize(original_files)
     new_files = padded_diff(file_labels)
 
     def file_masked(data):
         masked_data = data.copy()
         masked_data[new_files > 0] = 0
         return masked_data
 
-    framewise_disp = file_masked(df['framewise_displacement'].abs())
-    motion_summary = {
+    framewise_disp = file_masked(framewise_disp)
+    return {
         "mean_fd": [framewise_disp.mean()],
         "max_fd": [framewise_disp.max()],
         "max_rotation": [file_masked(np.abs(rotations)).max()],
         "max_translation": [file_masked(np.abs(translations)).max()],
         "max_rel_rotation": [file_masked(np.abs(drotations)).max()],
         "max_rel_translation": [file_masked(np.abs(dtranslations)).max()]
     }
-    return motion_summary
+
+
+def calculate_motion_summary(confounds_tsv):
+    if not isdefined(confounds_tsv) or confounds_tsv is None:
+        return {
+            "mean_fd": [np.nan],
+            "max_fd": [np.nan],
+            "max_rotation": [np.nan],
+            "max_translation": [np.nan],
+            "max_rel_rotation": [np.nan],
+            "max_rel_translation": [np.nan]
+        }
+    df = pd.read_csv(confounds_tsv, delimiter="\t")
+
+    # the default case where each output image comes from one input image
+    if 'trans_x' in df.columns:
+        translations = df[['trans_x', 'trans_y', 'trans_z']].to_numpy()
+        rotations = df[['rot_x', 'rot_y', 'rot_z']].to_numpy()
+        return motion_derivatives(translations, rotations, df['framewise_displacement'],
+                                  df['original_file'])
+
+    # If there was a PE Pair averaging, get motion from both
+    motion1 = motion_derivatives(df[['trans_x_1', 'trans_y_1', 'trans_z_1']].to_numpy(),
+                                 df[['rot_x_1', 'rot_y_1', 'rot_z_1']].to_numpy(),
+                                 df['framewise_displacement_1'],
+                                 df['original_file_1'])
+
+    motion2 = motion_derivatives(df[['trans_x_2', 'trans_y_2', 'trans_z_2']].to_numpy(),
+                                 df[['rot_x_2', 'rot_y_2', 'rot_z_2']].to_numpy(),
+                                 df['framewise_displacement_2'],
+                                 df['original_file_2'])
+
+    # Combine the FDs from both PE directions
+    # both_fd = np.column_stack([m1, m2])
+    # framewise_disp = both_fd[np.nanargmax(np.abs(both_fd), axis=1)]
+    def compare_series(key_name, comparator):
+        m1 = motion1[key_name][0]
+        m2 = motion2[key_name][0]
+        return [comparator(m1, m2)]
+
+    return {
+        "mean_fd": compare_series("mean_fd", lambda a, b: (a + b) / 2),
+        "max_fd": compare_series("max_fd", max),
+        "max_rotation": compare_series("max_rotation", max),
+        "max_translation": compare_series("max_translation", max),
+        "max_rel_rotation": compare_series("max_rel_rotation", max),
+        "max_rel_translation": compare_series("max_rel_translation", max)
+    }
 
 
 class _InteractiveReportInputSpec(TraitedSpec):
     raw_dwi_file = File(exists=True, mandatory=True)
     processed_dwi_file = File(exists=True, mandatory=True)
     confounds_file = File(exists=True, mandatory=True)
     mask_file = File(exists=True, mandatory=True)
@@ -653,7 +701,111 @@
     n_samples = labels.shape[0]
     max_label = labels.max()
     if max_label == 0:
         return [(1.0, 0.0, 0.0)] * n_samples
     labels = labels / max_label
     colors = np.array([cmap(label) for label in labels])
     return colors.tolist()
+
+
+class _ReconPeaksReportInputSpec(BaseInterfaceInputSpec):
+    mif_file = File(exists=True)
+    fib_file = File(exists=True)
+    odf_file = File(exists=True)
+    directions_file = File(exists=True)
+    mask_file = File(exists=True)
+    background_image = File(exists=True)
+    odf_rois = File(exists=True)
+    subtract_iso = traits.Bool(False, usedefault=True,
+                               desc='subtract isotropic component from ODFs')
+
+
+class _ReconPeaksReportOutputSpec(reporting.ReportCapableOutputSpec):
+    odf_report = File(exists=True)
+
+
+class ReconPeaksReport(SimpleInterface):
+    input_spec = _ReconPeaksReportInputSpec
+    output_spec = _ReconPeaksReportOutputSpec
+    _ncuts = 4
+    _padding = 4
+    _redirect_x = True
+
+    def _run_interface(self, runtime):
+        """Generate a reportlet."""
+        if isdefined(self.inputs.mif_file):
+            odf_img, directions = mif2amps(self.inputs.mif_file, runtime.cwd)
+        elif isdefined(self.inputs.fib_file):
+            odf_img, directions = fib2amps(self.inputs.fib_file,
+                                           self.inputs.background_image,
+                                           runtime.cwd)
+        elif isdefined(self.inputs.odf_file) and isdefined(self.inputs.directions_file):
+            odf_img = nb.load(self.inputs.odf_file)
+            directions = np.load(self.inputs.directions_file)
+        else:
+            raise Exception('Requires either a mif file or fib file')
+        odf_4d = odf_img.get_fdata()
+        sphere = HemiSphere(xyz=directions.astype(np.float))
+        if not isdefined(self.inputs.background_image) or self.inputs.background_image is None:
+            background_data = odf_4d.mean(3)
+        else:
+            background_data = nb.load(self.inputs.background_image).get_fdata()
+
+        peak_report = op.join(runtime.cwd, 'peak_report.png')
+        peak_slice_series(odf_4d, sphere, background_data, peak_report,
+                          n_cuts=self._ncuts, mask_image=self.inputs.mask_file,
+                          padding=self._padding)
+        self._results['out_report'] = peak_report
+
+        # Plot ODFs in interesting regions
+        if isdefined(self.inputs.odf_rois):
+            odf_report = op.join(runtime.cwd, 'odf_report.png')
+            odf_roi_plot(odf_4d, sphere, background_data, odf_report, self.inputs.odf_rois,
+                         subtract_iso=self.inputs.subtract_iso,
+                         mask=self.inputs.mask_file)
+            self._results['odf_report'] = odf_report
+        return runtime
+
+
+class _ConnectivityReportInputSpec(BaseInterfaceInputSpec):
+    connectivity_matfile = File(exists=True)
+
+
+class _ConnectivityReportOutputSpec(reporting.ReportCapableOutputSpec):
+    odf_report = File(exists=True)
+
+
+class ConnectivityReport(SimpleInterface):
+    input_spec = _ConnectivityReportInputSpec
+    output_spec = _ConnectivityReportOutputSpec
+
+    def _run_interface(self, runtime):
+        """Generate a reportlet."""
+        mat = loadmat(self.inputs.connectivity_matfile)
+        connectivity_keys = [key for key in mat.keys() if key.endswith('connectivity')]
+        atlases = sorted(set([key.split("_")[0] for key in connectivity_keys]))
+        measures = sorted(set(["_".join(key.split("_")[1:-1]) for key in connectivity_keys]))
+        nrows = len(atlases)
+        ncols = len(measures)
+        fig, ax = plt.subplots(nrows=nrows, ncols=ncols, squeeze=False)
+        for connectivity_key in connectivity_keys:
+            atlas = connectivity_key.split("_")[0]
+            measure = "_".join(connectivity_key.split("_")[1:-1])
+            row = atlases.index(atlas)
+            col = measures.index(measure)
+            ax[row, col].imshow(mat[connectivity_key], interpolation='nearest',
+                                cmap="Greys", aspect='equal')
+            ax[row, col].set_xticks([])
+            ax[row, col].set_yticks([])
+        fig.set_size_inches((ncols, nrows))
+        fig.subplots_adjust(left=0.05, top=0.95, wspace=0, hspace=0, bottom=0, right=1)
+
+        for measure_num, measure_name in enumerate(measures):
+            ax[0, measure_num].set_title(measure_name.replace('_', '/'),
+                                         fontdict={'fontsize': 6})
+        for atlas_num, atlas_name in enumerate(atlases):
+            ax[atlas_num, 0].set_ylabel(atlas_name, fontdict={'fontsize': 8})
+
+        conn_report = op.join(runtime.cwd, 'conn_report.svg')
+        fig.savefig(conn_report)
+        self._results['out_report'] = conn_report
+        return runtime
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/anatomical.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/anatomical.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/bids.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/bids.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     bval_file = File(exists=True)
     bvec_file = File(exists=True)
     b_file = File(exists=True)
     confounds_file = File(exists=True)
     dwi_file = File(exists=True)
     local_bvec_file = File()
     mask_file = File()
+    dwi_ref = File(exists=True)
 
 
 class QsiReconIngress(SimpleInterface):
     input_spec = QsiReconIngressInputSpec
     output_spec = QsiReconIngressOutputSpec
 
     def _run_interface(self, runtime):
@@ -107,14 +108,15 @@
         out_root, fname, ext = split_filename(self.inputs.dwi_file)
         self._results['bval_file'] = op.join(out_root, fname+".bval")
         self._results['bvec_file'] = op.join(out_root, fname+".bvec")
         self._get_if_exists('confounds_file', op.join(out_root, "*confounds.tsv"))
         self._get_if_exists('local_bvec_file', op.join(out_root, fname[:-3]+'bvec.nii*'))
         self._get_if_exists('b_file', op.join(out_root, fname+".b"))
         self._get_if_exists('mask_file', op.join(out_root, fname[:-11] + 'brain_mask.nii.gz'))
+        self._get_if_exists('dwi_ref', op.join(out_root, fname[:-16] + 'dwiref.nii.gz'))
         self._results['dwi_file'] = self.inputs.dwi_file
 
         # Get the anatomical data
         path_parts = out_root.split(op.sep)[:-1]  # remove "dwi"
         # Anat is above ses
         if path_parts[-1].startswith('ses'):
             path_parts.pop()
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/shoreline.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/shoreline.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/dipy.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/dipy.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,16 @@
 class DipyReconOutputSpec(TraitedSpec):
     fibgz = File()
     fod_sh_mif = File()
     extrapolated_dwi = File()
     extrapolated_bvals = File()
     extrapolated_bvecs = File()
     extrapolated_b = File()
+    odf_amplitudes = File()
+    odf_directions = File()
 
 
 class DipyReconInterface(SimpleInterface):
     input_spec = DipyReconInputSpec
     output_spec = DipyReconOutputSpec
 
     def _get_gtab(self, external_bvals=None, external_bvecs=None):
@@ -193,14 +195,22 @@
         # Convert to amplitudes for other software
         verts, faces = get_dsi_studio_ODF_geometry("odf8")
         num_dirs, _ = verts.shape
         hemisphere = num_dirs // 2
         x, y, z = verts[:hemisphere].T
         hs = HemiSphere(x=x, y=y, z=z)
         odf_amplitudes = nb.Nifti1Image(fit_obj.odf(hs), mask_img.affine, mask_img.header)
+        output_amps_file = fname_presuffix(self.inputs.dwi_file, suffix=suffix+"_amp.nii.gz",
+                                           newpath=runtime.cwd, use_ext=False)
+        output_dirs_file = fname_presuffix(self.inputs.dwi_file, suffix=suffix+"_dirs.npy",
+                                           newpath=runtime.cwd, use_ext=False)
+        odf_amplitudes.to_filename(output_amps_file)
+        np.save(output_dirs_file, verts[:hemisphere])
+        self._results['odf_amplitudes'] = output_amps_file
+        self._results['odf_directions'] = output_dirs_file
 
         if self.inputs.write_fibgz:
             output_fib_file = fname_presuffix(self.inputs.dwi_file, suffix=suffix+".fib",
                                               newpath=runtime.cwd, use_ext=False)
             LOGGER.info("Writing DSI Studio fib file %s", output_fib_file)
             amplitudes_to_fibgz(odf_amplitudes, verts, faces, output_fib_file, mask_img,
                                 num_fibers=5)
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/fmap.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/fmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1037,15 +1037,15 @@
         return b0_indices
     selected_indices = np.linspace(0, len(b0_indices)-1, num=max_per_spec,
                                    endpoint=True, dtype=np.int)
     return [b0_indices[idx] for idx in selected_indices]
 
 
 def add_epi_fmaps_to_dwi_b0s(epi_fmaps, b0_threshold, max_per_spec, dwi_spec_lines, dwi_imain):
-    """Add additional images from EPI fieldmaps or distortion correction.
+    """Add additional images from EPI fieldmaps for distortion correction.
 
     In order to fill out the maximum number of images per distortion group, images
     from files in the fmap/ directory can be added to those already extracted from the
     DWI series.
 
     Examples:
     ---------
@@ -1087,30 +1087,39 @@
 
     new_report = topup_selection_to_report(
         fmap_indices_to_add, fmap_original_files, fmap_spec_map, image_source='EPI fieldmap')
 
     return topup_imain, topup_spec_lines, new_report
 
 
-def eddy_inputs_from_dwi_files(origin_file_list, eddy_prefix):
-    unique_files = list(set(origin_file_list))
+def get_distortion_grouping(origin_file_list):
+    """Discover which distortion groups are present, then assign each volume to a group.
+    """
+    unique_files = sorted(set(origin_file_list))
+    unique_acqps = []
     line_lookup = {}
-    acqp_data = []
-    for line_num, unique_dwi in enumerate(unique_files):
+    for unique_dwi in unique_files:
         spec = read_nifti_sidecar(unique_dwi)
         spec_line = acqp_lines[spec['PhaseEncodingDirection']]
         acqp_line = spec_line % spec['TotalReadoutTime']
-        line_lookup[unique_dwi] = line_num + 1
-        acqp_data.append(acqp_line)
+        if acqp_line not in unique_acqps:
+            unique_acqps.append(acqp_line)
+        line_lookup[unique_dwi] = unique_acqps.index(acqp_line) + 1
+
+    group_numbers = [line_lookup[dwi_file] for dwi_file in origin_file_list]
+    return unique_acqps, group_numbers
+
+
+def eddy_inputs_from_dwi_files(origin_file_list, eddy_prefix):
+    unique_acqps, group_numbers = get_distortion_grouping(origin_file_list)
 
     # Create the acqp file
     acqp_file = eddy_prefix + "acqp.txt"
     with open(acqp_file, "w") as f:
-        f.write("\n".join(acqp_data))
+        f.write("\n".join(unique_acqps))
 
     # Create the index file
     index_file = eddy_prefix + "index.txt"
-    index_numbers = [line_lookup[dwi_file] for dwi_file in origin_file_list]
     with open(index_file, "w") as f:
-        f.write(" ".join(map(str, index_numbers)))
+        f.write(" ".join(map(str, group_numbers)))
 
     return acqp_file, index_file
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/eddy.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/eddy.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/niworkflows.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/niworkflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             # Get the slice counts
             mask_img = nb.load(mask_file)
             mask = mask_img.get_data() > 0
             masked_slices = (mask * np.arange(mask_img.shape[2])[np.newaxis, np.newaxis, :]
                              ).astype(np.int)
             slice_nums, slice_counts = np.unique(masked_slices[mask], return_counts=True)
             self.qc_data = {
-                'slice_scores': slice_scores.T,
+                'slice_scores': slice_scores,
                 'slice_counts': slice_counts}
 
         self.confounds = confounds
 
     def plot(self, figure=None):
         """Main plotter"""
         sns.set_style("whitegrid")
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/connectivity.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/connectivity.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/utils.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,25 @@
         np.savetxt(out_file, data, delimiter='\t', header='\t'.join(self.inputs.columns),
                    comments='')
 
         self._results['out_file'] = out_file
         return runtime
 
 
+class TestInputInputSpec(BaseInterfaceInputSpec):
+    test1 = traits.Any()
+
+
+class TestInput(SimpleInterface):
+    input_spec = TestInputInputSpec
+
+    def _run_interface(self, runtime):
+        return runtime
+
+
 class JoinTSVColumnsInputSpec(BaseInterfaceInputSpec):
     in_file = File(exists=True, mandatory=True, desc='input file')
     join_file = File(exists=True, mandatory=True, desc='file to be adjoined')
     side = traits.Enum('right', 'left', usedefault=True, desc='where to join')
     columns = traits.List(traits.Str, desc='header for columns')
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/itk.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/itk.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/images.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/images.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 Image tools interfaces
 ~~~~~~~~~~~~~~~~~~~~~~
 
 
 """
 
 import os
+from textwrap import indent
 import numpy as np
 import nibabel as nb
 import nilearn.image as nli
-from textwrap import indent
 from dipy.io import read_bvals_bvecs
 from nipype import logging
 from nipype.utils.filemanip import fname_presuffix
 from nipype.interfaces.base import (isdefined, traits, TraitedSpec, BaseInterfaceInputSpec,
                                     SimpleInterface, File, InputMultiObject, OutputMultiObject)
 from nipype.interfaces import fsl
 # from qsiprep.interfaces.images import (
@@ -64,89 +64,14 @@
         self._results['bvec_files'] = split_bvec_files
         self._results['b0_images'] = b0_paths
         self._results['b0_indices'] = b0_indices.tolist()
 
         return runtime
 
 
-class ConcatRPESplitsInputSpec(BaseInterfaceInputSpec):
-    # Plus images
-    dwi_plus = InputMultiObject(File(exists=True), desc='plus dwi file')
-    bvec_plus = InputMultiObject(File(exists=True), desc='plus bvec file')
-    bval_plus = InputMultiObject(File(exists=True), desc='plus bval file')
-    noise_images_plus = InputMultiObject(File(exists=True), desc='plus_noise_images')
-    bias_images_plus = InputMultiObject(File(exists=True), desc='plus bias images')
-    denoising_confounds_plus = File(exists=True, desc='confounds csv from merging plus')
-    validation_reports_plus = InputMultiObject(File(exists=True))
-
-    # Minus images
-    dwi_minus = InputMultiObject(File(exists=True), desc='minus dwi file')
-    bvec_minus = InputMultiObject(File(exists=True), desc='minus bvec file')
-    bval_minus = InputMultiObject(File(exists=True), desc='minus bval file')
-    noise_images_minus = InputMultiObject(File(exists=True), desc='minus_noise_images')
-    bias_images_minus = InputMultiObject(File(exists=True), desc='minus bias images')
-    denoising_confounds_minus = File(exists=True, desc='confounds csv from merging minus')
-    validation_reports_minus = InputMultiObject(File(exists=True))
-
-
-class ConcatRPESplitsOutputSpec(TraitedSpec):
-    dwi_file = OutputMultiObject(File(exists=True), desc='plus and minus merged into on series')
-    bvec_file = OutputMultiObject(File(exists=True), desc='concatenated bvec file')
-    bval_file = OutputMultiObject(File(exists=True), desc='concatenated bval file')
-    bias_images = OutputMultiObject(File(exists=True), desc='bias field images')
-    noise_images = OutputMultiObject(File(exists=True), desc='noise level images')
-    b0_images = OutputMultiObject(File(exists=True), desc='just the b0s')
-    b0_indices = traits.List(desc='list of indices for each b0 image')
-    original_files = traits.List(desc='list of source series for each dwi')
-    sdc_method = traits.Str("PEB/PEPOLAR Series (phase-encoding based / PE-POLARity)")
-    denoising_confounds = File(exists=True, desc='plus and minus confounds merged')
-    validation_reports = OutputMultiObject(File(exists=True))
-
-
-class ConcatRPESplits(SimpleInterface):
-    """Combine the outputs from the RPE series workflow into a SplitDWI-like object.
-
-    Plus series goes first, indices are adjusted for minus to be globally correct.
-    head motion affines are combined with to-ref affines and stored in dwi_to_ref_affines.
-    """
-
-    input_spec = ConcatRPESplitsInputSpec
-    output_spec = ConcatRPESplitsOutputSpec
-
-    def _run_interface(self, runtime):
-
-        plus_images = self.inputs.dwi_plus
-        plus_bvecs = self.inputs.bvec_plus
-        plus_bvals = self.inputs.bval_plus
-        plus_b0_images = self.inputs.b0_images_plus
-        plus_b0_indices = self.inputs.b0_indices_plus
-        plus_orig_files = self.inputs.original_images_plus
-        num_plus = len(plus_images)
-
-        minus_images = self.inputs.dwi_minus
-        minus_bvecs = self.inputs.bvec_minus
-        minus_bvals = self.inputs.bval_minus
-        minus_b0_images = self.inputs.b0_images_minus
-        minus_b0_indices = self.inputs.b0_indices_minus
-        minus_orig_files = self.inputs.original_images_minus
-
-        self._results['dwi_files'] = plus_images + minus_images
-        self._results['bval_files'] = plus_bvals + minus_bvals
-        self._results['bvec_files'] = plus_bvecs + minus_bvecs
-        self._results['b0_images'] = plus_b0_images + minus_b0_images
-        self._results['b0_indices'] = plus_b0_indices + [
-            num_plus + idx for idx in minus_b0_indices]
-        self._results['original_files'] = _flatten(plus_orig_files) \
-            + _flatten(minus_orig_files)
-        self._results['validation_reports'] = self.inputs.validation_reports_plus \
-            + self.inputs.validation_reports_minus
-        self._results['sdc_method'] = "PEB/PEPOLAR Series (TOPUP)"
-        return runtime
-
-
 def _flatten(in_list):
     out_list = []
     for item in in_list:
         if isinstance(item, (list, tuple)):
             out_list.extend(item)
         else:
             out_list.append(item)
```

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/__init__.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep/interfaces/ants.py` & `qsiprep-0.9.0b1/qsiprep/interfaces/ants.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     modality_weights = traits.List([1], usedefault=True)
     n4_bias_correct = traits.Bool(True, usedefault=True, argstr='-n %d')
     metric = traits.Str('CC', usedefault=True, argstr='-m %s', mandatory=True)
     transform = traits.Enum('BSplineSyN', 'SyN', 'Affine', usedefault=True,
                             argstr='-t %s', mandatory=True)
     output_prefix = traits.Str('antsBTP')
     gradient_step = traits.Float(0.25, usedefault=True, mandatory=True, argstr='-g %.3f')
+    use_full_affine = traits.Bool(False, usedefault=True, argstr='-y %d')
     usefloat = traits.Bool(True, argstr='-e %d', usedefault=True)
 
 
 class MultivariateTemplateConstruction2OutputSpec(TraitedSpec):
     templates = OutputMultiObject(File(exists=True), mandatory=True)
     forward_transforms = OutputMultiObject(
         OutputMultiObject(File(exists=True)), mandatory=True)
```

### Comparing `qsiprep-0.8.0rc3/versioneer.py` & `qsiprep-0.9.0b1/versioneer.py`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/LICENSE` & `qsiprep-0.9.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `qsiprep-0.8.0rc3/qsiprep.egg-info/SOURCES.txt` & `qsiprep-0.9.0b1/qsiprep.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 qsiprep/workflows/__init__.py
 qsiprep/workflows/anatomical.py
 qsiprep/workflows/base.py
 qsiprep/workflows/dwi/__init__.py
 qsiprep/workflows/dwi/base.py
 qsiprep/workflows/dwi/confounds.py
 qsiprep/workflows/dwi/derivatives.py
+qsiprep/workflows/dwi/distortion_group_merge.py
 qsiprep/workflows/dwi/finalize.py
 qsiprep/workflows/dwi/fsl.py
 qsiprep/workflows/dwi/hmc.py
 qsiprep/workflows/dwi/hmc_sdc.py
 qsiprep/workflows/dwi/intramodal_template.py
 qsiprep/workflows/dwi/merge.py
 qsiprep/workflows/dwi/pre_hmc.py
@@ -122,14 +123,15 @@
 qsiprep/workflows/fieldmap/__init__.py
 qsiprep/workflows/fieldmap/base.py
 qsiprep/workflows/fieldmap/fmap.py
 qsiprep/workflows/fieldmap/pepolar.py
 qsiprep/workflows/fieldmap/phdiff.py
 qsiprep/workflows/fieldmap/syn.py
 qsiprep/workflows/fieldmap/unwarp.py
+qsiprep/workflows/fieldmap/utils.py
 qsiprep/workflows/recon/__init__.py
 qsiprep/workflows/recon/anatomical.py
 qsiprep/workflows/recon/base.py
 qsiprep/workflows/recon/build_workflow.py
 qsiprep/workflows/recon/converters.py
 qsiprep/workflows/recon/dipy.py
 qsiprep/workflows/recon/dsi_studio.py
```

### Comparing `qsiprep-0.8.0rc3/qsiprep.egg-info/PKG-INFO` & `qsiprep-0.9.0b1/qsiprep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsiprep
-Version: 0.8.0rc3
+Version: 0.9.0b1
 Summary: qsiprep builds workflows for preprocessing and reconstructing q-space images
 Home-page: https://github.com/pennbbl/qsiprep
 Author: The PennBBL developers
 Author-email: Matthew.Cieslak@pennmedicine.upenn.edu
 Maintainer: Matt Cieslak
 Maintainer-email: Matthew.Cieslak@pennmedicine.upenn.edu
 License: 3-clause BSD
```

