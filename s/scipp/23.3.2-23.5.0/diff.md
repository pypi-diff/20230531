# Comparing `tmp/scipp-23.3.2.tar.gz` & `tmp/scipp-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipp-23.3.2.tar", last modified: Wed Apr 12 09:46:59 2023, max compression
+gzip compressed data, was "scipp-23.5.0.tar", last modified: Wed May 31 10:20:11 2023, max compression
```

## Comparing `scipp-23.3.2.tar` & `scipp-23.5.0.tar`

### file list

```diff
@@ -1,160 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-12 09:46:36.000000 scipp-23.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-04-12 09:46:59.716752 scipp-23.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-12 09:46:36.000000 scipp-23.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.700752 scipp-23.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/_binding.py
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/_scipp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/binning/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/binning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/compat/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5935 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/pandas_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/compat/xarray_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/configuration/config_default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/constants/
--rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.704752 scipp-23.3.2/src/scipp/coords/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/coord.py
--rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/coord_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5211 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     7528 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/rule.py
--rw-r--r--   0 runner    (1001) docker     (122)    12893 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/coords/transform_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/core/
--rw-r--r--   0 runner    (1001) docker     (122)     3653 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/_cpp_wrapper_util.py
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/_sizes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/bin_remapping.py
--rw-r--r--   0 runner    (1001) docker     (122)    26466 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/binning.py
--rw-r--r--   0 runner    (1001) docker     (122)    17954 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/bins.py
--rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/concepts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/cpp_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    41780 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/cpp_classes.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/cumulative.py
--rw-r--r--   0 runner    (1001) docker     (122)    19386 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/data_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5712 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/domains.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/groupby.py
--rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/like.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/logical.py
--rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/math.py
--rw-r--r--   0 runner    (1001) docker     (122)     9671 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/reduction.py
--rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/shape.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/structured.py
--rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/trigonometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/unary.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    29249 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/core/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/data/
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/extend_units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/format/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/format/_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     7534 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/format/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.708752 scipp-23.3.2/src/scipp/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/formatting_datagroup_html.py
--rw-r--r--   0 runner    (1001) docker     (122)    16472 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/formatting_html.py
--rw-r--r--   0 runner    (1001) docker     (122)     3221 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     7211 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/html/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/datagroup.css
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_atomic_row.html
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_collapsible_row.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_detail_list.html
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/dg_repr.html
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/icons-svg-inline.html
--rw-r--r--   0 runner    (1001) docker     (122)     9794 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/html/templates/style.css.template
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/io/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14803 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (122)     8046 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/object_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     6496 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12585 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/controller3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1278 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/displayable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure.py
--rw-r--r--   0 runner    (1001) docker     (122)    12821 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure2d.py
--rw-r--r--   0 runner    (1001) docker     (122)    17551 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/figure3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     8403 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/model3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    12741 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/panel.py
--rw-r--r--   0 runner    (1001) docker     (122)     3903 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/panel1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/panel3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/profile.py
--rw-r--r--   0 runner    (1001) docker     (122)    13330 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/resampling_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    10875 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view.py
--rw-r--r--   0 runner    (1001) docker     (122)     4109 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     6575 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/view3d.py
--rw-r--r--   0 runner    (1001) docker     (122)    13182 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/widgets.py
--rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/plotting/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/scipy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.712752 scipp-23.3.2/src/scipp/scipy/integrate/
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/integrate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/interpolate/
--rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/interpolate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/ndimage/
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/ndimage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (122)     8944 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/optimize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/scipy/signal/
--rw-r--r--   0 runner    (1001) docker     (122)     5097 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/scipy/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)    19028 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/spatial/
--rw-r--r--   0 runner    (1001) docker     (122)    11951 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/spatial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/sphinxext/autoplot.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5042 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/testing/assertions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7749 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/testing/strategies.py
--rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/units/
--rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:46:59.716752 scipp-23.3.2/src/scipp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/collapse_and_slices.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/profile.py
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/pyshell.py
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-04-12 09:46:36.000000 scipp-23.3.2/src/scipp/utils/to_string.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-05-31 10:19:47.000000 scipp-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2023-05-31 10:20:11.965467 scipp-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-31 10:19:47.000000 scipp-23.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.949467 scipp-23.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/
+-rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3496 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/_binding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/_scipp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/binning/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/binning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5935 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/pandas_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/compat/xarray_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/configuration/config_default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)     4941 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.953467 scipp-23.5.0/src/scipp/coords/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/coord.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2601 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/coord_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5211 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7528 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/rule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12893 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/coords/transform_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     3967 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/_cpp_wrapper_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/argument_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5742 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/assignments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/bin_remapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26466 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/binning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18006 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/bins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8807 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/cpp_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42413 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/cpp_classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21420 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/data_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/domains.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5258 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/logical.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9671 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8907 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/shape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/structured.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3782 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/trigonometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/unary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29249 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/core/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/extend_units.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/format/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/format/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7534 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/format/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.957467 scipp-23.5.0/src/scipp/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/formatting_datagroup_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16472 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/formatting_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3221 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7211 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.961467 scipp-23.5.0/src/scipp/html/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3254 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/datagroup.css
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_atomic_row.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_collapsible_row.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_detail_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/dg_repr.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/icons-svg-inline.html
+-rw-r--r--   0 runner    (1001) docker     (122)     9794 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/html/templates/style.css.template
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.961467 scipp-23.5.0/src/scipp/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15758 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8046 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/object_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.961467 scipp-23.5.0/src/scipp/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     6496 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12585 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/controller3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1278 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/displayable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12821 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5401 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17551 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/figure3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8403 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/model3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12741 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/panel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3903 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/panel1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/panel3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3002 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13330 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/resampling_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10875 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4109 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6575 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13182 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6713 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/plotting/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/integrate/
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/integrate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/interpolate/
+-rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/interpolate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/ndimage/
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/ndimage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (122)     8944 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/optimize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/scipy/signal/
+-rw-r--r--   0 runner    (1001) docker     (122)     5097 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/scipy/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19028 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/spatial/
+-rw-r--r--   0 runner    (1001) docker     (122)    11951 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/spatial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4183 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/sphinxext/autoplot.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5042 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/testing/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7749 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/testing/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/units/
+-rw-r--r--   0 runner    (1001) docker     (122)     6561 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 10:20:11.965467 scipp-23.5.0/src/scipp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/collapse_and_slices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/pyshell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-31 10:19:47.000000 scipp-23.5.0/src/scipp/utils/to_string.py
```

### Comparing `scipp-23.3.2/LICENSE` & `scipp-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/PKG-INFO` & `scipp-23.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipp
-Version: 23.3.2
+Version: 23.5.0
 Summary: Multi-dimensional data arrays with labeled dimensions
 Home-page: https://github.com/scipp/scipp
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD-3-Clause
 Project-URL: Documentation, https://scipp.github.io/
 Project-URL: Bug Tracker, https://github.com/scipp/scipp/issues
 Project-URL: Changelog, https://scipp.github.io/about/release-notes.html
```

### Comparing `scipp-23.3.2/src/scipp/__init__.py` & `scipp-23.5.0/src/scipp/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/_binding.py` & `scipp-23.5.0/src/scipp/_binding.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/compat/dict.py` & `scipp-23.5.0/src/scipp/compat/dict.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/compat/pandas_compat.py` & `scipp-23.5.0/src/scipp/compat/pandas_compat.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/compat/wrapping.py` & `scipp-23.5.0/src/scipp/compat/wrapping.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/compat/xarray_compat.py` & `scipp-23.5.0/src/scipp/compat/xarray_compat.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/configuration/__init__.py` & `scipp-23.5.0/src/scipp/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/configuration/config_default.yaml` & `scipp-23.5.0/src/scipp/configuration/config_default.yaml`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/constants/__init__.py` & `scipp-23.5.0/src/scipp/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/coords/coord.py` & `scipp-23.5.0/src/scipp/coords/coord.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/coords/coord_table.py` & `scipp-23.5.0/src/scipp/coords/coord_table.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/coords/graph.py` & `scipp-23.5.0/src/scipp/coords/graph.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/coords/rule.py` & `scipp-23.5.0/src/scipp/coords/rule.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/coords/transform_coords.py` & `scipp-23.5.0/src/scipp/coords/transform_coords.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/__init__.py` & `scipp-23.5.0/src/scipp/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 # __array_ufunc__ should be possible by converting non-scipp arguments to
 # variables. The most difficult part is probably mapping the ufunc to scipp
 # functions.
 for _cls in (Variable, DataArray, Dataset):
     setattr(_cls, '__array_ufunc__', None)
 del _cls
 
+
 from .arithmetic import add, divide, floor_divide, mod, multiply, negative, subtract
 from .binning import bin, group, hist, nanhist, rebin
 from .bins import lookup, bins, bins_like
 from .comparison import (
     less,
     greater,
     less_equal,
@@ -155,7 +156,15 @@
     logspace,
     arange,
     datetime,
     datetimes,
     epoch,
 )
 from .like import zeros_like, ones_like, empty_like, full_like
+
+from .assignments import assign_coords, assign_masks, assign_attrs
+
+setattr(Dataset, 'assign_coords', assign_coords)
+setattr(DataArray, 'assign_coords', assign_coords)
+setattr(DataArray, 'assign_masks', assign_masks)
+setattr(DataArray, 'assign_attrs', assign_attrs)
+del assign_coords, assign_masks, assign_attrs
```

### Comparing `scipp-23.3.2/src/scipp/core/_cpp_wrapper_util.py` & `scipp-23.5.0/src/scipp/core/_cpp_wrapper_util.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/_sizes.py` & `scipp-23.5.0/src/scipp/core/_sizes.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/arithmetic.py` & `scipp-23.5.0/src/scipp/core/arithmetic.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/bin_remapping.py` & `scipp-23.5.0/src/scipp/core/bin_remapping.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/binning.py` & `scipp-23.5.0/src/scipp/core/binning.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/bins.py` & `scipp-23.5.0/src/scipp/core/bins.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,27 +85,27 @@
       >>> vals = sc.array(dims=['x'], values=[3, 2, 1])
       >>> hist = sc.DataArray(data=vals, coords={'x': x})
       >>> sc.lookup(hist, 'x')[sc.array(dims=['event'], values=[0.1,0.4,0.1,0.6,0.9])]
       <scipp.Variable> (event: 5)      int64  [dimensionless]  [3, 2, ..., 2, 1]
     """
     if dim is None:
         dim = func.dim
-    if func.meta.is_edges(dim):
+    func = _cpp.DataArray(func.data, coords={dim: func.meta[dim]}, masks=func.masks)
+    if func.coords.is_edges(dim):
         if mode is not None:
             raise ValueError("Input is a histogram, 'mode' must not be set.")
         return Lookup(_cpp.buckets.map, func, dim, fill_value)
     if mode is None:
         mode = 'nearest'
     elif mode not in ['previous', 'nearest']:
-        raise ValueError(f"Mode most be one of ['previous', 'nearest'], got '{mode}'")
+        raise ValueError(f"Mode must be one of ['previous', 'nearest'], got '{mode}'")
     if mode == 'nearest' and func.sizes[dim] != 0:
-        coord = func.meta[dim]
+        coord = func.coords[dim]
         lowest = coord[dim, 0:0].max()  # trick to get lowest representable value
         parts = [lowest] if coord.sizes[dim] < 2 else [lowest, midpoints(coord, dim)]
-        func = func.copy(deep=False)
         func.coords[dim] = concat(parts, dim)
     return Lookup(_cpp.lookup_previous, func, dim, fill_value)
 
 
 class Bins:
     """Proxy for access to bin contents and operations on bins of a variable.
```

### Comparing `scipp-23.3.2/src/scipp/core/comparison.py` & `scipp-23.5.0/src/scipp/core/comparison.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/concepts.py` & `scipp-23.5.0/src/scipp/core/concepts.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/counts.py` & `scipp-23.5.0/src/scipp/core/counts.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/cpp_classes.pyi` & `scipp-23.5.0/src/scipp/core/cpp_classes.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,17 @@
 
     def pop(self, key, default=_NoDefault):
         ...
 
     def popitem(self) -> Tuple[str, Any]:
         ...
 
+    def set_aligned(self, key: str, aligned: bool) -> None:
+        ...
+
     def update(self, other: Any=None, /, **kwargs) -> None:
         ...
 
     def values(self) -> Coords_values_view:
         ...
 
 class Coords_items_view:
@@ -614,14 +617,23 @@
 
     def all(self, dim: Optional[str]=None) -> VariableLikeType:
         ...
 
     def any(self, dim: Optional[str]=None) -> VariableLikeType:
         ...
 
+    def assign_attrs(self, attrs: Optional[Dict[str, Variable]]=None, /, **attrs_kwargs) -> DataArray:
+        ...
+
+    def assign_coords(self, coords: Optional[Dict[str, Variable]]=None, /, **coords_kwargs) -> Union[DataArray, Dataset]:
+        ...
+
+    def assign_masks(self, masks: Optional[Dict[str, Variable]]=None, /, **masks_kwargs) -> DataArray:
+        ...
+
     def astype(self, type: Any, *, copy: bool=True) -> DataArray:
         ...
 
     @property
     def attrs(self) -> Coords:
         ...
 
@@ -1082,14 +1094,17 @@
 
     def all(self, dim: Optional[str]=None) -> VariableLikeType:
         ...
 
     def any(self, dim: Optional[str]=None) -> VariableLikeType:
         ...
 
+    def assign_coords(self, coords: Optional[Dict[str, Variable]]=None, /, **coords_kwargs) -> Union[DataArray, Dataset]:
+        ...
+
     @property
     def bins(self):
         ...
 
     @bins.setter
     def bins(self, bins: Bins):
         ...
@@ -1845,14 +1860,18 @@
 
     def _rename_dims(self, arg0: Dict[str, str]) -> Variable:
         ...
 
     def _repr_html_(self) -> str:
         ...
 
+    @property
+    def aligned(self) -> bool:
+        ...
+
     def all(self, dim: Optional[str]=None) -> VariableLikeType:
         ...
 
     def any(self, dim: Optional[str]=None) -> VariableLikeType:
         ...
 
     def astype(self, type: Any, *, copy: bool=True) -> Variable:
```

### Comparing `scipp-23.3.2/src/scipp/core/cumulative.py` & `scipp-23.5.0/src/scipp/core/cumulative.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/data_group.py` & `scipp-23.5.0/src/scipp/core/data_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,41 @@
     cast,
     overload,
 )
 
 import numpy as np
 
 from .. import _binding
-from .cpp_classes import DataArray, Dataset, DimensionError, Variable
+from .cpp_classes import (
+    DataArray,
+    Dataset,
+    DimensionError,
+    GroupByDataArray,
+    GroupByDataset,
+    Variable,
+)
 
 if TYPE_CHECKING:
     # typing imports data_group.
     # So the following import would create a cycle at runtime.
     from ..typing import ScippIndex
 
 
 def _item_dims(item):
     return getattr(item, 'dims', ())
 
 
+def _is_binned(item):
+    from .bins import Bins
+
+    if isinstance(item, Bins):
+        return True
+    return hasattr(item, 'bins') and item.bins is not None
+
+
 def _summarize(item):
     if isinstance(item, DataGroup):
         return f'{type(item).__name__}({len(item)}, {item.sizes})\n'
     if hasattr(item, 'sizes'):
         return f'{type(item).__name__}({item.sizes})\n'
     return str(item)
 
@@ -229,103 +244,156 @@
         # property provides a different set of attrs and methods.
         return self.apply(operator.attrgetter('bins'))
 
     def apply(self, func: Callable, *args, **kwargs) -> DataGroup:
         """Call func on all values and return new DataGroup containing the results."""
         return DataGroup({key: func(v, *args, **kwargs) for key, v in self.items()})
 
+    def _transform_dim(
+        self, func: Callable, *, dim: Union[None, str, Iterable[str]], **kwargs
+    ) -> DataGroup:
+        """Transform items that depend on one or more dimensions given by `dim`."""
+        dims = (dim,) if isinstance(dim, str) else dim
+
+        def intersects(item):
+            item_dims = _item_dims(item)
+            if dims is None:
+                return item_dims != ()
+            return set(dims).intersection(item_dims) != set()
+
+        return DataGroup(
+            {
+                key: v
+                if not intersects(v)
+                else operator.methodcaller(func, dim, **kwargs)(v)
+                for key, v in self.items()
+            }
+        )
+
+    def _reduce(
+        self, method: str, dim: Union[None, str, Tuple[str, ...]] = None, **kwargs
+    ) -> DataGroup:
+        reduce_all = operator.methodcaller(method, **kwargs)
+
+        def _reduce_child(v, dim):
+            if isinstance(v, (GroupByDataArray, GroupByDataset)):
+                child_dims = (dim,)
+            else:
+                child_dims = _item_dims(v)
+            # Reduction operations on binned data implicitly reduce over bin content.
+            # Therefore, a purely dimension-based logic is not sufficient to determine
+            # if the item has to be reduced or not.
+            binned = _is_binned(v)
+            if child_dims == () and not binned:
+                return v
+            if dim is None:
+                return reduce_all(v)
+            if isinstance(dim, str):
+                dims_to_reduce = dim if dim in child_dims else ()
+            else:
+                dims_to_reduce = tuple(d for d in dim if d in child_dims)
+            if dims_to_reduce == () and binned:
+                return reduce_all(v)
+            return (
+                v
+                if dims_to_reduce == tuple()
+                else operator.methodcaller(method, dims_to_reduce, **kwargs)(v)
+            )
+
+        return DataGroup({key: _reduce_child(v, dim) for key, v in self.items()})
+
     def copy(self, deep: bool = True) -> DataGroup:
         return copy.deepcopy(self) if deep else copy.copy(self)
 
     def all(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('all', *args, **kwargs))
+        return self._reduce('all', *args, **kwargs)
 
     def any(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('any', *args, **kwargs))
+        return self._reduce('any', *args, **kwargs)
 
     def astype(self, *args, **kwargs):
         return self.apply(operator.methodcaller('astype', *args, **kwargs))
 
     def bin(self, *args, **kwargs):
         return self.apply(operator.methodcaller('bin', *args, **kwargs))
 
     def broadcast(self, *args, **kwargs):
         return self.apply(operator.methodcaller('broadcast', *args, **kwargs))
 
     def ceil(self, *args, **kwargs):
         return self.apply(operator.methodcaller('ceil', *args, **kwargs))
 
-    def flatten(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('flatten', *args, **kwargs))
+    def flatten(self, dims: Union[None, Iterable[str]] = None, **kwargs):
+        return self._transform_dim('flatten', dim=dims, **kwargs)
 
     def floor(self, *args, **kwargs):
         return self.apply(operator.methodcaller('floor', *args, **kwargs))
 
-    def fold(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('fold', *args, **kwargs))
+    def fold(self, dim: str, **kwargs):
+        return self._transform_dim('fold', dim=dim, **kwargs)
 
     def group(self, *args, **kwargs):
         return self.apply(operator.methodcaller('group', *args, **kwargs))
 
     def groupby(self, *args, **kwargs):
         return self.apply(operator.methodcaller('groupby', *args, **kwargs))
 
     def hist(self, *args, **kwargs):
         return self.apply(operator.methodcaller('hist', *args, **kwargs))
 
     def max(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('max', *args, **kwargs))
+        return self._reduce('max', *args, **kwargs)
 
     def mean(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('mean', *args, **kwargs))
+        return self._reduce('mean', *args, **kwargs)
 
     def min(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('min', *args, **kwargs))
+        return self._reduce('min', *args, **kwargs)
 
     def nanhist(self, *args, **kwargs):
         return self.apply(operator.methodcaller('nanhist', *args, **kwargs))
 
     def nanmax(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('nanmax', *args, **kwargs))
+        return self._reduce('nanmax', *args, **kwargs)
 
     def nanmean(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('nanmean', *args, **kwargs))
+        return self._reduce('nanmean', *args, **kwargs)
 
     def nanmin(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('nanmin', *args, **kwargs))
+        return self._reduce('nanmin', *args, **kwargs)
 
     def nansum(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('nansum', *args, **kwargs))
+        return self._reduce('nansum', *args, **kwargs)
 
     def rebin(self, *args, **kwargs):
         return self.apply(operator.methodcaller('rebin', *args, **kwargs))
 
     def rename(self, *args, **kwargs):
         return self.apply(operator.methodcaller('rename', *args, **kwargs))
 
     def rename_dims(self, *args, **kwargs):
         return self.apply(operator.methodcaller('rename_dims', *args, **kwargs))
 
     def round(self, *args, **kwargs):
         return self.apply(operator.methodcaller('round', *args, **kwargs))
 
     def squeeze(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('squeeze', *args, **kwargs))
+        return self._reduce('squeeze', *args, **kwargs)
 
     def sum(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('sum', *args, **kwargs))
+        return self._reduce('sum', *args, **kwargs)
 
     def to(self, *args, **kwargs):
         return self.apply(operator.methodcaller('to', *args, **kwargs))
 
     def transform_coords(self, *args, **kwargs):
         return self.apply(operator.methodcaller('transform_coords', *args, **kwargs))
 
-    def transpose(self, *args, **kwargs):
-        return self.apply(operator.methodcaller('transpose', *args, **kwargs))
+    def transpose(self, dims: Union[None, Tuple[str, ...]] = None):
+        return self._transform_dim('transpose', dim=dims)
 
     def plot(self, *args, **kwargs):
         import plopp
 
         return plopp.plot(self, *args, **kwargs)
 
     def __eq__(
```

### Comparing `scipp-23.3.2/src/scipp/core/dataset.py` & `scipp-23.5.0/src/scipp/core/dataset.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/dimensions.py` & `scipp-23.5.0/src/scipp/core/dimensions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 # @author Simon Heybrock
 from typing import Dict, Optional
 
 from .._scipp.core import CoordError, DataArray, Dataset, Variable
 from ..typing import VariableLikeType
+from .argument_handlers import combine_dict_args
 from .bins import bins
 from .operations import merge
 
 
-def _combine_dims(
-    dims_dict: Optional[Dict[str, str]], names: Dict[str, str]
-) -> Dict[str, str]:
-    dims_dict = {} if dims_dict is None else dims_dict
-    if set(dims_dict).intersection(names):
-        raise ValueError(
-            'The names passed in the dict and as keyword arguments must be distinct.'
-            f'Got {dims_dict} and {names}'
-        )
-    return {**dims_dict, **names}
-
-
 def _rename_dims(
     self: VariableLikeType, dims_dict: Optional[Dict[str, str]] = None, /, **names: str
 ) -> VariableLikeType:
     """Rename dimensions.
 
     The renaming can be defined:
 
@@ -47,15 +36,15 @@
         Mapping of old to new names as keyword arguments.
 
     Returns
     -------
     :
         A new object with renamed dimensions.
     """
-    return self._rename_dims(_combine_dims(dims_dict, names))
+    return self._rename_dims(combine_dict_args(dims_dict, names))
 
 
 def _rename_variable(
     var: Variable, dims_dict: Dict[str, str] = None, /, **names: str
 ) -> Variable:
     """Rename dimension labels.
 
@@ -81,15 +70,15 @@
         A new variable with renamed dimensions which shares a buffer with the input.
 
     See Also
     --------
     scipp.Variable.rename_dims:
         Equivalent for ``Variable`` but differs for ``DataArray`` and ``Dataset``.
     """
-    return var.rename_dims(_combine_dims(dims_dict, names))
+    return var.rename_dims(combine_dict_args(dims_dict, names))
 
 
 def _rename_data_array(
     da: DataArray, dims_dict: Dict[str, str] = None, /, **names: str
 ) -> DataArray:
     """Rename the dimensions, coordinates, and attributes.
 
@@ -116,15 +105,15 @@
         Buffers are shared with the input.
 
     See Also
     --------
     scipp.DataArray.rename_dims:
         Only rename dimensions, not coordinates and attributes.
     """
-    renaming_dict = _combine_dims(dims_dict, names)
+    renaming_dict = combine_dict_args(dims_dict, names)
     out = da.rename_dims(renaming_dict)
     if out.bins is not None:
         out.data = bins(**out.bins.constituents)
     for old, new in renaming_dict.items():
         if new in out.meta:
             raise CoordError(
                 f"Cannot rename '{old}' to '{new}', since a coord or attr named {new} "
@@ -168,15 +157,15 @@
         Buffers are shared with the input.
 
     See Also
     --------
     scipp.Dataset.rename_dims:
         Only rename dimensions, not coordinates and attributes.
     """
-    renaming_dict = _combine_dims(dims_dict, names)
+    renaming_dict = combine_dict_args(dims_dict, names)
     ds_from_items = Dataset()
     for key, item in ds.items():
         dims_dict = {old: new for old, new in renaming_dict.items() if old in item.dims}
         ds_from_items[key] = _rename_data_array(item, dims_dict)
     dict_of_coords = {}
     for dim, coord in ds.coords.items():
         if dim not in ds_from_items.coords:
```

### Comparing `scipp-23.3.2/src/scipp/core/domains.py` & `scipp-23.5.0/src/scipp/core/domains.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/groupby.py` & `scipp-23.5.0/src/scipp/core/groupby.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/like.py` & `scipp-23.5.0/src/scipp/core/like.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/logical.py` & `scipp-23.5.0/src/scipp/core/logical.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/math.py` & `scipp-23.5.0/src/scipp/core/math.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/operations.py` & `scipp-23.5.0/src/scipp/core/operations.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/reduction.py` & `scipp-23.5.0/src/scipp/core/reduction.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/shape.py` & `scipp-23.5.0/src/scipp/core/shape.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/structured.py` & `scipp-23.5.0/src/scipp/core/structured.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/trigonometry.py` & `scipp-23.5.0/src/scipp/core/trigonometry.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/unary.py` & `scipp-23.5.0/src/scipp/core/unary.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/util.py` & `scipp-23.5.0/src/scipp/core/util.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/core/variable.py` & `scipp-23.5.0/src/scipp/core/variable.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/data/__init__.py` & `scipp-23.5.0/src/scipp/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/format/_parse.py` & `scipp-23.5.0/src/scipp/format/_parse.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/format/formatter.py` & `scipp-23.5.0/src/scipp/format/formatter.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/geometry.py` & `scipp-23.5.0/src/scipp/geometry.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/__init__.py` & `scipp-23.5.0/src/scipp/html/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/formatting_datagroup_html.py` & `scipp-23.5.0/src/scipp/html/formatting_datagroup_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         preview = escape(_format_multi_dim_data(var))
     elif isinstance(var, np.ndarray):
         parent_obj_str = "numpy"
         preview = f"shape={var.shape}, dtype={var.dtype}, values="
         preview += escape(_format_multi_dim_data(var))
 
     elif preview == '' and hasattr(var, "__str__"):
-        preview = escape(_format_atomic_value(var, maxidx=30))
+        preview = escape(_format_atomic_value(var, maxidx=80))
 
     html_tpl = load_atomic_row_tpl()
     return Template(html_tpl).substitute(
         depth=depth,
         name=escape(name),
         parent=escape(parent_obj_str),
         objtype=escape(objtype_str),
```

### Comparing `scipp-23.3.2/src/scipp/html/formatting_html.py` & `scipp-23.5.0/src/scipp/html/formatting_html.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/resources.py` & `scipp-23.5.0/src/scipp/html/resources.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/table.py` & `scipp-23.5.0/src/scipp/html/table.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/templates/datagroup.css` & `scipp-23.5.0/src/scipp/html/templates/datagroup.css`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/templates/dg_atomic_row.html` & `scipp-23.5.0/src/scipp/html/templates/dg_atomic_row.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/templates/dg_collapsible_row.html` & `scipp-23.5.0/src/scipp/html/templates/dg_collapsible_row.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/templates/dg_detail_list.html` & `scipp-23.5.0/src/scipp/html/templates/dg_detail_list.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/templates/dg_repr.html` & `scipp-23.5.0/src/scipp/html/templates/dg_repr.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/templates/icons-svg-inline.html` & `scipp-23.5.0/src/scipp/html/templates/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/html/templates/style.css.template` & `scipp-23.5.0/src/scipp/html/templates/style.css.template`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/io/hdf5.py` & `scipp-23.5.0/src/scipp/io/hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -389,21 +389,59 @@
     def read(group):
         _check_scipp_header(group, 'DataGroup')
         from ..core import DataGroup
 
         return DataGroup(_read_mapping(group['entries']))
 
 
+def _direct_io(cls, convert=None):
+    type_name = cls.__name__
+    if convert is None:
+        convert = cls
+
+    class GenericIO:
+        @staticmethod
+        def write(group, data):
+            _write_scipp_header(group, type_name)
+            group['entry'] = data
+            return group
+
+        @staticmethod
+        def read(group):
+            _check_scipp_header(group, type_name)
+            return convert(group['entry'][()])
+
+    return GenericIO
+
+
 class HDF5IO:
-    _handlers = dict(
-        zip(
-            ['Variable', 'DataArray', 'Dataset', 'DataGroup'],
-            [VariableIO, DataArrayIO, DatasetIO, DataGroupIO],
-        )
-    )
+    _handlers = {
+        'Variable': VariableIO,
+        'DataArray': DataArrayIO,
+        'Dataset': DatasetIO,
+        'DataGroup': DataGroupIO,
+        'str': _direct_io(str, convert=lambda b: b.decode('utf-8')),
+        'ndarray': _direct_io(np.ndarray, convert=lambda x: x),
+        **{
+            cls.__name__: _direct_io(cls)
+            for cls in (
+                int,
+                np.int64,
+                np.int32,
+                np.uint64,
+                np.uint32,
+                float,
+                np.float32,
+                np.float64,
+                bool,
+                np.bool_,
+                bytes,
+            )
+        },
+    }
 
     @classmethod
     def write(cls, group, data, **kwargs):
         name = data.__class__.__name__.replace('View', '')
         try:
             handler = cls._handlers[name]
         except KeyError:
@@ -461,12 +499,12 @@
        Will be removed in version 23.09.0.
     """
     import warnings
 
     from ..core.util import VisibleDeprecationWarning
 
     warnings.warn(
-        "scipp.io.hdf5.open_hdf5 is deprecated. Use scipp.io.hdf5.save_hdf5 instead."
+        "scipp.io.hdf5.open_hdf5 is deprecated. Use scipp.io.hdf5.load_hdf5 instead."
         "open_hdf5 will be removed in Scipp v23.09.0 (September 2023) or after.",
         VisibleDeprecationWarning,
     )
     return load_hdf5(filename)
```

### Comparing `scipp-23.3.2/src/scipp/logging.py` & `scipp-23.5.0/src/scipp/logging.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/object_list.py` & `scipp-23.5.0/src/scipp/object_list.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/operations.py` & `scipp-23.5.0/src/scipp/operations.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/__init__.py` & `scipp-23.5.0/src/scipp/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/controller.py` & `scipp-23.5.0/src/scipp/plotting/controller.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/controller1d.py` & `scipp-23.5.0/src/scipp/plotting/controller1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/controller2d.py` & `scipp-23.5.0/src/scipp/plotting/controller2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/controller3d.py` & `scipp-23.5.0/src/scipp/plotting/controller3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/dispatch.py` & `scipp-23.5.0/src/scipp/plotting/dispatch.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/displayable.py` & `scipp-23.5.0/src/scipp/plotting/displayable.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/figure.py` & `scipp-23.5.0/src/scipp/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/figure1d.py` & `scipp-23.5.0/src/scipp/plotting/figure1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/figure2d.py` & `scipp-23.5.0/src/scipp/plotting/figure2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/figure3d.py` & `scipp-23.5.0/src/scipp/plotting/figure3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/formatters.py` & `scipp-23.5.0/src/scipp/plotting/formatters.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/model.py` & `scipp-23.5.0/src/scipp/plotting/model.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/model1d.py` & `scipp-23.5.0/src/scipp/plotting/model1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/model2d.py` & `scipp-23.5.0/src/scipp/plotting/model2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/model3d.py` & `scipp-23.5.0/src/scipp/plotting/model3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/objects.py` & `scipp-23.5.0/src/scipp/plotting/objects.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/panel.py` & `scipp-23.5.0/src/scipp/plotting/panel.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/panel1d.py` & `scipp-23.5.0/src/scipp/plotting/panel1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/panel3d.py` & `scipp-23.5.0/src/scipp/plotting/panel3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/plot1d.py` & `scipp-23.5.0/src/scipp/plotting/plot1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/plot2d.py` & `scipp-23.5.0/src/scipp/plotting/plot2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/plot3d.py` & `scipp-23.5.0/src/scipp/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/profile.py` & `scipp-23.5.0/src/scipp/plotting/profile.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/resampling_model.py` & `scipp-23.5.0/src/scipp/plotting/resampling_model.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/toolbar.py` & `scipp-23.5.0/src/scipp/plotting/toolbar.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/tools.py` & `scipp-23.5.0/src/scipp/plotting/tools.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/view.py` & `scipp-23.5.0/src/scipp/plotting/view.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/view1d.py` & `scipp-23.5.0/src/scipp/plotting/view1d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/view2d.py` & `scipp-23.5.0/src/scipp/plotting/view2d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/view3d.py` & `scipp-23.5.0/src/scipp/plotting/view3d.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/widgets.py` & `scipp-23.5.0/src/scipp/plotting/widgets.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/plotting/wrapper.py` & `scipp-23.5.0/src/scipp/plotting/wrapper.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/reduction.py` & `scipp-23.5.0/src/scipp/reduction.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/scipy/integrate/__init__.py` & `scipp-23.5.0/src/scipp/scipy/integrate/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/scipy/interpolate/__init__.py` & `scipp-23.5.0/src/scipp/scipy/interpolate/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/scipy/ndimage/__init__.py` & `scipp-23.5.0/src/scipp/scipy/ndimage/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/scipy/optimize/__init__.py` & `scipp-23.5.0/src/scipp/scipy/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/scipy/signal/__init__.py` & `scipp-23.5.0/src/scipp/scipy/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/serialization.py` & `scipp-23.5.0/src/scipp/serialization.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/show.py` & `scipp-23.5.0/src/scipp/show.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/spatial/__init__.py` & `scipp-23.5.0/src/scipp/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/sphinxext/autoplot.py` & `scipp-23.5.0/src/scipp/sphinxext/autoplot.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/testing/assertions.py` & `scipp-23.5.0/src/scipp/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/testing/strategies.py` & `scipp-23.5.0/src/scipp/testing/strategies.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/typing.py` & `scipp-23.5.0/src/scipp/typing.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/units/__init__.py` & `scipp-23.5.0/src/scipp/units/__init__.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/utils/collapse_and_slices.py` & `scipp-23.5.0/src/scipp/utils/collapse_and_slices.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/utils/colors.py` & `scipp-23.5.0/src/scipp/utils/colors.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/utils/comparison.py` & `scipp-23.5.0/src/scipp/utils/comparison.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/utils/profile.py` & `scipp-23.5.0/src/scipp/utils/profile.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/utils/pyshell.py` & `scipp-23.5.0/src/scipp/utils/pyshell.py`

 * *Files identical despite different names*

### Comparing `scipp-23.3.2/src/scipp/utils/to_string.py` & `scipp-23.5.0/src/scipp/utils/to_string.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,20 +19,24 @@
     if var is not None:
         unit = var.unit if var.bins is None else var.bins.constituents["data"].unit
         if unit is not None:
             text += f" [{unit}]"
     return text
 
 
-def value_to_string(val, precision=3):
+def value_to_string(val, precision=3, max_str_len=80):
     """
     Convert a number to a human readable string.
     """
     if (not isinstance(val, float)) or (val == 0):
-        text = str(val)
+        raw_text = str(val)
+        if len(raw_text) > max_str_len:
+            text = f"{raw_text[:max_str_len-3]}..."
+        else:
+            text = raw_text
     elif (abs(val) >= 10.0 ** (precision + 1)) or (
         abs(val) <= 10.0 ** (-precision - 1)
     ):
         text = "{val:.{prec}e}".format(val=val, prec=precision)
     else:
         text = "{}".format(val)
         if len(text) > precision + 2 + (text[0] == '-'):
```

