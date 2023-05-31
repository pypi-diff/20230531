# Comparing `tmp/wemake-python-styleguide-0.9.0.tar.gz` & `tmp/wemake-python-styleguide-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wemake-python-styleguide-0.9.0.tar", last modified: Thu Jun 20 11:04:15 2019, max compression
+gzip compressed data, was "wemake-python-styleguide-0.9.1.tar", last modified: Fri Jul 12 18:56:15 2019, max compression
```

## Comparing `wemake-python-styleguide-0.9.0.tar` & `wemake-python-styleguide-0.9.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1072 2018-12-28 14:14:52.662013 wemake-python-styleguide-0.9.0/LICENSE
--rw-r--r--   0        0        0     5540 2019-06-20 08:29:46.385210 wemake-python-styleguide-0.9.0/README.md
--rw-r--r--   0        0        0     1872 2019-06-20 10:56:55.589085 wemake-python-styleguide-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.712787 wemake-python-styleguide-0.9.0/wemake_python_styleguide/__init__.py
--rw-r--r--   0        0        0     4818 2019-06-20 08:41:07.455308 wemake-python-styleguide-0.9.0/wemake_python_styleguide/checker.py
--rw-r--r--   0        0        0     3928 2019-06-20 10:15:44.711176 wemake-python-styleguide-0.9.0/wemake_python_styleguide/constants.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.713877 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/__init__.py
--rw-r--r--   0        0        0      819 2019-01-18 11:32:40.863664 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/collections.py
--rw-r--r--   0        0        0      413 2018-12-28 14:14:52.714112 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/filenames.py
--rw-r--r--   0        0        0     1852 2019-01-18 11:32:35.765931 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/functions.py
--rw-r--r--   0        0        0      285 2018-12-28 14:14:52.714709 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/imports.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.715064 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/__init__.py
--rw-r--r--   0        0        0     1319 2019-01-18 11:32:35.766931 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/access.py
--rw-r--r--   0        0        0     1115 2019-01-18 11:32:35.767267 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/builtins.py
--rw-r--r--   0        0        0     4518 2018-12-28 14:14:52.715933 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/logical.py
--rw-r--r--   0        0        0      800 2019-01-10 12:51:54.849109 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/name_nodes.py
--rw-r--r--   0        0        0     1227 2019-01-18 11:32:35.768040 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/nodes.py
--rw-r--r--   0        0        0     1551 2019-02-22 15:13:49.734693 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/operators.py
--rw-r--r--   0        0        0     1126 2019-02-27 12:55:54.840248 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/tokens.py
--rw-r--r--   0        0        0      503 2019-02-24 11:53:48.037697 wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/variables.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.716830 wemake-python-styleguide-0.9.0/wemake_python_styleguide/options/__init__.py
--rw-r--r--   0        0        0     6999 2019-06-20 08:49:37.950199 wemake-python-styleguide-0.9.0/wemake_python_styleguide/options/config.py
--rw-r--r--   0        0        0     1679 2019-06-20 08:58:33.235990 wemake-python-styleguide-0.9.0/wemake_python_styleguide/options/defaults.py
--rw-r--r--   0        0        0       63 2019-01-19 07:32:03.726507 wemake-python-styleguide-0.9.0/wemake_python_styleguide/presets/__init__.py
--rw-r--r--   0        0        0      628 2019-01-18 11:32:35.799885 wemake-python-styleguide-0.9.0/wemake_python_styleguide/presets/complexity.py
--rw-r--r--   0        0        0     1996 2019-06-20 08:29:46.389480 wemake-python-styleguide-0.9.0/wemake_python_styleguide/presets/general.py
--rw-r--r--   0        0        0      562 2019-01-18 11:32:35.802137 wemake-python-styleguide-0.9.0/wemake_python_styleguide/presets/tokens.py
--rw-r--r--   0        0        0        0 2019-06-20 08:54:12.525991 wemake-python-styleguide-0.9.0/wemake_python_styleguide/py.typed
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.717461 wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/__init__.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.717667 wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/ast/__init__.py
--rw-r--r--   0        0        0     1727 2019-01-23 08:23:18.523109 wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/ast/bugfixes.py
--rw-r--r--   0        0        0     2382 2019-04-15 09:35:12.598587 wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/ast/enhancements.py
--rw-r--r--   0        0        0     2257 2019-04-15 09:35:35.211299 wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/ast_tree.py
--rw-r--r--   0        0        0     2619 2019-06-20 08:58:17.095599 wemake-python-styleguide-0.9.0/wemake_python_styleguide/types.py
--rw-r--r--   0        0        0      499 2019-01-18 11:32:35.774877 wemake-python-styleguide-0.9.0/wemake_python_styleguide/version.py
--rw-r--r--   0        0        0      153 2018-12-28 14:14:52.718864 wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/__init__.py
--rw-r--r--   0        0        0     4439 2019-06-20 08:59:25.647353 wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/base.py
--rw-r--r--   0        0        0    46643 2019-06-20 10:37:20.279968 wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/best_practices.py
--rw-r--r--   0        0        0    17363 2019-06-20 08:52:03.006948 wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/complexity.py
--rw-r--r--   0        0        0    28792 2019-06-20 08:53:20.223317 wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/consistency.py
--rw-r--r--   0        0        0    16321 2019-06-20 08:54:05.778631 wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/naming.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.721108 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/__init__.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.721343 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/__init__.py
--rw-r--r--   0        0        0     1782 2019-06-20 08:42:25.961072 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/annotations.py
--rw-r--r--   0        0        0     2191 2019-06-20 08:42:32.232461 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/attributes.py
--rw-r--r--   0        0        0     6578 2019-06-20 08:42:39.272913 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/builtins.py
--rw-r--r--   0        0        0     6632 2019-06-20 08:55:58.402480 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/classes.py
--rw-r--r--   0        0        0     7267 2019-06-20 09:40:51.259276 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/comparisons.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.722576 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/__init__.py
--rw-r--r--   0        0        0      825 2019-06-20 08:41:56.114890 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/classes.py
--rw-r--r--   0        0        0     7943 2019-06-20 08:41:23.753834 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/counts.py
--rw-r--r--   0        0        0     5561 2019-06-20 08:41:35.814682 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/function.py
--rw-r--r--   0        0        0     2974 2019-06-20 08:41:45.218943 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/jones.py
--rw-r--r--   0        0        0     3010 2019-06-20 08:42:07.095875 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/nested.py
--rw-r--r--   0        0        0     1745 2019-06-20 08:42:17.607387 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/offset.py
--rw-r--r--   0        0        0     2468 2019-06-20 08:43:23.009588 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/conditions.py
--rw-r--r--   0        0        0     4728 2019-02-28 11:08:58.457170 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/exceptions.py
--rw-r--r--   0        0        0     6302 2019-06-20 10:36:59.633640 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/functions.py
--rw-r--r--   0        0        0     4090 2019-06-20 09:29:27.309398 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/imports.py
--rw-r--r--   0        0        0     9042 2019-06-20 08:32:42.987597 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/keywords.py
--rw-r--r--   0        0        0     6678 2019-02-24 11:52:48.853992 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/loops.py
--rw-r--r--   0        0        0     2598 2019-06-20 08:32:50.337214 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/modules.py
--rw-r--r--   0        0        0    10129 2019-06-20 08:32:56.872635 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/naming.py
--rw-r--r--   0        0        0     8202 2019-06-20 08:33:03.631533 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/statements.py
--rw-r--r--   0        0        0     7771 2019-06-20 08:33:09.556945 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/base.py
--rw-r--r--   0        0        0      737 2018-12-28 14:14:52.725384 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/decorators.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.725584 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/filenames/__init__.py
--rw-r--r--   0        0        0     2767 2019-06-20 10:09:29.538337 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/filenames/module.py
--rw-r--r--   0        0        0       24 2018-12-28 14:14:52.726831 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/__init__.py
--rw-r--r--   0        0        0     5403 2019-06-20 08:33:18.938216 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/comments.py
--rw-r--r--   0        0        0      952 2019-06-20 08:33:28.671878 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/keywords.py
--rw-r--r--   0        0        0     5601 2019-06-20 09:24:22.136005 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/primitives.py
--rw-r--r--   0        0        0     5267 2019-06-20 08:33:51.275872 wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/statements.py
--rw-r--r--   0        0        0     7584 1970-01-01 00:00:00.000000 wemake-python-styleguide-0.9.0/setup.py
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 wemake-python-styleguide-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2018-12-28 14:14:52.662013 wemake-python-styleguide-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5540 2019-07-12 18:50:01.173633 wemake-python-styleguide-0.9.1/README.md
+-rw-r--r--   0        0        0     1915 2019-07-12 18:54:27.709962 wemake-python-styleguide-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.712787 wemake-python-styleguide-0.9.1/wemake_python_styleguide/__init__.py
+-rw-r--r--   0        0        0     4818 2019-07-12 18:50:01.202244 wemake-python-styleguide-0.9.1/wemake_python_styleguide/checker.py
+-rw-r--r--   0        0        0     3928 2019-07-12 18:50:01.203860 wemake-python-styleguide-0.9.1/wemake_python_styleguide/constants.py
+-rw-r--r--   0        0        0       24 2019-07-12 18:50:01.204296 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/__init__.py
+-rw-r--r--   0        0        0      819 2019-07-12 18:50:01.204847 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/collections.py
+-rw-r--r--   0        0        0      413 2019-07-12 18:50:01.205375 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/filenames.py
+-rw-r--r--   0        0        0     1852 2019-07-12 18:50:01.205603 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/functions.py
+-rw-r--r--   0        0        0      285 2019-07-12 18:50:01.205767 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/imports.py
+-rw-r--r--   0        0        0       24 2019-07-12 18:50:01.205968 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/__init__.py
+-rw-r--r--   0        0        0     1319 2019-07-12 18:50:01.206593 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/access.py
+-rw-r--r--   0        0        0     1115 2019-07-12 18:50:01.207103 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/builtins.py
+-rw-r--r--   0        0        0     4518 2019-07-12 18:50:01.207332 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/logical.py
+-rw-r--r--   0        0        0      800 2019-07-12 18:50:01.207551 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/name_nodes.py
+-rw-r--r--   0        0        0     1227 2019-07-12 18:50:01.208577 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/nodes.py
+-rw-r--r--   0        0        0     1551 2019-07-12 18:50:01.209130 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/operators.py
+-rw-r--r--   0        0        0     1126 2019-07-12 18:50:01.209764 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/tokens.py
+-rw-r--r--   0        0        0      503 2019-07-12 18:50:01.210454 wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/variables.py
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.716830 wemake-python-styleguide-0.9.1/wemake_python_styleguide/options/__init__.py
+-rw-r--r--   0        0        0     6999 2019-07-12 18:50:01.211085 wemake-python-styleguide-0.9.1/wemake_python_styleguide/options/config.py
+-rw-r--r--   0        0        0     1679 2019-07-12 18:50:01.211766 wemake-python-styleguide-0.9.1/wemake_python_styleguide/options/defaults.py
+-rw-r--r--   0        0        0       63 2019-01-19 07:32:03.726507 wemake-python-styleguide-0.9.1/wemake_python_styleguide/presets/__init__.py
+-rw-r--r--   0        0        0      628 2019-07-12 18:50:01.213073 wemake-python-styleguide-0.9.1/wemake_python_styleguide/presets/complexity.py
+-rw-r--r--   0        0        0     1996 2019-07-12 18:50:01.213623 wemake-python-styleguide-0.9.1/wemake_python_styleguide/presets/general.py
+-rw-r--r--   0        0        0      562 2019-01-18 11:32:35.802137 wemake-python-styleguide-0.9.1/wemake_python_styleguide/presets/tokens.py
+-rw-r--r--   0        0        0        0 2019-06-20 08:54:12.525991 wemake-python-styleguide-0.9.1/wemake_python_styleguide/py.typed
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.717461 wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/__init__.py
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.717667 wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/ast/__init__.py
+-rw-r--r--   0        0        0     1727 2019-07-12 18:50:01.214582 wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/ast/bugfixes.py
+-rw-r--r--   0        0        0     2382 2019-04-15 09:35:12.598587 wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/ast/enhancements.py
+-rw-r--r--   0        0        0     2257 2019-07-12 18:50:01.215243 wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/ast_tree.py
+-rw-r--r--   0        0        0     2619 2019-07-12 18:50:01.215859 wemake-python-styleguide-0.9.1/wemake_python_styleguide/types.py
+-rw-r--r--   0        0        0      499 2019-01-18 11:32:35.774877 wemake-python-styleguide-0.9.1/wemake_python_styleguide/version.py
+-rw-r--r--   0        0        0      153 2019-07-12 18:50:01.216182 wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/__init__.py
+-rw-r--r--   0        0        0     4439 2019-06-20 08:59:25.647353 wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/base.py
+-rw-r--r--   0        0        0    46643 2019-07-12 18:50:01.217175 wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/best_practices.py
+-rw-r--r--   0        0        0    17363 2019-07-12 18:50:01.218093 wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/complexity.py
+-rw-r--r--   0        0        0    28792 2019-07-12 18:50:01.219241 wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/consistency.py
+-rw-r--r--   0        0        0    16321 2019-06-20 08:54:05.778631 wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/naming.py
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.721108 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/__init__.py
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.721343 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/__init__.py
+-rw-r--r--   0        0        0     1782 2019-06-20 08:42:25.961072 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/annotations.py
+-rw-r--r--   0        0        0     2191 2019-07-12 18:50:01.220171 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/attributes.py
+-rw-r--r--   0        0        0     6578 2019-07-12 18:50:01.220822 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/builtins.py
+-rw-r--r--   0        0        0     6632 2019-07-12 18:50:01.221534 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/classes.py
+-rw-r--r--   0        0        0     7267 2019-07-12 18:50:01.222174 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/comparisons.py
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.722576 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/__init__.py
+-rw-r--r--   0        0        0      825 2019-06-20 16:30:01.544650 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/classes.py
+-rw-r--r--   0        0        0     7943 2019-07-12 18:50:01.223050 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/counts.py
+-rw-r--r--   0        0        0     5561 2019-07-12 18:50:01.223981 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/function.py
+-rw-r--r--   0        0        0     2974 2019-06-20 08:41:45.218943 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/jones.py
+-rw-r--r--   0        0        0     3010 2019-07-12 18:50:01.224942 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/nested.py
+-rw-r--r--   0        0        0     1745 2019-06-20 08:42:17.607387 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/offset.py
+-rw-r--r--   0        0        0     2468 2019-07-12 18:50:01.225496 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/conditions.py
+-rw-r--r--   0        0        0     4728 2019-07-12 18:50:01.226604 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/exceptions.py
+-rw-r--r--   0        0        0     6302 2019-07-12 18:50:01.227486 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/functions.py
+-rw-r--r--   0        0        0     4090 2019-07-12 18:50:01.228237 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/imports.py
+-rw-r--r--   0        0        0     9042 2019-07-12 18:50:01.228854 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/keywords.py
+-rw-r--r--   0        0        0     6678 2019-07-12 18:50:01.229632 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/loops.py
+-rw-r--r--   0        0        0     2598 2019-07-12 18:50:01.230448 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/modules.py
+-rw-r--r--   0        0        0    10129 2019-07-12 18:50:01.231465 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/naming.py
+-rw-r--r--   0        0        0     8202 2019-07-12 18:50:01.232360 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/statements.py
+-rw-r--r--   0        0        0     7771 2019-07-12 18:50:01.233255 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/base.py
+-rw-r--r--   0        0        0      737 2018-12-28 14:14:52.725384 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/decorators.py
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.725584 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/filenames/__init__.py
+-rw-r--r--   0        0        0     2767 2019-07-12 18:50:01.234071 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/filenames/module.py
+-rw-r--r--   0        0        0       24 2018-12-28 14:14:52.726831 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/__init__.py
+-rw-r--r--   0        0        0     5403 2019-07-12 18:50:01.234904 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/comments.py
+-rw-r--r--   0        0        0      952 2019-06-20 08:33:28.671878 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/keywords.py
+-rw-r--r--   0        0        0     5601 2019-07-12 18:50:01.235479 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/primitives.py
+-rw-r--r--   0        0        0     5267 2019-07-12 18:50:01.236389 wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/statements.py
+-rw-r--r--   0        0        0     7601 1970-01-01 00:00:00.000000 wemake-python-styleguide-0.9.1/setup.py
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 wemake-python-styleguide-0.9.1/PKG-INFO
```

### Comparing `wemake-python-styleguide-0.9.0/LICENSE` & `wemake-python-styleguide-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/README.md` & `wemake-python-styleguide-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/pyproject.toml` & `wemake-python-styleguide-0.9.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 
 [tool.poetry]
 name = "wemake-python-styleguide"
-version = "0.9.0"
+version = "0.9.1"
 description = "The strictest and most opinionated python linter ever"
 
 license = "MIT"
 
 authors = [
   "Nikita Sobolev <mail@sobolevn.me>"
 ]
@@ -49,14 +49,16 @@
 astor = ">=0.7.1,<0.9.0"
 
 flake8-builtins = "^1.4"
 flake8-commas = "^2.0"
 flake8-quotes = ">=1,<3"
 flake8-comprehensions = ">=1.4,<3.0"
 flake8-docstrings = "^1.3"
+# Temporary fix for #636
+pydocstyle = "<4"
 flake8-string-format = "^0.2"
 flake8-coding = "^1.3"
 flake8-bugbear = "^19.3"
 flake8-pep3101 = "^1.2"
 flake8-debugger = "^3.1"
 flake8-isort = "^2.6"
 flake8-eradicate = "^0.2"
```

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/checker.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/checker.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/constants.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/constants.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/collections.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/collections.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/functions.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/functions.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/access.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/access.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/builtins.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/builtins.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/logical.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/logical.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/naming/name_nodes.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/naming/name_nodes.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/nodes.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/nodes.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/operators.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/operators.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/logics/tokens.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/logics/tokens.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/options/config.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/options/config.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/options/defaults.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/options/defaults.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/presets/complexity.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/presets/complexity.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/presets/general.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/presets/general.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/presets/tokens.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/presets/tokens.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/ast/bugfixes.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/ast/bugfixes.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/ast/enhancements.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/ast/enhancements.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/transformations/ast_tree.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/transformations/ast_tree.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/types.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/types.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/base.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/base.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/best_practices.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/best_practices.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/complexity.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/complexity.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/consistency.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/consistency.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/violations/naming.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/violations/naming.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/annotations.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/annotations.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/attributes.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/attributes.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/builtins.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/builtins.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/classes.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/classes.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/comparisons.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/comparisons.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/classes.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/classes.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/counts.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/counts.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/function.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/function.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/jones.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/jones.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/nested.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/nested.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/complexity/offset.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/complexity/offset.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/conditions.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/conditions.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/exceptions.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/exceptions.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/functions.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/functions.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/imports.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/imports.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/keywords.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/keywords.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/loops.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/loops.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/modules.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/modules.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/naming.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/naming.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/ast/statements.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/ast/statements.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/base.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/base.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/decorators.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/decorators.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/filenames/module.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/filenames/module.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/comments.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/comments.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/keywords.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/keywords.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/primitives.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/primitives.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/wemake_python_styleguide/visitors/tokenize/statements.py` & `wemake-python-styleguide-0.9.1/wemake_python_styleguide/visitors/tokenize/statements.py`

 * *Files identical despite different names*

### Comparing `wemake-python-styleguide-0.9.0/setup.py` & `wemake-python-styleguide-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,22 +37,23 @@
  'flake8-logging-format>=0.6,<0.7',
  'flake8-pep3101>=1.2,<2.0',
  'flake8-print>=3.1,<4.0',
  'flake8-quotes>=1,<3',
  'flake8-string-format>=0.2,<0.3',
  'flake8>=3.7,<4.0',
  'pep8-naming>=0.7,<0.9',
+ 'pydocstyle<4',
  'typing_extensions>=3.6,<4.0']
 
 entry_points = \
 {'flake8.extension': ['Z = wemake_python_styleguide.checker:Checker']}
 
 setup_kwargs = {
     'name': 'wemake-python-styleguide',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'The strictest and most opinionated python linter ever',
     'long_description': '# wemake-python-styleguide\n\n[![wemake.services](https://img.shields.io/badge/%20-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake.services)\n[![Python Version](https://img.shields.io/pypi/pyversions/wemake-python-styleguide.svg)](https://pypi.org/project/wemake-python-styleguide/)\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\n[![Build Status](https://travis-ci.org/wemake-services/wemake-python-styleguide.svg?branch=master)](https://travis-ci.org/wemake-services/wemake-python-styleguide) \n[![Coverage](https://coveralls.io/repos/github/wemake-services/wemake-python-styleguide/badge.svg?branch=master)](https://coveralls.io/github/wemake-services/wemake-python-styleguide?branch=master)\n[![Documentation Status](https://readthedocs.org/projects/wemake-python-styleguide/badge/?version=latest)](https://wemake-python-styleguide.readthedocs.io/en/latest/?badge=latest)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/wemake-services/wemake-python-styleguide/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/wemake-services/wemake-python-styleguide.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/wemake-services/wemake-python-styleguide/context:python)\n---\n\nWelcome to the strictest and most opinionated python linter ever.\n\n`wemake-python-styleguide` is actually a `flake8` plugin\nwith some other plugins as dependencies.\n\n```text\nThe Zen of Python, by Tim Peters\n\nBeautiful is better than ugly.\nExplicit is better than implicit.\nSimple is better than complex.\nComplex is better than complicated.\nFlat is better than nested.\nSparse is better than dense.\nReadability counts.\nSpecial cases aren\'t special enough to break the rules.\nAlthough practicality beats purity.\nErrors should never pass silently.\nUnless explicitly silenced.\nIn the face of ambiguity, refuse the temptation to guess.\nThere should be one-- and preferably only one-- obvious way to do it.\nAlthough that way may not be obvious at first unless you\'re Dutch.\nNow is better than never.\nAlthough never is often better than *right* now.\nIf the implementation is hard to explain, it\'s a bad idea.\nIf the implementation is easy to explain, it may be a good idea.\nNamespaces are one honking great idea -- let\'s do more of those!\n```\n\n## Installation\n\n```bash\npip install wemake-python-styleguide\n```\n\nYou will also need to create a `setup.cfg` file with [the following contents](https://wemake-python-styleguide.readthedocs.io/en/latest/pages/options/config.html#plugins).\n\nThis file is required to configure our linter and all 3rd party plugins it uses.\nHowever, this is a temporary solution.\nWe are working at providing the required configuration for you in the future.\n\nRunning:\n\n```bash\nflake8 your_module.py\n```\n\nThis app is still just good old `flake8`!\nAnd it won\'t change your existing workflow.\n\nSee ["Usage" section](https://wemake-python-styleguide.readthedocs.io/en/latest/pages/usage/setup.html)\nin the docs for examples and integrations.\n\n\n## What we are about\n\nWe have several primary objectives:\n\n0. Enforce `python3.6+` usage\n1. Significantly reduce complexity of your code and make it more maintainable\n2. Enforce "There should be one-- and preferably only one --obvious way to do it" rule to coding and naming styles\n3. Protect developers from possible errors and enforce best practices\n\nYou can find all error codes and plugins [in the docs](https://wemake-python-styleguide.readthedocs.io/en/latest/pages/violations/index.html).\n\n\n## What we are not\n\nWe are *not* planning to do the following things:\n\n0. Assume or check types, use `mypy` instead\n1. Reformat code, since we believe that developers should do that\n2. Check for `SyntaxError` or exceptions, write tests instead\n3. Appeal to everyone, this is **our** linter. But, you can [switch off](https://wemake-python-styleguide.readthedocs.io/en/latest/pages/usage/setup.html#ignoring-violations) any rules that you don\'t like\n\n\n## Show your style\n\nIf you use our linter - it means that your code is awesome.\nYou can be proud of it!\nAnd you should share your accomplishment with others\nby including a badge to your `README` file.\n\nIt looks like this:\n\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\n### Markdown\n\n```\n[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n```\n\n### Restructured text\n\n```\n.. image:: https://img.shields.io/badge/style-wemake-000000.svg\n    :target: https://github.com/wemake-services/wemake-python-styleguide\n```\n\n\n## Contributing\n\nWe warmly welcome all contributions!\n\nSee ["Contributing"](https://wemake-python-styleguide.readthedocs.io/en/latest/pages/contributing.html)\nsection in the documentation if you want to contribute.\nYou can start with [issues that need some help](https://github.com/wemake-services/wemake-python-styleguide/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) right now.\n',
     'author': 'Nikita Sobolev',
     'author_email': 'mail@sobolevn.me',
     'url': 'https://wemake-python-styleguide.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wemake-python-styleguide-0.9.0/PKG-INFO` & `wemake-python-styleguide-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wemake-python-styleguide
-Version: 0.9.0
+Version: 0.9.1
 Summary: The strictest and most opinionated python linter ever
 Home-page: https://wemake-python-styleguide.readthedocs.io
 Author: Nikita Sobolev
 Author-email: mail@sobolevn.me
 Keywords: flake8,flake8-plugin,linter,wemake.services,styleguide,code quality
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -35,9 +35,10 @@
 Requires-Dist: flake8-isort (>=2.6,<3.0)
 Requires-Dist: flake8-logging-format (>=0.6,<0.7)
 Requires-Dist: flake8-pep3101 (>=1.2,<2.0)
 Requires-Dist: flake8-print (>=3.1,<4.0)
 Requires-Dist: flake8-quotes (>=1,<3)
 Requires-Dist: flake8-string-format (>=0.2,<0.3)
 Requires-Dist: pep8-naming (>=0.7,<0.9)
+Requires-Dist: pydocstyle (<4)
 Requires-Dist: typing_extensions (>=3.6,<4.0)
 Project-URL: Repository, https://github.com/wemake-services/wemake-python-styleguide
```

