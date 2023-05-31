# Comparing `tmp/romancal-0.8.1.tar.gz` & `tmp/romancal-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romancal-0.8.1.tar", last modified: Tue Aug 23 19:07:22 2022, max compression
+gzip compressed data, was "romancal-0.9.0.tar", last modified: Mon Nov 14 18:47:05 2022, max compression
```

## Comparing `romancal-0.8.1.tar` & `romancal-0.9.0.tar`

### file list

```diff
@@ -1,243 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.134799 romancal-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-08-23 19:07:07.000000 romancal-0.8.1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-08-23 19:07:07.000000 romancal-0.8.1/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-08-23 19:07:07.000000 romancal-0.8.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-08-23 19:07:07.000000 romancal-0.8.1/.github/workflows/cancel_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-08-23 19:07:07.000000 romancal-0.8.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-08-23 19:07:07.000000 romancal-0.8.1/.github/workflows/label_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-23 19:07:07.000000 romancal-0.8.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7782 2022-08-23 19:07:07.000000 romancal-0.8.1/.github/workflows/roman_ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-08-23 19:07:07.000000 romancal-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-08-23 19:07:07.000000 romancal-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9401 2022-08-23 19:07:07.000000 romancal-0.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-23 19:07:07.000000 romancal-0.8.1/CODEOWNERS.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-08-23 19:07:07.000000 romancal-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-08-23 19:07:07.000000 romancal-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-08-23 19:07:07.000000 romancal-0.8.1/JenkinsfileRT
--rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-08-23 19:07:07.000000 romancal-0.8.1/JenkinsfileRT_dev
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-08-23 19:07:07.000000 romancal-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-08-23 19:07:07.000000 romancal-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-23 19:07:22.134799 romancal-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8547 2022-08-23 19:07:07.000000 romancal-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     5806 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   201304 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/_static/JWSTlogocrop.png
--rw-r--r--   0 runner    (1001) docker     (121)    59966 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/_static/stsci_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    14492 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/docs/exts/
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/exts/numfig.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/docs/roman/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/docs/roman/assign_wcs/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/assign_wcs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/assign_wcs/main.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/docs/roman/dark_current/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dark_current/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dark_current/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dark_current/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dark_current/reference_files.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.118799 romancal-0.8.1/docs/roman/datamodels/
--rw-r--r--   0 runner    (1001) docker     (121)    10608 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/datamodels/datamodels_asdf.rst
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/datamodels/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/datamodels/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5228 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/datamodels/models.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/dq_init/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dq_init/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dq_init/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dq_init/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/dq_init/reference_files.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/error_propagation/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/error_propagation/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/error_propagation/main.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/flatfield/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/flatfield/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/flatfield/main.rst
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/flatfield/reference_files.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/includes/
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/includes/standard_keywords.inc
--rw-r--r--   0 runner    (1001) docker     (121)     8967 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/jump/
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/jump/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/jump/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/jump/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/jump/reference_files.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/linearity/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/linearity/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/linearity/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/linearity/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/linearity/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/package_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/photom/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/photom/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/photom/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/photom/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/photom/reference_files.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)     3714 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/pipeline/exposure_pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/pipeline/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/pipeline/main.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.122799 romancal-0.8.1/docs/roman/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/ramp_fitting/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11545 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/ramp_fitting/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/ramp_fitting/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/ramp_fitting/reference_files.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/docs/roman/references_general/
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/dark_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/dark_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/dark_specific.inc
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/distortion_reffile.rst
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/distortion_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/flat_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/flat_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/gain_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/gain_reffile.rst
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/gain_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/gain_selection.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/linearity_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/linearity_reffile.rst
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/linearity_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/linearity_selection.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/mask_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/mask_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/photom_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/photom_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/readnoise_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/readnoise_reffile.rst
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/readnoise_selection.inc
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/readnoise_selection.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12478 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/references_general.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/saturation_reffile.inc
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/references_general/saturation_selection.inc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/docs/roman/refpix/
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/refpix/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/refpix/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/docs/roman/saturation/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/saturation/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/saturation/description.rst
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/saturation/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-23 19:07:07.000000 romancal-0.8.1/docs/roman/saturation/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-23 19:07:07.000000 romancal-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-23 19:07:07.000000 romancal-0.8.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-08-23 19:07:07.000000 romancal-0.8.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-08-23 19:07:07.000000 romancal-0.8.1/requirements-sdp.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/assign_wcs/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/assign_wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5526 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/assign_wcs/assign_wcs_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/assign_wcs/pointing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/assign_wcs/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/assign_wcs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/assign_wcs/tests/test_wcs.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/assign_wcs/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/dark_current/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dark_current/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4719 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dark_current/dark_current_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/dark_current/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dark_current/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4318 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dark_current/tests/test_dark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/dq_init/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dq_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dq_init/dq_init_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dq_init/dq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/dq_init/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     9774 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/dq_init/tests/test_dq_init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal/flatfield/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/flatfield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4473 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/flatfield/flat_field.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1520 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/flatfield/flat_field_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/flatfield/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/flatfield/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/flatfield/tests/test_flatfield.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/jump/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/jump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5332 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/jump/jump_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/jump/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/jump/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9819 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/jump/tests/test_jump_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3194 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/lib/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/tests/test_basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/lib/tests/test_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/linearity/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/linearity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/linearity/linearity_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/photom/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/photom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/photom/photom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/photom/photom_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/photom/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/photom/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10415 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/photom/tests/test_photom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/pipeline/exposure_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/ramp_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/ramp_fitting/ramp_fit_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/ramp_fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/ramp_fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8033 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/ramp_fitting/tests/test_ramp_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/regtest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11707 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    15168 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/regtestdata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/sdp_pools_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3233 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_dark_current.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_jump_det.py
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_linearity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_wfi_dq_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     6640 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_wfi_flat_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     5907 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_wfi_photom.py
--rw-r--r--   0 runner    (1001) docker     (121)    18681 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_wfi_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/regtest/test_wfi_saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/saturation/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/saturation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/saturation/saturation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1629 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/saturation/saturation_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.130799 romancal-0.8.1/romancal/saturation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/saturation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8846 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/saturation/tests/test_saturation.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.134799 romancal-0.8.1/romancal/stpipe/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/stpipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/stpipe/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/stpipe/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.134799 romancal-0.8.1/romancal/stpipe/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/stpipe/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3071 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/stpipe/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/stpipe/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/stpipe/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.134799 romancal-0.8.1/romancal/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5715 2022-08-23 19:07:07.000000 romancal-0.8.1/romancal/tests/base_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.126799 romancal-0.8.1/romancal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-23 19:07:22.000000 romancal-0.8.1/romancal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6457 2022-08-23 19:07:22.000000 romancal-0.8.1/romancal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-23 19:07:22.000000 romancal-0.8.1/romancal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-23 19:07:22.000000 romancal-0.8.1/romancal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-23 19:07:22.000000 romancal-0.8.1/romancal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-08-23 19:07:22.000000 romancal-0.8.1/romancal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-23 19:07:22.000000 romancal-0.8.1/romancal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 19:07:22.134799 romancal-0.8.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5024 2022-08-23 19:07:07.000000 romancal-0.8.1/scripts/okify_regtests
--rwxr-xr-x   0 runner    (1001) docker     (121)     1671 2022-08-23 19:07:07.000000 romancal-0.8.1/scripts/schema_editor
--rwxr-xr-x   0 runner    (1001) docker     (121)     3021 2022-08-23 19:07:07.000000 romancal-0.8.1/scripts/schemadoc
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-08-23 19:07:07.000000 romancal-0.8.1/scripts/verify_install_requires
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-08-23 19:07:22.134799 romancal-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-08-23 19:07:07.000000 romancal-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-11-14 18:46:53.000000 romancal-0.9.0/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-11-14 18:46:53.000000 romancal-0.9.0/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-11-14 18:46:53.000000 romancal-0.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-11-14 18:46:53.000000 romancal-0.9.0/.github/workflows/cancel_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-11-14 18:46:53.000000 romancal-0.9.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-11-14 18:46:53.000000 romancal-0.9.0/.github/workflows/label_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-14 18:46:53.000000 romancal-0.9.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     7865 2022-11-14 18:46:53.000000 romancal-0.9.0/.github/workflows/roman_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-14 18:46:53.000000 romancal-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-11-14 18:46:53.000000 romancal-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9904 2022-11-14 18:46:53.000000 romancal-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-11-14 18:46:53.000000 romancal-0.9.0/CODEOWNERS.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-11-14 18:46:53.000000 romancal-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-14 18:46:53.000000 romancal-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-11-14 18:46:53.000000 romancal-0.9.0/JenkinsfileRT
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-11-14 18:46:53.000000 romancal-0.9.0/JenkinsfileRT_dev
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2022-11-14 18:46:53.000000 romancal-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-11-14 18:46:53.000000 romancal-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-14 18:47:05.797317 romancal-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-11-14 18:46:53.000000 romancal-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/0.5.0
+-rw-r--r--   0 runner    (1001) docker     (121)     5806 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)    15406 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    47381 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/_static/roman_logo_black_w200px.png
+-rw-r--r--   0 runner    (1001) docker     (121)    18255 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/_static/roman_logo_white_w100px.png
+-rw-r--r--   0 runner    (1001) docker     (121)    59966 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/_static/stsci_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    14710 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/docs/exts/
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/exts/numfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/docs/roman/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/docs/roman/assign_wcs/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/assign_wcs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/assign_wcs/main.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/docs/roman/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dark_current/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dark_current/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dark_current/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dark_current/reference_files.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.781317 romancal-0.9.0/docs/roman/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (121)    10999 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/datamodels/datamodels_asdf.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/datamodels/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/datamodels/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5315 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/datamodels/models.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/dq_init/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dq_init/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dq_init/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dq_init/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/dq_init/reference_files.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/error_propagation/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/error_propagation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/error_propagation/main.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/flatfield/
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/flatfield/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2308 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/flatfield/main.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/flatfield/reference_files.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/includes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/includes/standard_keywords.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/jump/
+-rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/jump/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/jump/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/jump/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/jump/reference_files.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/linearity/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/linearity/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/linearity/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/linearity/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/linearity/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/package_index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/photom/
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/photom/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/photom/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/photom/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/photom/reference_files.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)     3714 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline/exposure_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline/main.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4256 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline_naming_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline_parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline_ref_files.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline_run.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/pipeline_steps.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.785317 romancal-0.9.0/docs/roman/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/ramp_fitting/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11545 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/ramp_fitting/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/ramp_fitting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/ramp_fitting/reference_files.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.789317 romancal-0.9.0/docs/roman/references_general/
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/dark_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/dark_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/dark_specific.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/distortion_reffile.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/distortion_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/flat_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/flat_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/gain_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/gain_reffile.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/gain_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/gain_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/linearity_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/linearity_reffile.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/linearity_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/linearity_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/mask_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/mask_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/photom_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/photom_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/readnoise_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/readnoise_reffile.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/readnoise_selection.inc
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/readnoise_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12478 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/references_general.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/saturation_reffile.inc
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/references_general/saturation_selection.inc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.789317 romancal-0.9.0/docs/roman/refpix/
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/refpix/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/refpix/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.789317 romancal-0.9.0/docs/roman/saturation/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/saturation/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/saturation/description.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/saturation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/saturation/reference_files.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.789317 romancal-0.9.0/docs/roman/stpipe/
+-rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/call_via_call.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/call_via_run.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11037 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/config_asdf.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/devel_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/devel_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9339 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/devel_step.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/parameter_files.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/user_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7112 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/user_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9801 2022-11-14 18:46:53.000000 romancal-0.9.0/docs/roman/stpipe/user_step.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-14 18:46:53.000000 romancal-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-14 18:46:53.000000 romancal-0.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-11-14 18:46:53.000000 romancal-0.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-11-14 18:46:53.000000 romancal-0.9.0/requirements-sdp.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.789317 romancal-0.9.0/romancal/
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.789317 romancal-0.9.0/romancal/assign_wcs/
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/assign_wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5526 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/assign_wcs/assign_wcs_step.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/assign_wcs/pointing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/assign_wcs/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/assign_wcs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/assign_wcs/tests/test_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/assign_wcs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dark_current/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4719 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dark_current/dark_current_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/dark_current/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dark_current/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4318 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dark_current/tests/test_dark.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/dq_init/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dq_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dq_init/dq_init_step.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dq_init/dq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/dq_init/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     9774 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/dq_init/tests/test_dq_init.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/flatfield/
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/flatfield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4473 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/flatfield/flat_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1520 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/flatfield/flat_field_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/flatfield/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/flatfield/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4197 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/flatfield/tests/test_flatfield.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/jump/
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/jump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6606 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/jump/jump_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/jump/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/jump/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9819 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/jump/tests/test_jump_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3194 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5283 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/tests/test_basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/lib/tests/test_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/linearity/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/linearity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/linearity/linearity_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/photom/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/photom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/photom/photom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/photom/photom_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/photom/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/photom/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10236 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/photom/tests/test_photom.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5765 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/pipeline/exposure_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/ramp_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7011 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/ramp_fitting/ramp_fit_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.793317 romancal-0.9.0/romancal/ramp_fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/ramp_fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8033 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/ramp_fitting/tests/test_ramp_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/romancal/regtest/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11707 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15168 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/regtestdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/sdp_pools_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3233 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_jump_det.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4415 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_wfi_dq_init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6640 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_wfi_flat_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5907 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_wfi_photom.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18681 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_wfi_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/regtest/test_wfi_saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/romancal/saturation/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/saturation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/saturation/saturation.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1629 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/saturation/saturation_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/romancal/saturation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/saturation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8846 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/saturation/tests/test_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/romancal/stpipe/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/stpipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/stpipe/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/stpipe/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/romancal/stpipe/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/stpipe/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3071 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/stpipe/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/stpipe/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/stpipe/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/romancal/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5715 2022-11-14 18:46:53.000000 romancal-0.9.0/romancal/tests/base_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.789317 romancal-0.9.0/romancal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-14 18:47:05.000000 romancal-0.9.0/romancal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-11-14 18:47:05.000000 romancal-0.9.0/romancal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 18:47:05.000000 romancal-0.9.0/romancal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-14 18:47:05.000000 romancal-0.9.0/romancal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 18:47:05.000000 romancal-0.9.0/romancal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-11-14 18:47:05.000000 romancal-0.9.0/romancal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-14 18:47:05.000000 romancal-0.9.0/romancal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:47:05.797317 romancal-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5024 2022-11-14 18:46:53.000000 romancal-0.9.0/scripts/okify_regtests
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1671 2022-11-14 18:46:53.000000 romancal-0.9.0/scripts/schema_editor
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3021 2022-11-14 18:46:53.000000 romancal-0.9.0/scripts/schemadoc
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-11-14 18:46:53.000000 romancal-0.9.0/scripts/verify_install_requires
+-rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-11-14 18:47:05.797317 romancal-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-11-14 18:46:53.000000 romancal-0.9.0/setup.py
```

### Comparing `romancal-0.8.1/.github/labeler.yml` & `romancal-0.9.0/.github/labeler.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 documentation:
   - 'docs/**/*'
   - any: [ '*.rst', '!CHANGES.rst' ]
   - '*.md'
-  - '.readthedocs.yml'
+  - '.readthedocs.yaml'
   - 'LICENSE'
 
 dependencies:
   - 'pyproject.toml'
   - 'setup.*'
   - 'requirements-*.txt'
   - 'MANIFEST.in'
```

### Comparing `romancal-0.8.1/.github/pull_request_template.md` & `romancal-0.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/.github/workflows/cancel_workflows.yml` & `romancal-0.9.0/.github/workflows/cancel_workflows.yml`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/.github/workflows/roman_ci.yml` & `romancal-0.9.0/.github/workflows/roman_ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -73,16 +73,16 @@
   test:
     name: test
     needs: [ style, audit, dependencies ]
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ ubuntu-latest, macos-latest ]
-        python: [ 3.8, 3.9, '3.10' ]
+        os: [ 'ubuntu-latest', 'macos-latest' ]
+        python: [ '3.8', '3.9', '3.10', '3.11' ]
     steps:
       - uses: actions/checkout@v3.0.2
       - uses: actions/setup-python@v4.1.0
         id: python
         with:
           python-version: ${{ matrix.python }}
       - uses: actions/cache@v3.0.5
@@ -95,16 +95,16 @@
   test_alldeps:
     name: test optional dependencies
     needs: [ test ]
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ ubuntu-latest, macos-latest ]
-        python: [ 3.8, 3.9, '3.10' ]
+        os: [ 'ubuntu-latest', 'macos-latest' ]
+        python: [ '3.8', '3.9', '3.10', '3.11' ]
     steps:
       - uses: actions/checkout@v3.0.2
       - uses: actions/setup-python@v4.1.0
         id: python
         with:
           python-version: ${{ matrix.python }}
       - uses: actions/cache@v3.0.5
@@ -117,16 +117,16 @@
   test_devdeps:
     name: test developer versions
     needs: [ test ]
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ ubuntu-latest, macos-latest ]
-        python: [ 3.8, 3.9, '3.10' ]
+        os: [ 'ubuntu-latest', 'macos-latest' ]
+        python: [ '3.8', '3.9', '3.10', '3.11' ]
     steps:
       - uses: actions/checkout@v3.0.2
       - uses: actions/setup-python@v4.1.0
         id: python
         with:
           python-version: ${{ matrix.python }}
       - uses: actions/cache@v3.0.5
@@ -140,19 +140,19 @@
   test_pyargs:
     name: test --pyargs
     needs: [ test ]
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ ubuntu-latest, macos-latest ]
-        python: [ 3.8, 3.9, '3.10' ]
+        os: [ 'ubuntu-latest', 'macos-latest' ]
+        python: [ '3.8', '3.9', '3.10', '3.11' ]
         exclude:
           - os: macos-latest
-            python: '3.10'
+            python: '3.11'
     steps:
       - uses: actions/checkout@v3.0.2
       - uses: actions/setup-python@v4.1.0
         id: python
         with:
           python-version: ${{ matrix.python }}
       - uses: actions/cache@v3.0.5
@@ -167,23 +167,25 @@
     needs: [ test ]
     runs-on: ${{ matrix.os }}
     continue-on-error: true
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest ]
-        python: [ 3.8, 3.9, '3.10' ]
-        numpy: [ '1.18.*', '1.19.*', '1.20.*', '1.21.*', '1.22.*' ]
+        python: [ '3.8', '3.9', '3.10', '3.11' ]
+        numpy: [ '1.20.*', '1.21.*', '1.22.*' ]
         exclude:
           - python: '3.10'
-            numpy: '1.18.*'
-          - python: '3.10'
-            numpy: '1.19.*'
-          - python: '3.10'
             numpy: '1.20.*'
+          - python: '3.11'
+            numpy: '1.20.*'
+          - python: '3.11'
+            numpy: '1.21.*'
+          - python: '3.11'
+            numpy: '1.22.*'
     steps:
       - uses: actions/checkout@v3.0.2
       - uses: actions/setup-python@v4.1.0
         id: python
         with:
           python-version: ${{ matrix.python }}
       - uses: actions/cache@v3.0.5
@@ -206,17 +208,16 @@
           python-version: 3.9
       - uses: actions/cache@v3.0.5
         with:
           path: ${{ env.pythonLocation }}
           key: test-coverage-${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('**/pyproject.toml', '**/setup.*') }}
       - run: pip install ".[test]" pytest-xdist pytest-cov
       - run: pip freeze
-      - run: pytest -n auto --pyargs romancal --cov-report xml --cov
-      - run: coverage report -m
-      - uses: codecov/codecov-action@master
+      - run: pytest -n auto --cov --cov-report xml --cov-report term-missing
+      - uses: codecov/codecov-action@v3
         with:
           file: ./coverage.xml
           flags: unit
           fail_ci_if_error: true
   build_docs:
     name: build HTML docs
     needs: [ test, test_alldeps, test_devdeps, test_pyargs, test_older_numpy ]
```

### Comparing `romancal-0.8.1/.gitignore` & `romancal-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/CHANGES.rst` & `romancal-0.9.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+0.9.0 (2022-11-14)
+==================
+
+- Additional changes to Roman's RTD page content [#600]
+
+- New Roman's RTD page layout [#596]
+
+- pin ``numpy`` to ``>=1.20`` [#592]
+
+jump
+----
+
+- Changes for new keywords (currently unused by Roman) to control snowball and shower flagging in jump detection. [#593]
+
+photom
+------
+
+- Updates so that the default suffix is used for spectroscopic data. [#594]
+
+- Change photom step to forcibly set the photometric keywords to ``None`` for spectroscopic data. [#591]
+
+
+
 0.8.1 (2022-08-23)
 ==================
 
 - pin ``asdf`` above ``2.12.1`` to fix issue with `jsonschema` release [#562]
 - pin `roman_datamodels` to newest feature version [#563]
 
 0.8.0 (2022-08-12)
@@ -17,15 +40,15 @@
 
 - include information about the distortion reference file used in the ``assign_wcs`` step [#542]
 
 flat
 ----
 
 - Removed try/except condition on Flat Reference file CRDS lookup. [#528]
-  
+
 general
 -------
 
 - Update pipeline steps to define the default suffix when saving the step results [#521]
 
 - Simplified reference file name and model storage in dq and flat steps. [#514]
```

### Comparing `romancal-0.8.1/CODE_OF_CONDUCT.md` & `romancal-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/CONTRIBUTING.md` & `romancal-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/JenkinsfileRT` & `romancal-0.9.0/JenkinsfileRT`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/JenkinsfileRT_dev` & `romancal-0.9.0/JenkinsfileRT_dev`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/LICENSE` & `romancal-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/PKG-INFO` & `romancal-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romancal
-Version: 0.8.1
+Version: 0.9.0
 Summary: Library for calibration of science observations from the Nancy Grace Roman Space Telescope
 Home-page: https://github.com/spacetelescope/romancal
 Author: Roman calibration pipeline developers
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/spacetelescope/romancal/issues
 Project-URL: Documentation, https://roman-pipeline.readthedocs.io/en/stable/
 Project-URL: Source Code, https://github.com/spacetelescope/romancal
```

### Comparing `romancal-0.8.1/README.md` & `romancal-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 | 0.4.2     | 0.3       | 011          | Sep  2021 | Release for Build 0.3                 |
 | 0.5.0     | 0.4       | 023          | Dec  2021 | Release for Build 0.4                 |
 | 0.6.0     | 0.5       | 030          | Mar  2022 | Release for Build 0.5                 |
 | 0.7.0     | 22Q3_B6   | 032          | May  2022 | Release for Build 22Q3_B6 (Build 0.6) |
 | 0.7.1     | 22Q3_B6   | 032          | May  2022 | Release for Build 22Q3_B6 (Build 0.6) |
 | 0.8.0     | 22Q4_B7   | 038          | Aug  2022 | Release for Build 22Q4_B7 (Build 0.7) |
 | 0.8.1     | 22Q4_B7   | 038          | Aug  2022 | Release for Build 22Q4_B7 (Build 0.7) |
+| 0.9.0     | 23Q1_B8   | 039          | Nov  2022 | Release for Build 23Q1_B8 (Build 8)   |
 
 Note: CRDS_CONTEXT values flagged with an asterisk in the above table are estimates
 (formal CONTEXT deliveries are only provided with final builds).
 
 ## Unit Tests
 
 ### Setup
```

### Comparing `romancal-0.8.1/docs/Makefile` & `romancal-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/_static/stsci_logo.png` & `romancal-0.9.0/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/conf.py` & `romancal-0.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     'sphinx.ext.autosummary',
     'sphinx.ext.napoleon',
     'sphinx_automodapi.automodapi',
     'sphinx_automodapi.automodsumm',
     'sphinx_automodapi.autodoc_enhancements',
     'sphinx_automodapi.smart_resolver',
     'sphinx_asdf',
+    'myst_parser',
     ]
 
 
 if on_rtd:
     extensions.append('sphinx.ext.mathjax')
 
 elif LooseVersion(sphinx.__version__) < LooseVersion('1.4'):
@@ -106,15 +107,18 @@
     extensions.append('sphinx.ext.imgmath')
 
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = {
+    '.rst': 'restructuredtext',
+    '.md': 'markdown',
+}
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
@@ -220,21 +224,24 @@
      'http://asdf-standard.readthedocs.io/en/latest/generated/stsci.edu/asdf/'),
 ]
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'stsci_rtd_theme'
+html_theme = 'sphinx_rtd_theme'
+html_logo = "_static/roman_logo_white_w100px.png"
+html_favicon = '_static/favicon.ico'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
-    "collapse_navigation": True
+    "collapse_navigation": True,
+    "display_version": True
     }
 #        "nosidebar": "false",
 #        "sidebarbgcolor": "#4db8ff",
 #        "sidebartextcolor": "black",
 #        "sidebarlinkcolor": "black",
 #        "headbgcolor": "white",
 #        }
@@ -256,15 +263,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-
+html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 # html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
```

### Comparing `romancal-0.8.1/docs/exts/numfig.py` & `romancal-0.9.0/docs/exts/numfig.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/make.bat` & `romancal-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/assign_wcs/main.rst` & `romancal-0.9.0/docs/roman/assign_wcs/main.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 
 Description
 ===========
 
 ``romancal.assign_wcs`` is the first step run on an image, after ``romancal.ramp_fitting``.
-It associates a World Coodrinate System (WCS) object with each science exposure. The WCS
-object transforms positions in the ``detector`` frame to positions in the ``world``
-coordinate frame - ICRS. The WCS can be accessed as an attribute of the ``meta`` object
+It associates a World Coordinate System (WCS) object with each science exposure. 
+Note that no fitting is performed in this step; it only creates a WCS object that 
+transforms positions in the ``detector`` frame to positions in the ``world``
+coordinate frame (ICRS) based on the telescope pointing and reference files provided by CRDS. 
+The constructed WCS object can be accessed as an attribute of the ``meta`` object
 when the file is opened as a data model. The forward direction of the transforms is
 from detector to world coordinates and the input positions are 0-based.
 
 ``romancal.assign_wcs`` uses `GWCS <https://github.com/spacetelescope/gwcs>`__ -
 a package for managing the World Coordinate System of astronomical data.
 It expects to find the basic WCS keywords in the
 ``model.meta.wcsinfo`` structure. Distortions are stored in reference files in the
 `ASDF <http://asdf-standard.readthedocs.org/en/latest/>`__  format.
 
 ``assign_wcs`` retrieves reference files from CRDS and creates a pipeline of transforms from
-input frame ``detector`` to a frame ``v2v3``. This part of the WCS pipeline may include
+input frame ``detector`` to the telescope frame ``v2v3`` [1]_. This part of the WCS pipeline may include
 intermediate coordinate frames. The basic WCS keywords are used to create
 the transform from frame ``v2v3`` to frame ``world``.
 
 Note: in earlier builds of the pipeline the distortions are not available.
 
 Basic WCS keywords and the transform from ``v2v3`` to ``world``
 ---------------------------------------------------------------
@@ -63,7 +65,13 @@
   >>> v2world = image.meta.wcs.get_transform('v2v3', 'world')
   >>> ra, dec = v2world(v2, v3)
   >>> x1, y1 = image.meta.wcs.invert(ra, dec)
 
 There are methods which allow the result of evaluating the WCS object
 to be an ``astropy.SkyCoord`` objext (as opposed to numbers) which allows
 further transformation of coordinates to different coordinate frames.
+
+.. rubric:: Footnotes
+
+.. [1] V2V3 is a frame defined by the two perpendicular axes that lay along the primary's mirror plane.
+        For completeness, V1 is also part of the telescope frame system, being the axis perpendicular 
+        to the primary mirror (i.e. along the telecope's optical axis).
```

### Comparing `romancal-0.8.1/docs/roman/dark_current/description.rst` & `romancal-0.9.0/docs/roman/dark_current/description.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 Algorithm
 ---------
 
 The dark current step removes dark current from a Roman exposure by subtracting
 dark current data stored in a dark reference file.
 
 The current implementation uses dark reference files that are matched to the
-MA table entry in the exposure metadata. The dark data are then subtracted,
+MA table entry in the exposure metadata. Note that the data reference file 
+for a science group (SCI) is named `data`. The dark data are then subtracted,
 group-by-group, from the science exposure groups, in which
 each SCI group of the dark data is subtracted from the corresponding SCI
 group of the science data.
 
 The ERR arrays of the science data are not modified.
 
 The DQ flags from the dark reference file are propagated into science
```

### Comparing `romancal-0.8.1/docs/roman/datamodels/datamodels_asdf.rst` & `romancal-0.9.0/docs/roman/datamodels/datamodels_asdf.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 .. _datamodels_asdf:
 
 
 Working with Roman datamodels and ASDF files
 ============================================
 
-If you've installed the roman calibration pipeline you should also have access
-to the standalone tool asdfinfo which allows access to asdf (and roman) files
+Please refer to `Roman Documentation <https://roman-datamodels.readthedocs.io/en/latest/>`_ 
+for more details about `roman_datamodels`.
+
+This section assumes that you are familiar with the ASDF standard format. 
+If that's not the case, a good starting point would be to go over the `ASDF Documentation <https://asdf-standard.readthedocs.io/>`_.
+
+If you have installed the roman calibration pipeline you should also have access
+to the standalone tool asdfinfo which allows access to `ASDF <https://asdf-standard.readthedocs.io/>`_ (and roman) files
 from the terminal prompt,::
 
     asdftool info r0000101001001001001_01101_0001_WFI16_cal.asdf
     root (AsdfObject)
     ├─asdf_library (Software)
     │ ├─author (str): The ASDF Developers
     ...
```

### Comparing `romancal-0.8.1/docs/roman/datamodels/metadata.rst` & `romancal-0.9.0/docs/roman/datamodels/metadata.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/datamodels/models.rst` & `romancal-0.9.0/docs/roman/datamodels/models.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .. _datamodels:
 
 About datamodels
 ================
 
 The purpose of the data model is to abstract away the peculiarities of
 the underlying file format.  The same data model may be used for data
-created from scratch in memory, or loaded from ASDF files or some future file
-format.
+created from scratch in memory, or loaded from 
+`ASDF <https://asdf-standard.readthedocs.io/>`_ files or some future file format.
 
 The detailed datamodel structure and specifics are contained in the
-documentation included with the roman_datamodels package found here (TBD).
+documentation included with the `roman_datamodels` package found `here <https://roman-datamodels.readthedocs.io/en/latest/>`_.
 
 Each model instance is created to contain a variety of attributes and data that
 are needed for analysis or to propagate information about the file and the
 contents of the file. For example, the `ImageModel` class has the following
 arrays associated with it:
 
     - `data`: The science data
@@ -98,22 +98,24 @@
 
 This will raise an exception if the file contains data of the wrong
 type.
 
 Saving a data model to a file
 -----------------------------
 
-Simply call the `save` method on the model instance.  The format to
-save into will be deduced from the filename.::
+Simply call the `save` method on the model instance:
+::
 
     im.save("myimage.asdf")
 
 .. note::
 
    This `save` always clobbers the output file.
+   
+   For now the only format supported is ASDF.
 
 
 Copying a model
 ---------------
 
 To create a new model based on another model, simply use its `copy`
 method.  This will perform a deep-copy: that is, no changes to the
```

### Comparing `romancal-0.8.1/docs/roman/dq_init/description.rst` & `romancal-0.9.0/docs/roman/dq_init/description.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/error_propagation/main.rst` & `romancal-0.9.0/docs/roman/error_propagation/main.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/flatfield/main.rst` & `romancal-0.9.0/docs/roman/flatfield/main.rst`

 * *Files 11% similar despite different names*

```diff
@@ -28,24 +28,34 @@
 Error Propagation
 -----------------
 The VAR_POISSON and VAR_RNOISE variance arrays of the science exposure
 are divided by the square of the flat-field value for each pixel.
 A flat-field variance array, VAR_FLAT, is created from the science exposure
 and flat-field reference file data using the following formula:
 
+ The flat-field is applied to the science data, in-place, according to:
+
 .. math::
-   SCI_{science} = SCI_{science} / SCI_{flat}
+   SCI^{\prime}_{science} = SCI_{science} / SCI_{flat}
+
+The flat-field data is also applied to the VAR_POISSON and VAR_RNOISE
+variance arrays,
 
 .. math::
    VAR\_POISSON_{science} = VAR\_POISSON_{science} / SCI_{flat}^2
 
 .. math::
    VAR\_RNOISE_{science} = VAR\_RNOISE_{science} / SCI_{flat}^2
 
+The variance for the flat-fielded data associated with the science
+data is determined using,
+
 .. math::
-   VAR\_FLAT_{science} = ( SCI_{science}^{2} / SCI_{flat}^{2} ) * ERR_{flat}^{2}
+   VAR\_FLAT_{science} = ( (SCI^{\prime}_{science})^{2} / SCI_{flat}^{2} ) * ERR_{flat}^{2}
+
+and finally the error that is associated with the science data is given by,
 
 .. math::
    ERR_{science} = \sqrt{VAR\_POISSON + VAR\_RNOISE + VAR\_FLAT}
 
 The total ERR array in the science exposure is updated as the square root
 of the quadratic sum of VAR_POISSON, VAR_RNOISE, and VAR_FLAT.
```

### Comparing `romancal-0.8.1/docs/roman/includes/standard_keywords.inc` & `romancal-0.9.0/docs/roman/includes/standard_keywords.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/introduction.rst` & `romancal-0.9.0/docs/roman/stpipe/devel_step.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,237 +1,285 @@
-Introduction
-============
+=====
+Steps
+=====
 
-This document provides instructions on running the Roman Science Calibration
-Pipeline (referred to as "the pipeline") and individual pipeline steps.
+.. _writing-a-step:
 
+Writing a step
+==============
 
-Reference Files
-===============
-
-Many pipeline steps rely on the use of reference files that contain different types of
-calibration data or information necessary for processing the data. The reference files are
-instrument-specific and are periodically updated as the data processing evolves and the
-understanding of the instruments improves. They are created, tested, and validated by the
-Roman Instrument Teams. They ensure all the files are in the correct format and have all
-required attributes. The files are then delivered to the Reference Data for Calibration
-and Tools (ReDCaT) Management Team. The result of this process is the files being ingested
-into the Roman Calibration Reference Data System (CRDS), and made available to the pipeline
-team and any other ground subsystem that needs access to them.
-
-Information about all the reference files used by the Calibration Pipeline can be found at
-:ref:`reference_file_information`,
-as well as in the documentation for each Calibration Step that uses a reference file.
-
-CRDS
-====
-
-CRDS reference file mappings are usually set by default to always give access
-to the most recent reference file deliveries and selection rules. On
-occasion it might be necessary or desirable to use one of the non-default
-mappings in order to, for example, run different versions of the pipeline
-software or use older versions of the reference files. This can be
-accomplished by setting the environment variable ``CRDS_CONTEXT`` to the
-desired project mapping version, e.g.
-::
+Writing a new step involves writing a class that has a `process`
+method to perform work and a `spec` member to define its configuration
+parameters.  (Optionally, the `spec` member may be defined in a
+separate `spec` file).
 
-$ export CRDS_CONTEXT='roman_0017.pmap'
+Inputs and outputs
+------------------
 
-Within STScI, the current storage location for all Roman CRDS reference files is:
-::
+A `Step` provides a full framework for handling I/O.
 
-/grp/crds/roman/references/roman/
+Steps get their inputs from two sources:
 
-Running From the Command Line
-=============================
+    - Configuration parameters come from the parameter file or the
+      command line and are set as member variables on the Step object
+      by the stpipe framework.
 
-Individual steps and pipelines (consisting of a series of steps) can be run
-from the command line using the ``strun`` command:
-::
+    - Arguments are passed to the Step’s `process` function as regular
+      function arguments.
 
-    $ strun <pipeline_name, class_name, or input_file>
+Parameters should be used to specify things that must be determined outside of
+the code by a user using the class. Arguments should be used to pass data that
+needs to go from one step to another as part of a larger pipeline. Another way
+to think about this is: if the user would want to examine or change the value,
+use a parameter.
 
-The first argument to ``strun`` must be one of either a pipeline name, python
-class of the step or pipeline to be run. The second argument to
-``strun`` is the name of the input data file to be processed.
-
-For example, the Stage 1 pipeline is implemented by the class
-:ref:`romancal.pipeline.ExposurePipeline <exposure_pipeline>`. The command to
-run this pipeline is:
-::
+The parameters are defined by the :ref:`Step.spec <the-spec-member>` member.
+
+Input Files, Associations, and Directories
+``````````````````````````````````````````
+
+It is presumed that all input files are co-resident in the same
+directory. This directory is whichever directory the first input file
+is found in. This is particularly important for associations. It is
+assumed that all files referenced by an association are in the same
+directory as the association file itself.
+
+Output Files and Directories
+````````````````````````````
+
+The step will generally return its output as a data model. Every step has
+implicitly created parameters `output_dir` and `output_file` which the user can
+use to specify the directory and file to save this model to. Since the `stpipe`
+architecture generally creates output file names, in general, it is expected
+that `output_file` be rarely specified, and that different sets of outputs be
+separated using `output_dir`.
+
+Output Suffix
+-------------
+
+There are three ways a step's results can be written to a file:
+
+1. Implicitly when a step is run from the command line or with
+   `Step.from_cmdline`
+
+2. Explicitly by specifying the parameter `save_results`
 
-  $ strun romancal.pipeline.ExposurePipeline r0008308002010007027_06311_0019_WFI01_uncal.asdf
+3. Explicitly by specifying a file name with the parameter
+   `output_file`
 
+In all cases, the file, or files, is/are created with an added suffix
+at the end of the base file name. By default this suffix is the class
+name of the step that produced the results. Use the `suffix` parameter
+to explicitly change the suffix.
+
+
+The Python class
+----------------
+
+At a minimum, the Python Step class should inherit from `stpipe.Step`, implement
+a ``process`` method to do the actual work of the step and have a `spec` member
+to describe its parameters.
+
+1. Objects from other Steps in a pipeline are passed as arguments to
+   the ``process`` method.
+
+2. The parameters described in :ref:`configuring-a-step`
+   are available as member variables on ``self``.
+
+3. To support the caching suspend/resume feature of pipelines, images
+   must be passed between steps as model objects.  To ensure you’re
+   always getting a model object, call the model constructor on the
+   parameter passed in.  It is good idea to use a `with` statement
+   here to ensure that if the input is a file path that the file will
+   be appropriately closed.
+
+4. Objects to pass to other Steps in the pipeline are simply returned
+   from the function.  To return multiple objects, return a tuple.
+
+5. The parameters for the step are described in the `spec` member in the
+   `configspec` format.
+
+6. Declare any CRDS reference files used by the Step.  (See
+   :ref:`interfacing-with-crds`).
 
-Pipeline classes also have a **pipeline name**, or **alias**, that can be used
-instead of thefull class specification. For example,
-``calroman.pipeline.ExposurePipeline`` has the alias ``roman_elp`` and
-can be run as
 ::
 
- $ strun roman_elp r0008308002010007027_06311_0019_WFI01_uncal.asdf
+    from romancal.stpipe import RomanStep
 
-Exit Status
------------
- ``strun`` produces the following exit status codes:
+    from roman_datamodels.datamodels import ImageModel
+    from my_awesome_astronomy_library import combine
 
- - 0: Successful completion of the step/pipeline
- - 1: General error occurred
- - 64: No science data found
+    class ExampleStep(RomanStep):
+        """
+        Every step should include a docstring.  This docstring will be
+        displayed by the `strun --help`.
+        """
 
- .. _intro_file_conventions:
+        # 1.
+        def process(self, image1, image2):
+            self.log.info("Inside ExampleStep")
 
-Input and Output File Conventions
-=================================
+            # 2.
+            threshold = self.threshold
 
-.. _intro_input_file_discussion:
+            # 3.
+            with ImageModel(image1) as image1, ImageModel(image2) as image2:
+                # 4.
+                with self.get_reference_file_model(image1, "flat_field") as flat:
+                    new_image = combine(image1, image2, flat, threshold)
 
-Input Files
------------
+            # 5.
+            return new_image
 
-There are two general types of input to any step or pipeline: references files
-and data files.  The references files, unless explicitly
-overridden, are provided through CRDS.
+       # 6.
+       spec = """
+       # This is the configspec file for ExampleStep
 
-Data files are the science input, such as exposure ASDF files. All files are
-assumed to be co-resident in the directory where the primary input file is
-located.
+       threshold = float(default=1.0)  # maximum flux
+       """
 
-.. _intro_output_file_discussion:
+       # 7.
+       reference_file_types = ['flat_field']
 
-Output Files
-------------
+The Python Step subclass may be installed anywhere that your Python
+installation can find it.  It does not need to be installed in the
+`stpipe` package.
 
-Output files will be created either in the current working directory, or where
-specified by the :ref:`output_dir <intro_output_directory>` parameter.
+.. _the-spec-member:
 
-File names for the outputs from pipelines and steps come from
-three different sources:
+The spec member
+---------------
 
-- The name of the input file
-- As specified by the :ref:`output_file <intro_output_file>` parameter
+The `spec` member variable is a string containing information about
+the parameters.  It is in the `configspec` format
+defined in the `ConfigObj` library that stpipe uses.
 
-Regardless of the source, each pipeline/step uses the name as a base
-name, onto which several different suffixes are appended, which
-indicate the type of data in that particular file. A list of the main suffixes
-can be :ref:`found below <pipeline_step_suffix_definitions>`.
+The `configspec` format defines the types of the parameters, as well as allowing
+an optional tree structure.
 
-The pipelines do not manage versions. When re-running a pipeline, previous files
-will be overwritten.
+The types of parameters are declared like this::
 
-Individual Step Outputs
-^^^^^^^^^^^^^^^^^^^^^^^
+    n_iterations = integer(1, 100)  # The number of iterations to run
+    factor = float()                # A multiplication factor
+    author = string()               # The author of the file
 
-If individual steps are executed without an output file name specified via
-the ``output_file`` parameter, the ``stpipe`` infrastructure
-automatically uses the input file name as the root of the output file name
-and appends the name of the step as an additional suffix to the input file
-name. If the input file name already has a known suffix, that suffix
-will be replaced. For example:
-::
+Note that each parameter may have a comment.  This comment is
+extracted and displayed in help messages and docstrings etc.
 
-   $ strun romancal.dq_init.DQInitStep r0008308002010007027_06311_0019_WFI01_uncal.asdf
+Parameters can be grouped into categories using
+ini-file-like syntax::
 
-produces an output file named
-``r0008308002010007027_06311_0019_WFI01_dq_init.asdf``.
+    [red]
+    offset = float()
+    scale = float()
 
-See :ref:`pipeline_step_suffix_definitions` for a list of the more common
-suffixes used.
+    [green]
+    offset = float()
+    scale = float()
 
-Parameters
-==========
+    [blue]
+    offset = float()
+    scale = float()
 
-All pipelines and steps have **parameters** that can be set to change various
-aspects of how they execute. To see what parameters are available for any given
-pipeline or step, use the ``-h`` option on ``strun``. Some examples are:
-::
+Default values may be specified on any parameter using the `default`
+keyword argument::
 
-   $ strun roman_elp -h
-   $ strun calroman.dq_init.DQInitStep -h
+    name = string(default="John Doe")
 
-To set a parameter, simply specify it on the command line. For example, to have
-:ref:`roman_elp <exposure_pipeline>` save the calibrated ramp files, the
-``strun`` command would be as follows:
-::
+While the most commonly useful parts of the configspec format are
+discussed here, greater detail can be found in the `configspec
+documentation
+<https://configobj.readthedocs.io/en/latest/>`_.
 
-   $ strun roman_elp r0008308002010007027_06311_0019_WFI01_uncal.asdf --save_calibrated_ramp=true
+Configspec types
+````````````````
 
-To specify parameter values for an individual step when running a pipeline
-use the syntax ``--steps.<step_name>.<parameter>=value``.
-For example, to override the default selection of a dark current reference
-file from CRDS when running a pipeline:
-::
+The following is a list of the commonly useful configspec types.
 
-    $ strun roman_elp r0008308002010007027_06311_0019_WFI01_uncal.asdf
-          --steps.dark_current.override_dark='my_dark.asdf'
+    `integer`: matches integer values. Takes optional `min` and `max`
+    arguments::
 
-Universal Parameters
---------------------
+        integer()
+        integer(3, 9)  # any value from 3 to 9
+        integer(min=0) # any positive value
+        integer(max=9)
 
-The set of parameters that are common to all pipelines and steps are referred to
-as **universal parameters** and are described below.
+    `float`: matches float values Has the same parameters as the
+    integer check.
 
-.. _intro_output_directory:
+    `boolean`: matches boolean values: True or False.
 
-Output Directory
-^^^^^^^^^^^^^^^^
+    `string`: matches any string. Takes optional keyword args `min`
+    and `max` to specify min and max length of string.
 
-By default, all pipeline and step outputs will drop into the current
-working directory, i.e., the directory in which the process is
-running. To change this, use the ``output_dir`` parameter. For example, to
-have all output from ``roman_elp``, including any saved
-intermediate steps, appear in the sub-directory ``calibrated``, use
-::
+    `list`: matches any list. Takes optional keyword args `min`, and
+    `max` to specify min and max sizes of the list. The list checks
+    always return a list.
 
-    $ strun roman_elp r0008308002010007027_06311_0019_WFI01_uncal.asdf
-        --output_dir=calibrated
+    `force_list`: matches any list, but if a single value is passed in
+    will coerce it into a list containing that value.
 
-``output_dir`` can be specified at the step level, overriding what was
-specified for the pipeline. From the example above, to change the name
-and location of the ``dark_current`` step, use the following
-::
+    `int_list`: Matches a list of integers. Takes the same arguments
+    as list.
+
+    `float_list`: Matches a list of floats. Takes the same arguments
+    as list.
+
+    `bool_list`: Matches a list of boolean values. Takes the same
+    arguments as list.
+
+    `string_list`: Matches a list of strings. Takes the same arguments
+    as list.
+
+    `option`: matches any from a list of options. You specify this
+    test with::
+
+        option('option 1', 'option 2', 'option 3')
+
+    Normally, steps will receive input files as parameters and return
+    output files from their process methods.  However, in cases where
+    paths to files should be specified in the parameter file,
+    there are some extra parameter types that stpipe provides that
+    aren’t part of the core configobj library.
+
+    `input_file`: Specifies an input file.  Relative paths are
+    resolved against the location of the parameter file.  The file
+    must also exist.
+
+    `output_file`: Specifies an output file.  Identical to
+    `input_file`, except the file doesn’t have to already exist.
+
+.. _interfacing-with-crds:
+
+Interfacing with CRDS
+---------------------
+
+If a Step uses CRDS to retrieve reference files, there are two
+things to do:
+
+1. Within the `process` method, call `self.get_reference_file` or
+   `self.get_reference_file_model` to get a reference file from CRDS.
+   These methods take as input a) a model for the input file, whose
+   metadata is used to do a CRDS bestref lookup, and b) a reference
+   file type, which is just a string to identify the kind of reference
+   file.
+
+2. Declare the reference file types used by the Step in the
+   `reference_file_types` member. This information is used by the stpipe
+   framework for two purposes: a) to pre-cache the reference files needed by a
+   Pipeline before any of the pipeline processing actually runs, and b) to add
+   override parameters to the Step's configspec.
+
+For each reference file type that the Step declares, an `override_*` parameter
+is added to the Step's configspec. For example, if a step declares the
+following::
+
+   reference_file_types = ['flat_field']
+
+then the user can override the flat field reference file using the
+parameter file::
+
+   override_flat_field = /path/to/my_reference_file.asdf
+
+or at the command line::
 
-    $ strun roman_elp r0008308002010007027_06311_0019_WFI01_uncal.asdf
-        --output_dir=calibrated
-        --steps.dark_current.output_file='dark_sub.asdf'
-        --steps.dark_current.output_dir='dark_calibrated'
-
-.. _intro_output_file:
-
-Output File
-^^^^^^^^^^^
-
-When running a pipeline, the ``stpipe`` infrastructure automatically passes the
-output data model from one step to the input of the next step, without
-saving any intermediate results to disk.
-
-.. _pipeline_step_suffix_definitions:
-
-Pipeline/Step Suffix Definitions
---------------------------------
-
-However the output file name is determined (:ref:`see above
-<intro_output_file_discussion>`), the various pipeline modules
-will use that file name, along with a set of predetermined suffixes, to compose
-output file names. The output file name suffix will always replace any known
-suffix of the input file name. Each pipeline module uses the appropriate suffix
-for the product(s) it is creating. The list of suffixes is shown in the
-following table. Replacement occurs only if the suffix is one known to the
-calibration code. Otherwise, the new suffix will simply be appended to the
-basename of the file.
-
-=============================================  ============
-Product                                        Suffix
-=============================================  ============
-Uncalibrated raw input                         uncal
-DQ initialization                              dq_init
-Saturation detection                           saturation
-Linearity correction                           linearity
-Dark current                                   dark_current
-Jump detection                                 jump
-Corrected ramp data                            rampfit
-Optional fitting results from ramp_fit step    fitopt
-Assign WCS                                     assign_wcs
-Flat field                                     flat
-Photometric calibration			       phot
-Calibrated image                               cal
-=============================================  ============
+   --override_flat_field=/path/to/my_reference_file.asdf
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `romancal-0.8.1/docs/roman/jump/arguments.rst` & `romancal-0.9.0/docs/roman/jump/arguments.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/jump/description.rst` & `romancal-0.9.0/docs/roman/jump/description.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/jump/reference_files.rst` & `romancal-0.9.0/docs/roman/jump/reference_files.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/linearity/description.rst` & `romancal-0.9.0/docs/roman/linearity/description.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/photom/description.rst` & `romancal-0.9.0/docs/roman/photom/description.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/pipeline/exposure_pipeline.rst` & `romancal-0.9.0/docs/roman/pipeline/exposure_pipeline.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/pipeline/main.rst` & `romancal-0.9.0/docs/roman/pipeline/main.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/ramp_fitting/arguments.rst` & `romancal-0.9.0/docs/roman/ramp_fitting/arguments.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/ramp_fitting/description.rst` & `romancal-0.9.0/docs/roman/ramp_fitting/description.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/ramp_fitting/reference_files.rst` & `romancal-0.9.0/docs/roman/ramp_fitting/reference_files.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/dark_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/dark_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/dark_selection.inc` & `romancal-0.9.0/docs/roman/references_general/dark_selection.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/dark_specific.inc` & `romancal-0.9.0/docs/roman/references_general/dark_specific.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/distortion_reffile.rst` & `romancal-0.9.0/docs/roman/references_general/distortion_reffile.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/distortion_selection.inc` & `romancal-0.9.0/docs/roman/references_general/distortion_selection.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/flat_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/flat_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/flat_selection.inc` & `romancal-0.9.0/docs/roman/references_general/flat_selection.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/gain_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/gain_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/linearity_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/linearity_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/mask_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/mask_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/mask_selection.inc` & `romancal-0.9.0/docs/roman/references_general/mask_selection.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/photom_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/photom_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/photom_selection.inc` & `romancal-0.9.0/docs/roman/references_general/photom_selection.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/readnoise_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/readnoise_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/readnoise_selection.inc` & `romancal-0.9.0/docs/roman/references_general/readnoise_selection.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/references_general.rst` & `romancal-0.9.0/docs/roman/references_general/references_general.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/references_general/saturation_reffile.inc` & `romancal-0.9.0/docs/roman/references_general/saturation_reffile.inc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/refpix/description.rst` & `romancal-0.9.0/docs/roman/refpix/description.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/docs/roman/saturation/description.rst` & `romancal-0.9.0/docs/roman/saturation/description.rst`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/requirements-dev.txt` & `romancal-0.9.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/assign_wcs/assign_wcs_step.py` & `romancal-0.9.0/romancal/assign_wcs/assign_wcs_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/assign_wcs/pointing.py` & `romancal-0.9.0/romancal/assign_wcs/pointing.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/assign_wcs/tests/test_wcs.py` & `romancal-0.9.0/romancal/assign_wcs/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/conftest.py` & `romancal-0.9.0/romancal/conftest.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/dark_current/dark_current_step.py` & `romancal-0.9.0/romancal/dark_current/dark_current_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/dark_current/tests/test_dark.py` & `romancal-0.9.0/romancal/dark_current/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/dq_init/dq_init_step.py` & `romancal-0.9.0/romancal/dq_init/dq_init_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/dq_init/dq_initialization.py` & `romancal-0.9.0/romancal/dq_init/dq_initialization.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/dq_init/tests/test_dq_init.py` & `romancal-0.9.0/romancal/dq_init/tests/test_dq_init.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/flatfield/flat_field.py` & `romancal-0.9.0/romancal/flatfield/flat_field.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/flatfield/flat_field_step.py` & `romancal-0.9.0/romancal/flatfield/flat_field_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/flatfield/tests/test_flatfield.py` & `romancal-0.9.0/romancal/flatfield/tests/test_flatfield.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/jump/jump_step.py` & `romancal-0.9.0/romancal/jump/jump_step.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,14 +28,20 @@
         rejection_threshold = float(default=4.0,min=0) # CR sigma rej thresh
         three_group_rejection_threshold = float(default=6.0,min=0) # CR sigma rej thresh
         four_group_rejection_threshold = float(default=5.0,min=0) # CR sigma rej thresh
         maximum_cores = option('none', 'quarter', 'half', 'all', default='none') # max number of processes to create
         flag_4_neighbors = boolean(default=True) # flag the four perpendicular neighbors of each CR
         max_jump_to_flag_neighbors = float(default=1000) # maximum jump sigma that will trigger neighbor flagging
         min_jump_to_flag_neighbors = float(default=10) # minimum jump sigma that will trigger neighbor flagging
+        min_sat_area = float(default=1.0) # minimum required area for the central saturation of snowballs
+        min_jump_area = float(default=5.0) # minimum area to trigger large events processing
+        expand_factor = float(default=2.0) # The expansion factor for the enclosing circles or ellipses
+        use_ellipses = boolean(default=False) # Use an enclosing ellipse rather than a circle for MIRI showers
+        sat_required_snowball = boolean(default=True) # Require the center of snowballs to be saturated
+        expand_large_events = boolean(default=False) # must be True to trigger snowball and shower flagging
     """
 
     reference_file_types = ['gain', 'readnoise']
 
     def process(self, input):
 
         # Open input as a Roman DataModel (single integration; 3D arrays)
@@ -75,14 +81,20 @@
             rej_thresh = self.rejection_threshold
             three_grp_rej_thresh = self.three_group_rejection_threshold
             four_grp_rej_thresh = self.four_group_rejection_threshold
             max_cores = self.maximum_cores
             max_jump_to_flag_neighbors = self.max_jump_to_flag_neighbors
             min_jump_to_flag_neighbors = self.min_jump_to_flag_neighbors
             flag_4_neighbors = self.flag_4_neighbors
+            min_sat_area = self.min_sat_area
+            min_jump_area = self.min_jump_area
+            expand_factor = self.expand_factor
+            use_ellipses = self.use_ellipses
+            sat_required_snowball = self.sat_required_snowball
+            expand_large_events = self.expand_large_events
 
             self.log.info('CR rejection threshold = %g sigma', rej_thresh)
             if self.maximum_cores != 'none':
                 self.log.info('Maximum cores to use = %s', max_cores)
 
             # Get the gain and readnoise reference files
             gain_filename = self.get_reference_file(input_model, 'gain')
@@ -112,15 +124,19 @@
             gdq, pdq = detect_jumps(frames_per_group, data, gdq, pdq, err,
                                     gain_2d, readnoise_2d, rej_thresh,
                                     three_grp_rej_thresh, four_grp_rej_thresh,
                                     max_cores,
                                     max_jump_to_flag_neighbors,
                                     min_jump_to_flag_neighbors,
                                     flag_4_neighbors,
-                                    dqflags_d)
+                                    dqflags_d,
+                                    min_sat_area=min_sat_area, min_jump_area=min_jump_area,
+                                    expand_factor=expand_factor, use_ellipses=use_ellipses,
+                                    sat_required_snowball=sat_required_snowball,
+                                    expand_large_events=expand_large_events)
 
             gdq = gdq[0, :, :, :]
             pdq = pdq[0, :, :]
             result.groupdq = gdq
             result.pixeldq = pdq
             gain_model.close()
             readnoise_model.close()
```

### Comparing `romancal-0.8.1/romancal/jump/tests/test_jump_step.py` & `romancal-0.9.0/romancal/jump/tests/test_jump_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/lib/basic_utils.py` & `romancal-0.9.0/romancal/lib/basic_utils.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/lib/dqflags.py` & `romancal-0.9.0/romancal/lib/dqflags.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/lib/suffix.py` & `romancal-0.9.0/romancal/lib/suffix.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/lib/tests/helpers.py` & `romancal-0.9.0/romancal/lib/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/lib/tests/test_suffix.py` & `romancal-0.9.0/romancal/lib/tests/test_suffix.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/linearity/linearity_step.py` & `romancal-0.9.0/romancal/linearity/linearity_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/photom/photom.py` & `romancal-0.9.0/romancal/photom/photom.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/photom/photom_step.py` & `romancal-0.9.0/romancal/photom/photom_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,26 +47,32 @@
                                                        photom_model)
                     output_model.meta.cal_step.photom = 'COMPLETE'
                 else:
                     self.log.warning('No photometric corrections for '
                                      'spectral data')
                     self.log.warning('Photom step will be skipped')
                     input_model.meta.cal_step.photom = 'SKIPPED'
+                    input_model.meta.photometry.pixelarea_arcsecsq = None
+                    input_model.meta.photometry.pixelarea_steradians = None
+                    input_model.meta.photometry.conversion_megajanskys = None
+                    input_model.meta.photometry.conversion_microjanskys = None
+                    input_model.meta.photometry.conversion_megajanskys_uncertainty = None
+                    input_model.meta.photometry.conversion_microjanskys_uncertainty = None
                     try:
                         photom_model.close()
                     except AttributeError:
                         pass
-                    return input_model
+                    output_model = input_model
 
             else:
                 # Skip Photom step if no photom file
                 self.log.warning('No PHOTOM reference file found')
                 self.log.warning('Photom step will be skipped')
                 input_model.meta.cal_step.photom = 'SKIPPED'
-                return input_model
+                output_model = input_model
 
         # Close the input and reference files
         input_model.close()
         try:
             photom_model.close()
         except AttributeError:
             pass
```

### Comparing `romancal-0.8.1/romancal/photom/tests/test_photom.py` & `romancal-0.9.0/romancal/photom/tests/test_photom.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,42 +236,34 @@
     # Select exposure type and optical element
     wfi_image.meta.exposure.type = "WFI_PRISM"
     wfi_image.meta.instrument.optical_element = "PRISM"
 
     # Set photometric values for spectroscopic data
     wfi_image.meta.photometry.pixelarea_steradians = 2.31307642258977E-14 * u.steradian
     wfi_image.meta.photometry.pixelarea_arcsecsq = 0.000984102303070964 * u.arcsecond * u.arcsecond
-    wfi_image.meta.photometry.conversion_megajanskys = None
-    wfi_image.meta.photometry.conversion_megajanskys_uncertainty = None
-    wfi_image.meta.photometry.conversion_microjanskys = None
-    wfi_image.meta.photometry.conversion_microjanskys_uncertainty = None
+    wfi_image.meta.photometry.conversion_megajanskys = -99999 * u.megajansky / u.steradian
+    wfi_image.meta.photometry.conversion_megajanskys_uncertainty = -99999 * u.megajansky / \
+                                                                   u.steradian
+    wfi_image.meta.photometry.conversion_microjanskys = -99999 * u.microjansky / u.arcsecond ** 2
+    wfi_image.meta.photometry.conversion_microjanskys_uncertainty = -99999 * u.microjansky / \
+                                                                    u.arcsecond ** 2
 
     # Create input model
     wfi_image_model = ImageModel(wfi_image)
 
     # Create photom model
     photom = testutil.mk_wfi_img_photom()
     photom_model = WfiImgPhotomRefModel(photom)
 
     # Run photom correction step
     result = PhotomStep.call(wfi_image_model, override_photom=photom_model)
 
     # Test that the data has not changed
     assert (np.allclose(result.data, wfi_image_model.data, rtol=1.e-7))
 
-    # Test that keywords are properly preserved
+    # Test that keywords are properly overwritten
     assert result.meta.photometry.conversion_megajanskys is None
     assert result.meta.photometry.conversion_microjanskys is None
     assert result.meta.photometry.conversion_megajanskys_uncertainty is None
     assert result.meta.photometry.conversion_microjanskys_uncertainty is None
-
-    # Set reference pixel areas
-    area_ster = 2.31307642258977E-14 * u.steradian
-    area_a2 = 0.000984102303070964 * u.arcsecond * u.arcsecond
-
-    # Tests for pixel areas
-    assert (np.isclose(result.meta.photometry.pixelarea_steradians.value,
-                        area_ster.value, atol=1.e-7))
-    assert result.meta.photometry.pixelarea_steradians.unit == area_ster.unit
-    assert (np.isclose(result.meta.photometry.pixelarea_arcsecsq.value,
-                        area_a2.value, atol=1.e-7))
-    assert result.meta.photometry.pixelarea_arcsecsq.unit == area_a2.unit
+    assert result.meta.photometry.pixelarea_steradians is None
+    assert result.meta.photometry.pixelarea_arcsecsq is None
```

### Comparing `romancal-0.8.1/romancal/pipeline/exposure_pipeline.py` & `romancal-0.9.0/romancal/pipeline/exposure_pipeline.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/ramp_fitting/ramp_fit_step.py` & `romancal-0.9.0/romancal/ramp_fitting/ramp_fit_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/ramp_fitting/tests/test_ramp_fit.py` & `romancal-0.9.0/romancal/ramp_fitting/tests/test_ramp_fit.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/conftest.py` & `romancal-0.9.0/romancal/regtest/conftest.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/regtestdata.py` & `romancal-0.9.0/romancal/regtest/regtestdata.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/sdp_pools_source.py` & `romancal-0.9.0/romancal/regtest/sdp_pools_source.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_dark_current.py` & `romancal-0.9.0/romancal/regtest/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_jump_det.py` & `romancal-0.9.0/romancal/regtest/test_jump_det.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_linearity.py` & `romancal-0.9.0/romancal/regtest/test_linearity.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_ramp_fitting.py` & `romancal-0.9.0/romancal/regtest/test_ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_wfi_dq_init.py` & `romancal-0.9.0/romancal/regtest/test_wfi_dq_init.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_wfi_flat_field.py` & `romancal-0.9.0/romancal/regtest/test_wfi_flat_field.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_wfi_photom.py` & `romancal-0.9.0/romancal/regtest/test_wfi_photom.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_wfi_pipeline.py` & `romancal-0.9.0/romancal/regtest/test_wfi_pipeline.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/regtest/test_wfi_saturation.py` & `romancal-0.9.0/romancal/regtest/test_wfi_saturation.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/saturation/saturation.py` & `romancal-0.9.0/romancal/saturation/saturation.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/saturation/saturation_step.py` & `romancal-0.9.0/romancal/saturation/saturation_step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/saturation/tests/test_saturation.py` & `romancal-0.9.0/romancal/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/step.py` & `romancal-0.9.0/romancal/step.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/stpipe/core.py` & `romancal-0.9.0/romancal/stpipe/core.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/stpipe/integration.py` & `romancal-0.9.0/romancal/stpipe/integration.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/stpipe/tests/test_core.py` & `romancal-0.9.0/romancal/stpipe/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/stpipe/tests/test_integration.py` & `romancal-0.9.0/romancal/stpipe/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/stpipe/utilities.py` & `romancal-0.9.0/romancal/stpipe/utilities.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal/tests/base_classes.py` & `romancal-0.9.0/romancal/tests/base_classes.py`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/romancal.egg-info/PKG-INFO` & `romancal-0.9.0/romancal.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romancal
-Version: 0.8.1
+Version: 0.9.0
 Summary: Library for calibration of science observations from the Nancy Grace Roman Space Telescope
 Home-page: https://github.com/spacetelescope/romancal
 Author: Roman calibration pipeline developers
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/spacetelescope/romancal/issues
 Project-URL: Documentation, https://roman-pipeline.readthedocs.io/en/stable/
 Project-URL: Source Code, https://github.com/spacetelescope/romancal
```

### Comparing `romancal-0.8.1/romancal.egg-info/SOURCES.txt` & `romancal-0.9.0/romancal.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .codecov.yml
 .gitignore
 .gitmodules
-.readthedocs.yml
+.readthedocs.yaml
 CHANGES.rst
 CODEOWNERS.txt
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 JenkinsfileRT
 JenkinsfileRT_dev
 LICENSE
@@ -20,24 +20,33 @@
 .github/labeler.yml
 .github/pull_request_template.md
 .github/workflows/cancel_workflows.yml
 .github/workflows/changelog.yml
 .github/workflows/label_pull_request.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/roman_ci.yml
+docs/0.5.0
 docs/Makefile
 docs/conf.py
 docs/conftest.py
 docs/index.rst
 docs/make.bat
-docs/_static/JWSTlogocrop.png
+docs/_static/favicon.ico
+docs/_static/roman_logo_black_w200px.png
+docs/_static/roman_logo_white_w100px.png
 docs/_static/stsci_logo.png
 docs/exts/numfig.py
 docs/roman/introduction.rst
 docs/roman/package_index.rst
+docs/roman/pipeline_installation.rst
+docs/roman/pipeline_naming_conventions.rst
+docs/roman/pipeline_parameters.rst
+docs/roman/pipeline_ref_files.rst
+docs/roman/pipeline_run.rst
+docs/roman/pipeline_steps.rst
 docs/roman/assign_wcs/index.rst
 docs/roman/assign_wcs/main.rst
 docs/roman/dark_current/arguments.rst
 docs/roman/dark_current/description.rst
 docs/roman/dark_current/index.rst
 docs/roman/dark_current/reference_files.rst
 docs/roman/datamodels/datamodels_asdf.rst
@@ -102,14 +111,25 @@
 docs/roman/references_general/saturation_selection.inc
 docs/roman/refpix/description.rst
 docs/roman/refpix/index.rst
 docs/roman/saturation/arguments.rst
 docs/roman/saturation/description.rst
 docs/roman/saturation/index.rst
 docs/roman/saturation/reference_files.rst
+docs/roman/stpipe/call_via_call.rst
+docs/roman/stpipe/call_via_run.rst
+docs/roman/stpipe/config_asdf.rst
+docs/roman/stpipe/devel_logging.rst
+docs/roman/stpipe/devel_pipeline.rst
+docs/roman/stpipe/devel_step.rst
+docs/roman/stpipe/index.rst
+docs/roman/stpipe/parameter_files.rst
+docs/roman/stpipe/user_logging.rst
+docs/roman/stpipe/user_pipeline.rst
+docs/roman/stpipe/user_step.rst
 romancal/__init__.py
 romancal/conftest.py
 romancal/step.py
 romancal.egg-info/PKG-INFO
 romancal.egg-info/SOURCES.txt
 romancal.egg-info/dependency_links.txt
 romancal.egg-info/entry_points.txt
```

### Comparing `romancal-0.8.1/scripts/okify_regtests` & `romancal-0.9.0/scripts/okify_regtests`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/scripts/schema_editor` & `romancal-0.9.0/scripts/schema_editor`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/scripts/schemadoc` & `romancal-0.9.0/scripts/schemadoc`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/scripts/verify_install_requires` & `romancal-0.9.0/scripts/verify_install_requires`

 * *Files identical despite different names*

### Comparing `romancal-0.8.1/setup.cfg` & `romancal-0.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 zip_safe = False
 python_requires = >=3.8
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	asdf>=2.12.1
 	astropy>=5.0.4
-	crds>=11.13.1
+	crds>=11.16.16
 	gwcs>=0.18.1
 	jsonschema>=3.0.2
-	numpy
+	numpy>=1.20
 	pyparsing>=2.4.7
 	requests>=2.22
-	roman_datamodels>=0.13.0
-	stcal>=0.7.2
+	roman_datamodels>=0.14.0
+	stcal>=1.2.1,<2.0
 	stpipe>=0.4.2,<1.0
 
 [options.extras_require]
 docs = 
 	matplotlib
 	sphinx
 	sphinx-automodapi
```

### Comparing `romancal-0.8.1/setup.py` & `romancal-0.9.0/setup.py`

 * *Files identical despite different names*

