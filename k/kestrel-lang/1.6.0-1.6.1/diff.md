# Comparing `tmp/kestrel-lang-1.6.0.tar.gz` & `tmp/kestrel-lang-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.6.0.tar", last modified: Wed May 17 20:40:51 2023, max compression
+gzip compressed data, was "kestrel-lang-1.6.1.tar", last modified: Wed May 31 15:55:47 2023, max compression
```

## Comparing `kestrel-lang-1.6.0.tar` & `kestrel-lang-1.6.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.499588 kestrel-lang-1.6.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.495588 kestrel-lang-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.499588 kestrel-lang-1.6.0/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.503588 kestrel-lang-1.6.0/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.503588 kestrel-lang-1.6.0/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.503588 kestrel-lang-1.6.0/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.507588 kestrel-lang-1.6.0/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.507588 kestrel-lang-1.6.0/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    20339 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.507588 kestrel-lang-1.6.0/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.511588 kestrel-lang-1.6.0/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.511588 kestrel-lang-1.6.0/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.511588 kestrel-lang-1.6.0/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.515588 kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.515588 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17937 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.515588 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 20:40:51.000000 kestrel-lang-1.6.0/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:40:51.523588 kestrel-lang-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_fast_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-17 20:40:35.000000 kestrel-lang-1.6.0/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-31 15:55:47.604294 kestrel-lang-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.588294 kestrel-lang-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.592294 kestrel-lang-1.6.1/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20339 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.596294 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 15:55:47.000000 kestrel-lang-1.6.1/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:55:47.600294 kestrel-lang-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_fast_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-31 15:55:26.000000 kestrel-lang-1.6.1/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.6.0/AUTHORS.rst` & `kestrel-lang-1.6.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/LICENSE.md` & `kestrel-lang-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/PKG-INFO` & `kestrel-lang-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.6.0
+Version: 1.6.1
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.6.0/README.rst` & `kestrel-lang-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/setup.cfg` & `kestrel-lang-1.6.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.6.0
+version = 1.6.1
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -33,15 +33,15 @@
 	requests
 	nest-asyncio>=1.5.6
 	lark>=1.1.5
 	pyarrow>=5.0.0
 	docker>=5.0.0
 	stix-shifter>=5.3.0
 	stix-shifter-utils>=5.3.0
-	firepit>=2.3.19
+	firepit>=2.3.20
 	typeguard
 tests_require = 
 	pytest
 
 [options.packages.find]
 where = src
```

### Comparing `kestrel-lang-1.6.0/src/kestrel/__main__.py` & `kestrel-lang-1.6.1/src/kestrel/__main__.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.6.1/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/analytics/interface.py` & `kestrel-lang-1.6.1/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/analytics/manager.py` & `kestrel-lang-1.6.1/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/codegen/commands.py` & `kestrel-lang-1.6.1/src/kestrel/codegen/commands.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/codegen/data.py` & `kestrel-lang-1.6.1/src/kestrel/codegen/data.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/codegen/display.py` & `kestrel-lang-1.6.1/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/codegen/queries.py` & `kestrel-lang-1.6.1/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/codegen/relations.py` & `kestrel-lang-1.6.1/src/kestrel/codegen/relations.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/codegen/summary.py` & `kestrel-lang-1.6.1/src/kestrel/codegen/summary.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/config.py` & `kestrel-lang-1.6.1/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/config.yaml` & `kestrel-lang-1.6.1/src/kestrel/config.yaml`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/datasource/interface.py` & `kestrel-lang-1.6.1/src/kestrel/datasource/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/datasource/manager.py` & `kestrel-lang-1.6.1/src/kestrel/datasource/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.6.1/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/exceptions.py` & `kestrel-lang-1.6.1/src/kestrel/exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/semantics/completor.py` & `kestrel-lang-1.6.1/src/kestrel/semantics/completor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/semantics/processor.py` & `kestrel-lang-1.6.1/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/semantics/reference.py` & `kestrel-lang-1.6.1/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/session.py` & `kestrel-lang-1.6.1/src/kestrel/session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.6.1/src/kestrel/symboltable/variable.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.6.1/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/syntax/kestrel.lark` & `kestrel-lang-1.6.1/src/kestrel/syntax/kestrel.lark`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 //
 // Variable definition
 //
 
 variables: VARIABLE ("," VARIABLE)*
 
-VARIABLE: ECNAME
+VARIABLE: CNAME
 
 //
 // Expression
 //
 
 expression: vtrans where_clause? attr_clause? sort_clause? limit_clause? offset_clause?
 
@@ -289,12 +289,12 @@
 
 SIMPLE_STRING: ECNAME
 
 // nearly Python string, but no [ubf]? as prefix options
 // check Lark example of Python parser for reference
 ADVANCED_STRING: /(r?)("(?!"").*?(?<!\\)(\\\\)*?"|'(?!'').*?(?<!\\)(\\\\)*?')/
 
-%import common (LETTER, DIGIT, WS, INT, WORD, NUMBER, _STRING_ESC_INNER)
+%import common (LETTER, DIGIT, WS, INT, WORD, NUMBER, CNAME, _STRING_ESC_INNER)
 %import common.SH_COMMENT -> COMMENT
 
 %ignore WS
 %ignore COMMENT
```

### Comparing `kestrel-lang-1.6.0/src/kestrel/syntax/parser.py` & `kestrel-lang-1.6.1/src/kestrel/syntax/parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/syntax/reference.py` & `kestrel-lang-1.6.1/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/syntax/utils.py` & `kestrel-lang-1.6.1/src/kestrel/syntax/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel/utils.py` & `kestrel-lang-1.6.1/src/kestrel/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.6.1/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.6.1/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.6.1/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.6.1/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.6.1/src/kestrel_datasource_stixbundle/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/config.py` & `kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from kestrel.exceptions import InvalidDataSource
 
 PROFILE_PATH_DEFAULT = CONFIG_DIR_DEFAULT / "stixshifter.yaml"
 PROFILE_PATH_ENV_VAR = "KESTREL_STIXSHIFTER_CONFIG"
 STIXSHIFTER_DEBUG_ENV_VAR = "KESTREL_STIXSHIFTER_DEBUG"  # debug mode for stix-shifter if the environment variable exists
 ENV_VAR_PREFIX = "STIXSHIFTER_"
 RETRIEVAL_BATCH_SIZE = 2000
+SINGLE_BATCH_TIMEOUT = 60
 FAST_TRANSLATE_CONNECTORS = []  # Suggested: ["qradar", "elastic_ecs"]
 ASYNC_TRANSLATION_WORKERS_CNT = 1
 
 
 _logger = logging.getLogger(__name__)
 
 
@@ -131,21 +132,55 @@
         if "auth" not in configuration:
             raise InvalidDataSource(
                 profile_name,
                 "stixshifter",
                 f'invalid {profile_name} configuration section: no "auth" field',
             )
 
+        if "options" not in connection:
+            connection["options"] = {}
+
         retrieval_batch_size = RETRIEVAL_BATCH_SIZE
-        if "options" in connection and "retrieval_batch_size" in connection["options"]:
-            # need to remove the non-stix-shifter field "retrieval_batch_size" to avoid stix-shifter error
-            retrieval_batch_size = connection["options"].pop("retrieval_batch_size")
+        if "retrieval_batch_size" in connection["options"]:
+            # remove the non-stix-shifter field "retrieval_batch_size" to avoid stix-shifter error
+            try:
+                retrieval_batch_size = int(
+                    connection["options"].pop("retrieval_batch_size")
+                )
+            except:
+                raise InvalidDataSource(
+                    profile_name,
+                    "stixshifter",
+                    f"invalid {profile_name} connection section: options.retrieval_batch_size",
+                )
+            # rename this field for stix-shifter use; x2 the size to ensure retrieval
             _logger.debug(
                 f"profile-loaded retrieval_batch_size: {retrieval_batch_size}"
             )
+        connection["options"]["result_limit"] = retrieval_batch_size * 2
+
+        single_batch_timeout = SINGLE_BATCH_TIMEOUT
+        if "single_batch_timeout" in connection["options"]:
+            # remove the non-stix-shifter field "single_batch_timeout" to avoid stix-shifter error
+            try:
+                single_batch_timeout = int(
+                    connection["options"].pop("single_batch_timeout")
+                )
+            except:
+                raise InvalidDataSource(
+                    profile_name,
+                    "stixshifter",
+                    f"invalid {profile_name} connection section: options.single_batch_timeout",
+                )
+            # rename this field for stix-shifter use
+            _logger.debug(
+                f"profile-loaded single_batch_timeout: {single_batch_timeout}"
+            )
+        connection["options"]["timeout"] = single_batch_timeout
+
     return connector_name, connection, configuration, retrieval_batch_size
 
 
 def load_profiles():
     config = load_user_config(PROFILE_PATH_ENV_VAR, PROFILE_PATH_DEFAULT)
     if config and "profiles" in config:
         _logger.debug(f"stix-shifter profiles found in config file")
```

### Comparing `kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/connector.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/src/kestrel_datasource_stixshifter/interface.py` & `kestrel-lang-1.6.1/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,16 @@
                 connector: elastic_ecs
                 connection:
                     host: elastic.securitylog.company.com
                     port: 9200
                     selfSignedCert: false # this means do NOT check cert
                     indices: host101
                     options:  # use any of this section when needed
-                        result_limit: 500000  # stix-shifter default: 10000
-                        retrieval_batch_size: 10000  # safe to set to 10000 to match default Elasticsearch page size; Kestrel default: 2000
-                        timeout: 300  # allow a query to run for 5 minutes (300 seconds) before timing out; stix-shifter default: 30
+                        retrieval_batch_size: 10000  # set to 10000 to match default Elasticsearch page size; Kestrel default across connectors: 2000
+                        single_batch_timeout: 120  # increase it if hit 60 seconds (Kestrel default) timeout error for each batch of retrieval
                         dialects:  # more info: https://github.com/opencybersecurityalliance/stix-shifter/tree/develop/stix_shifter_modules/elastic_ecs#dialects
                           - beats  # need it if the index is created by Filebeat/Winlogbeat/*beat
                 config:
                     auth:
                         id: VuaCfGcBCdbkQm-e5aOx
                         api_key: ui2lp2axTNmsyakw9tvNnw
             host102:
@@ -99,15 +98,14 @@
 .. _elastic_ecs config: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/stix_shifter_modules/elastic_ecs/configuration/lang_en.json
 .. _stix_shifter_modules/lang_en.json: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/stix_shifter_modules/lang_en.json
 
 """
 
 import asyncio
 import json
-import time
 import copy
 import logging
 
 
 from stix_shifter.stix_translation import stix_translation
 from stix_shifter.stix_transmission import stix_transmission
 from stix_shifter_utils.stix_translation.src.utils.transformer_utils import (
@@ -205,15 +203,15 @@
 
             translation = stix_translation.StixTranslation()
             transmission = stix_transmission.StixTransmission(
                 connector_name, connection_dict, configuration_dict
             )
 
             translation_options = copy.deepcopy(connection_dict.get("options", {}))
-            dsl = translation.translate(
+            dsl = await translation.translate_async(
                 connector_name, "query", query_metadata, pattern, translation_options
             )
 
             if "error" in dsl:
                 raise DataSourceError(
                     f"STIX-shifter translation from STIX to native query failed with message: {dsl['error']}"
                 )
@@ -255,38 +253,23 @@
                             store,
                         )
                     )
                     consumers.append(consumer)
 
             batch_index = 0
             for query in dsl["queries"]:
-                search_meta_result = transmission.query(query)
+                search_meta_result = await transmission.query_async(query)
                 if search_meta_result["success"]:
                     search_id = search_meta_result["search_id"]
-                    if transmission.is_async():
-                        time.sleep(1)
-                        status = transmission.status(search_id)
-                        if status["success"]:
-                            while (
-                                status["progress"] < 100
-                                and status["status"] == "RUNNING"
-                            ):
-                                status = transmission.status(search_id)
-                        else:
-                            stix_shifter_error_msg = (
-                                status["error"]
-                                if "error" in status
-                                else "details not avaliable"
-                            )
-                            raise DataSourceError(
-                                f"STIX-shifter transmission.status() failed with message: {stix_shifter_error_msg}"
-                            )
+
+                    await transmission_complete(transmission, search_id)
 
                     # run the producer and wait for completion
                     batch_index = await transmission_produce(
+                        connector_name,
                         transmission_queue,
                         transmission,
                         search_id,
                         retrieval_batch_size,
                         batch_index,
                     )
 
@@ -325,44 +308,83 @@
             ingestdir / f"{profile_index}_{batch_index}_{data_path_striped}.json"
         )
         return ingestbatchfile
 
     return ingest_stixbundle_filepath
 
 
+async def transmission_complete(transmission, search_id):
+    status = None
+    while True:
+        status = await transmission.status_async(search_id)
+        if not status["success"]:
+            stix_shifter_error_msg = (
+                status["error"] if "error" in status else "details not avaliable"
+            )
+            raise DataSourceError(
+                f"STIX-shifter transmission.status() failed with message: {stix_shifter_error_msg}"
+            )
+        elif status["progress"] < 100 and status["status"] == "RUNNING":
+            await asyncio.sleep(1)
+        else:
+            break
+
+
 async def transmission_produce(
-    transmission_queue, transmission, search_id, retrieval_batch_size, batch_index
+    connector_name,
+    transmission_queue,
+    transmission,
+    search_id,
+    retrieval_batch_size,
+    batch_index,
 ):
     result_retrieval_offset = 0
     has_remaining_results = True
     metadata = None
+    is_retry_cycle = False
     while has_remaining_results:
-        result_batch = transmission.results(
+        result_batch = await transmission.results_async(
             search_id, result_retrieval_offset, retrieval_batch_size, metadata
         )
         if result_batch["success"]:
             new_entries = result_batch["data"]
             if new_entries:
                 result_batch["batch_index"] = batch_index
                 await transmission_queue.put(result_batch)
                 result_retrieval_offset += len(new_entries)
                 batch_index += 1
             else:
                 has_remaining_results = False
             if "metadata" in result_batch:
                 metadata = result_batch["metadata"]
+            is_retry_cycle = False
         else:
             stix_shifter_error_msg = (
                 result_batch["error"]
                 if "error" in result_batch
                 else "details not avaliable"
             )
-            raise DataSourceError(
-                f"STIX-shifter transmission.results() failed with message: {stix_shifter_error_msg}"
-            )
+            if (
+                stix_shifter_error_msg.startswith(
+                    f"{connector_name} connector error => server timeout_error"
+                )
+                and not is_retry_cycle
+            ):
+                # mitigate https://github.com/opencybersecurityalliance/stix-shifter/issues/1493
+                # only give it one retry to mitigate high CPU occupation
+                # otherwise, it could be a real server connection issue
+                # /stix_shifter_utils/stix_transmission/utils/RestApiClientAsync.py
+                _logger.info(
+                    f"busy CPU; hit stix-shifter transmission aiohttp connection timeout; retry"
+                )
+                is_retry_cycle = True
+            else:
+                raise DataSourceError(
+                    f"STIX-shifter transmission.results() failed with message: {stix_shifter_error_msg}"
+                )
     return batch_index
 
 
 async def translation_ingest_consume(
     transmission_queue,
     translation,
     connector_name,
@@ -372,15 +394,15 @@
     query_id,
     store,
 ):
     while True:
         # wait for an item from the producer
         result_batch = await transmission_queue.get()
 
-        stixbundle = translation.translate(
+        stixbundle = await translation.translate_async(
             connector_name,
             "results",
             query_metadata,
             result_batch["data"],
             translation_options,
         )
 
@@ -412,42 +434,40 @@
     identity,
     query_id,
     store,
 ):
     while True:
         # wait for an item from the producer
         result_batch = await transmission_queue.get()
-        try:
-            await fast_translate(
-                connector_name,
-                result_batch["data"],
-                translation,
-                translation_options,
-                identity,
-                query_id,
-                store,
-            )
-        finally:
-            # Notify the queue that the item has been processed
-            transmission_queue.task_done()
+        await fast_translate(
+            connector_name,
+            result_batch["data"],
+            translation,
+            translation_options,
+            identity,
+            query_id,
+            store,
+        )
+        # Notify the queue that the item has been processed
+        transmission_queue.task_done()
 
 
 async def fast_translate(
     connector_name,
     connector_results,
     translation,
     translation_options,
     identity,
     query_id,
     store,
 ):
     # Use the alternate, faster DataFrame-based translation (in firepit)
     _logger.debug("Using fast translation for connector %s", connector_name)
     transformers = get_module_transformers(connector_name)
-    mapping = translation.translate(
+    mapping = await translation.translate_async(
         connector_name,
         stix_translation.MAPPING,
         None,
         None,
         translation_options,
     )
```

### Comparing `kestrel-lang-1.6.0/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.6.1/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.6.0
+Version: 1.6.1
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.6.0/src/kestrel_lang.egg-info/SOURCES.txt` & `kestrel-lang-1.6.1/src/kestrel_lang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_assign.py` & `kestrel-lang-1.6.1/tests/test_command_assign.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_disp.py` & `kestrel-lang-1.6.1/tests/test_command_disp.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_find.py` & `kestrel-lang-1.6.1/tests/test_command_find.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_get.py` & `kestrel-lang-1.6.1/tests/test_command_get.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_group.py` & `kestrel-lang-1.6.1/tests/test_command_group.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_join.py` & `kestrel-lang-1.6.1/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_load.py` & `kestrel-lang-1.6.1/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_merge.py` & `kestrel-lang-1.6.1/tests/test_command_merge.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_new.py` & `kestrel-lang-1.6.1/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_command_save.py` & `kestrel-lang-1.6.1/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_completion.py` & `kestrel-lang-1.6.1/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_display.py` & `kestrel-lang-1.6.1/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_exceptions.py` & `kestrel-lang-1.6.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_expressions.py` & `kestrel-lang-1.6.1/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_fast_translate.py` & `kestrel-lang-1.6.1/tests/test_fast_translate.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_parser.py` & `kestrel-lang-1.6.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_python_analytics.py` & `kestrel-lang-1.6.1/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_session.py` & `kestrel-lang-1.6.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.6.0/tests/test_stixshifter.py` & `kestrel-lang-1.6.1/tests/test_stixshifter.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         connector: elastic_ecs
         connection:
             host: elastic.securitylog.company.com
             port: 9200
             indices: host101
             options:
                 retrieval_batch_size: 10000
+                single_batch_timeout: 120
                 dialects:
                     - beats
         config:
             auth:
                 id: profileB
                 api_key: asdf
 """
@@ -77,21 +78,25 @@
 
         ss_config = s.config["datasources"]["kestrel_datasource_stixshifter"]
         ss_profiles = ss_config["profiles"]
         connector_name, connection, configuration, retrieval_batch_size = get_datasource_from_profiles("host101", ss_profiles)
         assert connector_name == "elastic_ecs"
         assert configuration["auth"]["id"] == "profileA"
         assert configuration["auth"]["api_key"] == "qwer"
+        assert connection["options"]["timeout"] == 60
+        assert connection["options"]["result_limit"] == 2000 * 2
         assert retrieval_batch_size == 2000
 
         with open(profile_file, "w") as pf:
             pf.write(profileB)
 
         s.data_source_manager.list_data_sources_from_scheme("stixshifter")
 
         # need to refresh the pointers since the dict is updated
         ss_profiles = ss_config["profiles"]
         connector_name, connection, configuration, retrieval_batch_size = get_datasource_from_profiles("host101", ss_profiles)
         assert connector_name == "elastic_ecs"
         assert configuration["auth"]["id"] == "profileB"
         assert configuration["auth"]["api_key"] == "asdf"
+        assert connection["options"]["timeout"] == 120
+        assert connection["options"]["result_limit"] == 10000 * 2
         assert retrieval_batch_size == 10000
```

### Comparing `kestrel-lang-1.6.0/tests/test_timestamped.py` & `kestrel-lang-1.6.1/tests/test_timestamped.py`

 * *Files identical despite different names*

