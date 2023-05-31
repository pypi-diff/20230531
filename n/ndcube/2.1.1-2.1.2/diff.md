# Comparing `tmp/ndcube-2.1.1.tar.gz` & `tmp/ndcube-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndcube-2.1.1.tar", last modified: Thu Mar  9 11:14:21 2023, max compression
+gzip compressed data, was "ndcube-2.1.2.tar", last modified: Wed May 31 18:16:38 2023, max compression
```

## Comparing `ndcube-2.1.1.tar` & `ndcube-2.1.2.tar`

### file list

```diff
@@ -1,127 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.447978 ndcube-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-09 11:13:59.000000 ndcube-2.1.1/.rtd-environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-09 11:13:59.000000 ndcube-2.1.1/.sunpy-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    24723 2023-03-09 11:13:59.000000 ndcube-2.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-09 11:13:59.000000 ndcube-2.1.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-09 11:13:59.000000 ndcube-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-03-09 11:14:21.447978 ndcube-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-09 11:13:59.000000 ndcube-2.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-09 11:13:59.000000 ndcube-2.1.1/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.435978 ndcube-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    24913 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25829 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/data_classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/extending_ndcube.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.435978 ndcube-2.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    83880 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/images/ndcollection_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   112680 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/images/ndcube_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   129621 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/images/ndcube_sliced_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   110370 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/images/ndcubesequence_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   132979 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/images/ndcubesequence_sliced_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/logo/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    41016 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/logo/ndcube.png
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/logo/ndcube.svg
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/nitpick-exceptions
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/reproject.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/rtd_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/slicing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/tabular_coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-09 11:13:59.000000 ndcube-2.1.1/docs/whatsnew/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-09 11:13:59.000000 ndcube-2.1.1/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-09 11:13:59.000000 ndcube-2.1.1/examples/creating_ndcube_from_fitsfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/examples/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-03-09 11:13:59.000000 ndcube-2.1.1/examples/dev/example_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-03-09 11:13:59.000000 ndcube-2.1.1/examples/slicing_ndcube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-09 11:13:59.000000 ndcube-2.1.1/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-09 11:13:59.000000 ndcube-2.1.1/licenses/TEMPLATE_LICENSE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/ndcube/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-09 11:14:21.000000 ndcube-2.1.1/ndcube/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17130 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/ndcube/extra_coords/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/extra_coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/extra_coords/extra_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    38000 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/extra_coords/table_coord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.443978 ndcube-2.1.1/ndcube/extra_coords/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18835 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/extra_coords/tests/test_extra_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/extra_coords/tests/test_lookup_table_coord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/global_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.443978 ndcube-2.1.1/ndcube/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/mixins/ndslicing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/ndcollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    54188 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/ndcube.py
--rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/ndcube_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.443978 ndcube-2.1.1/ndcube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/tests/test_global_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/tests/test_ndcollection.py
--rw-r--r--   0 runner    (1001) docker     (123)    48060 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/tests/test_ndcube.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/tests/test_ndcubesequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/tests/test_sequence_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.443978 ndcube-2.1.1/ndcube/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14303 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.443978 ndcube-2.1.1/ndcube/utils/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/sphinx/code_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.443978 ndcube-2.1.1/ndcube/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/tests/test_utils_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/tests/test_utils_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/tests/test_utils_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/tests/test_utils_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20534 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/utils/wcs_high_level_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.443978 ndcube-2.1.1/ndcube/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/mpl_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/mpl_sequence_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/plotting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.447978 ndcube-2.1.1/ndcube/visualization/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/visualization/tests/test_plotting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.447978 ndcube-2.1.1/ndcube/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.447978 ndcube-2.1.1/ndcube/wcs/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/compound_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/reordered_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/resampled_wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.447978 ndcube-2.1.1/ndcube/wcs/wrappers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/tests/test_compound_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/tests/test_reordered_wcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-03-09 11:13:59.000000 ndcube-2.1.1/ndcube/wcs/wrappers/tests/test_resampled_wcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 11:14:21.439978 ndcube-2.1.1/ndcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-03-09 11:14:21.000000 ndcube-2.1.1/ndcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-09 11:14:21.000000 ndcube-2.1.1/ndcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 11:14:21.000000 ndcube-2.1.1/ndcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 11:14:21.000000 ndcube-2.1.1/ndcube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-09 11:14:21.000000 ndcube-2.1.1/ndcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-09 11:14:21.000000 ndcube-2.1.1/ndcube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-03-09 11:13:59.000000 ndcube-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-03-09 11:14:21.447978 ndcube-2.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-03-09 11:13:59.000000 ndcube-2.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-03-09 11:13:59.000000 ndcube-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.297014 ndcube-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 18:16:20.000000 ndcube-2.1.2/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-31 18:16:20.000000 ndcube-2.1.2/.sunpy-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    25656 2023-05-31 18:16:20.000000 ndcube-2.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-31 18:16:20.000000 ndcube-2.1.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 18:16:20.000000 ndcube-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-31 18:16:38.297014 ndcube-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-31 18:16:20.000000 ndcube-2.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-31 18:16:20.000000 ndcube-2.1.2/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.265014 ndcube-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/1_to_2_transition_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.269014 ndcube-2.1.2/docs/explaining_ndcube/
+-rw-r--r--   0 runner    (1001) docker     (123)    24847 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25861 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/data_classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.269014 ndcube-2.1.2/docs/explaining_ndcube/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    83880 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcollection_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112680 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   129621 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_sliced_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   110370 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132979 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_sliced_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/reproject.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/slicing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/tabular_coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/explaining_ndcube/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/extending_ndcube.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.273014 ndcube-2.1.2/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/logo/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41016 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/logo/ndcube.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/logo/ndcube.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.273014 ndcube-2.1.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/extra_coords.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/ndcube.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/reference/wcs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/rtd_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.273014 ndcube-2.1.2/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 18:16:20.000000 ndcube-2.1.2/docs/whatsnew/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/creating_ndcube_from_fitsfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/examples/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/dev/example_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-31 18:16:20.000000 ndcube-2.1.2/examples/slicing_ndcube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 18:16:20.000000 ndcube-2.1.2/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 18:16:20.000000 ndcube-2.1.2/licenses/TEMPLATE_LICENSE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.277014 ndcube-2.1.2/ndcube/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.281014 ndcube-2.1.2/ndcube/extra_coords/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/extra_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38068 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/table_coord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.281014 ndcube-2.1.2/ndcube/extra_coords/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/tests/test_extra_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/extra_coords/tests/test_lookup_table_coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/global_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.285014 ndcube-2.1.2/ndcube/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/mixins/ndslicing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/ndcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54273 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/ndcube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23261 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/ndcube_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.285014 ndcube-2.1.2/ndcube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_global_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_ndcollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48060 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_ndcube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_ndcubesequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39107 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/tests/test_sequence_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.289014 ndcube-2.1.2/ndcube/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.289014 ndcube-2.1.2/ndcube/utils/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/sphinx/code_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.289014 ndcube-2.1.2/ndcube/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/tests/test_utils_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20562 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/utils/wcs_high_level_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/mpl_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/mpl_sequence_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/plotting_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/visualization/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/visualization/tests/test_plotting_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.293014 ndcube-2.1.2/ndcube/wcs/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/compound_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/reordered_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/resampled_wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.297014 ndcube-2.1.2/ndcube/wcs/wrappers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_compound_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_reordered_wcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-31 18:16:20.000000 ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_resampled_wcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:16:38.281014 ndcube-2.1.2/ndcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:16:37.000000 ndcube-2.1.2/ndcube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:16:38.000000 ndcube-2.1.2/ndcube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-31 18:16:20.000000 ndcube-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-31 18:16:38.297014 ndcube-2.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-05-31 18:16:20.000000 ndcube-2.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-05-31 18:16:20.000000 ndcube-2.1.2/tox.ini
```

### Comparing `ndcube-2.1.1/CHANGELOG.rst` & `ndcube-2.1.2/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+2.1.2 (2023-05-31)
+==================
+
+Backwards Incompatible Changes
+------------------------------
+
+- `ndcube.NDCollection.aligned_axes` attribute is now property. (`#607 <https://github.com/sunpy/ndcube/pull/607>`__)
+
+
+Bug Fixes
+---------
+
+- Keywords for ``sequence_axis_coords`` and ``sequence_axis_unit`` were not passed to the ``SequenceAnimator`` constructor.
+  This is now fixed. (`#607 <https://github.com/sunpy/ndcube/pull/607>`__)
+
+Improved Documentation
+----------------------
+
+- Sphinx nitpicky was enabled and lots of references were updated.
+- Overall documentation layout was adjusted to shrink the sidebar.
+
+
 v2.1.1 (2023-03-09)
 ===================
 
 Bug Fixes
 ---------
 
 - Fix docstring causing doc build problems for some users. (`#600 <https://github.com/sunpy/ndcube/pull/600>`__)
@@ -22,30 +44,30 @@
 
 
 Features
 --------
 
 - Implement new property, `ndcube.ExtraCoords.is_empty` that returns ``True`` if the object has got extra coords.  Otherwise return ``False``. (`#450 <https://github.com/sunpy/ndcube/pull/450>`__)
 - Add `ndcube.ExtraCoords.resample` method to resample extra coordinates by a certain factor in each array dimension. (`#450 <https://github.com/sunpy/ndcube/pull/450>`__)
-- Implement a new `ndcube.NDCube.rebin` method to combine integer numbers of pixels along each axis into larger pixels. (`#450 <https://github.com/sunpy/ndcube/pull/450>`__)
-- Add new methods to interpolate lookup table coordinates: `ndcube.extra_coords.table_coord.QuantityTableCoordinate.interpolate`, `ndcube.extra_coords.table_coord.SkyCoordTableCoordinate.interpolate`, `ndcube.extra_coords.table_coord.TimeTableCoordinate.interpolate`, `ndcube.extra_coords.table_coord.MultipleTableCoordinate.interpolate` (`#450 <https://github.com/sunpy/ndcube/pull/450>`__)
+- Implement a new :meth:`ndcube.NDCube.rebin` method to combine integer numbers of pixels along each axis into larger pixels. (`#450 <https://github.com/sunpy/ndcube/pull/450>`__)
+- Add new methods to interpolate lookup table coordinates: ``ndcube.extra_coords.table_coord.QuantityTableCoordinate.interpolate``, ``ndcube.extra_coords.table_coord.SkyCoordTableCoordinate.interpolate``, ``ndcube.extra_coords.table_coord.TimeTableCoordinate.interpolate``, `ndcube.extra_coords.table_coord.MultipleTableCoordinate.interpolate` (`#450 <https://github.com/sunpy/ndcube/pull/450>`__)
 - Add `ndcube.NDCubeSequence.crop` and `ndcube.NDCubeSequence.crop_by_values` methods which crop the `~ndcube.NDCubeSequence` based on input world coordinate ranges. (`#466 <https://github.com/sunpy/ndcube/pull/466>`__)
 - Add basic arithmetic methods between `~ndcube.NDCube` objects and broadcastable arrays,
-  scalars, and `~astropy.unit.Quantity` objects. Operations between two `~ndcube.NDCube` objects
+  scalars, and `~astropy.units.Quantity` objects. Operations between two `~ndcube.NDCube` objects
   are not supported. (`#541 <https://github.com/sunpy/ndcube/pull/541>`__)
 - Add `ndcube.NDCube.to` to convert cube to new unit. (`#586 <https://github.com/sunpy/ndcube/pull/586>`__)
-- Created `~ndcube.GlobalCoordsABC` and updated `~ndcube.NDCubeABC`, and `~ndcube.extra_coords.ExtraCoordsABC` to reflect official NDCube 2 API definition in SEP. (`#592 <https://github.com/sunpy/ndcube/pull/592>`__)
+- Created `~ndcube.GlobalCoordsABC` and updated `~ndcube.ndcube.NDCubeABC`, and `~ndcube.ExtraCoordsABC` to reflect official NDCube 2 API definition in SEP. (`#592 <https://github.com/sunpy/ndcube/pull/592>`__)
 
 
 Bug Fixes
 ---------
 
-- Fix bug #535 where `NDCollection` could not update when `aligned_axes` is `None` (`#538 <https://github.com/sunpy/ndcube/pull/538>`__)
-- Fix a bug where `aligned_axis_physical_types` caused `__str__`
-  to error when `aligned_axes` was `None`. (`#539 <https://github.com/sunpy/ndcube/pull/539>`__)
+- Fix bug #535 where `~ndcube.NDCollection` could not update when ``aligned_axes`` is `None` (`#538 <https://github.com/sunpy/ndcube/pull/538>`__)
+- Fix a bug where ``aligned_axis_physical_types`` caused ``__str__``
+  to error when ``aligned_axes`` was `None`. (`#539 <https://github.com/sunpy/ndcube/pull/539>`__)
 - Fix a bug where ``data_unit`` was not being correctly passed through to the underlying plotting
   function when animating a cube. (`#578 <https://github.com/sunpy/ndcube/pull/578>`__)
 
 
 Improved Documentation
 ----------------------
 
@@ -54,16 +76,16 @@
 
 v2.0.3 (2022-09-23)
 ===================
 
 Bug Fixes
 ---------
 
-- Dynamically copy docstring and function signature from `NDCube.plotter.plot()` to `NDCube.plot()`. (`#534 <https://github.com/sunpy/ndcube/pull/534>`__)
-- Fixed a bug where the `plot_axes` key was not respected when passing `axes` to `plot`
+- Dynamically copy docstring and function signature from ``ndcube.NDCube.plotter.plot`` to :meth:`ndcube.NDCube.plot`. (`#534 <https://github.com/sunpy/ndcube/pull/534>`__)
+- Fixed a bug where the ``plot_axes`` key was not respected when passing ``axes`` to ``plot``
   for 2D cubes. (`#551 <https://github.com/sunpy/ndcube/pull/551>`__)
 - Limit maximum reproject version to 0.9 due to API changes. ndcube 2.1 will support the
   new reproject keyword arguments. (`#564 <https://github.com/sunpy/ndcube/pull/564>`__)
 
 
 v2.0.2 (2022-05-10)
 ===================
@@ -102,131 +124,130 @@
 
 Backwards Incompatible Changes
 ------------------------------
 
 - Remove unused util functions and the ndcube WCS class.  Refactor util functions for converting between between data and WCS indices to reflect the APE14 nomenclature that distinguishes between array, pixel and world axes. (`#280 <https://github.com/sunpy/ndcube/pull/280>`__)
 - NDCubeSequence animation axes can no longer be set by extra coords. (`#294 <https://github.com/sunpy/ndcube/pull/294>`__)
 - ImageAnimatorNDCubeSequence, ImageAnimatorCubeLikeNDCubeSequence, LineAnimatorNDCubeSequence and LineAnimatorCubeLikeNDCubeSequence have been removed and replaced by NDCubeSequenceAnimator. (`#294 <https://github.com/sunpy/ndcube/pull/294>`__)
-- Change type of output of `.NDCollection.aligned_world_axis_physical_types` from tuple to list. This is to be consistent with output of `astropy.wcs.WCS.world_axis_physical_types`. (`#302 <https://github.com/sunpy/ndcube/pull/302>`__)
+- Change type of output of ``ndcube.NDCollection.aligned_world_axis_physical_types`` from tuple to list. This is to be consistent with output of `astropy.wcs.WCS.world_axis_physical_types`. (`#302 <https://github.com/sunpy/ndcube/pull/302>`__)
 - Change output type when common axis item is a slice that covers only one subcube. Previously this would return an NDCube. Now an NDCubeSequence is always returned unless the common axis item is an integer. Also, refactor NDCubeSequence.index_as_cube so codebase is simpler. (`#311 <https://github.com/sunpy/ndcube/pull/311>`__)
 - Replace NDCube.crop_by_coords and NDCube.crop_by_extra_coords with new method, NDCube.crop (`#316 <https://github.com/sunpy/ndcube/pull/316>`__)
 - Remove NDCubeSequence plotting. (`#322 <https://github.com/sunpy/ndcube/pull/322>`__)
 - Update `.NDCube.array_axis_physical_types` return physical types from extra coords as well as the WCS. (`#338 <https://github.com/sunpy/ndcube/pull/338>`__)
-- Rename `.ExtraCoords.add` method from previous name "add_coordinate". (`#394 <https://github.com/sunpy/ndcube/pull/394>`__)
-- The `~.NDcube` object no longer inherits from `astropy.nddata.NDArithmeticMixin` as the methods were not coordinate aware. (`#457 <https://github.com/sunpy/ndcube/pull/457>`__)
+- Rename `ndcube.ExtraCoords.add` method from previous name "add_coordinate". (`#394 <https://github.com/sunpy/ndcube/pull/394>`__)
+- The `~ndcube.NDCube` object no longer inherits from `astropy.nddata.NDArithmeticMixin` as the methods were not coordinate aware. (`#457 <https://github.com/sunpy/ndcube/pull/457>`__)
 
 
 Deprecations and Removals
 -------------------------
 
-- Remove `NDCube.pixel_to_world` and `NDCube.world_to_pixel`. (`#300 <https://github.com/sunpy/ndcube/pull/300>`__)
-- Remove ``world_axis_physical_types`` methods from `.NDCube` and  `.NDCubeSequence`. (`#302 <https://github.com/sunpy/ndcube/pull/302>`__)
-- Remove NDCubeSequence.sequence_axis_extra_coords. This is replaced by NDCubeSequence.sequence_axis_coords. (`#335 <https://github.com/sunpy/ndcube/pull/335>`__)
-- Remove `ndcube.NDCubeSequence.common_axis_extra_coords`.  Will be replaced by `ndcube.NDCubeSequence.common_axis_coords`. (`#344 <https://github.com/sunpy/ndcube/pull/344>`__)
-- Remove NDCollection.aligned_world_axis_physical_types.  It will be replaced by `~ndcube.NDCollection.aligned_axis_physical_types`. (`#347 <https://github.com/sunpy/ndcube/pull/347>`__)
+- Remove ``NDCube.pixel_to_world`` and ``NDCube.world_to_pixel``. (`#300 <https://github.com/sunpy/ndcube/pull/300>`__)
+- Remove ``world_axis_physical_types`` methods from `~ndcube.NDCube` and  `~ndcube.NDCubeSequence`. (`#302 <https://github.com/sunpy/ndcube/pull/302>`__)
+- Remove ``NDCubeSequence.sequence_axis_extra_coords``. This is replaced by ``NDCubeSequence.sequence_axis_coords``. (`#335 <https://github.com/sunpy/ndcube/pull/335>`__)
+- Remove ``ndcube.NDCubeSequence.common_axis_extra_coords``.  Will be replaced by `ndcube.NDCubeSequence.common_axis_coords`. (`#344 <https://github.com/sunpy/ndcube/pull/344>`__)
+- Remove ``NDCollection.aligned_world_axis_physical_types``.  It will be replaced by `~ndcube.NDCollection.aligned_axis_physical_types`. (`#347 <https://github.com/sunpy/ndcube/pull/347>`__)
 
 
 Features
 --------
 
-- Implement a new `.ExtraCoords` class which allows the specification of extra coordinates via lookup tables or WCS. This class exposes the extra coords as an APE 14 WCS object. (`#271 <https://github.com/sunpy/ndcube/pull/271>`__)
-- Add new method, `~ndcube.NDCube.axis_world_coord_values`, to return world coords for all pixels for all axes in WCS as quantity objects. (`#279 <https://github.com/sunpy/ndcube/pull/279>`__)
+- Implement a new `ndcube.ExtraCoords` class which allows the specification of extra coordinates via lookup tables or WCS. This class exposes the extra coords as an APE 14 WCS object. (`#271 <https://github.com/sunpy/ndcube/pull/271>`__)
+- Add new method, ``ndcube.NDCube.axis_world_coord_values``, to return world coords for all pixels for all axes in WCS as quantity objects. (`#279 <https://github.com/sunpy/ndcube/pull/279>`__)
 - Added a new method `ndcube.NDCube.array_axis_physical_types` to show which physical types are associated with each array axis. (`#281 <https://github.com/sunpy/ndcube/pull/281>`__)
 - Add properties to NDCubeSequence giving the world physical types for each array axis. (`#301 <https://github.com/sunpy/ndcube/pull/301>`__)
 - Add as_mpl_axes method to NDCube plotting mixin so the an NDCube can be provided to astropy WCSAxes as a projection. (`#314 <https://github.com/sunpy/ndcube/pull/314>`__)
 - Make pyplot colorbar work with the output on NDCube.plot when it is a 2D image. (`#314 <https://github.com/sunpy/ndcube/pull/314>`__)
 - Introduce a new class, `~ndcube.global_coords.GlobalCoords`, for holding scalar coordinates that don't apply to any pixel axes. (`#323 <https://github.com/sunpy/ndcube/pull/323>`__)
-- Implement `.NDCube.world_axis_coords` which returns high level coordinate
+- Implement `ndcube.NDCube.axis_world_coords` which returns high level coordinate
   objects for all, or a subset of, axes. (`#327 <https://github.com/sunpy/ndcube/pull/327>`__)
 - New property, NDCubeSequence.sequence_axis_coords creates lists of GlobalCoords from each NDCube in the sequence.  This replaces NDCubeSequence.sequence_axis_extra_coords, but because it uses the GlobaCoords infrastructure, can handle more than just coords that began as extra coords. (`#335 <https://github.com/sunpy/ndcube/pull/335>`__)
-- Implement `ndcube.NDCubeSequence.common_axis_coords` to replace `~ndcube.NDCubeSequence.common_axis_extra_coords`. In contrast to old property, this new property collates coordinates from the wcs as well as extra_coords. (`#344 <https://github.com/sunpy/ndcube/pull/344>`__)
-- New property, `ndcube.NDCollection.aligned_axis_physical_types`.  This replaces `~ndcube.NDCollection.aligned_world_axis_physical_types` and returns a list of tuples, where each tuple gives the physical types common between all memebers of the collection for a given aligned axis. (`#347 <https://github.com/sunpy/ndcube/pull/347>`__)
+- Implement `ndcube.NDCubeSequence.common_axis_coords` to replace ``~ndcube.NDCubeSequence.common_axis_extra_coords``. In contrast to old property, this new property collates coordinates from the wcs as well as extra_coords. (`#344 <https://github.com/sunpy/ndcube/pull/344>`__)
+- New property, `ndcube.NDCollection.aligned_axis_physical_types`.  This replaces ``~ndcube.NDCollection.aligned_world_axis_physical_types`` and returns a list of tuples, where each tuple gives the physical types common between all members of the collection for a given aligned axis. (`#347 <https://github.com/sunpy/ndcube/pull/347>`__)
 - Allow `ndcube.NDCubeSequence.explode_along_axis` to explode sequence along any axis, not just the common axis. (`#358 <https://github.com/sunpy/ndcube/pull/358>`__)
-- Plotting functionality on `NDCube` has been refactored to use pluggable
+- Plotting functionality on `~ndcube.NDCube` has been refactored to use pluggable
   "plotter" classes. All plotting functionality can now be accessed via the
-  `.NDCube.plotter` attribute, with `.NDCube.plot` becoming an alias for
-  `.NDCube.plotter.plot`.
+  `ndcube.NDCube.plotter` attribute, with `ndcube.NDCube.plot` becoming an alias for ``ndcube.NDCube.plotter.plot``.
 
   Advanced users, or package maintainers that which to customise the plotting
-  functionality of an ``NDCube`` instance can set the ``.plotter`` attribute of
+  functionality of an `~ndcube.NDCube` instance can set the ``.plotter`` attribute of
   a cube to be a subclass of `ndcube.visualization.BasePlotter` which then
-  customises the behaviour of the ``NDCube.plot()`` method and provides any other
+  customises the behaviour of the :meth:`ndcube.NDCube.plot` method and provides any other
   methods implemented on the plotter. (`#401 <https://github.com/sunpy/ndcube/pull/401>`__)
 - Preserve sliced-out coordinates from WCS in the GlobalCoords instance. (`#402 <https://github.com/sunpy/ndcube/pull/402>`__)
 - Enable instantiating an NDCube from an existing NDCube by copying extra/global coords. (`#404 <https://github.com/sunpy/ndcube/pull/404>`__)
-- Support exposing dropped dimensions when `.ExtraCoords` is sliced. (`#411 <https://github.com/sunpy/ndcube/pull/411>`__)
-- `~ExtraCoords` is now explicitly limited to one dimensional tables because of a limitation in our use of `astropy.modeling`. (`#414 <https://github.com/sunpy/ndcube/pull/414>`__)
+- Support exposing dropped dimensions when `~ndcube.ExtraCoords` is sliced. (`#411 <https://github.com/sunpy/ndcube/pull/411>`__)
+- `~ndcube.ExtraCoords` is now explicitly limited to one dimensional tables because of a limitation in our use of `astropy.modeling`. (`#414 <https://github.com/sunpy/ndcube/pull/414>`__)
 - Adds functionality to reproject an `~.NDCube` object to coordinates described by another WCS or FITS Header by calling the new `~.NDCube.reproject_to` method. (`#434 <https://github.com/sunpy/ndcube/pull/434>`__)
 - Change the ``edges=`` keyword to ``pixel_corners=`` in
-  `NDCube.axis_world_coords` and `NDCube.axis_world_coords_values` to make its
+  :meth:`ndcube.NDCube.axis_world_coords` and `ndcube.NDCube.axis_world_coords_values` to make its
   meaning clearer based on SEP feedback. (`#437 <https://github.com/sunpy/ndcube/pull/437>`__)
 - `~.NDCube.axis_world_coords` and `~.NDCube.axis_world_coords_values` now use a different, substantially faster and more memory efficient algorithm to generate the coordinates along all axes. (`#442 <https://github.com/sunpy/ndcube/pull/442>`__)
-- Extends `~.NDCube.reproject_to` functionality by supporting ``adaptive`` and ``exact`` algorithms for an `~NDCube` with 2D celestial WCS. (`#448 <https://github.com/sunpy/ndcube/pull/448>`__)
-- Introduce optional offset between old and new pixel grids in `~ndcube.wcs.wrappers.resampled_wcs.ResampledLowLevelWCS`. (`#449 <https://github.com/sunpy/ndcube/pull/449>`__)
-- `.ExtraCoords.from_lookup_table` accepts (a seqence of) ``physical_types`` as kwarg to set the types of its ``lookup_tables``. (`#451 <https://github.com/sunpy/ndcube/pull/451>`__)
+- Extends `ndcube.NDCube.reproject_to` functionality by supporting ``adaptive`` and ``exact`` algorithms for an `~ndcube.NDCube` with 2D celestial WCS. (`#448 <https://github.com/sunpy/ndcube/pull/448>`__)
+- Introduce optional offset between old and new pixel grids in `ndcube.wcs.wrappers.resampled_wcs.ResampledLowLevelWCS`. (`#449 <https://github.com/sunpy/ndcube/pull/449>`__)
+- `ndcube.ExtraCoords.from_lookup_tables` accepts (a sequence of) ``physical_types`` as kwarg to set the types of its ``lookup_tables``. (`#451 <https://github.com/sunpy/ndcube/pull/451>`__)
 - Create new plotter class for animating `~ndcube.NDCubeSequence` is the 2.0 framework. This class always sets the sequence axis as a slider and leverages `ndcube.NDCube.plot`. (`#456 <https://github.com/sunpy/ndcube/pull/456>`__)
 - Add ``__len__`` method to `~ndcube.NDCubeSequence` which makes ``len(sequence)`` return the number of cubes in the sequence. (`#464 <https://github.com/sunpy/ndcube/pull/464>`__)
 - Add ``__iter__`` method to `~ndcube.NDCubeSequence` which iterates through the cubes within the sequence. (`#465 <https://github.com/sunpy/ndcube/pull/465>`__)
-- Add property to `~ndcube.extra_coords.ExtraCoords` that returns a WCS of extra coords that describes all axes of associated cube. (`#472 <https://github.com/sunpy/ndcube/pull/472>`__)
+- Add property to `~ndcube.ExtraCoords` that returns a WCS of extra coords that describes all axes of associated cube. (`#472 <https://github.com/sunpy/ndcube/pull/472>`__)
 
 
 Bug Fixes
 ---------
 
-- Fix NDCollection.aligned_dimensions so it doesnt crash when components of collection are NDCubeSequences. (`#264 <https://github.com/sunpy/ndcube/pull/264>`__)
+- Fix `ndcube.NDCollection.aligned_dimensions` so it does not crash when components of collection are NDCubeSequences. (`#264 <https://github.com/sunpy/ndcube/pull/264>`__)
 - Generalize int type checking so it is independent of the bit-type of the OS. (`#269 <https://github.com/sunpy/ndcube/pull/269>`__)
-- Fix axis_world_coord_values when the WCS is 1D and ensure it always returns
+- Fix ``axis_world_coord_values`` when the WCS is 1D and ensure it always returns
   Quantities (`#287 <https://github.com/sunpy/ndcube/pull/287>`__)
-- Change name of NDCube.axis_world_coord_values to NDCube.axis_world_coords_values to be consistent with NDCube.axis_world_coords (`#293 <https://github.com/sunpy/ndcube/pull/293>`__)
+- Change name of ``NDCube.axis_world_coord_values`` to ``NDCube.axis_world_coords_values`` to be consistent with NDCube.axis_world_coords (`#293 <https://github.com/sunpy/ndcube/pull/293>`__)
 - Remove NDCubeSequence animation dependence of deprecated sunpy ImageAnimator and LineAnimator classes in favour of ArrayAnimatorWCS class. (`#294 <https://github.com/sunpy/ndcube/pull/294>`__)
 - Fix bug whereby common axis was not updated appropriately when slicing an NDCubeSequence. (`#310 <https://github.com/sunpy/ndcube/pull/310>`__)
-- Fix bug in NDCube.axis_world_coords_values when number of pixel and world dimensions differ. (`#319 <https://github.com/sunpy/ndcube/pull/319>`__)
+- Fix bug in ``NDCube.axis_world_coords_values`` when number of pixel and world dimensions differ. (`#319 <https://github.com/sunpy/ndcube/pull/319>`__)
 - Fixes bug in `~ndcube.utils.wcs.array_indices_for_world_objects` when the WCS input does not have a world_axis_object_components attribute. The fix causes the low_level_wcs version is tried before the code fails. This enables `ndcube.NDCube.combined_wcs` to be used with this function. (`#344 <https://github.com/sunpy/ndcube/pull/344>`__)
 - Fixes IndexError in `~ndcube.utils.wcs.array_indices_for_world_objects` which occurred when some of the world axes are dependent. (`#344 <https://github.com/sunpy/ndcube/pull/344>`__)
 - Stop `ndcube.NDCube.explode_along_axis` setting a common axis to the output `~ndcube.NDCubeSequence`.  The output sequence should have no common axis. (`#358 <https://github.com/sunpy/ndcube/pull/358>`__)
 - Enable 2-D NDCubes to be visualized as a 1-D animated line. (`#381 <https://github.com/sunpy/ndcube/pull/381>`__)
-- Ensure corner inputs to `ndcube.NDCube.crop` are converted to units stored in WCS as `~astropy.wcs.WCS.world_to_array_index_values` does not handle units. (`#382 <https://github.com/sunpy/ndcube/pull/382>`__)
-- updated ndcube github repository link in `ndcube.docs.installation.rst`. (`#392 <https://github.com/sunpy/ndcube/pull/392>`__)
+- Ensure corner inputs to :meth:`ndcube.NDCube.crop` are converted to units stored in WCS as `~astropy.wcs.WCS.world_to_array_index_values` does not handle units. (`#382 <https://github.com/sunpy/ndcube/pull/382>`__)
+- updated ndcube github repository link in "ndcube.docs.installation.rst". (`#392 <https://github.com/sunpy/ndcube/pull/392>`__)
 - Fix bug in NDCube.axis_world_coords_values when axes_coords is initially a
   bare astropy coordinate object rather than a list/tuple of coordinate objects. (`#400 <https://github.com/sunpy/ndcube/pull/400>`__)
 - Change the implementation of `.NDCube.crop` so that it takes into account all
   the corners of the world region specified by the upper and lower corners, not
   just those two points. (`#438 <https://github.com/sunpy/ndcube/pull/438>`__)
-- Ensure `NDCube` init forces WCS to become high level.
+- Ensure `~ndcube.NDCube` init forces WCS to become high level.
 
   This patches a bug in astropy. (`#447 <https://github.com/sunpy/ndcube/pull/447>`__)
 - Fix bug in `~ndcube.NDCube.axis_world_coords_values` which caused the units to be stripped when an ``axes`` input was given. (`#461 <https://github.com/sunpy/ndcube/pull/461>`__)
 - Fix bug in `~ndcube.utils.wcs.get_dependent_world_axes` where an erroneous matrix transpose caused an error for non-square axis correlation matrices and wrong results for diagonally non-symmetric ones. (`#471 <https://github.com/sunpy/ndcube/pull/471>`__)
-- Extend support for cropping an `~ndcube.NDCube` using an `~ndcube.extra_coords.ExtraCoords` instance as the wcs. (`#472 <https://github.com/sunpy/ndcube/pull/472>`__)
-- Fix check as to whether user inputs to `ndcube.wcs.wrappers.CompoundLowLevelWCS.world_to_pixel_values` result in consistent pixel values when world dimensions share pixel dimensions.  Previously this check was unreliable when non-trivial mapping between world and pixel dimensions was used. (`#472 <https://github.com/sunpy/ndcube/pull/472>`__)
+- Extend support for cropping an `~ndcube.NDCube` using an `~ndcube.ExtraCoords` instance as the wcs. (`#472 <https://github.com/sunpy/ndcube/pull/472>`__)
+- Fix check as to whether user inputs to `ndcube.wcs.wrappers.compound_wcs.CompoundLowLevelWCS.world_to_pixel_values` result in consistent pixel values when world dimensions share pixel dimensions.  Previously this check was unreliable when non-trivial mapping between world and pixel dimensions was used. (`#472 <https://github.com/sunpy/ndcube/pull/472>`__)
 - Fix slicing `~ndcube.ExtraCoords` made of lookup tables. This bug meant that mapping of coords to arrays axes was not adjusted when an axis was dropped. (`#482 <https://github.com/sunpy/ndcube/pull/482>`__)
 
 
 Improved Documentation
 ----------------------
 
-- Document accepted input to ``lookup_table`` in `.ExtraCoords` setting its ``physical_types``. (`#451 <https://github.com/sunpy/ndcube/pull/451>`__)
+- Document accepted input to ``lookup_table`` in `~ndcube.ExtraCoords` setting its ``physical_types``. (`#451 <https://github.com/sunpy/ndcube/pull/451>`__)
 - Improved information and formatting of ``__str__`` methods. (`#453 <https://github.com/sunpy/ndcube/pull/453>`__)
 
 
 Trivial/Internal Changes
 ------------------------
 
 - Simplify and speed up implementation of NDCubeSequence slicing. (`#251 <https://github.com/sunpy/ndcube/pull/251>`__)
 - Fix docstring formatting to help docs build. (`#262 <https://github.com/sunpy/ndcube/pull/262>`__)
 - Use pytest-mpl for figure tests. (`#312 <https://github.com/sunpy/ndcube/pull/312>`__)
 - Port the tests for NDCube to use pytest fixtures (`#318 <https://github.com/sunpy/ndcube/pull/318>`__)
-- Allow corner inputs to `~ndcube.NDCube.crop` to not be wrapped in a `tuple` is only one high level coordinate objects required. (`#380 <https://github.com/sunpy/ndcube/pull/380>`__)
+- Allow corner inputs to :meth:`~ndcube.NDCube.crop` to not be wrapped in a `tuple` is only one high level coordinate objects required. (`#380 <https://github.com/sunpy/ndcube/pull/380>`__)
 - Make sunpy an optional dependence. Without it, the _animate_cube plotting
   functionality will be disabled. (`#393 <https://github.com/sunpy/ndcube/pull/393>`__)
 - Adds a function to compare the physical types of two WCS objects. (`#433 <https://github.com/sunpy/ndcube/pull/433>`__)
-- Propagate reference to NDCube object through `~ndcube.extra_coords.ExtraCoords` string slicing. (`#454 <https://github.com/sunpy/ndcube/pull/454>`__)
+- Propagate reference to NDCube object through `~ndcube.ExtraCoords` string slicing. (`#454 <https://github.com/sunpy/ndcube/pull/454>`__)
 - Adds a function to identify invariant axes between two WCS objects. (`#459 <https://github.com/sunpy/ndcube/pull/459>`__)
 - The matplotlib animators code has been moved from `sunpy` to a new package
-  `mpl_animators` so ndcube no longer has an optional dependancy on sunpy. (`#484 <https://github.com/sunpy/ndcube/pull/484>`__)
+  `mpl_animators` so ndcube no longer has an optional dependency on sunpy. (`#484 <https://github.com/sunpy/ndcube/pull/484>`__)
 
 
 1.3.0 (2020-03-27)
 ==================
 
 Features
 --------
@@ -249,22 +270,22 @@
 1.2.0 (2019-09-10)
 ==================
 
 Features
 --------
 
 - Changed all instances of "missing_axis" to "missing_axes" (`#157 <https://github.com/sunpy/ndcube/pull/157>`__)
-- Added a feature to get the pixel_edges from `ndcube.NDCube.axis_world_coords` (`#174 <https://github.com/sunpy/ndcube/pull/174>`__)
+- Added a feature to get the pixel_edges from :meth:`ndcube.NDCube.axis_world_coords` (`#174 <https://github.com/sunpy/ndcube/pull/174>`__)
 
 
 Bug Fixes
 ---------
 
-- `ndcube.NDCube.world_axis_physical_types` now sets the axis label to the WCS CTYPE if no corresponding IVOA name can be found. (`#164 <https://github.com/sunpy/ndcube/pull/164>`__)
-- Fixed the bug of using `pixel_edges` instead of `pixel_values` in plotting (`#176 <https://github.com/sunpy/ndcube/pull/176>`__)
+- `ndcube.NDCube.wcs.world_axis_physical_types <astropy.wcs.wcsapi.BaseWCSWrapper>` now sets the axis label to the WCS CTYPE if no corresponding IVOA name can be found. (`#164 <https://github.com/sunpy/ndcube/pull/164>`__)
+- Fixed the bug of using ``pixel_edges`` instead of ``pixel_values`` in plotting (`#176 <https://github.com/sunpy/ndcube/pull/176>`__)
 - Fix 2D plotting from crashing when both data and WCS are 2D. (`#182 <https://github.com/sunpy/ndcube/pull/182>`__)
 - Fix the ability to pass a custom Axes to `ndcube.NDCube.plot` for a 2D cube. (`#204 <https://github.com/sunpy/ndcube/pull/204>`__)
 
 
 Trivial/Internal Changes
 ------------------------
 
@@ -272,35 +293,35 @@
 
 
 1.1
 ===
 
 API-Breaking Changes
 --------------------
-- `~ndcube.NDCubeBase.crop_by_extra_coord` API has been broken and
+- ``~ndcube.NDCubeBase.crop_by_extra_coord`` API has been broken and
   replaced.
   Old version:
   ``crop_by_extra_coord(min_coord_value, interval_width, coord_name)``.
   New version:
   ``crop_by_extra_coord(coord_name, min_coord_value,  max_coord_value)``.
   [#142]
 
 New Features
 ------------
 - Created a new `~ndcube.NDCubeBase` which has all the functionality
-  of `~ncube.NDCube` except the plotting.  The old ``NDCubeBase``
-  which outlined the ``NDCube`` API was renamed ``NDCubeABC``.
-  `~ndcube.NDCube` has all the same functionality as before except is
-  now simply inherits from `~ndcube.NDCubeBase` and
-  `~ndcube.mixins.plotting.NDCubePlotMixin`. [#101]
+  of `~ndcube.NDCube` except the plotting.  The old ``NDCubeBase``
+  which outlined the `ndcube.NDCube` API was renamed ``NDCubeABC``.
+  ``~ndcube.NDCube`` has all the same functionality as before except is
+  now simply inherits from ``~ndcube.NDCubeBase`` and
+  ``~ndcube.mixins.plotting.NDCubePlotMixin``. [#101]
 - Moved NDCubSequence plotting to a new mixin class,
   NDCubSequencePlotMixin, making the plotting an optional extra.  All
   the non-plotting functionality now lives in the NDCubeSequenceBase
   class. [#98]
-- Created a new `~ndcube.NDCubeBase.explode_along_axis` method that
+- Created a new ``~ndcube.NDCubeBase.explode_along_axis`` method that
   breaks an NDCube out into an NDCubeSequence along a chosen axis.  It
   is equivalent to
   `~ndcube.NDCubeSequenceBase.explode_along_axis`. [#118]
 - NDCubeSequence plot mixin can now animate a cube as a 1-D line if a single
   axis number is supplied to plot_axis_indices kwarg.
 
 API Changes
@@ -320,17 +341,17 @@
 
 Bug Fixes
 ---------
 - Allowed `~ndcube.NDCubeBase.axis_world_coords` to accept negative
   axis indices as arguments. [#106]
 - Fixed bug in ``NDCube.crop_by_coords`` in case where real world
   coordinate system was rotated relative to pixel grid. [#113].
-- `~ndcube.NDCubeBase.world_axis_physical_types` is now not
+- ``~ndcube.NDCubeBase.world_axis_physical_types`` is now not
   case-sensitive to the CTYPE values in the WCS. [#109]
-- `~ndcube.NDCubeBase.plot` now generates a 1-D line animation when
+- ``~ndcube.NDCubeBase.plot`` now generates a 1-D line animation when
   image_axis is an integer.
 
 
 1.0.1
 =====
 
 New Features
```

### Comparing `ndcube-2.1.1/LICENSE.rst` & `ndcube-2.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/PKG-INFO` & `ndcube-2.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ndcube
-Version: 2.1.1
-Summary: A package for multi-dimensional contiguious and non-contiguious coordinate aware arrays.
+Version: 2.1.2
+Summary: A package for multi-dimensional contiguous and non-contiguous coordinate aware arrays.
 Home-page: https://docs.sunpy.org/projects/ndcube/
 Download-URL: https://pypi.org/project/ndcube/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/ndcube/
 Project-URL: Documentation, https://docs.sunpy.org/projects/ndcube/
@@ -42,15 +42,15 @@
 
 |Latest Version| |codecov| |matrix| |Powered by NumFOCUS| |Powered by SunPy|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/ndcube.svg
    :target: https://pypi.python.org/pypi/ndcube/
    :alt: It is up to date, we promise
 .. |matrix| image:: https://img.shields.io/matrix/ndcube:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=openastronomy.modular.im
-   :target: https://openastronomy.element.io/#/room/#ndcube:openastronomy.org
+   :target: https://app.element.io/#/room/#ndcube:openastronomy.org
    :alt: join us on #ndcube:openastronom.org on matrix
 .. |codecov| image:: https://codecov.io/gh/sunpy/ndcube/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
    :alt: Best code cov this side of mars
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
    :alt: Go give them money
```

### Comparing `ndcube-2.1.1/README.rst` & `ndcube-2.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 |Latest Version| |codecov| |matrix| |Powered by NumFOCUS| |Powered by SunPy|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/ndcube.svg
    :target: https://pypi.python.org/pypi/ndcube/
    :alt: It is up to date, we promise
 .. |matrix| image:: https://img.shields.io/matrix/ndcube:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=openastronomy.modular.im
-   :target: https://openastronomy.element.io/#/room/#ndcube:openastronomy.org
+   :target: https://app.element.io/#/room/#ndcube:openastronomy.org
    :alt: join us on #ndcube:openastronom.org on matrix
 .. |codecov| image:: https://codecov.io/gh/sunpy/ndcube/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
    :alt: Best code cov this side of mars
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
    :alt: Go give them money
```

### Comparing `ndcube-2.1.1/RELEASE.rst` & `ndcube-2.1.2/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/Makefile` & `ndcube-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/conf.py` & `ndcube-2.1.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 source_suffix = '.rst'
 master_doc = 'index'
 default_role = 'obj'
 napoleon_use_rtype = False
 napoleon_google_docstring = False
 napoleon_use_param = False
 # TODO: Enable this in future.
-nitpicky = False
+nitpicky = True
 # This is not used. See docs/nitpick-exceptions file for the actual listing.
 nitpick_ignore = []
 for line in open('nitpick-exceptions'):
     if line.strip() == "" or line.startswith("#"):
         continue
     dtype, target = line.split(None, 1)
     target = target.strip()
@@ -85,15 +85,16 @@
               (None, 'http://data.astropy.org/intersphinx/numpy.inv')),
     'matplotlib': ('https://matplotlib.org/',
                    (None, 'http://data.astropy.org/intersphinx/matplotlib.inv')),
     'astropy': ('http://docs.astropy.org/en/stable/', None),
     'sunpy': ('https://docs.sunpy.org/en/stable/', None),
     'mpl_animators': ('https://docs.sunpy.org/projects/mpl-animators/en/stable/', None),
     'gwcs': ('https://gwcs.readthedocs.io/en/stable/', None),
-    'reproject': ("https://reproject.readthedocs.io/en/stable/", None)}
+    'reproject': ("https://reproject.readthedocs.io/en/stable/", None)
+    }
 
 # -- Options for HTML output
 from sunpy_sphinx_theme.conf import *  # NOQA
 
 html_logo = png_icon = 'logo/ndcube.png'
 html_favicon = 'logo/favicon.png'
 graphviz_output_format = 'svg'
```

### Comparing `ndcube-2.1.1/docs/coordinates.rst` & `ndcube-2.1.2/docs/explaining_ndcube/coordinates.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 .. _coordinates:
 
-==========================
-Coordinate Transformations
-==========================
+**************************
+Coordinate transformations
+**************************
 
 Introduction to WCS
 ===================
 
-To describe the mapping between array elements/pixels and real world coordinates, ndcube heavily leverages the World Coordinate System (WCS) framework, specifically the tools written by Astropy that implement this framework in Python.
+To describe the mapping between array elements/pixels and real world coordinates, `ndcube` heavily leverages the World Coordinate System (WCS) framework, specifically the tools written by Astropy that implement this framework in Python.
 WCS allows a wide variety of projections, rotations and transformations be stored and executed.
 Because it allows coordinates transformations to be stored functionally, rather than in memory-heavy lookup tables, and because it caters for both astronomy-specific coordinate systems (e.g. RA & Dec.) as well as simpler, more common ones (e.g. wavelength), WCS has become the most common coordinate transformation framework in astronomy.
 
 The most commonly used WCS implementation in Python is the `astropy.wcs.WCS` object, which stores critical information describing the coordinate transformations as required by the FITS data model (e.g. the reference pixel and its corresponding coordinate values, ``CRPIX`` and ``CRVAL``, and the projection type, ``CTYPE`` etc.).
 It also executes these transformations via methods like `~astropy.wcs.WCS.world_to_pixel` and `~astropy.wcs.WCS.pixel_to_world` which convert between pixel indices and world coordinate values.
 However, these methods are independent of the data array and the `~astropy.wcs.WCS` object carries little or no information about the data itself.
-That is why the ndcube package is needed.
+That is why the `ndcube` package is needed.
 
-Nonetheless, astropy's WCS implementation is a crucial pillar of ndcube, as is the more generalized offshoot, `gWCS <https://gwcs.readthedocs.io/en/stable/>`__, which provides greater generalization outside of the FITS data model.
-Crucially though for ndcube, both implementations adhere to the `Astropy WCS API <https://docs.astropy.org/en/stable/wcs/wcsapi.html>`__.
+Nonetheless, astropy's WCS implementation is a crucial pillar of `ndcube`, as is the more generalized offshoot, `gWCS <https://gwcs.readthedocs.io/en/stable/>`__, which provides greater generalization outside of the FITS data model.
+Crucially though for `ndcube`, both implementations adhere to the `Astropy WCS API <https://docs.astropy.org/en/stable/wcs/wcsapi.html>`__.
 A familiarity with WCS and the Astropy and gWCS Python implementations will be helpful (although hopefully not essential) in understanding this guide.
 We therefore encourage users to read `Astropy's WCS guide <https://docs.astropy.org/en/stable/wcs/>`__ and the `gWCS documentation <https://gwcs.readthedocs.io/en/stable/>`__ to learn more.
 
-In this section we will discuss the features ndcube has built upon these implementations to support the integration of data and coordinates.
+In this section we will discuss the features `ndcube` has built upon these implementations to support the integration of data and coordinates.
+
+.. _cube_coordinates:
 
-NDCube Coordinates
+NDCube coordinates
 ==================
 
 Although WCS objects are a powerful and concise way of storing complex functional coordinate transformations, their API can be cumbersome when the coordinates along a whole axis are desired.
-Making this process easy and intuitive is the purpose of the `ndcube.NDCube.axis_world_coords` method.
+Making this process easy and intuitive is the purpose of the :meth:`ndcube.NDCube.axis_world_coords` method.
 Using the attached WCS object, information on the data dimensions, and optional inputs from the user, this method returns high level coordinate objects --- e.g. `~astropy.coordinates.SkyCoord`, `~astropy.time.Time`, `~astropy.coordinates.SpectralCoord`, `~astropy.units.Quantity` --- containing the coordinates for each array element.
 Say we have a 3-D `~ndcube.NDCube` with a shape of ``(4, 4, 5)`` and physical types of space, space, wavelength.
 Now let's say we want the wavelength values along the spectral axis.
 We can do this in a couple ways.
-First we can provide `~ndcube.NDCube.axis_world_coords` with the array axis number of the spectral axis.
+First we can provide :meth:`~ndcube.NDCube.axis_world_coords` with the array axis number of the spectral axis.
 
 .. expanding-code-block:: python
   :summary: Click to reveal/hide instantiation of the NDCube.
 
   >>> import astropy.wcs
   >>> import numpy as np
 
@@ -57,26 +59,26 @@
   >>> my_cube = NDCube(data, wcs=wcs)
 
 .. code-block:: python
 
   >>> my_cube.axis_world_coords(2)
   (<SpectralCoord [1.02e-09, 1.04e-09, 1.06e-09, 1.08e-09, 1.10e-09] m>,)
 
-Alternatively we can provide a unique substring of the physical type of the coordinate, stored in `ndcube.NDCube.wcs.world_axis_physical_types`:
+Alternatively we can provide a unique substring of the physical type of the coordinate, stored in `ndcube.NDCube.wcs.world_axis_physical_types <astropy.wcs.wcsapi.BaseWCSWrapper>`:
 
 .. code-block:: python
 
   >>> my_cube.wcs.world_axis_physical_types
   ['em.wl', 'custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon']
   >>> # Since 'wl' is unique to the wavelength axis name, let's use that.
   >>> my_cube.axis_world_coords('wl')
   (<SpectralCoord [1.02e-09, 1.04e-09, 1.06e-09, 1.08e-09, 1.10e-09] m>,)
 
 As discussed above, some WCS axes are not independent.
-For those axes, `~ndcube.NDCube.axis_world_coords` returns objects with the same number of dimensions as dependent axes.
+For those axes, :meth:`~ndcube.NDCube.axis_world_coords` returns objects with the same number of dimensions as dependent axes.
 For example, helioprojective longitude and latitude are dependent.
 Therefore if we ask for longitude, we will get back a `~astropy.coordinates.SkyCoord` containing 2-D latitude and longitude arrays with the same shape as the array axes to which they correspond.
 For example:
 
 .. code-block:: python
 
   >>> celestial = my_cube.axis_world_coords('lon')[0]  # Must extract object from returned tuple with [0]
@@ -107,31 +109,31 @@
        [(3600.        , 4.56905253e-02), (3600.        , 1.80000000e+03),
         (3600.        , 3.59995431e+03), (3600.        , 5.39963453e+03)],
        [(5039.92178073, 4.56894119e-02), (5040.03143627, 1.79995614e+03),
         (5040.14110851, 3.59986658e+03), (5040.25079745, 5.39950295e+03)],
        [(6479.70323031, 4.56860725e-02), (6479.92250932, 1.79982456e+03),
         (6480.14182173, 3.59960344e+03), (6480.36116753, 5.39910830e+03)]]>)
 
-If the user wants the world coordinates for all the axes, the ``axes`` arg can set to ``None`` or simply omitted.
+If the user wants the world coordinates for all the axes, the ``axes`` arg can set to `None` or simply omitted.
 
 .. code-block:: python
 
   >>> my_cube.axis_world_coords()
   (<SpectralCoord [1.02e-09, 1.04e-09, 1.06e-09, 1.08e-09, 1.10e-09] m>, <SkyCoord (Helioprojective: obstime=None, rsun=695700.0 km, observer=None): (Tx, Ty) in arcsec
       [[(2160.07821927, 4.56894119e-02), (2159.96856373, 1.79995614e+03),
         (2159.85889149, 3.59986658e+03), (2159.74920255, 5.39950295e+03)],
        [(3600.        , 4.56905253e-02), (3600.        , 1.80000000e+03),
         (3600.        , 3.59995431e+03), (3600.        , 5.39963453e+03)],
        [(5039.92178073, 4.56894119e-02), (5040.03143627, 1.79995614e+03),
         (5040.14110851, 3.59986658e+03), (5040.25079745, 5.39950295e+03)],
        [(6479.70323031, 4.56860725e-02), (6479.92250932, 1.79982456e+03),
         (6480.14182173, 3.59960344e+03), (6480.36116753, 5.39910830e+03)]]>)
 
-By default `~ndcube.NDCube.axis_world_coords` returns the coordinates at the center of each pixel.
-However, the coordinates at the edges of each pixel can be obtained by setting the ``pixel_corners`` kwarg to ``True``.
+By default :meth:`~ndcube.NDCube.axis_world_coords` returns the coordinates at the center of each pixel.
+However, the coordinates at the edges of each pixel can be obtained by setting the ``pixel_corners`` keyword argument to `True`.
 For example:
 
 .. code-block:: python
 
   >>> my_cube.axis_world_coords(pixel_corners=True)
   (<SpectralCoord [1.01e-09, 1.03e-09, 1.05e-09, 1.07e-09, 1.09e-09, 1.11e-09] m>, <SkyCoord (Helioprojective: obstime=None, rsun=695700.0 km, observer=None): (Tx, Ty) in arcsec
       [[(1440.24341188, -899.79647591), (1440.07895112,  899.95636786),
@@ -146,19 +148,19 @@
        [(5759.75658812, -899.79647591), (5759.92104888,  899.95636786),
         (5760.08553469, 2699.84625127), (5760.25004555, 4499.59909505),
         (5760.41458147, 6298.94094507)],
        [(7199.36047891, -899.70880283), (7199.63452676,  899.86866585),
         (7199.90861634, 2699.58313412), (7200.18274766, 4499.1606028 ),
         (7200.45692072, 6298.32719784)]]>)
 
-Working with Raw Coordinates
+Working with raw coordinates
 ----------------------------
 
 If users would prefer not to deal with high level coordinate objects, they can elect to use `ndcube.NDCube.axis_world_coords_values`.
-The API for this method is the same as `~ndcube.NDCube.axis_world_coords`.
+The API for this method is the same as :meth:`~ndcube.NDCube.axis_world_coords`.
 The only difference is that a `~collections.namedtuple` of `~astropy.units.Quantity` objects are returned, one for each physical type requested.
 In the above case this means that there would be separate `~astropy.units.Quantity` objects for latitude and longitude, but they would both have the same 2-D shape.
 The `~astropy.units.Quantity` objects are returned in world order and correspond to the physical types in the `astropy.wcs.WCS.world_axis_physical_types`.
 The `~astropy.units.Quantity` objects do not contain important contextual information, such as reference frame, which is needed to fully interpret the coordinate values.
 However for some use cases this level of completeness is not needed.
 
 .. code-block:: python
@@ -184,15 +186,15 @@
 So far we have seen how `~ndcube.NDCube` uses its WCS object (``NDCube.wcs``) to store and perform coordinates transformations.
 But what if we have alternative or additional coordinates that are not represented by the WCS?
 For example, say we have a raster scan from a scanning slit spectrograph whose x-axis is folded in with time.
 This occurs because the x-axis is built up over sequential exposures taken at different slit positions.
 
 Our ``NDCube.wcs`` might describe latitude and longitude, but omit time.
 So how can we represent time without having to construct a whole new custom WCS object?
-One way is to use the `ndcube.ExtraCoords` class located at ``NDCube.extra_coords``.
+One way is to use the `ndcube.ExtraCoords` class located at `ndcube.NDCube.extra_coords`.
 It provides a mechanism of attaching coordinates to `~ndcube.NDCube` instances in addition to those in the primary WCS object.
 This may be desired because, as above, the primary WCS omits a physical type.
 Or it may be that the users have an alternative set of coordinates to the primary set at ``.wcs``.
 To demonstrate how to use `~ndcube.ExtraCoords`, let's start by creating a `~astropy.time.Time` object representing the time at each location along the first axis of ``my_cube``.
 
 .. code-block:: python
 
@@ -221,15 +223,15 @@
 The physical types of extra coordinates are also returned by `~ndcube.NDCube.array_axis_physical_types`.
 
 .. code-block:: python
 
   >>> my_cube.array_axis_physical_types
   [('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon', 'time'), ('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon'), ('em.wl',)]
 
-The values of the extra coordinates at each array index can be retrieved using and combination of `ndcube.NDCube.axis_world_coords` and `ndcube.NDCube.combined_wcs`.
+The values of the extra coordinates at each array index can be retrieved using and combination of :meth:`ndcube.NDCube.axis_world_coords` and `ndcube.NDCube.combined_wcs`.
 See :ref:`combined_wcs` below.
 
 .. _combined_wcs:
 
 Combined WCS
 ------------
 
@@ -299,52 +301,48 @@
   ['distance']
   >>> list(my_cube.global_coords.values())  # Returns a list of coordinate values
   [<Quantity 1. m>]
   >>> list(my_cube.global_coords.items())  # Returns a list of (name, value) pairs
   [('distance', <Quantity 1. m>)]
 
 A common use case for `~ndcube.GlobalCoords` is associated with slicing (:ref:`cube_slicing`).
-In addition to tracking and updating the `~ndcube.NDCube.wcs` and `~ndcube.NDCube.extra_coords` objects, `~ndcube.NDCube`'s slicing infrastucture also identifies when the array axes to which a coordinate corresponds are dropped.
+In addition to tracking and updating the `~ndcube.NDCube.wcs` and `~ndcube.NDCube.extra_coords` objects, `~ndcube.NDCube`'s slicing infrastructure also identifies when the array axes to which a coordinate corresponds are dropped.
 The values of dropped coordinates at the position where the `~ndcube.NDCube` was sliced are stored in the `astropy.wcs.WCS` instance from where `~ndcube.GlobalCoords` can access and return them.
 
 .. code-block:: python
 
   >>> my_2d_cube = my_cube[:, :, 0]
   >>> my_2d_cube.array_axis_physical_types  # Note the wavelength axis is now gone.
   [('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon', 'time'),
    ('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon')]
 
   >>> # The wavelength value at the slicing location is now in the GLobalCoords object.
-  >>> list(my_2d_cube.global_coords.keys())  # doctest: +SKIP
-  ['distance', 'em.wl']  # doctest: +SKIP
-  >>> my_2d_cube.global_coords.physical_types['em.wl']  # doctest: +SKIP
-  'em.wl'  # doctest: +SKIP
-  >>> my_2d_cube.global_coords['em.wl']  # doctest: +SKIP
+  >>> list(my_2d_cube.global_coords.keys())
+  ['distance', 'em.wl']
+  >>> my_2d_cube.global_coords.physical_types['em.wl']
+  'em.wl'
+  >>> my_2d_cube.global_coords['em.wl']
   <SpectralCoord 1e-9 m>
 
-.. _cube_coordinates:
-
-
 .. _sequence_coordinates:
 
-NDCubeSequence Coordinates
+NDCubeSequence coordinates
 ==========================
 
-Sequence Axis Coordinates
+Sequence axis coordinates
 -------------------------
 
 As described in the :ref:`ndcubesequence` section, the sequence axis can be thought of as an additional array axis perpendicular to those of the cubes within an `~ndcube.NDCubeSequence`.
 In that model, the `~ndcube.GlobalCoords` on each `~ndcube.NDCube` represent coordinate values along the sequence axis.
 The `ndcube.NDCubeSequence.sequence_axis_coords` property collates a list for each global coordinate with each element giving the coordinate value from the corresponding `~ndcube.NDCube`.
 These lists are returned as a `dict` with the keys being the coordinate names.
-To demonstrate this, let's call `ndcube.NDCube.sequence_axis_coords` on an `~ndcube.NDCubeSequence` whose cubes have `~ndcube.GlobalCoords`.
-(Click the "Instantiating NDCubeSequence" link below to reveal the code used to create the `~ndcube.NDCubeSequence`.)
+To demonstrate this, let's call `ndcube.NDCubeSequence.sequence_axis_coords` on an `~ndcube.NDCubeSequence` whose cubes have `~ndcube.GlobalCoords`.
 
 .. expanding-code-block:: python
-  :summary: Instantiating NDCubeSequence
+  :summary: Click the here to reveal the code used to create the NDCubeSequence.
 
   >>> import astropy.units as u
   >>> import astropy.wcs
   >>> import numpy as np
   >>> from ndcube import NDCube, NDCubeSequence
 
   >>> # Define data arrays.
@@ -384,15 +382,15 @@
 .. code-block:: python
 
   >>> my_sequence.sequence_axis_coords.keys()
   dict_keys(['distance'])
   >>> my_sequence.sequence_axis_coords['distance']
   [<Quantity 1. m>, <Quantity 2. m>, <Quantity 3. m>, <Quantity 4. m>]
 
-Common Axis Coordinates
+Common axis coordinates
 -----------------------
 
 The :ref:`ndcubesequence` section also explains how a common axis can be defined for a `~ndcube.NDCubeSequence`, signifying that the sequence axis is parallel to one of the `~ndcube.NDCube` array axes.
 Take the example of an `~ndcube.NDCubeSequence` of four 3-D NDCubes with axes of space-space-wavelength.
 Suppose that each cube represents a different interval in the spectral dimension and that the cubes are arranged in ascending wavelength order within the `~ndcube.NDCubeSequence`, i.e. ``common_axis=2``.
 If each NDCube has a shape of ``(4, 4, 5)``, then there are 20 positions along the common axis (5 array elements x 4 NDCubes).
```

### Comparing `ndcube-2.1.1/docs/data_classes.rst` & `ndcube-2.1.2/docs/explaining_ndcube/data_classes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 .. _data_classes:
 
-==========
-ND Objects
-==========
+**********
+ND objects
+**********
 
-ndcube provides its features via its data objects: `~ndcube.NDCube`, `~ndcube.NDCubeSequence` and `~ndcube.NDCollection`.
+`ndcube` provides its features via its data objects: `~ndcube.NDCube`, `~ndcube.NDCubeSequence` and `~ndcube.NDCollection`.
 This section describes the purpose of each and how they are structured and instantiated.
 To learn how to slice, visualize, and perform coordinate transformations with these classes, see the :ref:`slicing`, :ref:`plotting` and :ref:`coordinates` sections.
 
 .. _ndcube:
 
 NDCube
 ======
 
-`~ndcube.NDCube` is the primary data class the ndcube package.
-It's designed to manage a single data array and set of WCS transformations.
+`~ndcube.NDCube` is the primary data class the ndcube package provides.
+It is designed to manage a single data array and set of WCS transformations.
 `~ndcube.NDCube` provides unified slicing, visualization, coordinate transformation and self-inspection APIs which are independent of the number and physical types of axes.
 It can therefore be used for any type of data (e.g. images, spectra, timeseries, etc.) so long as those data are represented by an object that behaves like a `numpy.ndarray` and the coordinates by an object that adheres to the Astropy `WCS API <https://docs.astropy.org/en/stable/wcs/wcsapi.html>`__.
 This makes `~ndcube.NDCube` a powerful base class when developing tools for specific data types.
 
 Thanks to its inheritance from `astropy.nddata.NDData`, `~ndcube.NDCube` can hold optional supplementary data in addition to its data array and primary WCS transformations.
 These include:
-1. general metadata (located at ``.meta``);
-2. the unit of the data (an `astropy.units.Unit` or unit `str` located at ``.unit``);
-3. the uncertainty of each data value (subclass of `astropy.nddata.NDUncertainty` located at ``.uncertainty``); and a mask marking unreliable data values (boolean array located at ``.mask``). Note that in keeping with the convention of `numpy.ma.masked_array`, ``True`` means that the corresponding data value is masked, i.e. it is bad data, while ``False`` signifies good data.
+
+1. general metadata (located at ``.meta``)
+2. the unit of the data (an `astropy.units.Unit` or unit `str` located at ``.unit``)
+3. the uncertainty of each data value (subclass of `astropy.nddata.NDUncertainty` located at ``.uncertainty``)
+4. a mask marking unreliable data values (boolean array located at ``.mask``).
+   Note that in keeping with the convention of `numpy.ma.masked_array`, `True` means that the corresponding data value is masked, i.e., it is bad data, while `False` signifies good data.
 
 `~ndcube.NDCube` also provides classes for representing additional coordinates not included in the primary WCS object.
 These are `~ndcube.ExtraCoords` (located at ``.extra_coords``) --- for additional coordinates associated with specific array axes --- and `~ndcube.GlobalCoords` (located at ``.global_coords``) for scalar coordinates associated with the `~ndcube.NDCube` as a whole.
 These are discussed in the section in this guide on :ref:`coordinates`.
 
 The figure below shows a schematic of an `~ndcube.NDCube` instance and the relationships between its components.
 Array-based components are in blue (``.data``, ``.uncertainty``, and ``.mask``), metadata components in green (``.meta`` and ``.unit``), and coordinate components in red (``.wcs``, ``.extra_coords``, and ``.global_coords``).
@@ -65,15 +68,15 @@
 
   >>> # Now instantiate the NDCube
   >>> my_cube = NDCube(data, wcs=wcs)
 
 The data array is stored in ``my_cube.data`` while the WCS object is stored in ``my_cube.wcs``.
 The ``.data`` attribute should only be used to access specific raw data values.
 When manipulating/slicing the data it is better to slice the `~ndcube.NDCube` instance as a whole so as to ensure that supporting data --- e.g. coordinates, uncertainties, mask --- remain consistent.
-(See :ref:`cube_slicing`.)
+See :ref:`cube_slicing` for more information.
 
 To instantiate a more complex `~ndcube.NDCube` with metadata, a data unit, uncertainties and a mask, we can do the following:
 
 .. code-block:: python
 
   >>> import astropy.units as u
   >>> import astropy.wcs
@@ -90,26 +93,26 @@
   >>> wcs.wcs.ctype = 'WAVE', 'HPLT-TAN', 'HPLN-TAN'
   >>> wcs.wcs.cunit = 'Angstrom', 'deg', 'deg'
   >>> wcs.wcs.cdelt = 0.2, 0.5, 0.4
   >>> wcs.wcs.crpix = 0, 2, 2
   >>> wcs.wcs.crval = 10, 0.5, 1
   >>> wcs.wcs.cname = 'wavelength', 'HPC lat', 'HPC lon'
 
-  >>> # Define mask.  Initially set all elements unmasked.
+  >>> # Define mask. Initially set all elements unmasked.
   >>> mask = np.zeros_like(data, dtype=bool)
   >>> mask[0, 0][:] = True  # Now mask some values.
   >>> # Define uncertainty, metadata and unit.
   >>> uncertainty = StdDevUncertainty(np.sqrt(np.abs(data)))
   >>> meta = {"Description": "This is example NDCube metadata."}
   >>> unit = u.ct
 
   >>> # Instantiate NDCube with supporting data.
   >>> my_cube = NDCube(data, wcs=wcs, uncertainty=uncertainty, mask=mask, meta=meta, unit=unit)
 
-Attaching coordinates in addition to those described by ``NDCube.wcs`` via `~ndcube.ExtraCoords` and `~ndcube.GlobalCoords` is discussed in the :ref:`extra_coords` and :ref:`global_coords` sections.
+Attaching coordinates in addition to those described by ``.wcs`` via `~ndcube.ExtraCoords` and `~ndcube.GlobalCoords` is discussed in the :ref:`extra_coords` and :ref:`global_coords` sections.
 
 Dimensions and Physical Types
 -----------------------------
 
 `~ndcube.NDCube` has useful properties for inspecting its axes: `~ndcube.NDCube.dimensions` and `~ndcube.NDCube.array_axis_physical_types`.
 
 .. code-block:: python
@@ -126,42 +129,42 @@
 The tuples are arranged in array axis order, while the physical types inside each tuple are returned in world order.
 As more than one physical type can be associated with an array axis, the length of each tuple can be greater than 1.
 This is the case for the 1st and 2nd array array axes which are associated with the coupled world axes of helioprojective latitude and longitude.
 The axis names are in generated in accordance with the International Virtual Observatory Alliance (IVOA) `UCD1+ controlled vocabulary <http://www.ivoa.net/documents/REC/UCD/UCDlist-20070402.html>`__.
 
 .. _explode_cube:
 
-Explode NDCube Along Axis
--------------------------
+Explode NDCube along an axis
+----------------------------
 
-During analysis of some data --- say a of stack of images --- it may be necessary to make some different fine-pointing adjustments to each image that isn't accounted for the in the original WCS translations, e.g. due to satellite wobble.
-If these changes are not describable with a single WCS object, it may be desirable to break up the NDCube along a given axis into a sequence of (N-1)DCubes each with their own WCS.
+During analysis of some data --- say a of stack of images --- it may be necessary to make some different fine-pointing adjustments to each image that isn't accounted for the in the original WCS translations, e.g., due to satellite wobble.
+If these changes are not describable with a single WCS object, it may be desirable to break up the NDCube along a given axis into a sequence of (N-1)D cubes each with their own WCS.
 This would enable each WCS to be altered separately.
 
-This is the purpose of the `ndcube.NDCube.explode_along_axis` method.
+This is the purpose of the :meth:`ndcube.NDCube.explode_along_axis` method.
 To explode ``my_cube`` along the last array axis so that we have 5 2-D images, each at a different wavelength, simply call the `~ndcube.NDCube.explode_along_axis` and supply it with the array axis along which the `~ndcube.NDCube` should be exploded.
 
 .. code-block:: python
 
   >>> exploded = my_cube.explode_along_axis(2)
 
-This returns an `~ndcube.NDCubeSequence` with where the sequence axis acts as the wavelength axis.
+This returns an `~ndcube.NDCubeSequence` where the sequence axis acts as the wavelength axis.
 
 .. code-block:: python
 
   >>> exploded.dimensions
   (<Quantity 5. pix>, <Quantity 4. pix>, <Quantity 4. pix>)
   >>> exploded.array_axis_physical_types
   [('meta.obs.sequence',),
    ('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon'),
    ('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon')]
 
 To learn more about this object, read the :ref:`ndcubesequence` section below.
 
-And Much More!
+And much more!
 --------------
 
 `~ndcube.NDCube` provides many more helpful features, specifically for coordinate transformations, slicing and visualization.
 See the :ref:`cube_coordinates`, :ref:`cube_slicing` and :ref:`cube_plotting` sections to learn more.
 
 .. _ndcubesequence:
 
@@ -207,15 +210,15 @@
 Initializing an NDCubeSequence
 ------------------------------
 
 To initialize the most basic `~ndcube.NDCubeSequence`, all you need is a list of `~ndcube.NDCube` instances.
 Let's say we have four 3-D NDCubes with shapes of ``(4, 4, 5)`` and physical types of helioprojective longitude, latitude and wavelength.
 
 .. expanding-code-block:: python
-  :summary: Click to see NDCubes instantiated for use in the following NDCubeSequence
+  :summary: Click to see NDCubes instantiated for use in the following NDCubeSequence.
 
   >>> import astropy.units as u
   >>> import astropy.wcs
   >>> import numpy as np
   >>> from ndcube import NDCube, NDCubeSequence
 
   >>> # Define data arrays.
@@ -261,15 +264,15 @@
 
 .. code-block:: python
 
   >>> my_sequence = NDCubeSequence([cube0, cube1, cube2, cube3], common_axis=0)
 
 .. _dimensions:
 
-Dimensions and Physical Types
+Dimensions and physical types
 -----------------------------
 
 Analogous to `ndcube.NDCube.dimensions`, there is also a `ndcube.NDCubeSequence.dimensions` property for easily inspecting the shape of an `~ndcube.NDCubeSequence` instance.
 
 .. code-block:: python
 
   >>> my_sequence.dimensions
@@ -302,55 +305,55 @@
   >>> my_sequence.cube_like_array_axis_physical_types
   [('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon'),
    ('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon'),
    ('em.wl',)]
 
 .. _explode_sequence:
 
-Explode Along Axis
-------------------
+Explode along an axis
+---------------------
 
-Just like `~ndcube.NDCube`, `~ndcube.NDCubeSequence` has an `~ndcube.NDCubeSequence.explode_along_axis` method.
+Just like `~ndcube.NDCube`, `~ndcube.NDCubeSequence` has an :meth:`~ndcube.NDCubeSequence.explode_along_axis` method.
 Its purpose and API are exactly the same as `ndcube.NDCube.explode_along_axis` and we refer readers to the (:ref:`explode_cube`) section describing it.
 
 To demonstrate the behavior of `ndcube.NDCubeSequence.explode_along_axis` version of this method, let's consider ``my_sequence`` defined above.
 It contains four `~ndcube.NDCube` instances, each with a shape of ``(4, 4, 5)`` and physical types of helioprojective longitude, latitude and wavelength.
 Let's break up the cubes along the final (wavelength) axis so we have a sequence of 20 2D cubes, each representing a single image with a shape of ``(4, 4)``.
 To do this let's call `~ndcube.NDCube.explode_along_axis` and supply it with the array axis along which the cubes should be exploded.
 Note that the array axis numbers are relative to the NDCubes, not the NDCubeSequence.
 So to explode along the wavelength axis, we should use an array axis index of ``2``.
 
 .. code-block:: python
 
   >>> exploded_sequence = my_sequence.explode_along_axis(2)
 
-  >>> # Check old and new shapes of the squence
+  >>> # Check old and new shapes of the sequence
   >>> my_sequence.dimensions
   (<Quantity 4. pix>, <Quantity 4. pix>, <Quantity 4. pix>, <Quantity 5. pix>)
   >>> exploded_sequence.dimensions
   (<Quantity 20. pix>, <Quantity 4. pix>, <Quantity 4. pix>)
 
 Note that an `~ndcube.NDCubeSequence` can be exploded along any axis.
 A common axis need not be defined and if one is it need not be the axis along which the `~ndcube.NDCubeSequence` is exploded.
 
-And Much More
+And much more
 -------------
 
 `~ndcube.NDCubeSequence` provides many more helpful features, specifically for coordinate transformations, slicing and visualization.
 See the :ref:`sequence_coordinates`, :ref:`sequence_slicing` and :ref:`sequence_plotting` sections to learn more.
 
 .. _ndcollection:
 
 NDCollection
 ============
 
 `~ndcube.NDCollection` is a container class for grouping `~ndcube.NDCube` or `~ndcube.NDCubeSequence` instances in an unordered way.
 `~ndcube.NDCollection` therefore differs from `~ndcube.NDCubeSequence` in that the objects contained are not considered to be in any order, are not assumed to represent measurements of the same physical property, and they can have different dimensionalities.
 However `~ndcube.NDCollection` is more powerful than a simple `dict` because it enables us to identify axes that are aligned between the objects and hence provides some limited slicing functionality.
-(See :ref:`collection_slicing` to for more on slicing.)
+See :ref:`collection_slicing` to for more on slicing.
 
 One possible application of `~ndcube.NDCollection` is linking observations with derived data products.
 Let's say we have a 3-D `~ndcube.NDCube` representing space-space-wavelength.
 Then let's say we fit a spectral line in each pixel's spectrum and extract its linewidth.
 Now we have a 2D spatial map of linewidth with the same spatial axes as the original 3-D cube.
 There is a clear relationship between these two objects and so it makes sense to store them together.
 An `~ndcube.NDCubeSequence` is not appropriate here as the physical properties represented by the two objects is different, they do not have an order within their common coordinate space, and they do not have the same dimensionality.
@@ -390,34 +393,34 @@
   >>> my_collection.keys()
   dict_keys(['observations', 'linewidths'])
 
 Editing NDCollections
 ---------------------
 
 Because `~ndcube.NDCollection` inherits from `dict`, we can edit the collection using many of the same methods.
-These have the same or analogous APIs to the `dict` versions and include `del`, `~ndcube.NDCollection.pop`, and `~ndcube.NDCollection.update`.
+These have the same or analogous APIs to the `dict` versions and include `~ndcube.NDCollection.pop`, and `~ndcube.NDCollection.update`.
 Some `dict` methods may not be implemented on `~ndcube.NDCollection` if they are not consistent with its design.
 
 .. _aligned_axes:
 
-Aligned Axes
+Aligned axes
 ------------
 In the above example, the linewidth object's axes are aligned with the first two axes of the observations object.
 Designating these axes as aligned allows both members of the collection to be simultaneously sliced, thus enabling users to quickly and accurately crop their entire data set to a region of interest.
-(For more on this, see :ref:`collection_slicing`.)
+For more on this, see :ref:`collection_slicing`.
 There are a few ways to designate aligned axes.
 If the members of the collection have the same axis ordering, as is the case in our example, we can provide a single `tuple` of `int`, designating the array axes that are aligned.
-(Note that aligned axes must have the same lengths.)
+Note that aligned axes must have the same lengths.
 
 .. code-block:: python
 
   >>> my_collection = NDCollection([("observations", my_cube), ("linewidths", linewidth_cube)],
   ...                              aligned_axes=(0, 1))
 
-We can see which axes are aligned by inpecting the ``aligned_axes`` attribute:
+We can see which axes are aligned by inspecting the ``aligned_axes`` attribute:
 
 .. code-block:: python
 
   >>> my_collection.aligned_axes
   {'observations': (0, 1), 'linewidths': (0, 1)}
 
 This gives us the array axes for each ND object separately.
```

### Comparing `ndcube-2.1.1/docs/extending_ndcube.rst` & `ndcube-2.1.2/docs/extending_ndcube.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 .. _extending_ndcube:
 
-Extending ndcube in Other Packages
-==================================
+**************************************
+Extending ``ndcube`` in Other Packages
+**************************************
 
-This section is aimed at people developing packages which extend the functionality of ndcube data classes.
+This section is aimed at people developing packages which extend the functionality of ``ndcube`` data classes.
 
-Requiring ndcube in your package
---------------------------------
+Requiring ``ndcube`` in your package
+====================================
 
-ndcube has required dependencies on `astropy`, `gwcs` and `numpy`.
+ndcube has required dependencies on ``astropy``, ``gwcs`` and `numpy`.
 In addition to this it has two sets of optional dependencies:
 
-* ``plotting``, which requires `matplotlib` and `mpl_animators`. If you are using any of the `ndcube` objects directly with the default plotting implementation you probably want to include this extra in your requirements.
-* ``reproject``, which requires the `reproject` package. This is required to use the `NDCube.reproject_to` method.
+* ``plotting``, which requires `matplotlib` and `mpl_animators`.
+  If you are using any of the ``ndcube`` objects directly with the default plotting implementation you probably want to include this extra in your requirements.
+* ``reproject``, which requires the `reproject` package.
+  This is required to use the :meth:`ndcube.NDCube.reproject_to` method.
 
 When including ndcube in your package requirements you should include either of these extras using the ``ndcube[plotting]`` type syntax.
 If you wish for all extra requirements to be installed you can use ``ndcube[all]``.
 
+Subclassing an ``ndcube`` Data Class
+====================================
 
-Subclassing an ndcube Data Class
---------------------------------
-
-
-Before You Subclass
-###################
+Before you subclass
+-------------------
 
 The data classes in ndcube have been designed to be subclassed and extended.
 One word of warning before you write ``myclass(NDCube)`` though: think about if the functionality you are writing is more generally applicable.
 Imagine for a moment that you are writing a class which is specifically for a cube with space, space, wavelength axes so that you can do some operations like fitting along the wavelength axis.
-Your subclass of ``NDCube`` may provide great functionality for the users who have data which meet your assumptions.
+Your subclass of `~ndcube.NDCube` may provide great functionality for the users who have data which meet your assumptions.
 However, if I come along with a space, space, wavelength, time 4D cube I may want to make use of your fitting functions along the wavelength axis.
 
 **Can you write your functionality in a way that takes any ndcube object with any specific combination of physical types?**
 
-
 Subclassing
-###########
+-----------
 
 When you are subclassing, try to use as much of the upstream object properties as possible.
 Doing this will enable you to reuse functionality designed for all ndcube classes and hence make your life easier.
 For instance if your class has a special property ``.info`` it would not automatically be carried through operations such as slicing and reprojecting.
 You would need to customize all these operations.
 If instead you put an ``info`` key in the ``meta`` dictionary it would automatically be copied through the appropriate operations.
 
 If your subclass does have custom attributes you need to propagate through methods and functions, you will in most cases need to overload these methods in your subclass.
-On `.NDCube` the only method which returns another instance of your subclass is currently `~.NDCube.reproject_to`.
-
+On `~ndcube.NDCube` the only method which returns another instance of your subclass is currently `ndcube.NDCube.reproject_to`.
 
 .. _customizing_plotter:
 
-Customizing the Visualization
-#############################
+Customizing the visualization
+-----------------------------
 
-The ``.plotter`` attribute of the ``NDCube`` class is configurable and allows you to customize the visualization functionality.
+The ``.plotter`` attribute of the `~ndcube.NDCube` class is configurable and allows you to customize the visualization functionality.
 This can be as minor as changing the defaults or as complete as using an alternative visualization library.
 To customize the default type for your subclass, you first need to implement a custom class inheriting from `ndcube.visualization.BasePlotter`.
-This class should implement a default ``.plot`` method which will be called by the ``NDCube.plot`` method.
+This class should implement a default ``.plot`` method which will be called by the :meth:`ndcube.NDCube.plot` method.
 As many other methods as you wish can be implemented on the plotter, to be called using the ``.plotter.mymethod()`` API.
 
-Once you have a custom plotter class (e.g. ``CustomPlotter``) you can set this to be the default for all instances of your subclass by doing the following::
+Once you have a custom plotter class (e.g. ``CustomPlotter``) you can set this to be the default for all instances of your subclass by doing the following
+
+.. code-block:: python
 
   from ndcube.visualization import BasePlotter, PlotterDescriptor
   from ndcube import NDCube
 
   class CustomPlotter(BasePlotter):
       def plot(self):
           pass
```

### Comparing `ndcube-2.1.1/docs/images/ndcollection_diagram.png` & `ndcube-2.1.2/docs/explaining_ndcube/images/ndcollection_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/images/ndcube_diagram.png` & `ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/images/ndcube_sliced_diagram.png` & `ndcube-2.1.2/docs/explaining_ndcube/images/ndcube_sliced_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/images/ndcubesequence_diagram.png` & `ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/images/ndcubesequence_sliced_diagram.png` & `ndcube-2.1.2/docs/explaining_ndcube/images/ndcubesequence_sliced_diagram.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/index.rst` & `ndcube-2.1.2/docs/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,86 @@
-********************
-ndcube Documentation
-********************
+**********************
+`ndcube` documentation
+**********************
 
+`ndcube` is a SunPy Project affiliated package designed for handling N-dimensional data cubes described by WCS (World Coordinate System) transformations.
 
-Welcome to ndcube's documentation.
-
-ndcube is a SunPy-affiliated package designed for handling n-dimensional datacubes described by a WCS (World Coordinate System) translation.
-
-.. toctree::
-   :maxdepth: 1
-
-   introduction
-   installation
-   data_classes
-   coordinates
-   slicing
-   visualization
-   reproject
-   tabular_coordinates
-   api
-   extending_ndcube
-   generated/gallery/index
-   whatsnew/index
-
+The side bar on the left contains links to the various sections of the documentation.
 
 .. _getting_help:
 
-Getting Help
+Getting help
 ============
 
-If you are unsure of the general features of the ndcube package, your first stop should be this document which we strive to make as comprehensive, yet understandable, as possible.
-If you would like to know more about how to use a specific function, class, etc., documentation for each object is in the :ref:`api` of this guide.
-If you cannot find the answer to your issue there, would like to provide feedback, or would like help contributing code to ndcube, you can get help directly from the ndcube team in a number of ways.
+If you are unsure of the general features of the `ndcube` package, your first stop should be this document which we strive to make as comprehensive, yet understandable, as possible.
+If you would like to know more about how to use a specific function, class, etc., documentation for each object is in the :ref:`reference` of this guide.
+If you cannot find the answer to your issue there, would like to provide feedback, or would like help contributing code to `ndcube`, you can get help directly from the `ndcube` team in a number of ways.
 
 Live Chat
 ---------
 
-ndcube has a `matrix channel`_ which will open directly in your browser.
-You will need to register in order to comment but in there are many sunpy and ndcube users and developers, who will be happy to help.
+`ndcube` has a `matrix channel`_ which will open directly in your browser.
+You will need to register in order to comment but in there are many `sunpy` and `ndcube` users and developers, who will be happy to help.
 
-We could always use more voices and opinions in the discussions about ndcube and its development from both users and developers.
+We could always use more voices and opinions in the discussions about `ndcube` and its development from both users and developers.
 There are a number of ways to make your voice heard.
 Whether it be constructive criticism, inquiries about current or future capabilities, or flattering praise, we would love to hear from you.
 
-.. _`matrix channel`: https://openastronomy.element.io/#/room/#ndcube:openastronomy.org
+.. _`matrix channel`: https://app.element.io/#/room/#ndcube:openastronomy.org
 
-Reporting Bugs
+Reporting bugs
 --------------
 
 If you run into unexpected behavior or a bug please report it.
 All bugs are raised and stored on our `issue tracker`_.
 If you are not sure if your problem is a bug, you can either send a message to the chat room or open an issue.
 Ideally, we would like a short code example so we can run into the bug on our own machines.
 
 .. _issue tracker: https://github.com/sunpy/ndcube/issues
 
+Using `ndcube` in your project
+------------------------------
 
-Using ndcube in your project
-----------------------------
-
-The ndcube package has been built to be used directly, or where needed extended in your own package.
+The `ndcube` package has been built to be used directly, or where needed extended in your own package.
 Read more about :ref:`extending_ndcube`.
 Please come tell us about what you build with ndcube to help make it better for everyone.
 
 .. _contributing:
 
-Contributing to ndcube
-======================
+Contributing to `ndcube`
+========================
 
 We are always enthusiastic to welcome new users and developers who want to enhance the ndcube package.
 You can contribute in several ways, from providing feedback, reporting bugs, contributing code, and reviewing pull requests.
 There is a role for almost any level of engagement.
 
 If you would like to contribute code, it is strongly recommended that you first discuss your aims with the ndcube community.
 We strive to be an open and welcoming community for developers of all experience levels.
 Discussing your ideas before you start can give you new insights that will make your development easier, lead to a better end product, and reduce the chances of your work being regretfully rejected because of an issue you weren't aware of, e.g. the functionality already exists elsewhere.
 
 The best guide we provide comes from the `sunpy newcomers guide <https://docs.sunpy.org/en/latest/dev_guide/contents/newcomers.html>`__.
-The only think you will need to change is sunpy to ndcube e.g., ``https://github.com/<username>/sunpy.git sunpy-git`` to ``https://github.com/<username>/ndcube.git ndcube-git`` where appropriate.
+The only thing you will need to change is "sunpy" to "ndcube" e.g.,
+
+.. code-block:: console
+
+   https://github.com/<username>/sunpy.git sunpy-git
+
+to
+
+.. code-block:: console
+
+   https://github.com/<username>/ndcube.git ndcube-git
+
+where appropriate.
+
+.. toctree::
+   :maxdepth: 1
+   :hidden:
+
+   introduction
+   installation
+   explaining_ndcube/index
+   reference/index
+   generated/gallery/index
+   extending_ndcube
+   1_to_2_transition_guide
+   whatsnew/index
```

### Comparing `ndcube-2.1.1/docs/logo/favicon.png` & `ndcube-2.1.2/docs/logo/favicon.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/logo/ndcube.png` & `ndcube-2.1.2/docs/logo/ndcube.png`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/logo/ndcube.svg` & `ndcube-2.1.2/docs/logo/ndcube.svg`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/make.bat` & `ndcube-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/docs/reproject.rst` & `ndcube-2.1.2/docs/explaining_ndcube/reproject.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _reproject:
 
-=======================
-Reprojecting ND Objects
-=======================
+***********************
+Reprojecting ND objects
+***********************
 
-Reprojecting allows you to transform your ND Objects to a coordinate grid described by another WCS object.
-Using this feature it is possible to regrid ND Objects by providing an appropriate target WCS, for operations such as resampling or alignment.
+Reprojecting allows you to transform your ND objects to a coordinate grid described by another WCS object.
+Using this feature it is possible to regrid ND objects by providing an appropriate target WCS, for operations such as resampling or alignment.
 It also enables putting similar `~ndcube.NDCube` objects onto the same grid for more direct comparison.
 
 .. _cube_reproject:
 
 Reprojecting an NDCube
 ======================
 
@@ -51,11 +51,11 @@
   >>> target_wcs.wcs.crval = 10, 0.5, 1
 
   >>> reprojected_cube = my_cube.reproject_to(target_wcs=target_wcs, shape_out=(4, 4, 10))
 
 In the above example, the ``CDELT1`` parameter of the ``target_wcs`` was modified to 0.1 (from 0.2).
 This allowed us to upsample the wavelength axis by a factor of 2.
 Accordingly, the shape of the data was updated to ``(4, 4, 10)`` from the initial shape ``(4, 4, 5)``.
-The wavelength axis goes last since the aray shape and WCS shape are represented in opposite directions.
+The wavelength axis goes last since the array shape and WCS shape are represented in opposite directions.
 
 Currently, this method does not handle the ``mask``, ``extra_coords``, and ``uncertainty`` attributes.
 These values are dropped from the returned `~ndcube.NDCube`.
```

### Comparing `ndcube-2.1.1/docs/slicing.rst` & `ndcube-2.1.2/docs/explaining_ndcube/slicing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _slicing:
 
-==================
-Slicing ND Objects
-==================
+******************
+Slicing ND objects
+******************
 
-Arguably the most useful feature ndcube provides is the slicing of its data classes.
-Users can apply the standard slicing notation to ND objects (or real world coordinates in the case of `ndcube.NDCube.crop`) which alter the data and WCS transformations consistently and simultaneously.
+Arguably the most useful feature `ndcube` provides is the slicing of its data classes.
+Users can apply the standard slicing notation to ND objects (or real world coordinates in the case of :meth:`ndcube.NDCube.crop`) which alter the data and WCS transformations consistently and simultaneously.
 This enables users to rapidly and reliably identify and extract regions of interest in their data, thereby allowing them to move closer to the speed of thought during their analysis.
 
 .. _cube_slicing:
 
 Slicing NDCubes
 ===============
 
@@ -18,15 +18,15 @@
 This is achieved by applying the standard slicing API to the `~ndcube.NDCube`.
 Because many of the inspection properties such `~ndcube.NDCube.dimensions` and `~ndcube.NDCube.array_axis_physical_types` are calculated on the fly, the information they return after slicing is also consistent with the sliced `~ndcube.NDCube`.
 This makes `~ndcube.NDCube`'s slicing infrastructure very powerful.
 
 To slice ``my_cube``, simply do something like:
 
 .. expanding-code-block:: python
-  :summary: Expand to see <span class="pre">my_cube</span> instantiated.
+  :summary: Expand to see my_cube instantiated.
 
   >>> import astropy.units as u
   >>> import astropy.wcs
   >>> import numpy as np
   >>> from astropy.nddata import StdDevUncertainty
 
   >>> from ndcube import NDCube
@@ -38,15 +38,15 @@
   >>> wcs = astropy.wcs.WCS(naxis=3)
   >>> wcs.wcs.ctype = 'WAVE', 'HPLT-TAN', 'HPLN-TAN'
   >>> wcs.wcs.cunit = 'Angstrom', 'deg', 'deg'
   >>> wcs.wcs.cdelt = 0.2, 0.5, 0.4
   >>> wcs.wcs.crpix = 0, 2, 2
   >>> wcs.wcs.crval = 10, 0.5, 1
 
-  >>> # Define mask.  Initially set all elements unmasked.
+  >>> # Define mask. Initially set all elements unmasked.
   >>> mask = np.zeros_like(data, dtype=bool)
   >>> mask[0, 0][:] = True  # Now mask some values.
   >>> # Define uncertainty, metadata and unit.
   >>> uncertainty = StdDevUncertainty(np.sqrt(np.abs(data)))
   >>> meta = {"Description": "This is example NDCube metadata."}
   >>> unit = u.ct
 
@@ -54,15 +54,15 @@
   >>> my_cube = NDCube(data, wcs=wcs, uncertainty=uncertainty, mask=mask, meta=meta, unit=unit)
 
 .. code-block:: python
 
   >>> my_cube_roi = my_cube[1:3, 1:3]
 
 Comparing the figures below demonstrates the consequences of this operation.
-The first is the same pictoral representation of an `~ndcube.NDCube` and its components we saw in the :ref:`ndcube` section.
+The first is the same pictorial representation of an `~ndcube.NDCube` and its components we saw in the :ref:`ndcube` section.
 The blue squares represent array-based data, namely ``.data``, ``.uncertainty``, and ``.mask``.
 The green squares represent metadata, ``.metadata`` and ``.unit``.
 The red squares represent the coordinate objects, ``.wcs``, ``extra_coords``, and ``.global_coords``.
 Finally, the yellow ovals represent the inspection and analysis methods of `~ndcube.NDCube`.
 For ease of representation, we have only shown two dimensions.
 
 .. image:: images/ndcube_diagram.png
@@ -73,50 +73,51 @@
   :width: 800
   :alt: Components of an NDCube after slicing.
 
 The second image shows the same `~ndcube.NDCube` after the above slicing operation has been applied.
 The green metadata attributes and yellow methods remain unchanged.
 However, the blue arrays have all been consistently altered from their original size, represented by the dotted lines.
 The ``.wcs`` and ``.extra_coords`` coordinate objects have also change and are now pink.
-This signifies that their transfomations have been altered such that the array elements correspond to the same real world coordinate values as they did in the unsliced `~ndcube.NDCube`.
+This signifies that their transformations have been altered such that the array elements correspond to the same real world coordinate values as they did in the unsliced `~ndcube.NDCube`.
 This is despite the fact that their array indices have been altered because the array sizes have changed.
 In this example ``.global_coords`` object is unchanged.
 However, ``.global_coords`` is changed when slicing causes an axis to be dropped, e.g.:
 
 .. code-block:: python
 
   >>> my_2d_cube = my_cube[1:2, 1:3, 0]
 
 This example will create a 2-D `~ndcube.NDCube` where the last (wavelength) dimension is dropped.
 As a consequence, wavelength is no longer part of the WCS transformations.
 However, the wavelength value at the location where the `~ndcube.NDCube` was sliced can still be accessed via `~ndcube.NDCube.global_coords`.
 
 .. code-block:: python
 
-  >>> my_2d_cube.global_coords['em.wl']  # doctest: +SKIP
+  >>> my_2d_cube.global_coords['em.wl']
+  <SpectralCoord 1.02e-09 m>
 
 This is true for all coordinates, in both the ``.wcs`` and ``.extra_coords`` objects, that no longer correspond to any array axes after slicing.
 See the :ref:`global_coords` section for more.
 
 .. _ndcube_crop:
 
 Cropping with Real World Coordinates
 ------------------------------------
 
-In addition to slicing by index, `~ndcube.NDCube` supports slicing by real world coordinates via the `~ndcube.NDCube.crop` method.
-This takes two iterables of high level coordinate objects, e.g. `~astropy.time.Time`, `~astropy.coordinates.SkyCoord`, `~astropy.coordinates.SpectralCoord`, `~astropy,units.Quantity` etc.
+In addition to slicing by index, `~ndcube.NDCube` supports slicing by real world coordinates via the :meth:`~ndcube.NDCube.crop` method.
+This takes two iterables of high level coordinate objects, e.g. `~astropy.time.Time`, `~astropy.coordinates.SkyCoord`, `~astropy.coordinates.SpectralCoord`, `~astropy.units.Quantity` etc.
 Each iterable describes a single location in the data array in real world coordinates.
 The crop method identifies the smallest rectangular region in the data array that contains all the specified coordinates, and crops the `~ndcube.NDCube` to that region.
-It does not rebin or interpolate the data.  The order of the high level coordinate objects in each iterable must be the same as that expected by `astropy.wcs.wcsapi.BaseHighLevelWCS.world_to_array_index`, namely in world order.
+It does not rebin or interpolate the data. The order of the high level coordinate objects in each iterable must be the same as that expected by `astropy.wcs.wcsapi.BaseHighLevelWCS.world_to_array_index`, namely in world order.
 
-Users can also crop their `~ndcube.NDCube` with the `~ndcube.NDCube.crop_by_values` method.
-It differs from `~ndcube.NDCube.crop` only in that it accepts and returns iterables of `~astropy.units.Quantity` objects rather than high-level astropy coordinate objects.
+Users can also crop their `~ndcube.NDCube` with the :meth:`~ndcube.NDCube.crop_by_values` method.
+It differs from :meth:`~ndcube.NDCube.crop` only in that it accepts and returns iterables of `~astropy.units.Quantity` objects rather than high-level astropy coordinate objects.
 In one sense this makes the API simpler as the full coordinate information (e.g. observer frame, epoch etc.) required by high level coordinate objects need not be provided.
 But this also makes it less explicit and so has the potential to be slightly more obscure.
-We therefore expect that the majority of users will be better served by `~ndcube.NDCube.crop` while some developers building tools on top of `~ndcube.NDCube` may be better served by `~ndcube.NDCube.crop_by_values`.
+We therefore expect that the majority of users will be better served by :meth:`~ndcube.NDCube.crop` while some developers building tools on top of `~ndcube.NDCube` may be better served by :meth:`~ndcube.NDCube.crop_by_values`.
 
 In the following example we are working with a three dimensional (spectral, spatial, spatial) cube, and we wish to crop a smaller region of the spectral dimension and a smaller square in the spatial dimensions.
 To crop a rectangular region in the spatial axes, which correctly accounts for any rotation, we need to specify all four corners of the rectangle.
 However, along the one dimensional spectral dimension (which is not correlated to the spatial dimensions) we only need to specify two points.
 We achieve this by replacing the spectral coordinate with `None` in the last two points.
 This means that these world points are not used in calculating the pixel range to which the spectral axis will be cropped.
 
@@ -155,15 +156,15 @@
   :width: 800
   :alt: Schematic of an NDCubeSequence before slicing.
 
 Say we have four NDCubes in an `~ndcube.NDCubeSequence`, each of shape ``(4, 4, 5)``.
 Now suppose we want to obtain a region of interest from the 2nd, 3rd, and 4th cubes in the sequence.
 Let the region of interest in each cube be defined as between the 2nd and 3rd pixels (inclusive) in all cube dimensions.
 This would be a cumbersome slicing operation if treating the sub-cubes independently.
-(This would be made even worse without the power of `~ndcube.NDCube` where the data arrays, WCS objects, masks, uncertainty arrays, etc. would all have to be sliced independently!)
+This would be made even worse without the power of `~ndcube.NDCube` where the data arrays, WCS objects, masks, uncertainty arrays, etc. would all have to be sliced independently!
 However, with `~ndcube.NDCubeSequence` this becomes as simple as indexing a single array.
 
 .. expanding-code-block:: python
   :summary: Click to reveal/hide the instantiation of the NDCubeSequence.
 
   >>> import astropy.units as u
   >>> import astropy.wcs
@@ -269,15 +270,15 @@
   <Quantity [2., 3.] pix>
   >>> single_cube_roi.array_axis_physical_types
   [('custom:pos.helioprojective.lat', 'custom:pos.helioprojective.lon'),
    ('em.wl',)]
 
 This returns the same `~ndcube.NDCube` as above.
 However, also as above, we can induce the return type to be an `~ndcube.NDCubeSequence` by supplying a length-1 `slice`.
-As before, the same region of interest from the same sub-cube is represeted, just with sequence and common axes of length 1.
+As before, the same region of interest from the same sub-cube is represented, just with sequence and common axes of length 1.
 
 .. code-block:: python
 
   >>> roi_length1_sequence = my_sequence.index_as_cube[4:5, 1:3, 1:4]
   >>> roi_length1_sequence.dimensions
   (<Quantity 1. pix>, <Quantity 1. pix>, <Quantity 2. pix>, <Quantity 3. pix>)
   >>> roi_length1_sequence.array_axis_physical_types
@@ -325,15 +326,15 @@
 Non-aligned axes must be sliced separately.
 Nonetheless, `~ndcube.NDCollection`'s slicing capability represents one of its greatest advantages over a simple Python `dict`, making it a powerful tool for rapidly and reliably cropping multiple components of a data set to a region of interest.
 This has the potential to drastically speed up analysis workflows.
 
 To demonstrate, let's instantiate an `~ndcube.NDCollection` with aligned axes, as we did in the :ref:`ndcollection` section.
 
 .. expanding-code-block:: python
-  :summary: Click to reveal/hide the instantiation of the 'linewidths' cube.  We'll use "my_cube" defined above for the 'observations' cube.
+  :summary: Click to reveal/hide the instantiation of the 'linewidths' cube. We'll use "my_cube" defined above for the 'observations' cube.
 
   >>> # Define derived linewidth NDCube
   >>> linewidth_data = np.random.rand(4, 4) / 2 # dummy data
   >>> linewidth_wcs = astropy.wcs.WCS(naxis=2)
   >>> linewidth_wcs.wcs.ctype = 'HPLT-TAN', 'HPLN-TAN'
   >>> linewidth_wcs.wcs.cunit = 'deg', 'deg'
   >>> linewidth_wcs.wcs.cdelt = 0.5, 0.4
```

### Comparing `ndcube-2.1.1/docs/tabular_coordinates.rst` & `ndcube-2.1.2/docs/explaining_ndcube/tabular_coordinates.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 .. _tabular_coordinates:
 
-===================
-Tabular Coordinates
-===================
+*******************
+Tabular coordinates
+*******************
 
-So far we have assumed that we are constructing an NDCube using a WCS that has been read from a file or explicitly created.
+So far we have assumed that we are constructing an `~ndcube.NDCube` using a WCS that has been read from a file or explicitly created.
 However, in some cases we may have tables giving the coordinate values at each pixel and converting these into a WCS manually can be tedious.
 Therefore ndcube provides tools for constructing WCSes from such tables.
 
 Tabular coordinates are useful when there is no mathematical description of the axis, or when it's a natural fit for the data you have.
 It's worth considering that tabular coordinates are generally not as polished as a functional transform in a WCS.
 Therefore, if possible, building a functional WCS for your coordinate system is highly recommended.
 
-Tabular Coordinates and WCSes
+Tabular coordinates and WCSes
 =============================
 
 All coordinate information in ndcube is represented as a WCS.
-Even the `.ExtraCoords` class, which allows the user to add tabular data to axes, uses the
-`gwcs <https://gwcs.readthedocs.io/en/stable/>`_ library to store this information as a WCS.
+Even the `~ndcube.ExtraCoords` class, which allows the user to add tabular data to axes, uses the
+`gwcs <https://gwcs.readthedocs.io/en/stable/>`__ library to store this information as a WCS.
 This enables ndcube's coordinate transformation and plotting functions to leverage the same infrastructure, irrespective of whether the coordinates are functional or tabular.
 
 The FITS WCS standard also supports tabular axes with the ``-TAB`` CTYPE.
 Support for reading files using this convention has (reasonably) recently been added to Astropy, so if you have a FITS file using this convention you should be able to load it into a `~astropy.wcs.WCS` object.
 If you wish to be able to serialise your NDCube object to FITS files you will need to manually construct a WCS object using the ``-TAB`` convention.
 
 The functionality provided by ndcube makes it easy to construct a `gwcs.wcs.WCS` object backed by lookup tables.
 At the time of writing there are some known issues with the support for generic lookup tables in gwcs.
 
 Constructing a WCS from Lookup Tables
 =====================================
 
 ndcube supports constructing lookup tables from `~astropy.coordinates.SkyCoord`,  `~astropy.time.Time` and `~astropy.units.Quantity` objects.
-These objects are wrapped in `BaseTableCoordinate <.table_coord>` objects which can be composed together into a multi-dimensional WCS.
+These objects are wrapped in `~ndcube.extra_coords.BaseTableCoordinate` objects which can be composed together into a multi-dimensional WCS.
 
 .. note::
 
    Only one dimensional tables are currently supported. It is possible to construct higher dimensional lookup tables by "meshing" the inputs, which is described below.
 
 A simple example of constructing a WCS from a lookup table in a `.TimeTableCoordinate`
 is the following temporal axis::
@@ -60,15 +60,15 @@
   Parameters:
     points: (<Quantity [0., 1., 2., 3., 4., 5., 6., 7., 8., 9.] pix>,)
     lookup_table: [    0.  3600.  7200. 10800. 14400. 18000. 21600. 25200. 28800. 32400.] s
     method: linear
     fill_value: nan
     bounds_error: False)>
 
-This `gwcs.WCS` object can then be passed to the constructor of `.NDCube` alongside your array and other parameters.
+This `gwcs.wcs.WCS` object can then be passed to the constructor of `~ndcube.NDCube` alongside your array and other parameters.
 
 Combining Two Coordinates into a Single WCS
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 We can extend this example to be a space-space-time cube.
 In this example we are going to utilize the ``mesh=`` keyword argument for the first time.
 This keyword argument interprets the input to `.SkyCoordTableCoordinate` in a similar way to `numpy.meshgrid`.
```

### Comparing `ndcube-2.1.1/docs/visualization.rst` & `ndcube-2.1.2/docs/explaining_ndcube/visualization.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 .. _plotting:
 
-======================
-Visualizing ND Objects
-======================
+**********************
+Visualizing ND objects
+**********************
 
 .. _cube_plotting:
 
 Visualizing NDCubes
 ===================
 
 `~ndcube.NDCube` provides a simple-to-use, yet powerful visualization method, `~ndcube.NDCube.plot`, which produces sensible visualizations based on the dimensionality of the data and optional user inputs.
 It is intended to be a useful quicklook tool and not a replacement for high quality plots or animations, e.g. for publications.
 Let's define an `~ndcube.NDCube` as with a shape of ``(4, 4, 5)`` and physical axes of helioprojective longitude, latitude and wavelength.
-(Click the "Source code" link immediately below to see this `~ndcube.NDCube` instantiated.)
+Click the "Source code" link immediately below to see this `~ndcube.NDCube` instantiated.
 
 .. plot::
   :context: reset
   :nofigs:
 
   >>> import astropy.units as u
   >>> import astropy.wcs
@@ -33,15 +33,15 @@
   >>> wcs.wcs.ctype = 'WAVE', 'HPLT-TAN', 'HPLN-TAN'
   >>> wcs.wcs.cunit = 'Angstrom', 'deg', 'deg'
   >>> wcs.wcs.cdelt = 0.2, 0.5, 0.4
   >>> wcs.wcs.crpix = 0, 2, 2
   >>> wcs.wcs.crval = 10, 0.5, 1
   >>> wcs.wcs.cname = 'wavelength', 'HPC lat', 'HPC lon'
 
-  >>> # Define mask.  Initially set all elements unmasked.
+  >>> # Define mask. Initially set all elements unmasked.
   >>> mask = np.zeros_like(data, dtype=bool)
   >>> mask[-1, -1][:] = True  # Now mask some values.
   >>> # Define uncertainty, metadata and unit.
   >>> uncertainty = StdDevUncertainty(np.sqrt(np.abs(data)))
   >>> meta = {"Description": "This is example NDCube metadata."}
   >>> unit = u.ct
 
@@ -115,15 +115,15 @@
   :nofigs:
 
   >>> plt.clf()
   >>> plt.cla()
   >>> plt.close()
 
 Note that sometimes axis tickmarks are missing.
-This is a caused by a behavior in `~astropy.visualization.wcsaes.WCSAxes` whereby the ticks and labels are omitted if the plot extends beyond the valid range of the WCS projection.
+This is a caused by a behavior in `~astropy.visualization.wcsaxes.WCSAxes` whereby the ticks and labels are omitted if the plot extends beyond the valid range of the WCS projection.
 This can happen when `matplotlib` pads the axes and can be overcome by zooming into the image slightly so that the plot boundaries are again within the valid range of the WCS projection.
 
 Visualizations can be customized via the use of kwargs.
 For `~ndcube.NDCube` instances with more than one array axis, the ``plot_axes`` keyword is used to determine which array axes are displayed on which plot axes.
 It is set to a list with a length equal to the number of array axes in array axis order.
 The array axis to be displayed on the x-axis is marked by ``'x'`` in the corresponding element of the ``plot_axes`` list, while the array axis for the y-axis is marked with a ``'y'``.
 If no ``'y'`` axis is provided, a line animation is produced.
@@ -280,15 +280,16 @@
   >>> cube1.extra_coords.add('time', 0, timestamps1)
   >>> cube2 = NDCube(data2, wcs=wcs)
   >>> cube2.extra_coords.add('time', 0, timestamps2)
 
   >>> # Define the sequence
   >>> my_sequence = NDCubeSequence([cube0, cube1, cube2], common_axis=common_axis)
 
-To make a 4D array out of the data arrays within the `~ndcube.NDCubes` of `my_sequence`.
+To make a 4D array out of the data arrays within the constituent `~ndcube.NDCube` instances in
+``my_sequence``.
 
 .. code-block:: python
 
     >>> data4d = np.stack([cube.data for cube in my_sequence.data], axis=0)
     >>> data4d.shape
     (3, 3, 4, 5)
```

### Comparing `ndcube-2.1.1/examples/creating_ndcube_from_fitsfile.py` & `ndcube-2.1.2/examples/creating_ndcube_from_fitsfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 # `~ndcube.NDCube` from data stored in a FITS file.
 # Here we are using an example file from ``astropy``.
 
 image_file = get_pkg_data_filename('tutorials/FITS-images/HorseHead.fits')
 
 ###########################################################################
 # Lets extract the image data and the header information from the FITS file.
-# This can be achieved by using the functionality within `~astropy.io`.
+# This can be achieved by using the functionality within `astropy.io.fits`.
 # In this file the image information is located in the Primary HDU (extension 0).
+
 image_data = fits.getdata(image_file)
 image_header = fits.getheader(image_file)
 
 ##########################################################################
 # To create an `~ndcube.NDCube` object, we need both the data array and a
 # WCS object (e.g. an `~astropy.wcs.WCS`). Here the data WCS information is
-# within the header, which we can pass to `~astropy.wcs.WCS()` to create a WCS object.
+# within the header, which we can pass to :class:`~astropy.wcs.WCS` to create a WCS object.
 
 example_ndcube = NDCube(image_data, WCS(image_header))
 
 ##########################################################################
 # Now we have created an `~ndcube.NDCube` from this data.
 # We can inspect the `~ndcube.NDCube`, such as the WCS.
 
@@ -43,12 +44,12 @@
 
 ##########################################################################
 # and we can also inspect the dimensions.
 
 print(example_ndcube.dimensions)
 
 ##########################################################################
-# We can also quickly visualize the data using the `~ndcube.NDCube.plot()` method.
+# We can also quickly visualize the data using the :meth:`~ndcube.NDCube.plot` method.
 
 example_ndcube.plot()
 
 plt.show()
```

### Comparing `ndcube-2.1.1/examples/dev/example_template.py` & `ndcube-2.1.2/examples/dev/example_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # block. To include this new comment string we started the new block with a
 # long line of hashes.
 #
 # The sphinx-gallery parser will assume everything after this splitter and that
 # continues to start with a **comment hash and space** (respecting code style)
 # is text that has to be rendered in
 # html format. Keep in mind to always keep your comments always together by
-# comment hashes. That means to break a paragraph you still need to commend
+# comment hashes. That means to break a paragraph you still need to comment
 # that line break.
 #
 # In this example the next block of code produces some plotable data. Code is
 # executed, figure is saved and then code is presented next, followed by the
 # inlined figure.
 
 x = np.linspace(-np.pi, np.pi, 300)
```

### Comparing `ndcube-2.1.1/examples/slicing_ndcube.py` & `ndcube-2.1.2/examples/slicing_ndcube.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
-=======================================================
+==============================
 Examples of cropping an NDCube
-=======================================================
+==============================
 
 One of the powerful aspects of having coordinate-aware data stored as an
 `~ndcube.NDCube` is the ability to crop and slice the data and coordinates in a
-standarised and easy way.
+standardised and easy way.
 
 For example, there may be a region of interest you would like to crop out along a certain dimension
 of your cube. In this example, this method to slice an `~ndcube.NDCube` are illustrated.
-
 """
 import astropy.wcs
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import SkyCoord, SpectralCoord
 from sunpy.coordinates import frames
 
@@ -22,15 +21,15 @@
 ##############################################################################
 # Let's begin by creating an example `~ndcube.NDCube` object.
 # For this case, we'll generate an `~ndcube.NDCube` that consists of 3 dimensions
 # space-space-wavelength. This is analogous to an observation including images in multiple
 # wavelengths.
 # Lets first define a 3-D numpy array, and then define the WCS information that describes the
 # data. We'll just create an array of random numbers, and a WCS which consists of the coordinate information
-# which in this case will be in Helioprojective (i.e. an observation of the Sun) in latitute and longitude,
+# which in this case will be in Helioprojective (i.e. an observation of the Sun) in latitude and longitude,
 # and over several wavelengths in the range of 10.2 - 11 angstrom.
 
 # Define the data of random numbers. Here the spatial dimensions are (45, 45) and the wavelength dimension is 5.
 data = np.random.rand(5, 45, 45)
 # Define the WCS
 wcs = astropy.wcs.WCS(naxis=3)
 wcs.wcs.ctype = 'HPLT-TAN', 'HPLN-TAN', "WAVE"
@@ -39,116 +38,121 @@
 wcs.wcs.crpix = 2, 2, 0
 wcs.wcs.crval = 1, 1, 10
 wcs.wcs.cname = 'HPC lat', 'HPC lon', 'wavelength'
 # Instantiate the `~ndcube.NDCube`
 example_cube = NDCube(data, wcs=wcs)
 
 ##############################################################################
-# So we now have created an `~ndcube.NDCube` named `example_cube`.
+# So we now have created an `~ndcube.NDCube` named ``example_cube``.
 # You may have noticed that the order of the WCS is reversed to the array order - this
 # is normal convention, and something to remember throughout.
 # Now let's first inspect the cube.
 
 ##############################################################################
 # Here we can inspect the cube by plotting it
 example_cube.plot()
 
 ##############################################################################
-# We can also inspect the dimesions of the cube:
+# We can also inspect the dimensions of the cube:
 example_cube.dimensions
 
 ##############################################################################
 # We can also inspect the world coordinates for all array elements:
 example_cube.axis_world_coords()
 
-
 ##############################################################################
 # Slicing and cropping the cube
 # -----------------------------
 # An `~ndcube.NDCube` can be sliced and cropped both by array indexing (similar to the way a numpy
 # array in indexed) or by real world coordinates. When we use array indices we say we
-# are "slicing" the cube.  When we use world coordinates we say we are "cropping" the cube.
+# are "slicing" the cube. When we use world coordinates we say we are "cropping" the cube.
 # Let's begin by slicing by array index.
 
 ##############################################################################
 # Slicing by array index
 # ----------------------
-# To slice the `example_cube` so that we extract only one wavelength, we can do:
+# To slice the ``example_cube`` so that we extract only one wavelength, we can do:
 # by indexing as such
+
 sliced_cube = example_cube[1, :, :]
 # here we can see we are left with a 2-D cube which is an image at one wavelength.
 sliced_cube.dimensions
 
 # We can also index a region of interest of the cube at a particular wavelength.
 # Again note that we are slicing here based on the ``array`` index rather than cropping by
 # real world value
 
 sliced_cube = example_cube[1, 10:20, 20:40]
 sliced_cube.dimensions
 
-# now we can inspect the sliced cube, and see it's now a smaller region of interest.
+# Now we can inspect the sliced cube, and see it's now a smaller region of interest.
 sliced_cube.plot()
 
 ##############################################################################
-# Cropping cube using world coordinate values using `ndcube.NDCube.crop()`
-# ------------------------------------------------------------------------
+# Cropping cube using world coordinate values using :meth:`ndcube.NDCube.crop`
+# ----------------------------------------------------------------------------
 # In many cases it's more useful to crop a cube to a region of interest based
 # on real world coordinates such as points in space or over some spectral
-# range. This is achieved by the `ndcube.NDCube.crop()` method which takes high-level astropy coordinate objects,
-# such as `astropy.coordinate.SkyCoord`. `ndcube.NDCube.crop()` returns the smallest cube
+# range. This is achieved by the :meth:`ndcube.NDCube.crop` method which takes high-level astropy coordinate objects,
+# such as `~astropy.coordinates.SkyCoord`. :meth:`ndcube.NDCube.crop` returns the smallest cube
 # in array-index space that contains all the passed points.
 
 ##############################################################################
-# Let's first define some points over which to crop the `example_cube`. The points are
-# defined as iterables of scalar high-level coordinate objects.  We must provide the same
+# Let's first define some points over which to crop the ``example_cube``. The points are
+# defined as iterables of scalar high-level coordinate objects. We must provide the same
 # number of objects in each tuple as required by the WCS to describe all the world axes.
 # In this example, this means we need to provide a `~astropy.coordinates.SkyCoord` and
-# `~astropy.coordinates.SpectralCoord` in each iterable.  However, if we don't want to crop
+# `~astropy.coordinates.SpectralCoord` in each iterable. However, if we don't want to crop
 # by one of the coordinate types, e.g. wavelength, we can replace the corresponding
 # high-level coordinate object in each iterable with ``None``.
 # Let's first define two points in space (lat and long) we want to crop but keep all wavelengths:
+
 point1 = [SkyCoord(0*u.arcsec, 0*u.arcsec, frame=frames.Helioprojective), None]
 point2 = [SkyCoord(200*u.arcsec, 100*u.arcsec, frame=frames.Helioprojective), None]
 
 cropped_cube = example_cube.crop(point1, point2)
 
 ##############################################################################
-# Similar to before, we can inspect the dimesions of the sliced cube:
-cropped_cube.dimensions
+# Similar to before, we can inspect the dimensions of the sliced cube:
 
+cropped_cube.dimensions
 
 ##############################################################################
 # and we can visualize it:
+
 cropped_cube.plot()
 
 ##############################################################################
 # Now let's say we also want to crop out the image that includes a specific wavelength.
-# Let's define a new point, and then include it with the first two we passed to `~ndcube.NDCube.crop`.
+# Let's define a new point, and then include it with the first two we passed to :meth:`~ndcube.NDCube.crop`.
+
 point3 = [None, SpectralCoord(10.2*u.angstrom)]
 
 cropped_cube = example_cube.crop(point1, point2, point3)
 
 ##############################################################################
-# we can inspect the dimesions of the cropped cube:
-cropped_cube.dimensions
+# we can inspect the dimensions of the cropped cube:
 
+cropped_cube.dimensions
 
 ##############################################################################
 # and again visualize it:
+
 cropped_cube.plot()
 
 # Now let's say we instead want to crop over a wavelength range.
 # Let's define a new point, and then include it with the first two we passed to
-# `~ndcube.NDCube.crop`.
+# :meth:`~ndcube.NDCube.crop`.
 point4 = [None, SpectralCoord(10.6*u.angstrom)]
 
 cropped_cube = example_cube.crop(point1, point2, point3, point4)
 
 ##############################################################################
-# check dimensions:
+# Check dimensions:
+
 cropped_cube.dimensions
 
 ##############################################################################
 # Here we can just see how powerful this can be to easily crop over different world coordinates.
 # In fact we can make this simpler still by combining the SkyCoords and SpectralCoords into
 # just two points:
```

### Comparing `ndcube-2.1.1/licenses/TEMPLATE_LICENSE.rst` & `ndcube-2.1.2/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/conftest.py` & `ndcube-2.1.2/ndcube/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 This file contains a set of common fixtures to get a set of different but
-predicable NDCube objects.
+predictable NDCube objects.
 """
 import logging
 
 import astropy.nddata
 import astropy.units as u
 import dask.array
 import numpy as np
```

### Comparing `ndcube-2.1.1/ndcube/extra_coords/extra_coords.py` & `ndcube-2.1.2/ndcube/extra_coords/extra_coords.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class ExtraCoordsABC(abc.ABC):
     """
     A representation of additional world coordinates associated with pixel axes.
 
     ExtraCoords can be initialised by either specifying a
-    `~astropy.wcs.wcsapi.LowLevelWCS` object and a ``mapping``, or it can be
+    `~astropy.wcs.wcsapi.BaseLowLevelWCS` object and a ``mapping``, or it can be
     built up by specifying one or more lookup tables.
 
     Parameters
     ----------
     wcs
         The WCS specifying the extra coordinates.
     mapping
@@ -43,28 +43,28 @@
     def add(self,
             name: Union[str, Iterable[str]],
             array_dimension: Union[int, Iterable[int]],
             lookup_table: Any,
             physical_types: Union[str, Iterable[str]] = None,
             **kwargs):
         """
-        Add a coordinate to this ``ExtraCoords`` based on a lookup table.
+        Add a coordinate to this `~ndcube.ExtraCoords` based on a lookup table.
 
         Parameters
         ----------
         name : `str` or sequence of `str`
             The name(s) for these world coordinate(s).
         array_dimension : `int` or `tuple` of `int`
             The array dimension(s), to which this lookup table corresponds.
         lookup_table : `object` or sequence of `object`
-            The lookup table. A `BaseTableCoordinate <.table_coord>` subclass or anything
+            The lookup table. A `~ndcube.extra_coords.BaseTableCoordinate` subclass or anything
             that can instantiate one, i.e. currently a `~astropy.time.Time`,
             `~astropy.coordinates.SkyCoord`, or a (sequence of) `~astropy.units.Quantity`.
         physical_types: `str` or iterable of `str`, optional
-            Descriptor(s) of the `physical type <../data_classes.html#dimensions-and-physical-types>`_
+            Descriptor(s) of the :ref:`<dimensions and physical types <dimensions>`
             associated with each axis; length must match the number of dimensions in
             ``lookup_table``.
         """
 
     @abc.abstractmethod
     def keys(self) -> Iterable[str]:
         """
@@ -85,18 +85,18 @@
     @abc.abstractmethod
     def wcs(self) -> BaseHighLevelWCS:
         """
         A WCS object representing the world coordinates described by this ``ExtraCoords``.
 
         .. note::
             This WCS object does not map to the pixel dimensions of the data array
-            in the `.NDCube` object. It only includes pixel dimensions associated
+            in the `~ndcube.NDCube` object. It only includes pixel dimensions associated
             with the extra coordinates. For example, if there is only one extra coordinate
             associated with a single pixel dimension, this WCS will only have 1 pixel dimension,
-            even if the `.NDCube` object has a data array of 2-D or greater.
+            even if the `~ndcube.NDCube` object has a data array of 2-D or greater.
             Therefore using this WCS directly might lead to some confusing results.
 
         """
 
     @property
     @abc.abstractproperty
     def is_empty(self):
@@ -116,15 +116,15 @@
 
 
 class ExtraCoords(ExtraCoordsABC):
     """
     A representation of additional world coordinates associated with pixel axes.
 
     ExtraCoords can be initialised by either specifying a
-    `~astropy.wcs.wcsapi.LowLevelWCS` object and a ``mapping``, or it can be
+    `~astropy.wcs.wcsapi.BaseLowLevelWCS` object and a ``mapping``, or it can be
     built up by specifying one or more lookup tables.
 
     Parameters
     ----------
     wcs
         The WCS specifying the extra coordinates.
     mapping
@@ -150,37 +150,38 @@
         self._ndcube = ndcube
 
     @classmethod
     def from_lookup_tables(cls, names, pixel_dimensions, lookup_tables, physical_types=None):
         """
         Construct a new ExtraCoords instance from lookup tables.
 
-        This is a convience wrapper around `.add` which does not
+        This is a convenience wrapper around `ndcube.ExtraCoords.add` which does not
         expose all the options available in that method.
 
         Parameters
         ----------
         names : `tuple` of `str`
             The names of the world coordinates.
         pixel_dimensions : `tuple` of `int`
             The pixel dimensions (in the array) to which the ``lookup_tables``
             apply. Must be the same length as ``lookup_tables``.
         lookup_tables : iterable of `object`
             The lookup tables which specify the world coordinates for the ``pixel_dimensions``.
-            Must be `BaseTableCoordinate <.table_coord>` subclass instances or objects from
-            which to instantiate them (see `.ExtraCoords.add`).
+            Must be `~ndcube.extra_coords.BaseTableCoordinate` subclass instances or objects from
+            which to instantiate them (see `ndcube.ExtraCoords.add`).
         physical_types: sequence of `str` or of sequences of `str`, optional
-            Descriptors of the `physical types <../data_classes.html#dimensions-and-physical-types>`_
+            Descriptors of the :ref:`dimensions`
             associated with each axis in the tables. Must be the same length as ``lookup_tables``;
             and length of each element must match the number of dimensions in corresponding
             ``lookup_tables[i]``.
+            Defaults to `None`.
 
         Returns
         -------
-        `ndcube.extra_coords.ExtraCoords`
+        `ndcube.ExtraCoords`
 
         """
         if len(pixel_dimensions) != len(lookup_tables):
             raise ValueError(
                 "The length of pixel_dimensions and lookup_tables must match."
             )
 
@@ -424,34 +425,34 @@
         """
         Resample all extra coords by given factors in array-index-space.
 
         One resample factor must be supplied for each array axis in array-axis order.
 
         Parameters
         ----------
-        factor: `ìnt`, `float`, or iterable thereof.
+        factor: `int`, `float`, or iterable thereof.
             The factor by which each array axis is resampled.
             If scalar, same factor is applied to all axes.
             Otherwise a factor for each axis must be provided.
 
-        offset: `int` `float` of iterable therefore.
+        offset: `int`, `float`, or iterable therefore.
             The location on the underlying grid which corresponds
             to the zeroth element after resampling. If iterable, must have an entry
-            for each dimension.  If a scalar, the grid will be
+            for each dimension. If a scalar, the grid will be
             shifted by the same amount in all dimensions.
 
         ndcube: `~ndcube.NDCube`
             The NDCube instance with which the output ExtraCoords object is associated.
 
         kwargs
             All remaining kwargs are passed to `numpy.interp`.
 
         Returns
         -------
-        new_ec: `~ndcube.extra_coords.ExtraCoords`
+        new_ec: `~ndcube.ExtraCoords`
             A new ExtraCoords object holding the interpolated coords.
         """
         new_ec = type(self)(ndcube)
         if self.is_empty:
             return new_ec
         if self._ndcube is not None:
             cube_shape = self._ndcube.data.shape
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ndcube-2.1.1/ndcube/extra_coords/table_coord.py` & `ndcube-2.1.2/ndcube/extra_coords/table_coord.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from astropy.wcs.wcsapi.wrappers.sliced_wcs import combine_slices, sanitize_slices
 
 try:
     import scipy.interpolate
 except ImportError:
     pass
 
-__all__ = ['TimeTableCoordinate', 'SkyCoordTableCoordinate', 'QuantityTableCoordinate']
+__all__ = ['TimeTableCoordinate', 'SkyCoordTableCoordinate', 'QuantityTableCoordinate', "BaseTableCoordinate", "MultipleTableCoordinate"]
 
 
 class Length1Tabular(_Tabular):
     _input_units_allow_dimensionless = True
     _has_inverse_bounding_box = True
     _separable = True
 
@@ -238,15 +238,15 @@
         """
 
     @abc.abstractmethod
     def is_scalar(self):
         """
         Return a boolean if this coordinate is a scalar.
 
-        This is used by `.MultipleTableCoordinate` and `.ExtraCoords` to know
+        This is used by `.MultipleTableCoordinate` and `ndcube.ExtraCoords` to know
         if the dimension has been "dropped".
         """
 
     @property
     @abc.abstractmethod
     def frame(self):
         """
@@ -463,32 +463,32 @@
 class SkyCoordTableCoordinate(BaseTableCoordinate):
     """
     A lookup table created from a `~astropy.coordinates.SkyCoord`.
 
     Parameters
     ----------
     table: `~astropy.coordinates.SkyCoord`
-        SkyCoord of coordinates.  Only one can be provided.
+        SkyCoord of coordinates. Only one can be provided.
 
     mesh: `bool`
-        If True, world components of input SkyCoord are interpretted to represent
-        different array dimensions.  Input SkyCoord must be 1-D.
+        If True, world components of input SkyCoord are interpreted to represent
+        different array dimensions. Input SkyCoord must be 1-D.
 
     names: `str` or `list` of `str`
         Custom names for the components of the SkyCoord. If provided, a name must
         be given for each component.
 
     physical_types: str` or `list` of `str`
         Physical types of the components of the SkyCoord. If provided,
         a physical type must be given for each component.
 
     Notes
     -----
     If mesh is True, underlying SkyCoord must always be "square" due to nature of
-    `~astropy.coordiantes.SkyCoord`, i.e. the lat and lon components are always the
+    `~astropy.coordinates.SkyCoord`, i.e. the lat and lon components are always the
     same length.
     """
 
     def __init__(self, *tables, mesh=False, names=None, physical_types=None):
         if not len(tables) == 1 and isinstance(tables[0], SkyCoord):
             raise ValueError("SkyCoordLookupTable can only be constructed from a single SkyCoord object")
         if mesh and tables[0].ndim > 1:
@@ -648,15 +648,15 @@
             raise ValueError("New array grids must all be same shape.")
         if mesh_output is None:
             if new_array_grids[0].ndim > 1:
                 mesh_output = False
             else:
                 mesh_output = self.mesh
 
-        # Build old array grids.  Note self._slice give the slice item(s) required to
+        # Build old array grids. Note self._slice give the slice item(s) required to
         # make the underlying SkyCoord match the dimensionality of the associated data cube.
         old_array_grids = [np.arange(d)[slc] for d, slc in zip(shape, self._slice)]
         # Iterate through components and interpolate each.
         if self.mesh:
             new_components = [np.interp(new_grid, old_grid, comp, **kwargs)
                               for new_grid, old_grid, comp
                               in zip(new_array_grids, old_array_grids, self._sliced_components)]
@@ -681,15 +681,15 @@
 class TimeTableCoordinate(BaseTableCoordinate):
     """
     A lookup table based on a `~astropy.time.Time`, will always be one dimensional.
 
     Parameters
     ----------
     table: `~astropy.time.Time`
-        Time coordinates.  Only one can be provided and must be 1D.
+        Time coordinates. Only one can be provided and must be 1D.
 
     names: `str` or `list` of `str`
         Custom names for the components of the SkyCoord. If provided, a name must
         be given for each component.
 
     physical_types: str` or `list` of `str`
         Physical types of the components of the SkyCoord. If provided,
@@ -761,15 +761,15 @@
         Kwargs are passed to underlying interpolation function.
 
         Parameters
         ----------
         new_array_grids: array-like
             The array index values at which the the new values of the
             coords are desired. A grid must be supplied for each pixel
-            axis (in array-axis order).  All grids must be the same shape.
+            axis (in array-axis order). All grids must be the same shape.
 
         Returns
         -------
         new_coord: `~ndcube.extra_coords.table_coord.TimeTableCoordinate`
             New TableCoordinate object holding the interpolated coords.
 
         """
@@ -785,15 +785,15 @@
         new_coord = type(self)(new_table, names=self.names, physical_types=self.physical_types)
         new_coord._dropped_world_dimensions = self._dropped_world_dimensions
         return new_coord
 
 
 class MultipleTableCoordinate(BaseTableCoordinate):
     """
-    A Holder for multiple `.BaseTableCoordinate` objects.
+    A Holder for multiple `ndcube.extra_coords.BaseTableCoordinate` objects.
 
     This class allows the generation of a gWCS from many `.BaseTableCoordinate`
     objects.
 
     Parameters
     ----------
     lookup_tables : `BaseTableCoordinate`
@@ -952,15 +952,15 @@
         Kwargs are passed to underlying interpolation function.
 
         Parameters
         ----------
         new_array_grids: array-like
             The array index values at which the the new values of the
             coords are desired. A grid must be supplied for each pixel
-            axis (in array-axis order).  All grids must be the same shape.
+            axis (in array-axis order). All grids must be the same shape.
 
         Returns
         -------
         new_coord: `~ndcube.extra_coords.table_coord.MultipleTableCoordinate`
             New TableCoordinate object holding the interpolated coords.
 
         """
```

### Comparing `ndcube-2.1.1/ndcube/extra_coords/tests/test_extra_coords.py` & `ndcube-2.1.2/ndcube/extra_coords/tests/test_extra_coords.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import pytest
 from astropy.coordinates import SkyCoord
 from astropy.time import Time, TimeDelta
 from astropy.wcs import WCS
 
 from ndcube import NDCube
-from ndcube.extra_coords import ExtraCoords
+from ndcube.extra_coords.extra_coords import ExtraCoords
 from ndcube.wcs.wrappers import ResampledLowLevelWCS
 
 # Fixtures
 
 
 @pytest.fixture
 def time_lut():
```

### Comparing `ndcube-2.1.1/ndcube/extra_coords/tests/test_lookup_table_coord.py` & `ndcube-2.1.2/ndcube/extra_coords/tests/test_lookup_table_coord.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/global_coords.py` & `ndcube-2.1.2/ndcube/global_coords.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,27 @@
 import numpy as np
 from astropy.coordinates.sky_coordinate import SkyCoord
 from astropy.wcs.wcsapi.high_level_api import default_order
 from astropy.wcs.wcsapi.utils import deserialize_class
 
 from ndcube.utils.wcs import validate_physical_types
 
-__all__ = ['GlobalCoordsABC', 'GlobalCoords']
-
 
 class GlobalCoordsABC(Mapping):
     """
-    A structured representation of coordinate information applicable to a whole NDCubeABC.
+    A structured representation of coordinate information applicable to a whole `~ndcube.ndcube.NDCubeABC`.
 
     This class acts as a mapping between coordinate name and the coordinate object.
     In addition to this a physical type is stored for each coordinate name.
     A concrete implementation of this class must fulfill the `Mapping` ABC,
     including methods such as ``__iter__`` and ``__len__``.
 
     Parameters
     ----------
-    ndcube : `.NDCube`, optional
+    ndcube : `~ndcube.NDCube`, optional
         The parent ndcube for this object. Used to extract global coordinates
         from the wcs and extra coords of the ndcube. If not specified only
         coordinates explicitly added will be shown.
     """
     @abc.abstractmethod
     def add(self, name: str, physical_type: str, coord: Any):
         """
@@ -88,15 +86,15 @@
         super().__init__()
         self._ndcube = ndcube
         self._internal_coords = OrderedDict()
 
     @staticmethod
     def _convert_dropped_to_internal(dropped_dimensions):
         """
-        Convert the `~astropy.wcs.wcsapi.wrappers.SlicedLowLevelWCS` style
+        Convert the `~astropy.wcs.wcsapi.SlicedLowLevelWCS` style
         ``dropped_world_dimensions`` dictionary to the GlobalCoords internal
         representation.
         """
         # Most of this method is adapted from
         # astropy.wcs.wcsapi.high_level_wcs.HighLevelWCSMixin.pixel_to_world
 
         new_internal_coords = {}
```

### Comparing `ndcube-2.1.1/ndcube/mixins/ndslicing.py` & `ndcube-2.1.2/ndcube/mixins/ndslicing.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/ndcollection.py` & `ndcube-2.1.2/ndcube/ndcollection.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 
 class NDCollection(dict):
     """
     Class for holding and manipulating an unordered collection of NDCubes or NDCubeSequences.
 
     Parameters
     ----------
-    data: sequence of `tuple`s of (`str`, `~ndcube.NDCube` or `~ndcube.NDCubeSequence`)
+    data: sequence of `tuple` of (`str`, `~ndcube.NDCube` or `~ndcube.NDCubeSequence`)
         The names and data cubes/sequences to held in the collection.
 
-    aligned_axes: `tuple` of `int`, `tuple` of `tuple`s of `int`, 'all', or None, optional
+    aligned_axes: `tuple` of `int`, `tuple` of `tuple` of `int`, 'all', or None, optional
         Axes of each cube/sequence that are aligned in numpy order.
         If elements are int, then the same axis numbers in all cubes/sequences are aligned.
         If elements are tuples of ints, then there must be one tuple for every cube/sequence.
         Each element of each tuple gives the axes of each cube/sequence that are aligned.
         If 'all', all axes are aligned in natural order, i.e. the 0th axes of all cubes
         are aligned, as are the 1st, and so on.
-        Default=None
+        Default is `None`.
 
     meta: `dict`, optional
         General metadata for the overall collection.
 
     Example
     -------
     Say the collection holds two NDCubes, each of 3 dimensions.
@@ -38,15 +38,15 @@
     means that axis 1 (0-based counting) of cube0 is aligned with axis 1 of cube1,
     and axis 2 of cube0 is aligned with axis 2 of cube1.
     However, if
 
     >>> aligned_axes = ((0, 1), (2, 1))  # doctest: +SKIP
 
     then the first tuple corresponds to cube0 and the second with cube1.
-    This is interpretted as axis 0 of cube0 is aligned with axis 2 of cube1 while
+    This is interpreted as axis 0 of cube0 is aligned with axis 2 of cube1 while
     axis 1 of cube0 is aligned with axis 1 of cube1.
     """
 
     def __init__(self, key_data_pairs, aligned_axes=None, meta=None, **kwargs):
         # Enter data and metadata into object.
         super().__init__(key_data_pairs)
         self.meta = meta
@@ -61,21 +61,28 @@
             else:
                 aligned_axes = dict(zip(keys, aligned_axes))
         if kwargs:
             raise TypeError(
                 f"__init__() got an unexpected keyword argument: '{list(kwargs.keys())[0]}'"
             )
         # Attach aligned axes to object.
-        self.aligned_axes = aligned_axes
-        if self.aligned_axes is None:
+        self._aligned_axes = aligned_axes
+        if self._aligned_axes is None:
             self.n_aligned_axes = 0
         else:
             self.n_aligned_axes = len(self.aligned_axes[keys[0]])
 
     @property
+    def aligned_axes(self):
+        """
+        The axes of each array that are aligned in numpy order.
+        """
+        return self._aligned_axes
+
+    @property
     def _first_key(self):
         return list(self.keys())[0]
 
     def __str__(self):
         return (textwrap.dedent(f"""\
             NDCollection
             ------------
@@ -100,16 +107,16 @@
             ]
 
     @property
     def aligned_axis_physical_types(self):
         """
         The physical types common to all members that are associated with each aligned axis.
 
-        One tuple is retured for each axis as there can be more than one physical type
-        associated with an aligned axis.  If there are no physical types associated
+        One tuple is returned for each axis as there can be more than one physical type
+        associated with an aligned axis. If there are no physical types associated
         with an aligned that is common to all collection members, an empty tuple is
         returned for that axis.
         """
         if self.aligned_axes is None:
             return None
         # Get array axis physical types for each aligned axis for all members of collection.
         collection_types = [np.array(cube.array_axis_physical_types,
```

### Comparing `ndcube-2.1.1/ndcube/ndcube.py` & `ndcube-2.1.2/ndcube/ndcube.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,23 @@
     pass
 
 from astropy.wcs import WCS
 from astropy.wcs.utils import _split_matrix
 from astropy.wcs.wcsapi import BaseHighLevelWCS, HighLevelWCSWrapper
 
 from ndcube import utils
-from ndcube.extra_coords import ExtraCoords, ExtraCoordsABC
+from ndcube.extra_coords.extra_coords import ExtraCoords, ExtraCoordsABC
 from ndcube.global_coords import GlobalCoords, GlobalCoordsABC
 from ndcube.mixins import NDCubeSlicingMixin
 from ndcube.ndcube_sequence import NDCubeSequence
 from ndcube.utils.wcs_high_level_conversion import values_to_high_level_objects
 from ndcube.visualization import PlotterDescriptor
 from ndcube.wcs.wrappers import CompoundLowLevelWCS, ResampledLowLevelWCS
 
-__all__ = ['NDCubeABC', 'NDCubeBase', 'NDCube']
+__all__ = ['NDCubeABC', 'NDCubeLinkedDescriptor']
 
 # Create mapping to masked array types based on data array type for use in analysis methods.
 ARRAY_MASK_MAP = {}
 ARRAY_MASK_MAP[np.ndarray] = np.ma.masked_array
 try:
     import dask.array
     ARRAY_MASK_MAP[dask.array.core.Array] = dask.array.ma.masked_array
@@ -62,15 +62,15 @@
     @abc.abstractmethod
     def combined_wcs(self) -> BaseHighLevelWCS:
         """
         The WCS transform for the NDCube, including the coordinates specified in ``.extra_coords``.
 
         This transform should implement the high level wcsapi, and have
         ``pixel_n_dim`` equal to the number of array dimensions in the
-        `.NDCube`. The number of world dimensions should be equal to the
+        `~ndcube.NDCube`. The number of world dimensions should be equal to the
         number of world dimensions in ``self.wcs`` and in ``self.extra_coords`` combined.
         """
 
     @property
     @abc.abstractmethod
     def array_axis_physical_types(self) -> Iterable[Tuple[str, ...]]:
         """
@@ -79,16 +79,16 @@
         Returns an iterable of tuples where each tuple corresponds to an array axis and
         holds strings denoting the WCS physical types associated with that array axis.
         Since multiple physical types can be associated with one array axis, tuples can
         be of different lengths. Likewise, as a single physical type can correspond to
         multiple array axes, the same physical type string can appear in multiple tuples.
 
         The physical types returned by this property are drawn from the
-        `~NDCube.combined_wcs` property so they include the coordinates contained in
-        `~NDCube.extra_coords`.
+        `~ndcube.NDCube.combined_wcs` property so they include the coordinates contained in
+        `~ndcube.NDCube.extra_coords`.
         """
 
     @abc.abstractmethod
     def axis_world_coords(self,
                           *axes: Union[int, str],
                           pixel_corners: bool = False,
                           wcs: Optional[Union[BaseHighLevelWCS, ExtraCoordsABC]] = None
@@ -96,15 +96,15 @@
         """
         Returns objects representing the world coordinates of pixel centers for a desired axes.
 
         Parameters
         ----------
         axes: `int` or `str`, or multiple `int` or `str`, optional
             Axis number in numpy ordering or unique substring of
-            `~ndcube.NDCube.world_axis_physical_types`
+            `ndcube.NDCube.wcs.world_axis_physical_types <astropy.wcs.wcsapi.BaseWCSWrapper>`
             of axes for which real world coordinates are desired.
             Not specifying axes inputs causes results for all axes to be returned.
         pixel_corners: `bool`, optional
             If `True` then instead of returning the coordinates at the centers of the pixels,
             the coordinates at the pixel corners will be returned. This
             increases the size of the output by 1 in all dimensions as all corners are returned.
         wcs: `astropy.wcs.wcsapi.BaseHighLevelWCS`, optional
@@ -135,31 +135,32 @@
     def axis_world_coords_values(self,
                                  *axes: Union[int, str],
                                  pixel_corners: bool = False,
                                  wcs: Optional[Union[BaseHighLevelWCS, ExtraCoordsABC]] = None
                                  ) -> Iterable[u.Quantity]:
         """
         Returns the world coordinate values of all pixels for desired axes.
-        In contrast to `axis_world_coords()`, this method returns `~astropy.units.Quantity` objects. which only
-        provide units rather than full coordinate metadata provided by high-level coordinate objects.
+        In contrast to :meth:`ndcube.NDCube.axis_world_coords`, this method returns
+        `~astropy.units.Quantity` objects. Which only provide units rather than full
+        coordinate metadata provided by high-level coordinate objects.
 
         Parameters
         ----------
         axes: `int` or `str`, or multiple `int` or `str`, optional
             Axis number in numpy ordering or unique substring of
-            `~ndcube.NDCube.wcs.world_axis_physical_types`
+            `ndcube.NDCube.wcs.world_axis_physical_types <astropy.wcs.wcsapi.BaseWCSWrapper>`
             of axes for which real world coordinates are desired.
             axes=None implies all axes will be returned.
 
         pixel_corners: `bool`, optional
             If `True` then coordinates at pixel corners will be returned rather than at pixel centers.
             This increases the size of the output along each dimension by 1
             as all corners are returned.
 
-        wcs: `~astropy.wcs.wcsapi.BaseHighLevelWCS` or `~ndcube.extra_coords.ExtraCoordsABC`, optional
+        wcs: `~astropy.wcs.wcsapi.BaseHighLevelWCS` or `~ndcube.ExtraCoordsABC`, optional
             The WCS object to be used to calculate the world coordinates.
             Although technically this can be any valid WCS, it will typically be
             ``self.wcs``, ``self.extra_coords``, or ``self.combined_wcs``, combing both
             the WCS and extra coords.
             Defaults to the ``.wcs`` property.
 
         Returns
@@ -200,23 +201,23 @@
             in the data array in real world coordinates.
 
             The coordinates of the points as they are passed to
             `~astropy.wcs.wcsapi.BaseHighLevelWCS.world_to_array_index`.
             Therefore their number and order must be compatible with the API
             of that method, i.e. they must be passed in world order.
 
-        wcs: `~astropy.wcs.wcsapi.BaseHighLevelWCS` or `~ndcube.extra_coords.ExtraCoordsABC`
+        wcs: `~astropy.wcs.wcsapi.BaseHighLevelWCS` or `~ndcube.ExtraCoordsABC`
             The WCS to use to calculate the pixel coordinates based on the input.
             Will default to the ``.wcs`` property if not given. While any valid WCS
             could be used it is expected that either the ``.wcs`` or
             ``.extra_coords`` properties will be used.
 
         Returns
         -------
-        result: `~ndcube..ndcube.NDCubeABC`
+        `~ndcube.ndcube.NDCubeABC`
 
         Examples
         --------
         An example of cropping a region of interest on the Sun from a 3-D image-time cube:
         >>> point1 = [SkyCoord(-50*u.deg, -40*u.deg, frame=frames.HeliographicStonyhurst), None]  # doctest: +SKIP
         >>> point2 = [SkyCoord(0*u.deg, -6*u.deg, frame=frames.HeliographicStonyhurst), None]  # doctest: +SKIP
         >>> NDCube.crop(point1, point2) # doctest: +SKIP
@@ -231,50 +232,47 @@
                        ) -> "NDCubeABC":
         """
         Crop using real world coordinates.
         This method crops the NDCube to the smallest bounding box in pixel space that
         contains all the provided world coordinate points.
 
         This function takes points as iterables of low-level coordinate objects,
-        i.e. `~astropy.units.Quantity` objects.  This differs from `~ndcube.NDCube.crop()`
+        i.e. `~astropy.units.Quantity` objects. This differs from :meth:`~ndcube.NDCube.crop`
         which takes high-level coordinate objects requiring all the relevant coordinate
-        information such as coordinate frame etc.  Hence this method's API is more basic
+        information such as coordinate frame etc. Hence this method's API is more basic
         but less explicit.
 
-
         Parameters
         ----------
         points: iterable
             Tuples of coordinate values, the length of the tuples must be
             equal to the number of world dimensions. These points are
             passed to ``wcs.world_to_array_index_values`` so their units
             and order must be compatible with that method.
 
         units: `str` or `~astropy.units.Unit`
             If the inputs are set without units, the user must set the units
             inside this argument as `str` or `~astropy.units.Unit` objects.
             The length of the iterable must equal the number of world dimensions
             and must have the same order as the coordinate points.
 
-        wcs: `~astropy.wcs.wcsapi.BaseHighLevelWCS` or `~ndcube.extra_coords.ExtraCoordsABC`
+        wcs: `~astropy.wcs.wcsapi.BaseHighLevelWCS` or `~ndcube.ExtraCoordsABC`
             The WCS to use to calculate the pixel coordinates based on the input.
             Will default to the ``.wcs`` property if not given. While any valid WCS
             could be used it is expected that either the ``.wcs`` or
             ``.extra_coords`` properties will be used.
 
         Returns
         -------
-        result: `~ndcube.ndcube.NDCubeABC`
-
+        `~ndcube.ndcube.NDCubeABC`
 
         Examples
         --------
         An example of cropping a region of interest on the Sun from a 3-D image-time cube:
         >>> NDCube.crop_by_values((-600, -600, 0), (0, 0, 0), units=(u.arcsec, u.arcsec, u.s)) # doctest: +SKIP
-
         """
 
 
 class NDCubeLinkedDescriptor:
     """
     A descriptor which gives the property a reference to the cube to which it is attached.
     """
@@ -320,41 +318,41 @@
 
 class NDCubeBase(NDCubeABC, astropy.nddata.NDData, NDCubeSlicingMixin):
     """
     Class representing N-D data described by a single array and set of WCS transformations.
 
     Parameters
     ----------
-    data: array-like or `astropy.nddata.NDData`
+    data : array-like or `astropy.nddata.NDData`
         The array holding the actual data in this object.
 
-    wcs: `astropy.wcs.wcsapi.BaseLowLevelWCS`, `astropy.wcs.wcsapi.BaseHighLevelWCS`, optional
+    wcs : `astropy.wcs.wcsapi.BaseLowLevelWCS`, `astropy.wcs.wcsapi.BaseHighLevelWCS`, optional
         The WCS object containing the axes' information, optional only if
         ``data`` is an `astropy.nddata.NDData` object.
 
-    uncertainty : any type, optional
+    uncertainty : Any, optional
         Uncertainty in the dataset. Should have an attribute uncertainty_type
         that defines what kind of uncertainty is stored, for example "std"
         for standard deviation or "var" for variance. A metaclass defining such
-        an interface is `~astropy.nddata.NDUncertainty` - but isn’t mandatory.
+        an interface is `~astropy.nddata.NDUncertainty` - but isn't mandatory.
         If the uncertainty has no such attribute the uncertainty is stored as
         `~astropy.nddata.UnknownUncertainty`.
         Defaults to None.
 
-    mask : any type, optional
+    mask : Any, optional
         Mask for the dataset. Masks should follow the numpy convention
         that valid data points are marked by `False` and invalid ones with `True`.
         Defaults to `None`.
 
     meta : dict-like object, optional
         Additional meta information about the dataset. If no meta is provided
         an empty dictionary is created.
 
     unit : Unit-like or `str`, optional
-        Unit for the dataset. Strings that can be converted to a `~astropy.unit.Unit` are allowed.
+        Unit for the dataset. Strings that can be converted to a `~astropy.units.Unit` are allowed.
         Default is `None` which results in dimensionless units.
 
     copy : bool, optional
         Indicates whether to save the arguments as copy. `True` copies every attribute
         before saving it while `False` tries to save every parameter as reference.
         Note however that it is not always possible to save the input as reference.
         Default is `False`.
@@ -670,41 +668,41 @@
         """
         Reprojects the instance to the coordinates described by another WCS object.
 
         Parameters
         ----------
         target_wcs : `astropy.wcs.wcsapi.BaseHighLevelWCS`, `astropy.wcs.wcsapi.BaseLowLevelWCS`,
             or `astropy.io.fits.Header`
-            The WCS object to which the ``NDCube`` is to be reprojected.
+            The WCS object to which the `ndcube.NDCube` is to be reprojected.
 
-        algorithm: `str` {'interpolation', 'adaptive', 'exact'}
+        algorithm: {'interpolation' | 'adaptive' | 'exact'}
             The algorithm to use for reprojecting.
-            When set to `'interpolation'` `~reproject.reproject_interp` is used,
-            when set to `'adaptive'` `~reproject.reproject_adaptive` is used and
-            when set to `'exact'` `~reproject.reproject_exact` is used.
+            When set to "interpolation" `~reproject.reproject_interp` is used,
+            when set to "adaptive" `~reproject.reproject_adaptive` is used and
+            when set to "exact" `~reproject.reproject_exact` is used.
 
         shape_out: `tuple`, optional
             The shape of the output data array. The ordering of the dimensions must follow NumPy
             ordering and not the WCS pixel shape.
             If not specified, `~astropy.wcs.wcsapi.BaseLowLevelWCS.array_shape` attribute
             (if available) from the low level API of the ``target_wcs`` is used.
 
         return_footprint : `bool`
-            If `True`` the footprint is returned in addition to the new `~ndcube.NDCube`.
+            If `True` the footprint is returned in addition to the new `~ndcube.NDCube`.
             Defaults to `False`.
 
         **reproject_args
             All other arguments are passed through to the reproject function
             being called. The function being called depends on the
             ``algorithm=`` keyword argument, see that for more details.
 
         Returns
         -------
         reprojected_cube : `ndcube.NDCube`
-            A new resultant NDCube object, the supplied ``target_wcs`` will be the ``.wcs`` attribute of the output ``NDCube``.
+            A new resultant NDCube object, the supplied ``target_wcs`` will be the ``.wcs`` attribute of the output `~ndcube.NDCube`.
 
         footprint: `numpy.ndarray`
             Footprint of the input array in the output array.
             Values of 0 indicate no coverage or valid values in the input
             image, while values of 1 indicate valid values.
 
         See Also
@@ -787,23 +785,23 @@
     data: `numpy.ndarray`
         The array holding the actual data in this object.
 
     wcs: `astropy.wcs.wcsapi.BaseLowLevelWCS`, `astropy.wcs.wcsapi.BaseHighLevelWCS`, optional
         The WCS object containing the axes' information, optional only if
         ``data`` is an `astropy.nddata.NDData` object.
 
-    uncertainty : any type, optional
+    uncertainty : Any, optional
         Uncertainty in the dataset. Should have an attribute uncertainty_type
         that defines what kind of uncertainty is stored, for example "std"
         for standard deviation or "var" for variance. A metaclass defining
-        such an interface is NDUncertainty - but isn’t mandatory. If the uncertainty
+        such an interface is NDUncertainty - but isn't mandatory. If the uncertainty
         has no such attribute the uncertainty is stored as UnknownUncertainty.
         Defaults to None.
 
-    mask : any type, optional
+    mask : Any, optional
         Mask for the dataset. Masks should follow the numpy convention
         that valid data points are marked by False and invalid ones with True.
         Defaults to None.
 
     meta : dict-like object, optional
         Additional meta information about the dataset. If no meta is provided
         an empty collections.OrderedDict is created. Default is None.
@@ -820,20 +818,20 @@
     copy : bool, optional
         Indicates whether to save the arguments as copy. True copies every attribute
         before saving it while False tries to save every parameter as reference.
         Note however that it is not always possible to save the input as reference.
         Default is False.
 
     """
-    # Enabling the NDCube reflected operators is a bit subtle.  The NDCube
+    # Enabling the NDCube reflected operators is a bit subtle. The NDCube
     # reflected operator will be used only if the Quantity non-reflected operator
-    # returns NotImplemented.  The Quantity operator strips the unit from the
+    # returns NotImplemented. The Quantity operator strips the unit from the
     # Quantity and tries to combine the value with the NDCube using NumPy's
-    # __array_ufunc__().  If NumPy believes that it can proceed, this will result
-    # in an error.  We explicitly set __array_ufunc__ = None so that the NumPy
+    # __array_ufunc__(). If NumPy believes that it can proceed, this will result
+    # in an error. We explicitly set __array_ufunc__ = None so that the NumPy
     # call, and consequently the Quantity operator, will return NotImplemented.
     __array_ufunc__ = None
 
     # We special case the default mpl plotter here so that we can only import
     # matplotlib when `.plotter` is accessed and raise an ImportError at the
     # last moment.
     plotter = PlotterDescriptor(default_type="mpl_plotter")
@@ -855,15 +853,15 @@
             return plotter._as_mpl_axes()
 
     def plot(self, *args, **kwargs):
         """
         A convenience function for the plotters default ``plot()`` method.
 
         Calling this method is the same as calling ``cube.plotter.plot``, the
-        behaviour of this method can change if the `NDCube.plotter` class is
+        behaviour of this method can change if the `ndcube.NDCube.plotter` class is
         set to a different ``Plotter`` class.
 
         """
         if self.plotter is None:
             raise NotImplementedError(
                 "This NDCube object does not have a .plotter defined so "
                 "no default plotting functionality is available.")
@@ -947,22 +945,22 @@
         """Convert instance to another unit.
 
         Converts the data, uncertainty and unit and returns a new instance
         with other attributes unchanged.
 
         Parameters
         ----------
-        new_unit: `astropy.unit.Unit`
+        new_unit: `astropy.units.Unit`
             The unit to convert to.
         kwargs:
             Passed to the unit conversion method, self.unit.to.
 
         Returns
         -------
-        : `ǸDCube`
+        : `~ndcube.NDCube`
             A new instance with the new unit and data and uncertainties scales accordingly.
         """
         return self * (self.unit.to(new_unit, **kwargs) * new_unit / self.unit)
 
     def rebin(self, bin_shape, operation=np.mean, operation_ignores_mask=False, handle_mask=np.all,
               propagate_uncertainties=False, new_unit=None, **kwargs):
         """
@@ -990,48 +988,48 @@
             If True, masked values are used in calculating rebinned value.
         handle_mask: `None` or function
             Function to apply to each bin in the mask to calculate the new mask values.
             If `None` resultant mask is `None`.
             Default is `numpy.all`
         propagate_uncertainties: `bool` or function.
             If False, uncertainties are dropped.
-            If True, default algorithm is used (`~ndcube.utils.cube.propagate_rebin_uncertainty`)
+            If True, default algorithm is used (`~ndcube.utils.cube.propagate_rebin_uncertainties`)
             Can also be set to a function which performs custom uncertainty propagation.
             Additional kwargs provided to this method are passed onto this function.
-            See Notes section on how to write a custom propagate_uncertainties function.
+            See Notes section on how to write a custom ``propagate_uncertainties`` function.
         new_unit: `astropy.units.Unit`, optional
             If the rebinning operation alters the data unit, the new unit can be
             provided here.
         kwargs
             All kwargs are passed to the error propagation function.
 
         Returns
         -------
-        new_cube: `NDCube`
+        new_cube: `~ndcube.NDCube`
             The resolution-degraded cube.
 
         References
         ----------
         https://mail.scipy.org/pipermail/numpy-discussion/2010-July/051760.html
 
         Notes
         -----
         **Rebining Algorithm**
         Rebinning is achieved by reshaping the N-D array to a 2N-D array and
         applying the function over the odd-numbered axes. To demonstrate,
-        consider the following example.  Let's say you have an array::
+        consider the following example. Let's say you have an array::
 
              x = np.array([[0, 0, 0, 1, 1, 1],
                            [0, 0, 1, 1, 0, 0],
                            [1, 1, 0, 0, 1, 1],
                            [0, 0, 0, 0, 1, 1],
                            [1, 0, 1, 0, 1, 1],
                            [0, 0, 1, 0, 0, 0]])
 
-        and you want to sum over 2x2 non-overlapping sub-arrays.  This summing can
+        and you want to sum over 2x2 non-overlapping sub-arrays. This summing can
         be done by reshaping the array::
 
              y = x.reshape(3,2,3,2)
 
         and then summing over the 1st and third directions::
 
              y2 = y.sum(axis=3).sum(axis=1)
@@ -1057,20 +1055,20 @@
             True elements cause corresponding uncertainty elements to be ignored.
             False elements cause corresponding uncertainty elements to be propagated.
             Must have same shape as above.
             If None, no uncertainties are ignored.
 
         All kwarg inputs to the rebin method are also passed on transparently to the
         propagation function. Hence additional inputs to the propagation function can be
-        included as kwargs to `ndcube.NDCube.rebin`.
+        included as kwargs to :meth:`ndcube.NDCube.rebin`.
 
         The shape of the uncertainty, data and mask inputs are such that the first
         dimension represents the pixels in a given bin whose data and uncertainties
-        are aggregated by the rebin process.  The shape of the remaining dimensions
-        must be the same as the final rebinned data.  A silly but informative
+        are aggregated by the rebin process. The shape of the remaining dimensions
+        must be the same as the final rebinned data. A silly but informative
         example of a custom propagation function might be::
 
              def my_propagate(uncertainty, data, mask, **kwargs):
                  # As a silly example, propagate uncertainties by summing those in same bin.
                  # Note not all args are used, but function must accept them.
                  n_pixels_per_bin = data.shape[0]  # 1st dimension of inputs gives pixels in bin.
                  final_shape = data.shape[1:]  # Trailing dims give shape of put rebinned data.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ndcube-2.1.1/ndcube/ndcube_sequence.py` & `ndcube-2.1.2/ndcube/ndcube_sequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 import astropy.units as u
 import numpy as np
 
 from ndcube import utils
 from ndcube.visualization.descriptor import PlotterDescriptor
 
-__all__ = ['NDCubeSequence']
-
 
 class NDCubeSequenceBase:
     """
     Class representing a sequence of `~ndcube.NDCube`-like objects.
 
     The cubes are assumed to have the same dimensionality and axis physical types.
 
@@ -143,16 +141,16 @@
 
     @property
     def common_axis_coords(self):
         """
         The coordinate values at each location along the common axis across all cubes.
 
         Only coordinates associated with the common axis in all cubes in the sequence
-        are returned.  Coordinates from different cubes are concatenated along the
-        common axis.  They thus represent the coordinate values at each location as
+        are returned. Coordinates from different cubes are concatenated along the
+        common axis. They thus represent the coordinate values at each location as
         if all cubes in the sequence were concatenated along the common axis.
         """
         common_axis = self._common_axis
         # Get coordinate objects associated with the common axis in all cubes.
         common_axis_names = set.intersection(*[set(cube.array_axis_physical_types[common_axis])
                                                for cube in self.data])
         common_coords = []
@@ -233,31 +231,31 @@
         return self._new_instance(result_cubes, common_axis=new_common_axis, meta=self.meta)
 
     def crop(self, *points, wcses=None):
         """
         Crop cubes in sequence to smallest pixel-space bounding box containing the input points.
 
         Each input point is given as a tuple of high-level world coordinate objects.
-        This method does not crop the sequence axis.  Instead input points
-        are passed to the crop method of cubes in sequence.  Note, therefore,
+        This method does not crop the sequence axis. Instead input points
+        are passed to the crop method of cubes in sequence. Note, therefore,
         that the input points do not include an entry for world coords only
         associated with the sequence axis.
         For a description of how the bounding box is defined, see the docstring
-        of the `ndcube.NDCube.crop` method.
+        of the :meth:`ndcube.NDCube.crop` method.
         In cases where the cubes are not aligned, all cubes are cropped
-        to the same region in pixel space.  This region will be the smallest
+        to the same region in pixel space. This region will be the smallest
         that encompasses the input points in all cubes while maintaining
         consistent array shape between the cubes.
 
         Parameters
         ----------
         points:
-            Passed to `ndcube.NDCube.crop` as the points arg without checking.
+            Passed to :meth:`ndcube.NDCube.crop` as the points arg without checking.
 
-        wcses: iterable of WCS objects or `str` (optional)
+        wcses: iterable of WCS objects or `str`, optional
             The WCS objects to be used to crop the cubes.
             There must by one WCS per cube.
             Alternatively, can be a string giving the name of the cube wcs attribute to be used,
             namely, 'wcs', 'combined_wcs', or 'extra_coords'.
             Default=None is equivalent to 'wcs'.
 
         Returns
@@ -269,34 +267,34 @@
         return self[item]
 
     def crop_by_values(self, lower_corner, upper_corner, units=None, wcses=None):
         """
         Crop cubes in sequence to smallest pixel-space bounding box containing the input points.
 
         Each input point is given as a tuple of low-level world coordinate objects.
-        This method does not crop the sequence axis.  Instead input points
-        are passed to the `ndcube.NDCube.crop_by_values` method of cubes in sequence.  Note, therefore,
+        This method does not crop the sequence axis. Instead input points
+        are passed to the :meth:`ndcube.NDCube.crop_by_values` method of cubes in sequence. Note, therefore,
         that the input points do not include an entry for world coords only
         associated with the sequence axis.
         For a description of how the bounding box is defined, see the docstring
         of the NDCube.crop_by_values method.
         In cases where the cubes are not aligned, all cubes are cropped
-        to the same region in pixel space.  This region will be the smallest
+        to the same region in pixel space. This region will be the smallest
         that encompasses the input points in all cubes while maintaining
         consistent array shape between the cubes.
 
         Parameters
         ----------
         points:
-            Passed to `ndcube.NDCube.crop` as the points arg without checking.
+            Passed to :meth:`ndcube.NDCube.crop` as the points arg without checking.
 
         units:
-            Passed to `ndcube.NDCube.crop_by_values` as the ``units`` kwarg.
+            Passed to :meth:`ndcube.NDCube.crop_by_values` as the ``units`` kwarg.
 
-        wcses: iterable of WCS objects or `str` (optional)
+        wcses: iterable of WCS objects or `str`, optional
             The WCS objects to be used to crop the cubes. There must by one WCS per cube.
             Alternatively, can be a string giving the name of the cube wcs attribute to be used,
             namely, 'wcs', 'combined_wcs', or 'extra_coords'.
             Default=None is equivalent to 'wcs'.
 
         Returns
         -------
@@ -310,40 +308,40 @@
         """
         Get the slice item with which to crop an NDCubeSequence given crop inputs.
 
         Input points are passed to the crop method of cubes in sequence.
         Note, therefore, that the input points do not include an entry for world
         coords only associated with the sequence axis.
         To learn how the bounding box is defined, see the docstrings of NDCube's
-        `~ndcube.NDCube.crop` and `~ndcube.NDCube.crop_by_values` methods.
+        :meth:`~ndcube.NDCube.crop` and :meth:`~ndcube.NDCube.crop_by_values` methods.
         In cases where the cubes are not aligned, all cubes are cropped
-        to the same region in pixel space.  This region will be the smallest
+        to the same region in pixel space. This region will be the smallest
         that encompasses the input world ranges in all cubes while maintaining
         consistent array shape between the cubes.
 
         Parameters
         ----------
         points:
-            Passed to `ndcube.NDCube.crop_by_values` as the ``points`` arg.
+            Passed to :meth:`ndcube.NDCube.crop_by_values` as the ``points`` arg.
 
-        wcses: iterable of WCS objects or `str` (optional)
+        wcses: iterable of WCS objects or `str`, optional
             The WCS objects to be used to crop the cubes. There must by one WCS per cube.
             Alternatively, can be a string giving the name of the cube wcs attribute to be used,
             namely, 'wcs', 'combined_wcs', or 'extra_coords'.
             Default=None is equivalent to 'wcs'.
 
         crop_by_values: `bool`
             Determines what function to use when determining slices of cubes.
             If True, inputs are assumed to be low-level coordinate objects and
             the crop_by_values util is used.
             If False, inputs are assumined to be high-level coordinate objects and
             the crop util is used.
 
-        units: (optiona)
-            Passed to `ndcube.NDCube.crop_by_values` as the ``units`` kwarg.
+        units: `astropy.units.Unit`, optional
+            Passed to :meth:`ndcube.NDCube.crop_by_values` as the ``units`` kwarg.
             Only used if crop_by_values is True.
         """
         n_cubes = len(self.data)
         cube_ndim = len(self.dimensions[1:])
         starts = np.zeros((n_cubes, cube_ndim), dtype=int)
         stops = np.zeros((n_cubes, cube_ndim), dtype=int)
         if wcses is None:
```

### Comparing `ndcube-2.1.1/ndcube/tests/helpers.py` & `ndcube-2.1.2/ndcube/tests/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def figure_test(test_function):
     """
     A decorator for a test that verifies the hash of the current figure or the
     returned figure, with the name of the test function as the hash identifier
     in the library. A PNG is also created in the 'result_image' directory,
     which is created on the current path.
 
-    All such decorated tests are marked with `pytest.mark.mpl_image` for convenient filtering.
+    All such decorated tests are marked with ``pytest.mark.mpl_image`` for convenient filtering.
     """
     hash_library_name = get_hash_library_name()
     hash_library_file = Path(__file__).parent / ".." / "visualization" / "tests" / hash_library_name
 
     @pytest.mark.remote_data
     @pytest.mark.mpl_image_compare(hash_library=hash_library_file.resolve(),
                                    savefig_kwargs={'metadata': {'Software': None}},
@@ -121,15 +121,15 @@
 
 def assert_wcs_are_equal(wcs1, wcs2):
     """
     Assert function for testing two wcs object.
 
     Used in testing NDCube.
     Also checks if both the wcs objects are instance
-    of `SlicedLowLevelWCS`
+    of `~astropy.wcs.wcsapi.SlicedLowLevelWCS`.
     """
 
     if not isinstance(wcs1, BaseLowLevelWCS):
         wcs1 = wcs1.low_level_wcs
     if not isinstance(wcs2, BaseLowLevelWCS):
         wcs2 = wcs2.low_level_wcs
     # Check the APE14 attributes of both the WCS
```

### Comparing `ndcube-2.1.1/ndcube/tests/test_global_coords.py` & `ndcube-2.1.2/ndcube/tests/test_global_coords.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/tests/test_ndcollection.py` & `ndcube-2.1.2/ndcube/tests/test_ndcollection.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/tests/test_ndcube.py` & `ndcube-2.1.2/ndcube/tests/test_ndcube.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/tests/test_ndcubesequence.py` & `ndcube-2.1.2/ndcube/tests/test_ndcubesequence.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/tests/test_sequence_plotting.py` & `ndcube-2.1.2/ndcube/tests/test_sequence_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
 # def test_sequence_plot_as_cube_1D_plot(test_input, test_kwargs, expected_values):
 #     # Unpack expected values
 #     expected_x_data, expected_y_data, expected_xlabel, expected_ylabel, \
 #       expected_xlim, expected_ylim = expected_values
 #     # Run plot method
 #     output = test_input.plot_as_cube(**test_kwargs)
 #     # Check values are correct
-#     # Check type of ouput plot object
+#     # Check type of output plot object
 #     assert isinstance(output, matplotlib.axes.Axes)
 #     # Check x and y data are correct.
 #     assert np.allclose(output.lines[0].get_xdata(), expected_x_data)
 #     assert np.allclose(output.lines[0].get_ydata(), expected_y_data)
 #     # Check x and y axis labels are correct.
 #     assert output.axes.get_xlabel() == expected_xlabel
 #     assert output.axes.get_ylabel() == expected_ylabel
```

### Comparing `ndcube-2.1.1/ndcube/utils/collection.py` & `ndcube-2.1.2/ndcube/utils/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numbers
 
 import numpy as np
 
+__all__ = ['assert_aligned_axes_compatible']
+
 
 def _sanitize_aligned_axes(keys, data, aligned_axes):
     if aligned_axes is None:
         return None
     # If aligned_axes set to "all", assume all axes are aligned in order.
     elif isinstance(aligned_axes, str) and aligned_axes.lower() == "all":
         # Check all cubes are of same shape
@@ -105,15 +107,15 @@
     if check_dimensions != {1}:
         raise ValueError("Aligned axes are not all of same length.")
 
     return aligned_axes
 
 
 def _update_aligned_axes(drop_aligned_axes_indices, aligned_axes, first_key):
-    # Remove dropped axes from aligned_axes.  MUST BE A BETTER WAY TO DO THIS.
+    # Remove dropped axes from aligned_axes. MUST BE A BETTER WAY TO DO THIS.
     if len(drop_aligned_axes_indices) <= 0:
         new_aligned_axes = tuple(aligned_axes.values())
     elif len(drop_aligned_axes_indices) == len(aligned_axes[first_key]):
         new_aligned_axes = None
     else:
         new_aligned_axes = []
         for key in aligned_axes.keys():
```

### Comparing `ndcube-2.1.1/ndcube/utils/cube.py` & `ndcube-2.1.2/ndcube/utils/cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 def sanitize_wcs(func):
     """
     A wrapper for NDCube methods to sanitise the wcs argument.
 
     This decorator is only designed to be used on methods of NDCube.
 
-    It will find the wcs argument, keyword or positional and if it is None, set
-    it to `self.wcs`.
+    It will find the wcs argument, keyword or positional and if it is `None`, set
+    it to ``self.wcs``.
     It will then verify that the WCS has a matching number of pixel dimensions
     to the dimensionality of the array. It will finally verify that the object
     passed is a HighLevelWCS object, or an ExtraCoords object.
     """
     # This needs to be here to prevent a circular import
-    from ndcube.extra_coords import ExtraCoords
+    from ndcube.extra_coords.extra_coords import ExtraCoords
 
     @wraps(func)
     def wcs_wrapper(*args, **kwargs):
         sig = inspect.signature(func)
         params = sig.bind(*args, **kwargs)
         wcs = params.arguments.get('wcs', None)
         self = params.arguments['self']
@@ -81,15 +81,15 @@
     if all(values_are_none):
         return True, points, wcs
     # Not not all points are of same length, error.
     if len(set(n_coords)) != 1:
         raise ValueError("All points must have same number of coordinate objects."
                          f"Number of objects in each point: {n_coords}")
     # Import must be here to avoid circular import.
-    from ndcube.extra_coords import ExtraCoords
+    from ndcube.extra_coords.extra_coords import ExtraCoords
     if isinstance(wcs, ExtraCoords):
         # Determine how many dummy axes are needed
         n_dummy_axes = len(wcs._cube_array_axes_without_extra_coords)
         if n_dummy_axes > 0:
             points = [point + [None] * n_dummy_axes for point in points]
         # Convert extra coords to WCS describing whole cube.
         wcs = wcs.cube_wcs
@@ -105,15 +105,15 @@
 
     Parameters
     ----------
     points : iterable of iterables
         Each iterable represents a point in real world space.
         Each element in a point gives the real world coordinate value of the point
         in high-level coordinate objects or quantities.
-        (Must be consistenly high or low level within and across points.)
+        (Must be consistently high or low level within and across points.)
         Objects must be in the order required by
         wcs.world_to_array_index/world_to_array_index_values.
 
     wcs : `~astropy.wcs.wcsapi.BaseHighLevelWCS`, `~astropy.wcs.wcsapi.BaseLowLevelWCS`
         The WCS to use to convert the world coordinates to array indices.
 
     crop_by_values : `bool`
@@ -200,19 +200,19 @@
                          "This is not supported.")
     return tuple(item)
 
 
 def propagate_rebin_uncertainties(uncertainty, data, mask, operation, operation_ignores_mask=False,
                                   propagation_operation=None, correlation=0, **kwargs):
     """
-    Default algorithm for uncertainty propagation in `~NDCubeBase.rebin`.
+    Default algorithm for uncertainty propagation in :meth:`~ndcube.NDCube.rebin`.
 
     First dimension of uncertainty, data and mask inputs represent the pixels
     in the bin being aggregated by the rebin process while the latter dimensions
-    must have the same shape as the rebinned data.  The operation input is the
+    must have the same shape as the rebinned data. The operation input is the
     function used to aggregate elements in the first dimension, e.g. `numpy.sum`.
 
     Parameters
     ----------
     uncertainty: `astropy.nddata.NDUncertainty`
         Cannot be instance of `astropy.nddata.UnknownUncertainty`.
         The uncertainties associated with the data. The first dimension represents
```

### Comparing `ndcube-2.1.1/ndcube/utils/misc.py` & `ndcube-2.1.2/ndcube/utils/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import astropy.units as u
 
-__all__ = ['unique_sorted']
+__all__ = ['unique_sorted', 'convert_quantities_to_units']
 
 
 def unique_sorted(iterable):
     """
     Return unique values in the order they are first encountered in the iterable.
     """
     lookup = set()  # a temporary lookup set
```

### Comparing `ndcube-2.1.1/ndcube/utils/sequence.py` & `ndcube-2.1.2/ndcube/utils/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     This requires the common_axis item to be a slice item.
     If it is an int, this function should not be used.
 
     Parameters
     ----------
     item: iterable of `int` or `slice`
-        The slicing item.  The common axis entry must be a `slice`
+        The slicing item. The common axis entry must be a `slice`
 
     common_axis: `int`
         The index of the item corresponding to the common axis.
 
     common_axis_lengths: iterable of `int`
         The lengths of each cube in the sequence along the common axis.
```

### Comparing `ndcube-2.1.1/ndcube/utils/sphinx/code_context.py` & `ndcube-2.1.2/ndcube/utils/sphinx/code_context.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/utils/tests/test_utils_collection.py` & `ndcube-2.1.2/ndcube/utils/tests/test_utils_collection.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/utils/tests/test_utils_cube.py` & `ndcube-2.1.2/ndcube/utils/tests/test_utils_cube.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/utils/tests/test_utils_sequence.py` & `ndcube-2.1.2/ndcube/utils/tests/test_utils_sequence.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/utils/tests/test_utils_wcs.py` & `ndcube-2.1.2/ndcube/utils/tests/test_utils_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/utils/wcs.py` & `ndcube-2.1.2/ndcube/utils/wcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Author: Ankit Baruah and Daniel Ryan <ryand5@tcd.ie>
-
 """
 Miscellaneous WCS utilities.
 """
 
 import numbers
 from collections import UserDict
 
@@ -73,19 +71,19 @@
     reflected_axis: `numpy.ndarray` of `int`
         The axis number(s) after reflection.
     """
     # Check type of input.
     if not isinstance(axis, np.ndarray):
         raise TypeError(f"input must be of array type. Got type: {type(axis)}")
     if axis.dtype.char not in np.typecodes['AllInteger']:
-        raise TypeError(f"input dtype must be of int type.  Got dtype: {axis.dtype})")
+        raise TypeError(f"input dtype must be of int type. Got dtype: {axis.dtype})")
     # Convert negative indices to positive equivalents.
     axis[axis < 0] += naxes
     if any(axis > naxes - 1):
-        raise IndexError("Axis out of range.  "
+        raise IndexError("Axis out of range. "
                          f"Number of axes = {naxes}; Axis numbers requested = {axis}")
     # Reflect axis about center of number of axes.
     reflected_axis = naxes - 1 - axis
 
     return reflected_axis
 
 
@@ -96,15 +94,15 @@
     Parameters
     ----------
     pixel_axis: `int`
         The pixel axis index/indices for which the world axes are desired.
 
     axis_correlation_matrix: `numpy.ndarray` of `bool`
         2D boolean correlation matrix defining the dependence between the pixel and world axes.
-        Format same as `astropy.wcs.BaseLowLevelWCS.axis_correlation_matrix`.
+        Format same as `astropy.wcs.wcsapi.BaseLowLevelWCS.axis_correlation_matrix`.
 
     Returns
     -------
     world_axes: `numpy.ndarray`
         The world axis indices corresponding to the pixel axis.
     """
     return np.arange(axis_correlation_matrix.shape[0])[axis_correlation_matrix[:, pixel_axis]]
@@ -113,19 +111,19 @@
 def world_axis_to_pixel_axes(world_axis, axis_correlation_matrix):
     """
     Gets the pixel axis indices corresponding to the index of a world axis.
 
     Parameters
     ----------
     world_axis: `int`
-        The index of the physical type for which the pixes axes are desired.
+        The index of the physical type for which the pixels axes are desired.
 
     axis_correlation_matrix: `numpy.ndarray` of `bool`
         2D boolean correlation matrix defining the dependence between the pixel and world axes.
-        Format same as `astropy.wcs.BaseLowLevelWCS.axis_correlation_matrix`.
+        Format same as `astropy.wcs.wcsapi.BaseLowLevelWCS.axis_correlation_matrix`.
 
     Returns
     -------
     pixel_axes: `numpy.ndarray`
         The pixel axis indices corresponding to the world axis.
     """
     return np.arange(axis_correlation_matrix.shape[1])[axis_correlation_matrix[world_axis]]
@@ -136,15 +134,15 @@
     Gets the world axis physical types corresponding to a pixel axis.
 
     Parameters
     ----------
     pixel_axis: `int`
         The pixel axis number(s) for which the world axis numbers are desired.
 
-    wcs: `astropy.wcs.BaseLowLevelWCS`
+    wcs: `astropy.wcs.wcsapi.BaseLowLevelWCS`
         The WCS object defining the relationship between pixel and world axes.
 
     Returns
     -------
     physical_types: `numpy.ndarray` of `str`
         The physical types corresponding to the pixel axis.
     """
@@ -156,15 +154,15 @@
     Gets the pixel axis indices corresponding to a world axis physical type.
 
     Parameters
     ----------
     physical_type: `int`
         The pixel axis number(s) for which the world axis numbers are desired.
 
-    wcs: `astropy.wcs.BaseLowLevelWCS`
+    wcs: `astropy.wcs.wcsapi.BaseLowLevelWCS`
         The WCS object defining the relationship between pixel and world axes.
 
     Returns
     -------
     pixel_axes: `numpy.ndarray`
         The pixel axis indices corresponding to the physical type.
     """
@@ -180,16 +178,16 @@
 
     Parameters
     ----------
     physical_type: `str`
         The physical type or a substring unique to a physical type.
 
     world_axis_physical_types: sequence of `str`
-        All available physical types.  Ordering must be same as
-        `astropy.wcs.BaseLowLevelWCS.world_axis_physical_types`
+        All available physical types. Ordering must be same as
+        `astropy.wcs.wcsapi.BaseLowLevelWCS.world_axis_physical_types`
 
     Returns
     -------
     world_axis: `numbers.Integral`
         The world axis index of the physical type.
     """
     # Find world axis index described by physical type.
@@ -227,19 +225,19 @@
     Parameters
     ----------
     wcs_axis: `int`
         Index of axis (in WCS ordering convention) for which dependent axes are desired.
 
     axis_correlation_matrix: `numpy.ndarray` of `bool`
         2D boolean correlation matrix defining the dependence between the pixel and world axes.
-        Format same as `astropy.wcs.BaseLowLevelWCS.axis_correlation_matrix`.
+        Format same as `astropy.wcs.wcsapi.BaseLowLevelWCS.axis_correlation_matrix`.
 
     Returns
     -------
-    dependent_pixel_axes: `np.ndarray` of `int`
+    dependent_pixel_axes: `numpy.ndarray` of `int`
         Sorted indices of pixel axes dependent on input axis in WCS ordering convention.
     """
     # The axis_correlation_matrix is (n_world, n_pixel) but we want to know
     # which pixel coordinates are linked to which other pixel coordinates.
     # To do this we take a column from the matrix and find if there are
     # any entries in common with all other columns in the matrix.
     world_dep = axis_correlation_matrix[:, pixel_axis:pixel_axis + 1]
@@ -265,19 +263,19 @@
     Parameters
     ----------
     array_axis: `int`
         Index of array axis (in numpy ordering convention) for which dependent axes are desired.
 
     axis_correlation_matrix: `numpy.ndarray` of `bool`
         2D boolean correlation matrix defining the dependence between the pixel and world axes.
-        Format same as `astropy.wcs.BaseLowLevelWCS.axis_correlation_matrix`.
+        Format same as `astropy.wcs.wcsapi.BaseLowLevelWCS.axis_correlation_matrix`.
 
     Returns
     -------
-    dependent_array_axes: `np.ndarray` of `int`
+    dependent_array_axes: `numpy.ndarray` of `int`
         Sorted indices of array axes dependent on input axis in numpy ordering convention.
     """
     naxes = axis_correlation_matrix.shape[1]
     pixel_axis = convert_between_array_and_pixel_axes(np.array([array_axis], dtype=int), naxes)[0]
     dependent_pixel_axes = get_dependent_pixel_axes(pixel_axis, axis_correlation_matrix)
     dependent_array_axes = convert_between_array_and_pixel_axes(dependent_pixel_axes, naxes)
     return np.sort(dependent_array_axes)
@@ -293,19 +291,19 @@
     Parameters
     ----------
     world_axis: `int`
         Index of axis (in WCS ordering convention) for which dependent axes are desired.
 
     axis_correlation_matrix: `numpy.ndarray` of `bool`
         2D boolean correlation matrix defining the dependence between the pixel and world axes.
-        Format same as `astropy.wcs.BaseLowLevelWCS.axis_correlation_matrix`.
+        Format same as `astropy.wcs.wcsapi.BaseLowLevelWCS.axis_correlation_matrix`.
 
     Returns
     -------
-    dependent_world_axes: `np.ndarray` of `int`
+    dependent_world_axes: `numpy.ndarray` of `int`
         Sorted indices of pixel axes dependent on input axis in WCS ordering convention.
     """
     # The axis_correlation_matrix is (n_world, n_pixel) but we want to know
     # which world coordinates are linked to which other world coordinates.
     # To do this we take a row from the matrix and find if there are
     # any entries in common with all other rows in the matrix.
     pixel_dep = axis_correlation_matrix[world_axis:world_axis + 1]
@@ -318,20 +316,20 @@
     Given a world axis physical type, return the dependent physical types including the input type.
 
     Parameters
     ----------
     physical_type: `str`
         The world axis physical types whose dependent physical types are desired.
 
-    wcs: `astropy.wcs.BaseLowLevelWCS`
+    wcs: `astropy.wcs.wcsapi.BaseLowLevelWCS`
         The WCS object defining the relationship between pixel and world axes.
 
     Returns
     -------
-    dependent_physical_types: `np.ndarray` of `str`
+    dependent_physical_types: `numpy.ndarray` of `str`
         Physical types dependent on the input physical type.
     """
     world_axis_physical_types = wcs.world_axis_physical_types
     world_axis = physical_type_to_world_axis(physical_type, world_axis_physical_types)
     dependent_world_axes = get_dependent_world_axes(world_axis, wcs.axis_correlation_matrix)
     dependent_physical_types = np.array(world_axis_physical_types)[dependent_world_axes]
     return dependent_physical_types
@@ -416,16 +414,16 @@
     object_names = np.array([wao_comp[0]
                              for wao_comp in wcs.low_level_wcs.world_axis_object_components])
     array_indices = [[]] * len(object_names)
     for world_index, oname in enumerate(object_names):
         # If this world index is deselected by axes= then skip
         if world_index not in world_indices:
             continue
-        # Select the first occurence of the object name.
-        # Other occurences are ignored so as to return duplicate coordinate objects.
+        # Select the first occurrence of the object name.
+        # Other occurrences are ignored so as to return duplicate coordinate objects.
         oinds = np.atleast_1d(object_names == oname).nonzero()[0][0]
         # Calculate the array axes corresponding the coordinate's world axis
         # and enter them into the element of the array indices array corresponding
         # to the relevant world coordinate object.
         pixel_index = world_axis_to_pixel_axes(world_index, wcs.axis_correlation_matrix)
         array_index = convert_between_array_and_pixel_axes(pixel_index, wcs.pixel_n_dim)
         array_indices[oinds] = tuple(array_index[::-1])  # Invert from pixel order to array order
@@ -460,15 +458,15 @@
 def compare_wcs_physical_types(source_wcs, target_wcs):
     """
     Checks to see if two WCS objects have the same physical types in the same order.
 
     Parameters
     ----------
     source_wcs : `astropy.wcs.wcsapi.BaseHighLevelWCS` or `astropy.wcs.wcsapi.BaseLowLevelWCS`
-        The WCS which is currently in use, usually `self.wcs`.
+        The WCS which is currently in use, usually "ndcube.NDCube.wcs".
 
     target_wcs : `astropy.wcs.wcsapi.BaseHighLevelWCS` or `astropy.wcs.wcsapi.BaseLowLevelWCS`
         The WCS object on which the NDCube is to be reprojected.
 
     Returns
     -------
     result : `bool`
```

### Comparing `ndcube-2.1.1/ndcube/utils/wcs_high_level_conversion.py` & `ndcube-2.1.2/ndcube/utils/wcs_high_level_conversion.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/version.py` & `ndcube-2.1.2/ndcube/version.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/visualization/base.py` & `ndcube-2.1.2/ndcube/visualization/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 
     @abc.abstractmethod
     def plot(self, *args, **kwargs):
         """
         The default plot method.
 
         ``Plotter`` classes should provide a ``plot()`` method which is called
-        when users access `.NDCube.plot`. It should strive to provide a good
+        when users access `ndcube.NDCube.plot`. It should strive to provide a good
         overview of the cube by default but the behaviour is left to the
         implementation.
 
         The ``plot()`` method **should** accept ``**kwargs``.
         """
```

### Comparing `ndcube-2.1.1/ndcube/visualization/descriptor.py` & `ndcube-2.1.2/ndcube/visualization/descriptor.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/visualization/mpl_plotter.py` & `ndcube-2.1.2/ndcube/visualization/mpl_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,28 +41,28 @@
             axis.
 
         axes_coordinates: `list`, optional
             A list of length equal to the number of pixel dimensions. For each
             axis the value of the list should either be a string giving the
             world axis type or `None` to use the default axis from the WCS.
 
-        data_unit: `astropy.unit.Unit`
+        data_unit: `astropy.units.Unit`
             The data is changed to the unit given or the ``NDCube.unit`` if not
             given.
 
         wcs: `astropy.wcs.wcsapi.BaseHighLevelWCS`
             The WCS object to define the coordinates of the plot axes.
 
         kwargs :
             Additional keyword arguments are given to the underlying plotting infrastructure
             which depends on the dimensionality of the data and whether 1 or 2 plot_axes are
             defined:
             - Animations: `mpl_animators.ArrayAnimatorWCS`
-            - Static 2-D images: `matplotllib.pyplot.imshow`
-            - Static 1-D line plots: `matplotllib.pyplot.plot`
+            - Static 2-D images: `matplotlib.pyplot.imshow`
+            - Static 1-D line plots: `matplotlib.pyplot.plot`
         """
         naxis = self._ndcube.wcs.pixel_n_dim
 
         if not axes_coordinates:
             axes_coordinates = [...]
             plot_wcs = self._ndcube.wcs.low_level_wcs
         else:
```

### Comparing `ndcube-2.1.1/ndcube/visualization/mpl_sequence_plotter.py` & `ndcube-2.1.2/ndcube/visualization/mpl_sequence_plotter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from astropy.wcs.wcsapi import BaseLowLevelWCS
 from mpl_animators import ArrayAnimatorWCS
 
 from .base import BasePlotter
 from .plotting_utils import prep_plot_kwargs
 
-__all__ = ['MatplotlibSequencePlotter']
+__all__ = ['MatplotlibSequencePlotter', 'SequenceAnimator']
 
 
 class MatplotlibSequencePlotter(BasePlotter):
     """
     Provide visualization methods for NDCubeSequence which use `matplotlib`.
 
     This plotter delegates much of the visualization to the `ndcube.NDCube.plot`
@@ -17,48 +17,48 @@
 
     def plot(self, sequence_axis_coords=None, sequence_axis_unit=None, **kwargs):
         """
         Visualize the `~ndcube.NDCubeSequence`.
 
         Parameters
         ----------
-        sequence_axis_coords: `str` or array-like (optional)
+        sequence_axis_coords: `str` or array-like, optional
             The real world value of each step along the sequene axis.
             If `str`, the values are taken from `ndcube.NDCubeSequence.sequence_axis_coords`.
 
-        sequence_axis_unit: `str` or `astropy.units.Unit` (optional)
+        sequence_axis_unit: `str` or `astropy.units.Unit`, optional
             The unit in which to display the sequence_axis_coords.
         """
         sequence_dims = self._ndcube.dimensions
         if len(sequence_dims) == 2:
             raise NotImplementedError("Visualizing sequences of 1-D cubes not currently supported.")
         else:
             return self.animate(sequence_axis_coords, sequence_axis_unit, **kwargs)
 
     def animate(self, sequence_axis_coords=None, sequence_axis_unit=None, **kwargs):
         """
         Animate the `~ndcube.NDCubeSequence` with the sequence axis as a slider.
 
-        **kwargs are passed to
+        Keyword arguments are passed to
         `ndcube.visualization.mpl_plotter.MatplotlibPlotter.plot` and therefore only
         apply to cube axes, not the sequence axis.
-        See that method's docstring for definition of **kwargs.
+        See that method's docstring for definition of keyword arguments.
 
         Parameters
         ----------
         sequence_axis_coords: `str` optional
             The name of the coordinate in `~ndcube.NDCubeSequence.sequence_axis_coords`
             to be used as the slider pixel values.
             If None, array indices will be used.
 
-        sequence_axis_units: `astropy.units.Unit` or `str` (optional)
+        sequence_axis_units: `astropy.units.Unit` or `str`, optional
             The unit in which the sequence_axis_coordinates should be displayed.
             If None, the default unit will be used.
         """
-        return SequenceAnimator(self._ndcube, sequence_axis_coords=None, sequence_axis_unit=None, **kwargs)
+        return SequenceAnimator(self._ndcube, sequence_axis_coords=sequence_axis_coords, sequence_axis_unit=sequence_axis_unit, **kwargs)
 
 
 class SequenceAnimator(ArrayAnimatorWCS):
     """
     Animate an NDCubeSequence of NDCubes with >1 dimension.
 
     The sequence axis is always set as a sliders axis.
@@ -67,19 +67,19 @@
     which is assumed to exist and to call a matplotlib-based animator.
 
     Parameters
     ----------
     sequence: `~ndcube.NDCubeSequence`
         The sequence to animate.
 
-    sequence_axis_coords: `str` or array-like (optional)
+    sequence_axis_coords: `str` or array-like, optional
         The real world value of each step along the sequene axis.
         If `str`, the values are taken from `ndcube.NDCubeSequence.sequence_axis_coords`.
 
-    sequence_axis_unit: `str` or `astropy.units.Unit` (optional)
+    sequence_axis_unit: `str` or `astropy.units.Unit`, optional
         The unit in which to display the sequence_axis_coords.
     """
 
     def __init__(self, sequence, sequence_axis_coords=None, sequence_axis_unit=None, **kwargs):
         if sequence_axis_coords is not None:
             raise NotImplementedError("Setting sequence_axis_coords not yet supported.")
         if sequence_axis_unit is not None:
@@ -109,13 +109,13 @@
             self._cubes[0].wcs, self._plot_axes, self._axes_units, self._data_unit)
         if not isinstance(wcs, BaseLowLevelWCS):
             wcs = wcs.low_level_wcs
         super().__init__(data, wcs, plot_axes, coord_params=coord_params, **base_kwargs)
 
     def _sequence_slider_function(self, val, artist, slider):
         self._sequence_idx = int(val)
-        self.data, self.wcs, _plot_axes, _coord_params = self._cubes[self._sequence_idx].plotter._prep_animate_args(
+        self.data, self.wcs, _, _ = self._cubes[self._sequence_idx].plotter._prep_animate_args(
             self._cubes[self._sequence_idx].wcs, self._plot_axes, self._axes_units, self._data_unit)
         if self.plot_dimensionality == 1:
             self.update_plot_1d(val, artist, slider)
         elif self.plot_dimensionality == 2:
             self.update_plot_2d(val, artist, slider)
```

### Comparing `ndcube-2.1.1/ndcube/visualization/plotting_utils.py` & `ndcube-2.1.2/ndcube/visualization/plotting_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import astropy.units as u
 
+__all__ = ['prep_plot_kwargs', 'set_wcsaxes_format_units']
+
 
 def _expand_ellipsis(ndim, plist):
     if Ellipsis in plist:
         if plist.count(Ellipsis) > 1:
             raise IndexError("Only single ellipsis ('...') is permitted.")
 
         # Replace the Ellipsis with the correct number of slice(None)s
```

### Comparing `ndcube-2.1.1/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json` & `ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_353_ft_261_astropy_51_animators_100.json`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json` & `ndcube-2.1.2/ndcube/visualization/tests/figure_hashes_mpl_dev_ft_261_astropy_dev_animators_dev.json`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/visualization/tests/test_plotting.py` & `ndcube-2.1.2/ndcube/visualization/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/visualization/tests/test_plotting_utils.py` & `ndcube-2.1.2/ndcube/visualization/tests/test_plotting_utils.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/wcs/wrappers/compound_wcs.py` & `ndcube-2.1.2/ndcube/wcs/wrappers/compound_wcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     This is a very stripped down version of `astropy.modeling.models.Mapping`
     to be able to handle input of arbitrary type.
 
     Parameters
     ----------
     mapping : tuple
         A tuple of integers representing indices of the inputs to this model
-        to return and in what order to return them.  See
+        to return and in what order to return them. See
         :ref:`compound-model-mappings` for more details.
 
     """
 
     def __init__(self, mapping):
         self.mapping = mapping
         self.n_inputs = max(mapping) + 1
```

### Comparing `ndcube-2.1.1/ndcube/wcs/wrappers/reordered_wcs.py` & `ndcube-2.1.2/ndcube/wcs/wrappers/reordered_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/wcs/wrappers/resampled_wcs.py` & `ndcube-2.1.2/ndcube/wcs/wrappers/resampled_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/wcs/wrappers/tests/test_compound_wcs.py` & `ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_compound_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/wcs/wrappers/tests/test_reordered_wcs.py` & `ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_reordered_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube/wcs/wrappers/tests/test_resampled_wcs.py` & `ndcube-2.1.2/ndcube/wcs/wrappers/tests/test_resampled_wcs.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/ndcube.egg-info/PKG-INFO` & `ndcube-2.1.2/ndcube.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ndcube
-Version: 2.1.1
-Summary: A package for multi-dimensional contiguious and non-contiguious coordinate aware arrays.
+Version: 2.1.2
+Summary: A package for multi-dimensional contiguous and non-contiguous coordinate aware arrays.
 Home-page: https://docs.sunpy.org/projects/ndcube/
 Download-URL: https://pypi.org/project/ndcube/
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Project-URL: Source Code, https://github.com/sunpy/ndcube/
 Project-URL: Documentation, https://docs.sunpy.org/projects/ndcube/
@@ -42,15 +42,15 @@
 
 |Latest Version| |codecov| |matrix| |Powered by NumFOCUS| |Powered by SunPy|
 
 .. |Latest Version| image:: https://img.shields.io/pypi/v/ndcube.svg
    :target: https://pypi.python.org/pypi/ndcube/
    :alt: It is up to date, we promise
 .. |matrix| image:: https://img.shields.io/matrix/ndcube:openastronomy.org.svg?colorB=%23FE7900&label=Chat&logo=matrix&server_fqdn=openastronomy.modular.im
-   :target: https://openastronomy.element.io/#/room/#ndcube:openastronomy.org
+   :target: https://app.element.io/#/room/#ndcube:openastronomy.org
    :alt: join us on #ndcube:openastronom.org on matrix
 .. |codecov| image:: https://codecov.io/gh/sunpy/ndcube/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/sunpy/sunpy
    :alt: Best code cov this side of mars
 .. |Powered by NumFOCUS| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: https://numfocus.org
    :alt: Go give them money
```

### Comparing `ndcube-2.1.1/ndcube.egg-info/SOURCES.txt` & `ndcube-2.1.2/ndcube.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,38 +5,47 @@
 MANIFEST.in
 README.rst
 RELEASE.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+docs/1_to_2_transition_guide.rst
 docs/Makefile
-docs/api.rst
 docs/conf.py
-docs/coordinates.rst
-docs/data_classes.rst
 docs/extending_ndcube.rst
 docs/index.rst
 docs/installation.rst
 docs/introduction.rst
 docs/make.bat
 docs/nitpick-exceptions
-docs/reproject.rst
 docs/rtd_requirements.txt
-docs/slicing.rst
-docs/tabular_coordinates.rst
-docs/visualization.rst
-docs/images/ndcollection_diagram.png
-docs/images/ndcube_diagram.png
-docs/images/ndcube_sliced_diagram.png
-docs/images/ndcubesequence_diagram.png
-docs/images/ndcubesequence_sliced_diagram.png
+docs/explaining_ndcube/coordinates.rst
+docs/explaining_ndcube/data_classes.rst
+docs/explaining_ndcube/index.rst
+docs/explaining_ndcube/reproject.rst
+docs/explaining_ndcube/slicing.rst
+docs/explaining_ndcube/tabular_coordinates.rst
+docs/explaining_ndcube/visualization.rst
+docs/explaining_ndcube/images/ndcollection_diagram.png
+docs/explaining_ndcube/images/ndcube_diagram.png
+docs/explaining_ndcube/images/ndcube_sliced_diagram.png
+docs/explaining_ndcube/images/ndcubesequence_diagram.png
+docs/explaining_ndcube/images/ndcubesequence_sliced_diagram.png
 docs/logo/favicon.png
 docs/logo/ndcube.png
 docs/logo/ndcube.svg
+docs/reference/extra_coords.rst
+docs/reference/index.rst
+docs/reference/mixins.rst
+docs/reference/ndcube.rst
+docs/reference/tests.rst
+docs/reference/utils.rst
+docs/reference/visualization.rst
+docs/reference/wcs.rst
 docs/whatsnew/changelog.rst
 docs/whatsnew/index.rst
 examples/README.txt
 examples/creating_ndcube_from_fitsfile.py
 examples/slicing_ndcube.py
 examples/dev/example_template.py
 licenses/README.rst
```

### Comparing `ndcube-2.1.1/ndcube.egg-info/requires.txt` & `ndcube-2.1.2/ndcube.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,27 @@
 pytest-doctestplus>=0.9.0
 sphinx
 sphinx-automodapi
 sphinx-changelog>=1.1.0
 sphinx-gallery
 sphinxext-opengraph
 sunpy-sphinx-theme
-towncrier<22.12.0
 matplotlib>=3.2
 mpl_animators>=1.0
 reproject>=0.7.1
 
 [docs]
 matplotlib
 pytest-doctestplus>=0.9.0
 sphinx
 sphinx-automodapi
 sphinx-changelog>=1.1.0
 sphinx-gallery
 sphinxext-opengraph
 sunpy-sphinx-theme
-towncrier<22.12.0
 sunpy>=4.0.0
 
 [plotting]
 matplotlib>=3.2
 mpl_animators>=1.0
 
 [reproject]
```

### Comparing `ndcube-2.1.1/pyproject.toml` & `ndcube-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/setup.cfg` & `ndcube-2.1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 url = https://docs.sunpy.org/projects/ndcube/
 download_url = https://pypi.org/project/ndcube/
 project_urls = 
 	Source Code = https://github.com/sunpy/ndcube/
 	Documentation = https://docs.sunpy.org/projects/ndcube/
 	Changelog = https://docs.sunpy.org/projects/ndcube/en/stable/whatsnew/changelog.html
 	Issue Tracker = https://github.com/sunpy/ndcube/issues
-description = A package for multi-dimensional contiguious and non-contiguious coordinate aware arrays.
+description = A package for multi-dimensional contiguous and non-contiguous coordinate aware arrays.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 edit_on_github = True
 github_project = sunpy/ndcube
 platform = any
 keywords = nddata, science, sun, wcs, gwcs, coordinates, sunpy, astropy, solar, spectroscopy
 classifiers = 
@@ -56,15 +56,14 @@
 	pytest-doctestplus>=0.9.0
 	sphinx
 	sphinx-automodapi
 	sphinx-changelog>=1.1.0
 	sphinx-gallery
 	sphinxext-opengraph
 	sunpy-sphinx-theme
-	towncrier<22.12.0
 	sunpy>=4.0.0
 plotting = 
 	matplotlib>=3.2
 	mpl_animators>=1.0
 reproject = 
 	reproject>=0.7.1
 
@@ -139,11 +138,22 @@
 	pragma: no cover
 	except ImportError
 	raise AssertionError
 	raise NotImplementedError
 	def main\(.*\):
 	pragma: py{ignore_python_version}
 
+[codespell]
+skip = *.asdf,*.fits,*.fts,*.header,*.json,*.xsh,*cache*,*egg*,*extern*,.git,.idea,.tox,_build,*truncated,*.,*svg,*.bib
+ignore-words-list = 
+	alog,
+	nd,
+	nin,
+	observ,
+	ot,
+	te,
+	upto
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ndcube-2.1.1/setup.py` & `ndcube-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `ndcube-2.1.1/tox.ini` & `ndcube-2.1.2/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     devdeps: matplotlib>=0.0dev0
     devdeps: git+https://github.com/sunpy/sunpy
     devdeps: git+https://github.com/sunpy/mpl-animators
     devdeps: git+https://github.com/spacetelescope/gwcs
     # These are specific online extras we use to run the online tests.
     online: pytest-rerunfailures
     online: pytest-timeout
-    # Oldest Dependancies
+    # Oldest Dependencies
     oldestdeps: sunpy<4.0
     oldestdeps: astropy<4.3
     oldestdeps: gwcs<0.16
     oldestdeps: numpy<1.18
     oldestdeps: matplotlib<3.3
     oldestdeps: mpl_animators<1.1
     oldestdeps: reproject==0.7.1
```

