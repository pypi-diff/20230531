# Comparing `tmp/webviz-ert-0.5.4.tar.gz` & `tmp/webviz-ert-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webviz-ert-0.5.4.tar", last modified: Mon Feb 27 12:55:22 2023, max compression
+gzip compressed data, was "webviz-ert-0.5.5.tar", last modified: Wed May 31 14:09:19 2023, max compression
```

## Comparing `webviz-ert-0.5.4.tar` & `webviz-ert-0.5.5.tar`

### file list

```diff
@@ -1,120 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.836862 webviz-ert-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-27 12:55:22.836862 webviz-ert-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.824862 webviz-ert-0.5.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/ci/jenkins/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/ci/jenkins/testkomodo.sh
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 12:55:22.836862 webviz-ert-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/controllers/test_controller_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/controllers/test_response_correlation_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/snake_oil_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/data/spe1_st/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/field_properties.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/field_properties_priors
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/obs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/data/spe1_st/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/resources/SPE1CASE2.DATA.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/data/spe1_st/resources/refcase/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/resources/refcase/SPE1CASE2.SMSPEC
--rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/resources/refcase/SPE1CASE2.UNSMRY
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/spe1.ert
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/data/spe1_st/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/data/spe1_st/tests/test_webviz_ert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/models/test_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/models/test_response_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/plots/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/test_data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.828862 webviz-ert-0.5.4/tests/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.832862 webviz-ert-0.5.4/tests/views/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/assets/ert-style.css
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/test_ensemble_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/test_general_stuff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/test_observation_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/test_parameter_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/test_plot_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/test_response_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/tests/views/test_state_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.832862 webviz-ert-0.5.4/webviz_ert/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.832862 webviz-ert-0.5.4/webviz_ert/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70732 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/assets/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/assets/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/assets/ert-style.css
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/assets/ert-style.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/assets/webviz-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.832862 webviz-ert-0.5.4/webviz_ert/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/controller_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/element_dropdown_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/ensemble_selector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/multi_parameter_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/multi_response_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/observation_response_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/parameter_comparison_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/parameter_selector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/plot_view_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/controllers/response_correlation_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.832862 webviz-ert-0.5.4/webviz_ert/data_loader/
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/data_loader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.836862 webviz-ert-0.5.4/webviz_ert/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/plot_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/realization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/models/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.836862 webviz-ert-0.5.4/webviz_ert/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/plugins/_observation_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/plugins/_parameter_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/plugins/_response_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/plugins/_response_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/plugins/_webviz_ert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.836862 webviz-ert-0.5.4/webviz_ert/views/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/correlation_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/element_dropdown_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/ensemble_selector_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/misfit_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/parallel_coordinates_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/parameter_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/plot_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/response_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-02-27 12:55:12.000000 webviz-ert-0.5.4/webviz_ert/views/selector_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 12:55:22.832862 webviz-ert-0.5.4/webviz_ert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-02-27 12:55:22.000000 webviz-ert-0.5.4/webviz_ert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-02-27 12:55:22.000000 webviz-ert-0.5.4/webviz_ert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 12:55:22.000000 webviz-ert-0.5.4/webviz_ert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-27 12:55:22.000000 webviz-ert-0.5.4/webviz_ert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 12:55:22.000000 webviz-ert-0.5.4/webviz_ert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-27 12:55:22.000000 webviz-ert-0.5.4/webviz_ert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-27 12:55:22.000000 webviz-ert-0.5.4/webviz_ert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.890355 webviz-ert-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-31 14:09:19.890355 webviz-ert-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/ci/testkomodo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:09:19.890355 webviz-ert-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/controllers/test_controller_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/controllers/test_response_correlation_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/snake_oil_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/data/spe1_st/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/field_properties.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/field_properties_priors
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/obs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/data/spe1_st/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/resources/SPE1CASE2.DATA.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/data/spe1_st/resources/refcase/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/resources/refcase/SPE1CASE2.SMSPEC
+-rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/resources/refcase/SPE1CASE2.UNSMRY
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/spe1.ert
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/data/spe1_st/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/data/spe1_st/tests/test_webviz_ert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/models/test_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/models/test_response_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.882355 webviz-ert-0.5.5/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/plots/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/test_data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.886355 webviz-ert-0.5.5/tests/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.886355 webviz-ert-0.5.5/tests/views/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/assets/ert-style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/test_ensemble_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/test_general_stuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/test_observation_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/test_parameter_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/test_plot_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/test_response_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/tests/views/test_state_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.886355 webviz-ert-0.5.5/webviz_ert/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.886355 webviz-ert-0.5.5/webviz_ert/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70732 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/assets/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/assets/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/assets/ert-style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/assets/ert-style.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/assets/webviz-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.886355 webviz-ert-0.5.5/webviz_ert/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/controller_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/element_dropdown_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/ensemble_selector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/multi_parameter_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/multi_response_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/observation_response_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/parameter_comparison_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/parameter_selector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/plot_view_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/controllers/response_correlation_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.890355 webviz-ert-0.5.5/webviz_ert/data_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/data_loader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.890355 webviz-ert-0.5.5/webviz_ert/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/plot_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/realization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/models/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.890355 webviz-ert-0.5.5/webviz_ert/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/plugins/_observation_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/plugins/_parameter_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/plugins/_response_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/plugins/_response_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/plugins/_webviz_ert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.890355 webviz-ert-0.5.5/webviz_ert/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/correlation_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/element_dropdown_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/ensemble_selector_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/misfit_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/parallel_coordinates_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/parameter_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/plot_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/response_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-31 14:09:10.000000 webviz-ert-0.5.5/webviz_ert/views/selector_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:09:19.886355 webviz-ert-0.5.5/webviz_ert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-31 14:09:19.000000 webviz-ert-0.5.5/webviz_ert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-31 14:09:19.000000 webviz-ert-0.5.5/webviz_ert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:09:19.000000 webviz-ert-0.5.5/webviz_ert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-31 14:09:19.000000 webviz-ert-0.5.5/webviz_ert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:09:19.000000 webviz-ert-0.5.5/webviz_ert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-31 14:09:19.000000 webviz-ert-0.5.5/webviz_ert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:09:19.000000 webviz-ert-0.5.5/webviz_ert.egg-info/top_level.txt
```

### Comparing `webviz-ert-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md` & `webviz-ert-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md` & `webviz-ert-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/.github/workflows/publish_to_pypi.yml` & `webviz-ert-0.5.5/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/.github/workflows/python.yml` & `webviz-ert-0.5.5/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/.gitignore` & `webviz-ert-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/CODE_OF_CONDUCT.md` & `webviz-ert-0.5.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/CONTRIBUTING.md` & `webviz-ert-0.5.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/LICENSE` & `webviz-ert-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/PKG-INFO` & `webviz-ert-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviz-ert
-Version: 0.5.4
+Version: 0.5.5
 Summary: Webviz plugins for ERT
 Author: Equinor
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Dash
 Classifier: Framework :: Flask
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `webviz-ert-0.5.4/README.md` & `webviz-ert-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/ci/jenkins/testkomodo.sh` & `webviz-ert-0.5.5/ci/testkomodo.sh`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/setup.py` & `webviz-ert-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             "ParameterComparison = webviz_ert.plugins:ParameterComparison",
             "ResponseCorrelation = webviz_ert.plugins:ResponseCorrelation",
         ],
     },
     install_requires=[
         "dash-bootstrap-components",
         "dash-daq",
+        "pandas<2",
         "requests",
         "webviz-config>=0.0.40",
         "webviz-config-equinor",
         "webviz-subsurface-components",
     ],
     tests_require=TESTS_REQUIRE,
     extras_require={"tests": TESTS_REQUIRE},
```

### Comparing `webviz-ert-0.5.4/tests/conftest.py` & `webviz-ert-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/controllers/test_controller_functions.py` & `webviz-ert-0.5.5/tests/controllers/test_controller_functions.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/controllers/test_response_correlation_controller.py` & `webviz-ert-0.5.5/tests/controllers/test_response_correlation_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/data/snake_oil_data.py` & `webviz-ert-0.5.5/tests/data/snake_oil_data.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/data/spe1_st/resources/SPE1CASE2.DATA.jinja2` & `webviz-ert-0.5.5/tests/data/spe1_st/resources/SPE1CASE2.DATA.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/data/spe1_st/resources/refcase/SPE1CASE2.SMSPEC` & `webviz-ert-0.5.5/tests/data/spe1_st/resources/refcase/SPE1CASE2.SMSPEC`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/data/spe1_st/resources/refcase/SPE1CASE2.UNSMRY` & `webviz-ert-0.5.5/tests/data/spe1_st/resources/refcase/SPE1CASE2.UNSMRY`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/data/spe1_st/spe1.ert` & `webviz-ert-0.5.5/tests/data/spe1_st/spe1.ert`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/data/spe1_st/tests/test_webviz_ert.py` & `webviz-ert-0.5.5/tests/data/spe1_st/tests/test_webviz_ert.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         dash_duo_handle.wait_for_contains_text(
             "#" + plugin.uuid(selector),
             key,
         )
 
 
 @pytest.mark.spe1
+@pytest.mark.xfail(reason="Fails because ert>5 no longer supports ert-storage")
 def test_webviz_parameter_comparison(dash_duo):
     plugin = setup_plugin(dash_duo, __name__, ParameterComparison)
 
     # Wait for the ensemble selector to be initialized
     dash_duo.wait_for_contains_text(
         "#" + plugin.uuid("ensemble-multi-selector"),
         "default",
@@ -41,14 +42,15 @@
     ensemble_name = select_first(dash_duo, "#" + plugin.uuid("ensemble-multi-selector"))
     _verify_keys_in_menu(
         dash_duo, plugin, parameter_keys, "parameter-selector-multi-param"
     )
 
 
 @pytest.mark.spe1
+@pytest.mark.xfail(reason="Fails because ert>5 no longer supports ert-storage")
 def test_webviz_response_correlation(dash_duo):
     plugin = setup_plugin(dash_duo, __name__, ResponseCorrelation)
 
     ensemble = "default"
     response = "WOPT:PROD"
     parameter = "FIELD_PROPERTIES:POROSITY::0"
     index = "2016-01-01"
@@ -80,14 +82,15 @@
     dash_duo.wait_for_contains_text(
         "#" + plugin.uuid("parameter-deactivator-param"),
         f"×{parameter}",
     )
 
 
 @pytest.mark.spe1
+@pytest.mark.xfail(reason="Fails because ert>5 no longer supports ert-storage")
 def test_webviz_response_comparison(dash_duo):
     plugin = setup_plugin(dash_duo, __name__, ResponseComparison)
 
     # Wait for the ensemble selector to be initialized
     dash_duo.wait_for_contains_text(
         "#" + plugin.uuid("ensemble-multi-selector"),
         "default",
@@ -115,14 +118,15 @@
     param_plot_id = "#" + plugin.uuid(param_name.replace(":", "\\:"))
     dash_duo.wait_for_element(param_plot_id)
 
     # assert dash_duo.get_logs() == [], "browser console should contain no error"
 
 
 @pytest.mark.spe1
+@pytest.mark.xfail(reason="Fails because ert>5 no longer supports ert-storage")
 def test_webviz_observation_analyzer(dash_duo):
     plugin = setup_plugin(dash_duo, __name__, ObservationAnalyzer)
 
     # Wait for the ensemble selector to be initialized
     dash_duo.wait_for_contains_text(
         "#" + plugin.uuid("ensemble-multi-selector"),
         "default",
```

### Comparing `webviz-ert-0.5.4/tests/models/test_ensemble_model.py` & `webviz-ert-0.5.5/tests/models/test_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/plots/test_controller.py` & `webviz-ert-0.5.5/tests/plots/test_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/views/assets/ert-style.css` & `webviz-ert-0.5.5/tests/views/assets/ert-style.css`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/views/test_ensemble_selector.py` & `webviz-ert-0.5.5/tests/views/test_ensemble_selector.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/views/test_general_stuff.py` & `webviz-ert-0.5.5/tests/views/test_general_stuff.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/views/test_observation_view.py` & `webviz-ert-0.5.5/tests/views/test_observation_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/views/test_parameter_selector.py` & `webviz-ert-0.5.5/tests/views/test_parameter_selector.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/views/test_plot_view.py` & `webviz-ert-0.5.5/tests/views/test_plot_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/tests/views/test_response_correlation.py` & `webviz-ert-0.5.5/tests/views/test_response_correlation.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,17 @@
     # other
     for wanted_response in wanted_responses:
         response_selector_id = plugin.uuid("parameter-selector-multi-resp")
         select_by_name(dash_duo, f"#{response_selector_id}", wanted_response)
 
         plot_id = plugin.uuid("response-overview")
 
-        # check that y axis label spells out "Value"
-        dash_duo.wait_for_text_to_equal(f"#{plot_id} text.ytitle", "Value")
+        # check that y axis label spells out "Value"; test is flaky so longer
+        # timeout.
+        dash_duo.wait_for_text_to_equal(f"#{plot_id} text.ytitle", "Value", timeout=20)
 
         # check that one has date, the other has index as x axis label
         if wanted_response == "FOPR":
             dash_duo.wait_for_text_to_equal(f"#{plot_id} text.xtitle", "Date")
         else:
             dash_duo.wait_for_text_to_equal(f"#{plot_id} text.xtitle", "Index")
 
@@ -59,15 +60,17 @@
     select_ensemble(dash_duo, plugin, "default3")
 
     expected_responses_with_observations = ["FOPR", "WOPR:OP1"]
 
     response_selector_id = "#" + plugin.uuid("parameter-selector-multi-resp")
 
     dash_duo.wait_for_text_to_equal(
-        response_selector_id, "\n".join(expected_responses_with_observations)
+        response_selector_id,
+        "\n".join(expected_responses_with_observations),
+        timeout=20,
     )
 
 
 def test_info_text_appears_as_expected(
     mock_data,
     dash_duo,
 ):
@@ -79,10 +82,10 @@
     select_ensemble(dash_duo, plugin, ensemble)
     select_response(dash_duo, plugin, response, wait_for_plot=False)
     select_parameter(dash_duo, plugin, parameter, wait_for_plot=False)
     info_text_selector = f"#{plugin.uuid('info-text')}"
     expected_text = "".join(
         [f"RESPONSE: {response}", f"INDEX: {index}", f"PARAMETER: {parameter}"]
     )
-    dash_duo.wait_for_text_to_equal(info_text_selector, expected_text)
+    dash_duo.wait_for_text_to_equal(info_text_selector, expected_text, timeout=20)
 
     # assert dash_duo.get_logs() == [], "browser console should contain no error"
```

### Comparing `webviz-ert-0.5.4/tests/views/test_state_saving.py` & `webviz-ert-0.5.5/tests/views/test_state_saving.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/__main__.py` & `webviz-ert-0.5.5/webviz_ert/__main__.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/assets/__init__.py` & `webviz-ert-0.5.5/webviz_ert/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/assets/bootstrap-grid.css` & `webviz-ert-0.5.5/webviz_ert/assets/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/assets/bootstrap.min.css` & `webviz-ert-0.5.5/webviz_ert/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/assets/ert-style.css` & `webviz-ert-0.5.5/webviz_ert/assets/ert-style.css`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/assets/ert-style.json` & `webviz-ert-0.5.5/webviz_ert/assets/ert-style.json`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/__init__.py` & `webviz-ert-0.5.5/webviz_ert/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/controller_functions.py` & `webviz-ert-0.5.5/webviz_ert/controllers/controller_functions.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/element_dropdown_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/element_dropdown_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/ensemble_selector_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/ensemble_selector_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/multi_parameter_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/multi_parameter_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/multi_response_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/multi_response_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/observation_response_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/observation_response_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/parameter_comparison_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/parameter_comparison_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/parameter_selector_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/parameter_selector_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/plot_view_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/plot_view_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/controllers/response_correlation_controller.py` & `webviz-ert-0.5.5/webviz_ert/controllers/response_correlation_controller.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/data_loader/__init__.py` & `webviz-ert-0.5.5/webviz_ert/data_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/models/__init__.py` & `webviz-ert-0.5.5/webviz_ert/models/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/models/ensemble_model.py` & `webviz-ert-0.5.5/webviz_ert/models/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/models/observation.py` & `webviz-ert-0.5.5/webviz_ert/models/observation.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/models/parameter_model.py` & `webviz-ert-0.5.5/webviz_ert/models/parameter_model.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/models/plot_model.py` & `webviz-ert-0.5.5/webviz_ert/models/plot_model.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/models/realization.py` & `webviz-ert-0.5.5/webviz_ert/models/realization.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/models/response.py` & `webviz-ert-0.5.5/webviz_ert/models/response.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/plugins/_observation_analyzer.py` & `webviz-ert-0.5.5/webviz_ert/plugins/_observation_analyzer.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/plugins/_parameter_comparison.py` & `webviz-ert-0.5.5/webviz_ert/plugins/_parameter_comparison.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/plugins/_response_comparison.py` & `webviz-ert-0.5.5/webviz_ert/plugins/_response_comparison.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/plugins/_response_correlation.py` & `webviz-ert-0.5.5/webviz_ert/plugins/_response_correlation.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/plugins/_webviz_ert.py` & `webviz-ert-0.5.5/webviz_ert/plugins/_webviz_ert.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/element_dropdown_view.py` & `webviz-ert-0.5.5/webviz_ert/views/element_dropdown_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/ensemble_selector_view.py` & `webviz-ert-0.5.5/webviz_ert/views/ensemble_selector_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/misfit_view.py` & `webviz-ert-0.5.5/webviz_ert/views/misfit_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/parallel_coordinates_view.py` & `webviz-ert-0.5.5/webviz_ert/views/parallel_coordinates_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/parameter_view.py` & `webviz-ert-0.5.5/webviz_ert/views/parameter_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/plot_view.py` & `webviz-ert-0.5.5/webviz_ert/views/plot_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/response_view.py` & `webviz-ert-0.5.5/webviz_ert/views/response_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert/views/selector_view.py` & `webviz-ert-0.5.5/webviz_ert/views/selector_view.py`

 * *Files identical despite different names*

### Comparing `webviz-ert-0.5.4/webviz_ert.egg-info/PKG-INFO` & `webviz-ert-0.5.5/webviz_ert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviz-ert
-Version: 0.5.4
+Version: 0.5.5
 Summary: Webviz plugins for ERT
 Author: Equinor
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Dash
 Classifier: Framework :: Flask
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `webviz-ert-0.5.4/webviz_ert.egg-info/SOURCES.txt` & `webviz-ert-0.5.5/webviz_ert.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup.py
 test_requirements.txt
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/publish_to_pypi.yml
 .github/workflows/python.yml
-ci/jenkins/testkomodo.sh
+ci/testkomodo.sh
 tests/__init__.py
 tests/conftest.py
 tests/test_data_loader.py
 tests/controllers/test_controller_functions.py
 tests/controllers/test_response_correlation_controller.py
 tests/data/__init__.py
 tests/data/snake_oil_data.py
```

