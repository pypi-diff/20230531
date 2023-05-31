# Comparing `tmp/stcal-1.3.7.tar.gz` & `tmp/stcal-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stcal-1.3.7.tar", last modified: Wed Apr 26 13:59:59 2023, max compression
+gzip compressed data, was "stcal-1.3.8.tar", last modified: Wed May 31 17:06:43 2023, max compression
```

## Comparing `stcal-1.3.7.tar` & `stcal-1.3.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.752149 stcal-1.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/label_pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 13:59:46.000000 stcal-1.3.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-26 13:59:46.000000 stcal-1.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 13:59:46.000000 stcal-1.3.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-04-26 13:59:46.000000 stcal-1.3.7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-26 13:59:46.000000 stcal-1.3.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-26 13:59:46.000000 stcal-1.3.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-26 13:59:46.000000 stcal-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-26 13:59:59.748149 stcal-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-04-26 13:59:46.000000 stcal-1.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-26 13:59:46.000000 stcal-1.3.7/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-26 13:59:46.000000 stcal-1.3.7/benchmarks/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/docs/stcal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.672149 stcal-1.3.7/docs/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/jump/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/jump/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/package_index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/docs/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/ramp_fitting/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 13:59:46.000000 stcal-1.3.7/docs/stcal/ramp_fitting/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-26 13:59:46.000000 stcal-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 13:59:59.752149 stcal-1.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.668148 stcal-1.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/basic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/dark_current/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dark_current/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dark_current/dark_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dark_current/dark_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dqflags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/dynamicdq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/jump/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32158 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/jump.py
--rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/jump/twopoint_difference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/linearity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/linearity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/linearity/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal/ramp_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)   127063 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/ols_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    56430 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/ramp_fitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.680148 stcal-1.3.7/src/stcal/saturation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/saturation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-26 13:59:46.000000 stcal-1.3.7/src/stcal/saturation/saturation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.676149 stcal-1.3.7/src/stcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 13:59:59.000000 stcal-1.3.7/src/stcal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 13:59:58.000000 stcal-1.3.7/src/stcal.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.716149 stcal-1.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/current_gdqfits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 13:59:59.748149 stcal-1.3.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/data/input_gdq_flarge.fits
--rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/data/large_event_input_dq_cube2.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/data/snowball1.fits
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_dark_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_dq.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_jump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)    48431 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_ramp_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_ramp_fitting_gls_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43187 2023-04-26 13:59:46.000000 stcal-1.3.7/tests/test_twopoint_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-26 13:59:46.000000 stcal-1.3.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.497736 stcal-1.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.417734 stcal-1.3.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/label_pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-31 17:06:32.000000 stcal-1.3.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-31 17:06:32.000000 stcal-1.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 17:06:32.000000 stcal-1.3.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-31 17:06:32.000000 stcal-1.3.8/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-31 17:06:32.000000 stcal-1.3.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-31 17:06:32.000000 stcal-1.3.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 17:06:32.000000 stcal-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-31 17:06:43.497736 stcal-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-31 17:06:32.000000 stcal-1.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-31 17:06:32.000000 stcal-1.3.8/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-31 17:06:32.000000 stcal-1.3.8/benchmarks/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/stcal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/jump/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/jump/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/package_index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/docs/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)    16733 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/ramp_fitting/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-31 17:06:32.000000 stcal-1.3.8/docs/stcal/ramp_fitting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-31 17:06:32.000000 stcal-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:06:43.497736 stcal-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.417734 stcal-1.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/src/stcal/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/basic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/dark_current/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dark_current/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dark_current/dark_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13391 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dark_current/dark_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dqflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/dynamicdq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/jump/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32158 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/jump/twopoint_difference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/linearity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/linearity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/linearity/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/ramp_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58471 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126980 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/ols_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10029 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56279 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/ramp_fitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.425734 stcal-1.3.8/src/stcal/saturation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/saturation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-31 17:06:32.000000 stcal-1.3.8/src/stcal/saturation/saturation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.421733 stcal-1.3.8/src/stcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 17:06:43.000000 stcal-1.3.8/src/stcal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:06:42.000000 stcal-1.3.8/src/stcal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.461735 stcal-1.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 33557760 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/current_gdqfits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:06:43.497736 stcal-1.3.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 20975040 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/data/input_gdq_flarge.fits
+-rw-r--r--   0 runner    (1001) docker     (123) 12588480 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/data/large_event_input_dq_cube2.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/data/snowball1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_dark_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_dq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_jump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53269 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_ramp_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_ramp_fitting_gls_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43187 2023-05-31 17:06:32.000000 stcal-1.3.8/tests/test_twopoint_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-31 17:06:32.000000 stcal-1.3.8/tox.ini
```

### Comparing `stcal-1.3.7/.github/labeler.yml` & `stcal-1.3.8/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/.github/pull_request_template.md` & `stcal-1.3.8/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/.github/workflows/ci.yml` & `stcal-1.3.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/.github/workflows/publish-to-pypi.yml` & `stcal-1.3.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/.gitignore` & `stcal-1.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/.readthedocs.yaml` & `stcal-1.3.8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/CHANGES.rst` & `stcal-1.3.8/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 1.4.0 (unreleased)
 ==================
 
 Bug Fixes
 ---------
 
-- 
+-
 
 Changes to API
 --------------
 
 - 
 
 Other
 -----
 
 - 
 
-1.3.7 (unreleased)
+1.3.8 (2023-05-31)
+==================
+
+Bug Fixes
+---------
+
+dark_current
+~~~~~~~~~~~~
+
+- Fixed handling of MIRI segmented data files so that the correct dark
+  integrations get subtracted from the correct science integrations. [#165]
+
+ramp_fitting
+~~~~~~~~~~~~
+
+- Correct the "averaging" of the final image slope by properly excluding
+  variances as a part of the denominator from integrations with invalid slopes.
+  [#167]
+- Removing the usage of ``numpy.where`` where possible for perfomance
+  reasons. [#169]
+
+1.3.7 (2023-04-26)
 ==================
 
 Bug Fixes
 ---------
 
 ramp_fitting
 ~~~~~~~~~~~~
```

### Comparing `stcal-1.3.7/CODE_OF_CONDUCT.md` & `stcal-1.3.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/CONTRIBUTING.md` & `stcal-1.3.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/LICENSE` & `stcal-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/PKG-INFO` & `stcal-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.3.7
+Version: 1.3.8
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.3.7/README.md` & `stcal-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/benchmarks/dark_current.py` & `stcal-1.3.8/benchmarks/dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/benchmarks/linearity.py` & `stcal-1.3.8/benchmarks/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/benchmarks/ramp_fitting.py` & `stcal-1.3.8/benchmarks/ramp_fitting.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/benchmarks/saturation.py` & `stcal-1.3.8/benchmarks/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/docs/Makefile` & `stcal-1.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/docs/conf.py` & `stcal-1.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/docs/stcal/jump/description.rst` & `stcal-1.3.8/docs/stcal/jump/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/docs/stcal/ramp_fitting/description.rst` & `stcal-1.3.8/docs/stcal/ramp_fitting/description.rst`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/pyproject.toml` & `stcal-1.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'License :: OSI Approved :: BSD License',
     'Programming Language :: Python :: 3',
 ]
 dependencies = [
     'astropy >=5.0.4',
     'scipy >=1.6.0',
     'numpy >=1.20',
-    'opencv-python >=4.6.0.66',
+    'opencv-python-headless >=4.6.0.66',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 docs = [
     'numpydoc',
     'packaging >=17',
```

### Comparing `stcal-1.3.7/src/stcal/dark_current/dark_class.py` & `stcal-1.3.8/src/stcal/dark_current/dark_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,19 +94,24 @@
             if isinstance(science_model.err,u.Quantity):
                 self.err = science_model.err.value
             else:
                 self.err = science_model.err
 
             self.exp_nframes = science_model.meta.exposure.nframes
             self.exp_groupgap = science_model.meta.exposure.groupgap
+            try:  # JWST only
+                self.exp_intstart = science_model.meta.exposure.integration_start
+            except AttributeError:
+                self.exp_intstart = None
 
             self.cal_step = None
         else:
             self.data = None
             self.groupdq = None
             self.pixeldq = None
             self.err = None
 
             self.exp_nframes = None
             self.exp_groupgap = None
+            self.exp_intstart = None
 
             self.cal_step = None
```

### Comparing `stcal-1.3.7/src/stcal/dark_current/dark_sub.py` & `stcal-1.3.8/src/stcal/dark_current/dark_sub.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,18 +139,18 @@
             averaged_dark.save = True
             averaged_dark.output_name = dark_output
 
     else:
 
         # Create a frame-averaged version of the dark data to match
         # the nframes and groupgap settings of the science data.
-        # If the data are from MIRI, the darks are integration-dependent and
-        # we average them with a seperate routine.
+        # If the data are from JWST/MIRI, the darks are integration-dependent
+        # and we average them with a seperate routine.
 
-        if len(dark_data.data.shape) == 4:
+        if len(dark_data.data.shape) == 4:  # only MIRI uses 4-D darks
             averaged_dark = average_dark_frames_4d(
                 dark_data, sci_nints, sci_ngroups, sci_nframes, sci_groupgap
             )
         else:
             averaged_dark = average_dark_frames_3d(
                 dark_data, sci_ngroups, sci_nframes, sci_groupgap
             )
@@ -169,15 +169,15 @@
     return output_data, averaged_dark
 
 
 def average_dark_frames_3d(dark_data, ngroups, nframes, groupgap):
     """
     Averages the individual frames of data in a dark reference
     file to match the group structure of a science data set.
-    This routine is not used for MIRI (see average_MIRIdark_frames)
+    This routine is not used for JWST/MIRI (see average_dark_frames_4d).
 
     Parameters
     ----------
     dark_data : DarkData
         the input dark data
 
     ngroups : int
@@ -236,16 +236,17 @@
     return avg_dark
 
 
 def average_dark_frames_4d(dark_data, nints, ngroups, nframes, groupgap):
     """
     Averages the individual frames of data in a dark reference
     file to match the group structure of a science data set.
-    MIRI needs a separate routine because the darks are integration dependent.
-    We need an average dark for each dark integration.
+    JWST/MIRI needs a separate routine because the darks are
+    integration-dependent and hence 4D in shape, instead of 3D.
+    An average dark is created for each integration.
 
     Parameters
     ----------
     dark_data : DarkData
         the input dark data
 
     nints : int
@@ -335,14 +336,19 @@
 
     Returns
     -------
     output : data model object
         dark-subtracted science data
     """
 
+    # The integration start number is only needed for JWST/MIRI data.
+    # It defaults to 1 if the keyword is not in the science data.
+    int_start = 1 if science_data.exp_intstart is None else science_data.exp_intstart
+
+    # Determine the number of integrations contained in the dark reference file
     if len(dark_data.data.shape) == 4:
         dark_nints = dark_data.data.shape[0]
     else:
         dark_nints = 1
 
     log.debug("subtract_dark: nints=%d, ngroups=%d, size=%d,%d",
               science_data.data.shape[0], science_data.data.shape[1],
@@ -357,30 +363,33 @@
         darkdq = dark_data.groupdq[0, 0, :, :].copy()
         for i in range(1, dark_nints):
             darkdq = np.bitwise_or(darkdq, dark_data.groupdq[i, 0, :, :])
     else:
         # All other instruments have a single 2D dark DQ array
         darkdq = dark_data.groupdq
 
-    # Combine the dark and science DQ data
+    # Propagate the dark DQ data into the science DQ data
     output.pixeldq = np.bitwise_or(science_data.pixeldq, darkdq)
 
     # Loop over all integrations in input science data
     for i in range(science_data.data.shape[0]):
 
-        if len(dark_data.data.shape) == 4:
-            # use integration-specific dark data
-            if i < dark_nints:
+        if len(dark_data.data.shape) == 4:  # MIRI data
+            # Apply the first dark_nints-1 integrations from the dark ref file
+            # to the first few science integrations. There's an additional
+            # check of the starting integration number in case the science
+            # data are segmented.
+            if i < dark_nints and int_start == 1:
                 dark_sci = dark_data.data[i]
             else:
-                # for science integrations beyond the number of
+                # For science integrations beyond the number of
                 # dark integrations, use the last dark integration
                 dark_sci = dark_data.data[-1]
         else:
-            # use single-integration dark data
+            # Use single-integration dark data
             dark_sci = dark_data.data
 
         # Loop over all groups in this integration
         for j in range(science_data.data.shape[1]):
             # subtract the dark from the science data
             output.data[i, j] -= dark_sci[j]
```

### Comparing `stcal-1.3.7/src/stcal/dqflags.py` & `stcal-1.3.8/src/stcal/dqflags.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal/jump/jump.py` & `stcal-1.3.8/src/stcal/jump/jump.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal/jump/twopoint_difference.py` & `stcal-1.3.8/src/stcal/jump/twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal/linearity/linearity.py` & `stcal-1.3.8/src/stcal/linearity/linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal/ramp_fitting/gls_fit.py` & `stcal-1.3.8/src/stcal/ramp_fitting/gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal/ramp_fitting/ols_fit.py` & `stcal-1.3.8/src/stcal/ramp_fitting/ols_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -939,18 +939,15 @@
 
             # Get appropriate sections
             gdq_sect = groupdq[num_int, :, :, :]
             rn_sect = readnoise_2d[rlo:rhi, :]
             gain_sect = gain_2d[rlo:rhi, :]
 
             # Reset all saturated groups in the input data array to NaN
-            where_sat = np.where(np.bitwise_and(gdq_sect, ramp_data.flags_saturated))
-
-            data_sect[where_sat] = np.NaN
-            del where_sat
+            data_sect[np.bitwise_and(gdq_sect, ramp_data.flags_saturated).astype(bool)] = np.NaN
 
             # Calculate the slope of each segment
             # note that the name "opt_res", which stands for "optional results",
             # is deceiving; this in fact contains all the per-integration and
             # per-segment results that will eventually be used to compute the
             # final slopes, sigmas, etc. for the main (non-optional) products
             t_dq_cube, inv_var, opt_res, f_max_seg, num_seg = \
@@ -961,19 +958,16 @@
 
             # Populate 3D num_seg { integ, y, x } with 2D num_seg for this data
             #  section (y,x) and integration (num_int)
             sect_shape = data_sect.shape[-2:]
             num_seg_per_int[num_int, rlo:rhi, :] = num_seg.reshape(sect_shape)
 
             # Populate integ-spec slice which is set if 0th group has SAT
-            wh_sat0 = np.where(np.bitwise_and(gdq_sect[0, :, :], ramp_data.flags_saturated))
-            if len(wh_sat0[0]) > 0:
-                sat_0th_group_int[num_int, rlo:rhi, :][wh_sat0] = 1
-
-            del wh_sat0
+            sat_0th_group_int[num_int, rlo:rhi, :][np.bitwise_and(
+                    gdq_sect[0, :, :], ramp_data.flags_saturated).astype(bool)] = 1
 
             pixeldq_sect = pixeldq[rlo:rhi, :].copy()
             dq_int[num_int, rlo:rhi, :] = utils.dq_compress_sect(
                 ramp_data, num_int, t_dq_cube, pixeldq_sect).copy()
 
             del t_dq_cube
 
@@ -1297,14 +1291,20 @@
 
     slope_by_var4 = opt_res.slope_seg.copy() / var_both4
 
     del var_both4
 
     s_slope_by_var3 = slope_by_var4.sum(axis=1)  # sum over segments (not integs)
     s_slope_by_var2 = s_slope_by_var3.sum(axis=0)  # sum over integrations
+
+    # Ensure bad integrations don't contribute to the denominator
+    # for slope calculations
+    invalid_data = ramp_data.flags_saturated | ramp_data.flags_do_not_use
+    wh_invalid = np.where(np.bitwise_and(dq_int, invalid_data))
+    s_inv_var_both3[wh_invalid] = 0.
     s_inv_var_both2 = s_inv_var_both3.sum(axis=0)
 
     # Compute the 'dataset-averaged' slope
     # Suppress, then re-enable harmless arithmetic warnings
     warnings.filterwarnings("ignore", ".*invalid value.*", RuntimeWarning)
     warnings.filterwarnings("ignore", ".*divide by zero.*", RuntimeWarning)
     slope_dataset2 = s_slope_by_var2 / s_inv_var_both2
@@ -1414,16 +1414,15 @@
     # Compress all integration's dq arrays to create 2D PIXELDDQ array for
     #   primary output
     final_pixeldq = utils.dq_compress_final(dq_int, ramp_data)
 
     # For invalid slope calculations set to NaN.  Pixels flagged as SATURATED or
     # DO_NOT_USE have invalid data.
     invalid_data = ramp_data.flags_saturated | ramp_data.flags_do_not_use
-    wh_invalid = np.where(np.bitwise_and(final_pixeldq, invalid_data))
-    c_rates[wh_invalid] = np.nan
+    c_rates[np.bitwise_and(final_pixeldq, invalid_data).astype(bool)] = np.nan
 
     if dq_int is not None:
         del dq_int
 
     tstop = time.time()
 
     utils.log_stats(c_rates)
@@ -1487,19 +1486,19 @@
 
     Returns
     -------
     pow_wt : ndarray
         weighting exponent, 1-D float
     """
     pow_wt = snr.copy() * 0.0
-    pow_wt[np.where(snr > 5.)] = 0.4
-    pow_wt[np.where(snr > 10.)] = 1.0
-    pow_wt[np.where(snr > 20.)] = 3.0
-    pow_wt[np.where(snr > 50.)] = 6.0
-    pow_wt[np.where(snr > 100.)] = 10.0
+    pow_wt[snr > 5.] = 0.4
+    pow_wt[snr > 10.] = 1.0
+    pow_wt[snr > 20.] = 3.0
+    pow_wt[snr > 50.] = 6.0
+    pow_wt[snr > 100.] = 10.0
 
     return pow_wt.ravel()
 
 
 def interpolate_power(snr):
     """
     Using the given SNR, interpolate the weighting exponent, which is from
@@ -1707,17 +1706,15 @@
         #   group in the current segement.  We want to include it as part of
         #   the current segment, but exclude all other groups with any other
         #   flag.
 
         # Find CRs in the ramp.
         jump_det = ramp_data.flags_jump_det
         mask_2d_jump = mask_2d.copy()
-        wh_jump = np.where(gdq_sect_r == jump_det)
-        mask_2d_jump[wh_jump] = True
-        del wh_jump
+        mask_2d_jump[gdq_sect_r == jump_det] = True
 
         # Add back possible CRs at the beginning of a ramp that were excluded
         # above.
         wh_mask_2d = np.where(mask_2d)
         mask_2d[np.maximum(wh_mask_2d[0] - 1, 0), wh_mask_2d[1]] = True
         del wh_mask_2d
 
@@ -3191,19 +3188,15 @@
     #    now they are just place-holders
     variance_s = np.zeros(npix, dtype=np.float32) + utils.LARGE_VARIANCE
     sig_slope_s = slope_s * 0.
     intercept_s = slope_s * 0.
     sig_intercept_s = slope_s * 0.
 
     # For saturated pixels, overwrite slope with benign values.
-    wh_sat0 = np.where(np.logical_not(mask_2d[0, :]))
-
-    if len(wh_sat0[0]) > 0:
-        sat_pix = wh_sat0[0]
-        slope_s[sat_pix] = 0.
+    slope_s[np.logical_not(mask_2d[0, :])] = 0.
 
     return slope_s, intercept_s, variance_s, sig_intercept_s, sig_slope_s
 
 
 def check_both_groups_good(gdq):
     """
     Special case checker for 2 group ramps.  This checks to see if both groups
```

### Comparing `stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit.py` & `stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal/ramp_fitting/ramp_fit_class.py` & `stcal-1.3.8/src/stcal/ramp_fitting/ramp_fit_class.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal/ramp_fitting/utils.py` & `stcal-1.3.8/src/stcal/ramp_fitting/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,19 +505,17 @@
     # Create integration-specific sections of input arrays for determination
     #   of the variances.
     gdq_2d = gdq_sect[:, :, :].reshape((nreads, npix))
     gain_1d = gain_sect.reshape(npix)
     gdq_2d_nan = gdq_2d.copy()  # group dq with SATS will be replaced by nans
     gdq_2d_nan = gdq_2d_nan.astype(np.float32)
 
-    wh_sat = np.where(np.bitwise_and(gdq_2d, ramp_data.flags_saturated))
-    if len(wh_sat[0]) > 0:
-        gdq_2d_nan[wh_sat] = np.nan  # set all SAT groups to nan
-
-    del wh_sat
+    # set all SAT groups to nan
+    gdq_2d_nan[np.bitwise_and(
+            gdq_2d, ramp_data.flags_saturated).astype(bool)] = np.nan
 
     # Get lengths of semiramps for all pix [number_of_semiramps, number_of_pix]
     segs = np.zeros_like(gdq_2d)
 
     # Counter of semiramp for each pixel
     sr_index = np.zeros(npix, dtype=np.uint8)
     pix_not_done = np.ones(npix, dtype=bool)  # initialize to True
@@ -560,17 +558,16 @@
 
     # Create reshaped version [ segs, y, x ] to simplify computation
     segs_beg_3 = segs_beg.reshape(max_seg, imshape[0], imshape[1])
     segs_beg_3 = remove_bad_singles(segs_beg_3)
 
     # Create a version 1 less for later calculations for the variance due to
     #   Poisson, with a floor=1 to handle single-group segments
-    wh_pos_3 = np.where(segs_beg_3 > 1)
     segs_beg_3_m1 = segs_beg_3.copy()
-    segs_beg_3_m1[wh_pos_3] -= 1
+    segs_beg_3_m1[segs_beg_3 > 1] -= 1
     segs_beg_3_m1[segs_beg_3_m1 < 1] = 1
 
     # For a segment, the variance due to Poisson noise
     #   = slope/(tgroup * gain * (ngroups-1)),
     #   where slope is the estimated median slope, tgroup is the group time,
     #   and ngroups is the number of groups in the segment.
     #   Here the denominator of this quantity will be computed, which will be
@@ -732,16 +729,15 @@
 
     var_p3[var_p3 > LARGE_VARIANCE_THRESHOLD] = 0.
     var_r3[var_r3 > LARGE_VARIANCE_THRESHOLD] = 0.
     var_both3[var_both3 > LARGE_VARIANCE_THRESHOLD] = 0.
 
     data = slope_int / effintim
     invalid_data = ramp_data.flags_saturated | ramp_data.flags_do_not_use
-    wh_invalid = np.where(np.bitwise_and(dq_int, invalid_data))
-    data[wh_invalid] = np.nan
+    data[np.bitwise_and(dq_int, invalid_data).astype(bool)] = np.nan
 
     err = np.sqrt(var_both3)
     dq = dq_int
     var_poisson = var_p3
 
     var_rnoise = var_r3
     integ_info = (data, dq, var_poisson, var_rnoise, err)
@@ -1377,15 +1373,15 @@
     set_flag : int
         Flag to set if flag is found in each integration.
     """
     nints = integ_dq.shape[0]
 
     # Find where flag is set
     test_dq = np.zeros(integ_dq.shape, dtype=np.uint32)
-    test_dq[np.where(np.bitwise_and(integ_dq, flag))] = 1
+    test_dq[np.bitwise_and(integ_dq, flag).astype(bool)] = 1
 
     # Sum over all integrations
     test_sum = test_dq.sum(axis=0)
     all_set = np.where(test_sum == nints)
 
     # If flag is set in all integrations, then set the set_flag
     final_dq[all_set] = np.bitwise_or(final_dq[all_set], set_flag)
@@ -1495,18 +1491,15 @@
     median_diffs_2d = np.zeros(imshape, dtype=np.float32)
 
     for integ in range(nints):
         data_sect = ramp_data.data[integ, :, :, :].copy()
         gdq_sect = ramp_data.groupdq[integ, :, :, :]
 
         # Reset all saturated groups in the input data array to NaN
-        where_sat = np.where(np.bitwise_and(gdq_sect, ramp_data.flags_saturated))
-
-        data_sect[where_sat] = np.NaN
-        del where_sat
+        data_sect[np.bitwise_and(gdq_sect, ramp_data.flags_saturated).astype(bool)] = np.NaN
 
         data_sect = data_sect / group_time
 
         if one_groups_time_adjustment is not None:
             one_groups_locs = ramp_data.one_groups_locs[integ]
             tmp_dsect = data_sect[0, :, :]
             tmp_dsect[one_groups_locs] = tmp_dsect[one_groups_locs] * one_groups_time_adjustment
@@ -1640,12 +1633,12 @@
     sat_flag : uint
         The data quality flag for SATURATED
 
     num_sat_groups : int
         The number of saturated groups in an integration of interest.
     """
     sat_groups = np.zeros(intdq.shape, dtype=int)
-    sat_groups[np.where(np.bitwise_and(intdq, sat_flag))] = 1
+    sat_groups[np.bitwise_and(intdq, sat_flag).astype(bool)] = 1
     nsat_groups = sat_groups.sum(axis=0)
     wh_nsat_groups = np.where(nsat_groups == num_sat_groups)
 
     return wh_nsat_groups
```

### Comparing `stcal-1.3.7/src/stcal/saturation/saturation.py` & `stcal-1.3.8/src/stcal/saturation/saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/src/stcal.egg-info/PKG-INFO` & `stcal-1.3.8/src/stcal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stcal
-Version: 1.3.7
+Version: 1.3.8
 Summary: STScI tools and algorithms used in calibration pipelines
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2020 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stcal-1.3.7/src/stcal.egg-info/SOURCES.txt` & `stcal-1.3.8/src/stcal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/current_gdqfits` & `stcal-1.3.8/tests/current_gdqfits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/data/input_gdq_flarge.fits` & `stcal-1.3.8/tests/data/input_gdq_flarge.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/data/large_event_input_dq_cube2.fits` & `stcal-1.3.8/tests/data/large_event_input_dq_cube2.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/data/snowball1.fits` & `stcal-1.3.8/tests/data/snowball1.fits`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/test_dark_current.py` & `stcal-1.3.8/tests/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/test_dq.py` & `stcal-1.3.8/tests/test_dq.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/test_jump.py` & `stcal-1.3.8/tests/test_jump.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/test_linearity.py` & `stcal-1.3.8/tests/test_linearity.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/test_ramp_fitting.py` & `stcal-1.3.8/tests/test_ramp_fitting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 
 from stcal.ramp_fitting.ramp_fit import ramp_fit_data
 from stcal.ramp_fitting.ramp_fit_class import RampData
 
+
 DELIM = "-" * 70
 
 # single group intergrations fail in the GLS fitting
 # so, keep the two method test separate and mark GLS test as
 # expected to fail.  Needs fixing, but the fix is not clear
 # to me. [KDG - 19 Dec 2018]
 
@@ -1191,14 +1192,145 @@
     np.testing.assert_allclose(cvr, check, tol, tol)
 
     check = np.array([[[0.02353317, 0.02258242, 0.]],
                       [[0.03073696, 0.        , 0.]]])
     np.testing.assert_allclose(cerr, check, tol, tol)
 
 
+def test_invalid_integrations():
+    """
+    Tests a multi-integration data set with bad data in multiple integrations
+    to ensure these integrations to do not contribute to the final slope
+    calculation for the image.
+
+    The data and group DQ flags were taken from data used for JP-3004.  The
+    suppress_one_group is defaulted to True.  With this data and flag set
+    there are only two good integrations.
+    """
+    nints, ngroups, nrows, ncols = 8, 5, 1, 1
+    rnval, gval = 6.097407, 5.5
+    frame_time, nframes, groupgap = 2.77504, 1, 0
+
+    dims = nints, ngroups, nrows, ncols
+    var = rnval, gval
+    tm = frame_time, nframes, groupgap
+
+    ramp, gain, rnoise = create_blank_ramp_data(dims, var, tm)
+    int_data = [
+        [17343.719, 32944.32 , 48382.062, 63066.062, 58844.7  ],
+        [19139.965, 34863.45 , 50415.816, 52806.453, 59525.01 ],
+        [19020.926, 34759.785, 50351.984, 52774.695, 59533.586],
+        [19060.592, 34772.496, 50247.75 , 52781.04 , 59509.086],
+        [19011.01 , 34768.832, 50247.547, 52829.46 , 59557.85 ],
+        [18939.426, 34680.39 , 50175.406, 52685.527, 59486.184],
+        [19009.908, 34748.207, 50274.14 , 52723.406, 59523.812],
+        [19072.715, 34844.24 , 50421.906, 52781.83 , 59527.06 ]
+    ]
+    int_dq = [
+        [DNU, GOOD, JUMP, GOOD, DNU | SAT],
+        [DNU, GOOD, JUMP, SAT, DNU | SAT],
+        [DNU, GOOD, JUMP, SAT, DNU | SAT],
+        [DNU, GOOD, GOOD, SAT, DNU | SAT],
+        [DNU, GOOD, JUMP, SAT, DNU | SAT],
+        [DNU, GOOD, JUMP, SAT, DNU | SAT],
+        [DNU, GOOD, JUMP, SAT, DNU | SAT],
+        [DNU, GOOD, JUMP, SAT, DNU | SAT]
+    ]
+
+    for integ in range(nints):
+        ramp.data[integ, :, 0, 0] = np.array(int_data[integ], dtype=np.float32)
+        ramp.groupdq[integ, :, 0, 0] = np.array(int_dq[integ], dtype=np.uint8)
+
+    ramp.suppress_one_group_ramps = True
+
+    save_opt, ncores, bufsize, algo = False, "none", 1024 * 30000, "OLS"
+    slopes, cube, ols_opt, gls_opt = ramp_fit_data(
+        ramp, bufsize, save_opt, rnoise, gain, algo,"optimal", ncores, dqflags)
+
+    tol = 1.e-5
+
+    # Check slopes information
+    sdata, sdq, svp, svr, serr = slopes
+
+
+    check = np.array([[5434.022]])
+    np.testing.assert_allclose(sdata, check, tol, tol)
+
+    check = np.array([[JUMP]])
+    np.testing.assert_allclose(sdq, check, tol, tol)
+
+    check = np.array([[46.189373]])
+    np.testing.assert_allclose(svp, check, tol, tol)
+
+    check = np.array([[0.6034785]])
+    np.testing.assert_allclose(svr, check, tol, tol)
+
+    check = np.array([[6.84053]])
+    np.testing.assert_allclose(serr, check, tol, tol)
+
+    # Check slopes information
+    cdata, cdq, cvp, cvr, cerr = cube
+
+    check = np.array([5291.4556, np.nan, np.nan, 5576.588,
+                      np.nan, np.nan, np.nan, np.nan], dtype=np.float32)
+    np.testing.assert_allclose(cdata[:, 0, 0], check, tol, tol)
+
+    check = np.array([JUMP, JUMP | DNU, JUMP | DNU, GOOD,
+                      JUMP | DNU, JUMP | DNU, JUMP | DNU, JUMP | DNU], dtype=np.uint8)
+    np.testing.assert_allclose(cdq[:, 0, 0], check, tol, tol)
+
+    check = np.array([369.51498, 369.51498, 369.51498, 369.51498,
+                      369.51498, 369.51498, 369.51498, 369.51498], dtype=np.float32)
+    np.testing.assert_allclose(cvp[:, 0, 0], check, tol, tol)
+
+    check = np.array([4.827828, 4.827828, 4.827828, 4.827828,
+                      4.827828, 4.827828, 4.827828, 4.827828], dtype=np.float32)
+    np.testing.assert_allclose(cvr[:, 0, 0], check, tol, tol)
+
+    check = np.array([19.348047, 19.348047, 19.348047, 19.348047,
+                      19.348047, 19.348047, 19.348047, 19.348047], dtype=np.float32)
+    np.testing.assert_allclose(cerr[:, 0, 0], check, tol, tol)
+
+
+def test_one_group():
+    """
+    Test ngroups = 1
+    """
+    nints, ngroups, nrows, ncols = 1, 1, 1, 1
+    rnval, gval = 10., 5.
+    frame_time, nframes, groupgap = 10.736, 4, 1
+
+    dims = nints, ngroups, nrows, ncols
+    var = rnval, gval
+    tm = frame_time, nframes, groupgap
+
+    ramp, gain, rnoise = create_blank_ramp_data(dims, var, tm)
+
+    ramp.data[0, 0, 0, 0] = 105.31459
+
+    save_opt, ncores, bufsize, algo = False, "none", 1024 * 30000, "OLS"
+    slopes, cube, ols_opt, gls_opt = ramp_fit_data(
+        ramp, bufsize, save_opt, rnoise, gain, algo,"optimal", ncores, dqflags)
+
+    tol = 1e-5
+    sdata, sdq, svp, svr, serr = slopes
+    assert abs(sdata[0, 0] - 1.9618962) < tol
+    assert sdq[0, 0] == 0
+    assert abs(svp[0, 0] - 0.02923839) < tol
+    assert abs(svr[0, 0] - 0.03470363) < tol
+    assert abs(serr[0, 0] - 0.2528676) < tol
+
+    cdata, cdq, cvp, cvr, cerr = cube
+    assert abs(sdata[0, 0] - cdata[0, 0, 0]) < tol
+    assert sdq[0, 0] == cdq[0, 0, 0]
+    assert abs(svp[0, 0] - cvp[0, 0, 0]) < tol
+    assert abs(svr[0, 0] - cvr[0, 0, 0]) < tol
+    assert abs(serr[0, 0] - cerr[0, 0, 0]) < tol
+
+
 def create_blank_ramp_data(dims, var, tm):
     """
     Create empty RampData classes, as well as gain and read noise arrays,
     based on dimensional, variance, and timing input.
     """
     nints, ngroups, nrows, ncols = dims
     rnval, gval = var
```

### Comparing `stcal-1.3.7/tests/test_ramp_fitting_gls_fit.py` & `stcal-1.3.8/tests/test_ramp_fitting_gls_fit.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/test_saturation.py` & `stcal-1.3.8/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tests/test_twopoint_difference.py` & `stcal-1.3.8/tests/test_twopoint_difference.py`

 * *Files identical despite different names*

### Comparing `stcal-1.3.7/tox.ini` & `stcal-1.3.8/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -56,22 +56,24 @@
     xdist: pytest-xdist
     jwst: jwst[test] @ git+https://github.com/spacetelescope/jwst.git
     romancal: romancal[test] @ git+https://github.com/spacetelescope/romancal.git
     oldestdeps: minimum_dependencies
 pass_env =
     CI
 set_env =
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
     jwst: CRDS_SERVER_URL=https://jwst-crds.stsci.edu
     romancal: CRDS_SERVER_URL=https://roman-crds.stsci.edu
     jwst,romancal: CRDS_PATH={package_root}/crds_cache
     jwst,romancal: CRDS_CLIENT_RETRY_COUNT=3
     jwst,romancal: CRDS_CLIENT_RETRY_DELAY_SECONDS=20
 commands_pre =
     oldestdeps: minimum_dependencies stcal --filename requirements-min.txt
     oldestdeps: pip install -r requirements-min.txt
+    devdeps: pip install numpy>=0.0.dev0 scipy>=0.0.dev0 git+https://github.com/astropy/astropy -U --upgrade-strategy eager
     pip freeze
 commands =
     pytest \
     warnings: -W error \
     xdist: -n auto \
     jwst: --pyargs jwst --ignore-glob=timeconversion --ignore-glob=associations --ignore-glob=*/scripts/* \
     romancal: --pyargs romancal \
```

