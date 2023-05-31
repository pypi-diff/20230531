# Comparing `tmp/quark-engine-23.4.1.tar.gz` & `tmp/quark-engine-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quark-engine-23.4.1.tar", last modified: Wed Apr 26 07:28:06 2023, max compression
+gzip compressed data, was "quark-engine-23.5.1.tar", last modified: Wed May 31 09:01:49 2023, max compression
```

## Comparing `quark-engine-23.4.1.tar` & `quark-engine-23.5.1.tar`

### file list

```diff
@@ -1,76 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 07:27:50.000000 quark-engine-23.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-04-26 07:28:06.557241 quark-engine-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-26 07:27:50.000000 quark-engine-23.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/apkinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/core/axmlreader/
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/axmlreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/axmlreader/axml_definition
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.553241 quark-engine-23.4.1/quark/core/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/interface/baseapkinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/parallelquark.py
--rw-r--r--   0 runner    (1001) docker     (123)    30135 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/quark.py
--rw-r--r--   0 runner    (1001) docker     (123)    19911 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/rzapkinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/core/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/bytecodeobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/methodobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/registerobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/ruleobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/core/struct/tableobject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/evaluator/pyeval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/forensic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/forensic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/forensic/forensic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/forensic/vt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/freshquark.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/radiocontrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/rulegeneration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/script/
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/ciphey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/script/frida/
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/frida/agent.js
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/objection.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/script/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/utils/weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark/webreport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/analysis_report_layout.html
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-26 07:27:51.000000 quark-engine-23.4.1/quark/webreport/genrule_report_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/quark_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 07:28:06.000000 quark-engine-23.4.1/quark_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:28:06.557241 quark-engine-23.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-26 07:27:51.000000 quark-engine-23.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:28:06.557241 quark-engine-23.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/test_freshquark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-26 07:27:51.000000 quark-engine-23.4.1/tests/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 09:01:40.000000 quark-engine-23.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-05-31 09:01:49.125172 quark-engine-23.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-31 09:01:40.000000 quark-engine-23.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.121172 quark-engine-23.5.1/quark/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13512 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.121172 quark-engine-23.5.1/quark/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/apkinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.121172 quark-engine-23.5.1/quark/core/axmlreader/
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/axmlreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/axmlreader/axml_definition
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.121172 quark-engine-23.5.1/quark/core/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/interface/baseapkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/parallelquark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30135 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/quark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19911 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/rzapkinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark/core/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/struct/bytecodeobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/struct/methodobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/struct/registerobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/struct/ruleobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/core/struct/tableobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/evaluator/pyeval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark/forensic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/forensic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/forensic/forensic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/forensic/vt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/freshquark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/radiocontrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/rulegeneration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark/script/
+-rw-r--r--   0 runner    (1001) docker     (123)    21277 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/script/ciphey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark/script/frida/
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/script/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/script/frida/agent.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/script/objection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/script/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/utils/weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark/webreport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/webreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21921 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/webreport/analysis_report_layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/webreport/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-05-31 09:01:40.000000 quark-engine-23.5.1/quark/webreport/genrule_report_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:49.125172 quark-engine-23.5.1/quark_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-05-31 09:01:49.000000 quark-engine-23.5.1/quark_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 09:01:49.000000 quark-engine-23.5.1/quark_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:01:49.000000 quark-engine-23.5.1/quark_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 09:01:49.000000 quark-engine-23.5.1/quark_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-31 09:01:49.000000 quark-engine-23.5.1/quark_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 09:01:49.000000 quark-engine-23.5.1/quark_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:01:49.125172 quark-engine-23.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-31 09:01:40.000000 quark-engine-23.5.1/setup.py
```

### Comparing `quark-engine-23.4.1/LICENSE` & `quark-engine-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/PKG-INFO` & `quark-engine-23.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quark-engine
-Version: 23.4.1
+Version: 23.5.1
 Summary: An Obfuscation-Neglect Android Malware Scoring System
 Home-page: https://github.com/quark-engine/quark-engine
 Author: YuShiang Dang, ShengFeng Lu, KunYu Chen
 Author-email: pulorsok@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -67,28 +67,31 @@
 *   Quark Script is now in a beta version. We'll keep releasing practical APIs and analysis scenarios.
 *   **See API document [here](https://quark-engine.readthedocs.io/en/latest/quark_script.html#introduce-of-quark-script-apis).**
 
 # CWE Showcases
 *   [CWE-020](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-20-in-android-application-diva-apk)  Improper Input Validation 
 *   [CWE-022](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-22-in-android-application-ovaa-apk-and-insecurebankv2-apk)  Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal') 
 *   [CWE-023](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-23-in-android-application-ovaa-apk-and-insecurebankv2-apk)  Relative Path Traversal
+*   [CWE-073](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-73-in-android-application-ovaa-apk)   External Control of File Name or Path 
+*   [CWE-088](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-88-in-android-application-vuldroid-apk)  Improper Neutralization of Argument Delimiters in a Command
 *   [CWE-089](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-89-in-android-application-androgoat-apk)  Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection') 
 *   [CWE-094](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-94-in-android-application-ovaa-apk)  Improper Control of Generation of Code ('Code Injection') 
 *   [CWE-295](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-295-in-android-application-insecureshop-apk)  Improper Certificate Validation 
 *   [CWE-312](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-312-in-android-application-ovaa-apk)  Cleartext Storage of Sensitive Information 
 *   [CWE-319](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-319-in-android-application-ovaa-apk)  Cleartext Transmission of Sensitive Information 
 *   [CWE-327](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-327-in-android-application-injuredandroid-apk)  Use of a Broken or Risky Cryptographic Algorithm 
 *   [CWE-328](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-328-in-android-application-allsafe-apk)  Use of Weak Hash 
 *   [CWE-338](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-338-in-android-application-pivva-apk)  Use of Cryptographically Weak Pseudo-Random Number Generator (PRNG) 
 *   [CWE-489](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-489-in-android-application-allsafe-apk-androgoat-apk-pivaa-apk)  Active Debug Code 
 *   [CWE-532](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-532-in-android-application-dvba-apk)  Insertion of Sensitive Information into Log File 
 *   [CWE-749](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-749-in-android-application-mstg-android-java-apk)  Exposed Dangerous Method or Function 
 *   [CWE-780](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-780-in-android-application-mstg-android-java-apk)  Use of RSA Algorithm without OAEP 
 *   [CWE-798](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-798-in-android-application-ovaa-apk)  Use of Hard-coded Credentials 
 *   [CWE-921](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-921-in-android-application-ovaa-apk)  Storage of Sensitive Data in a Mechanism without Access Control 
+*   [CWE-925](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-925-in-android-application-insecurebankv2-androgoat)  Improper Verification of Intent by Broadcast Receiver
 *   [CWE-926](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-926-in-android-application-dvba-apk)  Improper Export of Android Application Components 
  
 # Quick Start
 
 In this section, we will show how to detect CWE-798 with Quark Script.
 
 ### Step 1: Environments Requirements
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quark-engine Version: 23.4.1 Summary: An
+Metadata-Version: 2.1 Name: quark-engine Version: 23.5.1 Summary: An
 Obfuscation-Neglect Android Malware Scoring System Home-page: https://
 github.com/quark-engine/quark-engine Author: YuShiang Dang, ShengFeng Lu, KunYu
 Chen Author-email: pulorsok@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Topic ::
 Security Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,49 +28,56 @@
 apis).** # CWE Showcases * [CWE-020](https://quark-engine.readthedocs.io/en/
 latest/quark_script.html#detect-cwe-20-in-android-application-diva-apk)
 Improper Input Validation * [CWE-022](https://quark-engine.readthedocs.io/en/
 latest/quark_script.html#detect-cwe-22-in-android-application-ovaa-apk-and-
 insecurebankv2-apk) Improper Limitation of a Pathname to a Restricted Directory
 ('Path Traversal') * [CWE-023](https://quark-engine.readthedocs.io/en/latest/
 quark_script.html#detect-cwe-23-in-android-application-ovaa-apk-and-
-insecurebankv2-apk) Relative Path Traversal * [CWE-089](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-89-in-android-
-application-androgoat-apk) Improper Neutralization of Special Elements used in
-an SQL Command ('SQL Injection') * [CWE-094](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-94-in-android-
-application-ovaa-apk) Improper Control of Generation of Code ('Code Injection')
-* [CWE-295](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-295-in-android-application-insecureshop-apk)
-Improper Certificate Validation * [CWE-312](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-312-in-android-
-application-ovaa-apk) Cleartext Storage of Sensitive Information * [CWE-319]
+insecurebankv2-apk) Relative Path Traversal * [CWE-073](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-73-in-android-
+application-ovaa-apk) External Control of File Name or Path * [CWE-088](https:/
+/quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-88-in-
+android-application-vuldroid-apk) Improper Neutralization of Argument
+Delimiters in a Command * [CWE-089](https://quark-engine.readthedocs.io/en/
+latest/quark_script.html#detect-cwe-89-in-android-application-androgoat-apk)
+Improper Neutralization of Special Elements used in an SQL Command ('SQL
+Injection') * [CWE-094](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-94-in-android-application-ovaa-apk) Improper
+Control of Generation of Code ('Code Injection') * [CWE-295](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-295-in-android-
+application-insecureshop-apk) Improper Certificate Validation * [CWE-312]
 (https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-
-319-in-android-application-ovaa-apk) Cleartext Transmission of Sensitive
-Information * [CWE-327](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-327-in-android-application-injuredandroid-apk) Use
-of a Broken or Risky Cryptographic Algorithm * [CWE-328](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-328-in-android-
-application-allsafe-apk) Use of Weak Hash * [CWE-338](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-338-in-android-
-application-pivva-apk) Use of Cryptographically Weak Pseudo-Random Number
-Generator (PRNG) * [CWE-489](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-489-in-android-application-allsafe-apk-androgoat-
-apk-pivaa-apk) Active Debug Code * [CWE-532](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-532-in-android-
-application-dvba-apk) Insertion of Sensitive Information into Log File * [CWE-
-749](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-
-cwe-749-in-android-application-mstg-android-java-apk) Exposed Dangerous Method
-or Function * [CWE-780](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-780-in-android-application-mstg-android-java-apk)
-Use of RSA Algorithm without OAEP * [CWE-798](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-798-in-android-
-application-ovaa-apk) Use of Hard-coded Credentials * [CWE-921](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-921-in-android-
-application-ovaa-apk) Storage of Sensitive Data in a Mechanism without Access
-Control * [CWE-926](https://quark-engine.readthedocs.io/en/latest/
+312-in-android-application-ovaa-apk) Cleartext Storage of Sensitive Information
+* [CWE-319](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-319-in-android-application-ovaa-apk) Cleartext
+Transmission of Sensitive Information * [CWE-327](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-327-in-android-
+application-injuredandroid-apk) Use of a Broken or Risky Cryptographic
+Algorithm * [CWE-328](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-328-in-android-application-allsafe-apk) Use of
+Weak Hash * [CWE-338](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-338-in-android-application-pivva-apk) Use of
+Cryptographically Weak Pseudo-Random Number Generator (PRNG) * [CWE-489](https:
+//quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-489-in-
+android-application-allsafe-apk-androgoat-apk-pivaa-apk) Active Debug Code *
+[CWE-532](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-532-in-android-application-dvba-apk) Insertion of
+Sensitive Information into Log File * [CWE-749](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-749-in-android-
+application-mstg-android-java-apk) Exposed Dangerous Method or Function * [CWE-
+780](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-
+cwe-780-in-android-application-mstg-android-java-apk) Use of RSA Algorithm
+without OAEP * [CWE-798](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-798-in-android-application-ovaa-apk) Use of Hard-
+coded Credentials * [CWE-921](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-921-in-android-application-ovaa-apk) Storage of
+Sensitive Data in a Mechanism without Access Control * [CWE-925](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-925-in-android-
+application-insecurebankv2-androgoat) Improper Verification of Intent by
+Broadcast Receiver * [CWE-926](https://quark-engine.readthedocs.io/en/latest/
 quark_script.html#detect-cwe-926-in-android-application-dvba-apk) Improper
 Export of Android Application Components # Quick Start In this section, we will
 show how to detect CWE-798 with Quark Script. ### Step 1: Environments
 Requirements * Quark requires Python 3.8 or above. ### Step 2: Install Quark
 Engine * Install Quark Engine by running: ```bash $ pip3 install -U quark-
 engine ``` ### Step 3: Prepare Quark Script, Detection Rule and the Sample File
 1. Get the CWE-798 Quark Script and the detection rule [here](https://quark-
```

### Comparing `quark-engine-23.4.1/README.md` & `quark-engine-23.5.1/quark_engine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: quark-engine
+Version: 23.5.1
+Summary: An Obfuscation-Neglect Android Malware Scoring System
+Home-page: https://github.com/quark-engine/quark-engine
+Author: YuShiang Dang, ShengFeng Lu, KunYu Chen
+Author-email: pulorsok@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
     <a href="https://www.blackhat.com/asia-21/arsenal/schedule/index.html#quark-engine-storyteller-of-android-malware-22458">
         <img alt="Black Hat Arsenal" src="https://img.shields.io/badge/Black%20Hat%20Arsenal-Asia%202021-blue">
     </a>
     <a href="https://conference.hitb.org/hitb-lockdown002/sessions/quark-engine-an-obfuscation-neglect-android-malware-scoring-system/">
         <img alt="HITB" src="https://img.shields.io/badge/HITB-Lockdown%20002-red">
     </a>
@@ -52,28 +67,31 @@
 *   Quark Script is now in a beta version. We'll keep releasing practical APIs and analysis scenarios.
 *   **See API document [here](https://quark-engine.readthedocs.io/en/latest/quark_script.html#introduce-of-quark-script-apis).**
 
 # CWE Showcases
 *   [CWE-020](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-20-in-android-application-diva-apk)  Improper Input Validation 
 *   [CWE-022](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-22-in-android-application-ovaa-apk-and-insecurebankv2-apk)  Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal') 
 *   [CWE-023](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-23-in-android-application-ovaa-apk-and-insecurebankv2-apk)  Relative Path Traversal
+*   [CWE-073](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-73-in-android-application-ovaa-apk)   External Control of File Name or Path 
+*   [CWE-088](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-88-in-android-application-vuldroid-apk)  Improper Neutralization of Argument Delimiters in a Command
 *   [CWE-089](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-89-in-android-application-androgoat-apk)  Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection') 
 *   [CWE-094](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-94-in-android-application-ovaa-apk)  Improper Control of Generation of Code ('Code Injection') 
 *   [CWE-295](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-295-in-android-application-insecureshop-apk)  Improper Certificate Validation 
 *   [CWE-312](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-312-in-android-application-ovaa-apk)  Cleartext Storage of Sensitive Information 
 *   [CWE-319](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-319-in-android-application-ovaa-apk)  Cleartext Transmission of Sensitive Information 
 *   [CWE-327](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-327-in-android-application-injuredandroid-apk)  Use of a Broken or Risky Cryptographic Algorithm 
 *   [CWE-328](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-328-in-android-application-allsafe-apk)  Use of Weak Hash 
 *   [CWE-338](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-338-in-android-application-pivva-apk)  Use of Cryptographically Weak Pseudo-Random Number Generator (PRNG) 
 *   [CWE-489](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-489-in-android-application-allsafe-apk-androgoat-apk-pivaa-apk)  Active Debug Code 
 *   [CWE-532](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-532-in-android-application-dvba-apk)  Insertion of Sensitive Information into Log File 
 *   [CWE-749](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-749-in-android-application-mstg-android-java-apk)  Exposed Dangerous Method or Function 
 *   [CWE-780](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-780-in-android-application-mstg-android-java-apk)  Use of RSA Algorithm without OAEP 
 *   [CWE-798](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-798-in-android-application-ovaa-apk)  Use of Hard-coded Credentials 
 *   [CWE-921](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-921-in-android-application-ovaa-apk)  Storage of Sensitive Data in a Mechanism without Access Control 
+*   [CWE-925](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-925-in-android-application-insecurebankv2-androgoat)  Improper Verification of Intent by Broadcast Receiver
 *   [CWE-926](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-926-in-android-application-dvba-apk)  Improper Export of Android Application Components 
  
 # Quick Start
 
 In this section, we will show how to detect CWE-798 with Quark Script.
 
 ### Step 1: Environments Requirements
```

#### html2text {}

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1 Name: quark-engine Version: 23.5.1 Summary: An
+Obfuscation-Neglect Android Malware Scoring System Home-page: https://
+github.com/quark-engine/quark-engine Author: YuShiang Dang, ShengFeng Lu, KunYu
+Chen Author-email: pulorsok@gmail.com Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Topic ::
+Security Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE
                  [Black_Hat_Arsenal] [HITB] [rootcon] [defcon]
       [build_status] [codecov] [license] [python_version] [PyPi_Download]
                                    [Twitter]
                        [https://i.imgur.com/8GwkWei.png]
 # Quark Script - Dig Vulnerabilities in the BlackBox ### Innovative &
 Interactive * The goal of Quark Script aims to provide an innovative way for
 mobile security researchers to analyze or **pentest** the targets. * Based on
@@ -20,49 +28,56 @@
 apis).** # CWE Showcases * [CWE-020](https://quark-engine.readthedocs.io/en/
 latest/quark_script.html#detect-cwe-20-in-android-application-diva-apk)
 Improper Input Validation * [CWE-022](https://quark-engine.readthedocs.io/en/
 latest/quark_script.html#detect-cwe-22-in-android-application-ovaa-apk-and-
 insecurebankv2-apk) Improper Limitation of a Pathname to a Restricted Directory
 ('Path Traversal') * [CWE-023](https://quark-engine.readthedocs.io/en/latest/
 quark_script.html#detect-cwe-23-in-android-application-ovaa-apk-and-
-insecurebankv2-apk) Relative Path Traversal * [CWE-089](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-89-in-android-
-application-androgoat-apk) Improper Neutralization of Special Elements used in
-an SQL Command ('SQL Injection') * [CWE-094](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-94-in-android-
-application-ovaa-apk) Improper Control of Generation of Code ('Code Injection')
-* [CWE-295](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-295-in-android-application-insecureshop-apk)
-Improper Certificate Validation * [CWE-312](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-312-in-android-
-application-ovaa-apk) Cleartext Storage of Sensitive Information * [CWE-319]
+insecurebankv2-apk) Relative Path Traversal * [CWE-073](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-73-in-android-
+application-ovaa-apk) External Control of File Name or Path * [CWE-088](https:/
+/quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-88-in-
+android-application-vuldroid-apk) Improper Neutralization of Argument
+Delimiters in a Command * [CWE-089](https://quark-engine.readthedocs.io/en/
+latest/quark_script.html#detect-cwe-89-in-android-application-androgoat-apk)
+Improper Neutralization of Special Elements used in an SQL Command ('SQL
+Injection') * [CWE-094](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-94-in-android-application-ovaa-apk) Improper
+Control of Generation of Code ('Code Injection') * [CWE-295](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-295-in-android-
+application-insecureshop-apk) Improper Certificate Validation * [CWE-312]
 (https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-
-319-in-android-application-ovaa-apk) Cleartext Transmission of Sensitive
-Information * [CWE-327](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-327-in-android-application-injuredandroid-apk) Use
-of a Broken or Risky Cryptographic Algorithm * [CWE-328](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-328-in-android-
-application-allsafe-apk) Use of Weak Hash * [CWE-338](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-338-in-android-
-application-pivva-apk) Use of Cryptographically Weak Pseudo-Random Number
-Generator (PRNG) * [CWE-489](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-489-in-android-application-allsafe-apk-androgoat-
-apk-pivaa-apk) Active Debug Code * [CWE-532](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-532-in-android-
-application-dvba-apk) Insertion of Sensitive Information into Log File * [CWE-
-749](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-
-cwe-749-in-android-application-mstg-android-java-apk) Exposed Dangerous Method
-or Function * [CWE-780](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-780-in-android-application-mstg-android-java-apk)
-Use of RSA Algorithm without OAEP * [CWE-798](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-798-in-android-
-application-ovaa-apk) Use of Hard-coded Credentials * [CWE-921](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-921-in-android-
-application-ovaa-apk) Storage of Sensitive Data in a Mechanism without Access
-Control * [CWE-926](https://quark-engine.readthedocs.io/en/latest/
+312-in-android-application-ovaa-apk) Cleartext Storage of Sensitive Information
+* [CWE-319](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-319-in-android-application-ovaa-apk) Cleartext
+Transmission of Sensitive Information * [CWE-327](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-327-in-android-
+application-injuredandroid-apk) Use of a Broken or Risky Cryptographic
+Algorithm * [CWE-328](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-328-in-android-application-allsafe-apk) Use of
+Weak Hash * [CWE-338](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-338-in-android-application-pivva-apk) Use of
+Cryptographically Weak Pseudo-Random Number Generator (PRNG) * [CWE-489](https:
+//quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-489-in-
+android-application-allsafe-apk-androgoat-apk-pivaa-apk) Active Debug Code *
+[CWE-532](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-532-in-android-application-dvba-apk) Insertion of
+Sensitive Information into Log File * [CWE-749](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-749-in-android-
+application-mstg-android-java-apk) Exposed Dangerous Method or Function * [CWE-
+780](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-
+cwe-780-in-android-application-mstg-android-java-apk) Use of RSA Algorithm
+without OAEP * [CWE-798](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-798-in-android-application-ovaa-apk) Use of Hard-
+coded Credentials * [CWE-921](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-921-in-android-application-ovaa-apk) Storage of
+Sensitive Data in a Mechanism without Access Control * [CWE-925](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-925-in-android-
+application-insecurebankv2-androgoat) Improper Verification of Intent by
+Broadcast Receiver * [CWE-926](https://quark-engine.readthedocs.io/en/latest/
 quark_script.html#detect-cwe-926-in-android-application-dvba-apk) Improper
 Export of Android Application Components # Quick Start In this section, we will
 show how to detect CWE-798 with Quark Script. ### Step 1: Environments
 Requirements * Quark requires Python 3.8 or above. ### Step 2: Install Quark
 Engine * Install Quark Engine by running: ```bash $ pip3 install -U quark-
 engine ``` ### Step 3: Prepare Quark Script, Detection Rule and the Sample File
 1. Get the CWE-798 Quark Script and the detection rule [here](https://quark-
```

### Comparing `quark-engine-23.4.1/quark/cli.py` & `quark-engine-23.5.1/quark/cli.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/analysis.py` & `quark-engine-23.5.1/quark/core/analysis.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/apkinfo.py` & `quark-engine-23.5.1/quark/core/apkinfo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/axmlreader/__init__.py` & `quark-engine-23.5.1/quark/core/axmlreader/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/axmlreader/axml_definition` & `quark-engine-23.5.1/quark/core/axmlreader/axml_definition`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/interface/baseapkinfo.py` & `quark-engine-23.5.1/quark/core/interface/baseapkinfo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/parallelquark.py` & `quark-engine-23.5.1/quark/core/parallelquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/quark.py` & `quark-engine-23.5.1/quark/core/quark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/rzapkinfo.py` & `quark-engine-23.5.1/quark/core/rzapkinfo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/struct/bytecodeobject.py` & `quark-engine-23.5.1/quark/core/struct/bytecodeobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/struct/methodobject.py` & `quark-engine-23.5.1/quark/core/struct/methodobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/struct/registerobject.py` & `quark-engine-23.5.1/quark/core/struct/registerobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/struct/ruleobject.py` & `quark-engine-23.5.1/quark/core/struct/ruleobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/core/struct/tableobject.py` & `quark-engine-23.5.1/quark/core/struct/tableobject.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/evaluator/pyeval.py` & `quark-engine-23.5.1/quark/evaluator/pyeval.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/forensic/forensic.py` & `quark-engine-23.5.1/quark/forensic/forensic.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/forensic/vt_analysis.py` & `quark-engine-23.5.1/quark/forensic/vt_analysis.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/freshquark.py` & `quark-engine-23.5.1/quark/freshquark.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/logo.py` & `quark-engine-23.5.1/quark/logo.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/radiocontrast.py` & `quark-engine-23.5.1/quark/radiocontrast.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/report.py` & `quark-engine-23.5.1/quark/report.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/rulegeneration.py` & `quark-engine-23.5.1/quark/rulegeneration.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/script/__init__.py` & `quark-engine-23.5.1/quark/script/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is part of Quark-Engine - https://github.com/quark-engine/quark-engine
 # See the file 'LICENSE' for copying permission.
 
 import re
 import functools
 from os import PathLike
 from os.path import abspath, isfile, join
-from typing import Any, List, Tuple, Union
+from typing import Any, Iterable, List, Tuple, Union
 
 from quark.config import DIR_PATH as QUARK_RULE_PATH
 from quark.core.analysis import QuarkAnalysis
 from quark.core.interface.baseapkinfo import XMLElement
 from quark.core.quark import Quark
 from quark.core.struct.methodobject import MethodObject
 from quark.core.struct.ruleobject import RuleObject as Rule
@@ -109,14 +109,54 @@
 
         :return: True/False
         """
         exported = self._getAttribute("exported", self.hasIntentFilter())
         return exported
 
 
+class Receiver:
+    def __init__(self, xml: XMLElement) -> None:
+        self.xml: XMLElement = xml
+
+    def __str__(self) -> str:
+        return self._getAttribute("name")
+
+    def _getAttribute(
+        self, attributeName: str, defaultValue: Any = None
+    ) -> Any:
+        realAttributeName = (
+            f"{{http://schemas.android.com/apk/res/android}}{attributeName}"
+        )
+        return self.xml.get(realAttributeName, defaultValue)
+
+    def hasIntentFilter(self) -> bool:
+        """Check if the receiver has an intent filter.
+
+        :return: True/False
+        """
+        return self.xml.find("intent-filter") is not None
+
+    def isExported(self) -> bool:
+        """Check if the receiver is exported.
+
+        According to the documentation from Android Developer guide.
+        "
+        If the attribute exported is unspecified, the default value depends on whether
+        the broadcast receiver contains intent filters.
+        If the receiver contains at least one intent filter,
+        then the default value is "true".
+        Otherwise, the default value is "false".
+        "
+
+        :return: True/False
+        """
+        exported = self._getAttribute("exported", self.hasIntentFilter())
+        return str(exported).lower() == 'true'
+
+
 class Method:
     def __init__(
         self,
         quarkResultInstance: "QuarkResult" = None,
         methodObj: MethodObject = None,
         quark: "Quark" = None,
         behavior: "Behavior" = None,
@@ -519,14 +559,26 @@
     """
     quark = _getQuark(samplePath)
     apkinfo = quark.apkinfo
 
     return [Activity(xml) for xml in apkinfo.activities]
 
 
+def getReceivers(samplePath: PathLike) -> List[Receiver]:
+    """Get receivers from a target sample.
+
+    :param samplePath: target file
+    :return: python list containing receivers
+    """
+    quark = _getQuark(samplePath)
+    apkinfo = quark.apkinfo
+
+    return [Receiver(xml) for xml in apkinfo.receivers]
+
+
 def getApplication(samplePath: PathLike) -> Application:
     """Get the application element from the manifest file of the target sample.
 
     :param samplePath: the file path of the target sample
     :return: the application element of the target sample
     """
     quark = _getQuark(samplePath)
@@ -575,7 +627,45 @@
         methodInstance = Method(methodObj=method)
         caller_set = quark.apkinfo.upperfunc(method)
         caller_methods += [
             _wrapMethodObject(quark, caller, methodInstance)
             for caller in list(caller_set)
         ]
     return caller_methods
+
+
+def checkMethodCalls(
+        samplePath: PathLike,
+        targetMethod: Union[Tuple[str, str, str], MethodObject],
+        checkMethods: List[Tuple[str, str, str]]) -> bool:
+    """Check if any of the specific methods shown in the `targetMethod`
+
+    :param samplePath: target file
+    :param targetMethod: python list contains the class name,
+                         method name, and descriptor of the target method
+                         or a Method Object.
+    :param checkMethods: python list contains the class name,
+                         method name, and descriptor of the target method
+
+    :return: bool that indicate specific methods can be called or defined within a `target method` or not.
+    """
+    targetMethodSet = set()
+    checkMethodSet = set()
+    targetLowerFuncSet = set()
+
+    quark = _getQuark(samplePath)
+    if isinstance(targetMethod, Iterable):
+        # Find the method in the APK with the given class name, method name, and descriptor
+        targetMethodSet.update(quark.apkinfo.find_method(*targetMethod))
+    else:
+        # targetMethod is already a Method object
+        targetMethodSet.add(MethodObject)
+
+    if not targetMethodSet:
+        return False
+
+    for candidate in checkMethods:
+        checkMethodSet.update(quark.apkinfo.find_method(*candidate))
+
+    targetLowerFuncSet = {i for i, _ in quark.apkinfo.lowerfunc(targetMethodSet.pop())}
+
+    return any(checkMethodSet.intersection(targetLowerFuncSet))
```

### Comparing `quark-engine-23.4.1/quark/script/frida/__init__.py` & `quark-engine-23.5.1/quark/script/frida/__init__.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/script/frida/agent.js` & `quark-engine-23.5.1/quark/script/frida/agent.js`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/script/objection.py` & `quark-engine-23.5.1/quark/script/objection.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/utils/colors.py` & `quark-engine-23.5.1/quark/utils/colors.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/utils/graph.py` & `quark-engine-23.5.1/quark/utils/graph.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/utils/output.py` & `quark-engine-23.5.1/quark/utils/output.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/utils/pprint.py` & `quark-engine-23.5.1/quark/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/utils/regex.py` & `quark-engine-23.5.1/quark/utils/regex.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/utils/tools.py` & `quark-engine-23.5.1/quark/utils/tools.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/utils/weight.py` & `quark-engine-23.5.1/quark/utils/weight.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/webreport/analysis_report_layout.html` & `quark-engine-23.5.1/quark/webreport/analysis_report_layout.html`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/webreport/generate.py` & `quark-engine-23.5.1/quark/webreport/generate.py`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark/webreport/genrule_report_layout.html` & `quark-engine-23.5.1/quark/webreport/genrule_report_layout.html`

 * *Files identical despite different names*

### Comparing `quark-engine-23.4.1/quark_engine.egg-info/PKG-INFO` & `quark-engine-23.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: quark-engine
-Version: 23.4.1
-Summary: An Obfuscation-Neglect Android Malware Scoring System
-Home-page: https://github.com/quark-engine/quark-engine
-Author: YuShiang Dang, ShengFeng Lu, KunYu Chen
-Author-email: pulorsok@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Security
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
     <a href="https://www.blackhat.com/asia-21/arsenal/schedule/index.html#quark-engine-storyteller-of-android-malware-22458">
         <img alt="Black Hat Arsenal" src="https://img.shields.io/badge/Black%20Hat%20Arsenal-Asia%202021-blue">
     </a>
     <a href="https://conference.hitb.org/hitb-lockdown002/sessions/quark-engine-an-obfuscation-neglect-android-malware-scoring-system/">
         <img alt="HITB" src="https://img.shields.io/badge/HITB-Lockdown%20002-red">
     </a>
@@ -67,28 +52,31 @@
 *   Quark Script is now in a beta version. We'll keep releasing practical APIs and analysis scenarios.
 *   **See API document [here](https://quark-engine.readthedocs.io/en/latest/quark_script.html#introduce-of-quark-script-apis).**
 
 # CWE Showcases
 *   [CWE-020](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-20-in-android-application-diva-apk)  Improper Input Validation 
 *   [CWE-022](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-22-in-android-application-ovaa-apk-and-insecurebankv2-apk)  Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal') 
 *   [CWE-023](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-23-in-android-application-ovaa-apk-and-insecurebankv2-apk)  Relative Path Traversal
+*   [CWE-073](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-73-in-android-application-ovaa-apk)   External Control of File Name or Path 
+*   [CWE-088](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-88-in-android-application-vuldroid-apk)  Improper Neutralization of Argument Delimiters in a Command
 *   [CWE-089](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-89-in-android-application-androgoat-apk)  Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection') 
 *   [CWE-094](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-94-in-android-application-ovaa-apk)  Improper Control of Generation of Code ('Code Injection') 
 *   [CWE-295](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-295-in-android-application-insecureshop-apk)  Improper Certificate Validation 
 *   [CWE-312](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-312-in-android-application-ovaa-apk)  Cleartext Storage of Sensitive Information 
 *   [CWE-319](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-319-in-android-application-ovaa-apk)  Cleartext Transmission of Sensitive Information 
 *   [CWE-327](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-327-in-android-application-injuredandroid-apk)  Use of a Broken or Risky Cryptographic Algorithm 
 *   [CWE-328](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-328-in-android-application-allsafe-apk)  Use of Weak Hash 
 *   [CWE-338](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-338-in-android-application-pivva-apk)  Use of Cryptographically Weak Pseudo-Random Number Generator (PRNG) 
 *   [CWE-489](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-489-in-android-application-allsafe-apk-androgoat-apk-pivaa-apk)  Active Debug Code 
 *   [CWE-532](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-532-in-android-application-dvba-apk)  Insertion of Sensitive Information into Log File 
 *   [CWE-749](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-749-in-android-application-mstg-android-java-apk)  Exposed Dangerous Method or Function 
 *   [CWE-780](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-780-in-android-application-mstg-android-java-apk)  Use of RSA Algorithm without OAEP 
 *   [CWE-798](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-798-in-android-application-ovaa-apk)  Use of Hard-coded Credentials 
 *   [CWE-921](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-921-in-android-application-ovaa-apk)  Storage of Sensitive Data in a Mechanism without Access Control 
+*   [CWE-925](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-925-in-android-application-insecurebankv2-androgoat)  Improper Verification of Intent by Broadcast Receiver
 *   [CWE-926](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-926-in-android-application-dvba-apk)  Improper Export of Android Application Components 
  
 # Quick Start
 
 In this section, we will show how to detect CWE-798 with Quark Script.
 
 ### Step 1: Environments Requirements
```

#### html2text {}

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1 Name: quark-engine Version: 23.4.1 Summary: An
-Obfuscation-Neglect Android Malware Scoring System Home-page: https://
-github.com/quark-engine/quark-engine Author: YuShiang Dang, ShengFeng Lu, KunYu
-Chen Author-email: pulorsok@gmail.com Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
-v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Topic ::
-Security Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
                  [Black_Hat_Arsenal] [HITB] [rootcon] [defcon]
       [build_status] [codecov] [license] [python_version] [PyPi_Download]
                                    [Twitter]
                        [https://i.imgur.com/8GwkWei.png]
 # Quark Script - Dig Vulnerabilities in the BlackBox ### Innovative &
 Interactive * The goal of Quark Script aims to provide an innovative way for
 mobile security researchers to analyze or **pentest** the targets. * Based on
@@ -28,49 +20,56 @@
 apis).** # CWE Showcases * [CWE-020](https://quark-engine.readthedocs.io/en/
 latest/quark_script.html#detect-cwe-20-in-android-application-diva-apk)
 Improper Input Validation * [CWE-022](https://quark-engine.readthedocs.io/en/
 latest/quark_script.html#detect-cwe-22-in-android-application-ovaa-apk-and-
 insecurebankv2-apk) Improper Limitation of a Pathname to a Restricted Directory
 ('Path Traversal') * [CWE-023](https://quark-engine.readthedocs.io/en/latest/
 quark_script.html#detect-cwe-23-in-android-application-ovaa-apk-and-
-insecurebankv2-apk) Relative Path Traversal * [CWE-089](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-89-in-android-
-application-androgoat-apk) Improper Neutralization of Special Elements used in
-an SQL Command ('SQL Injection') * [CWE-094](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-94-in-android-
-application-ovaa-apk) Improper Control of Generation of Code ('Code Injection')
-* [CWE-295](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-295-in-android-application-insecureshop-apk)
-Improper Certificate Validation * [CWE-312](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-312-in-android-
-application-ovaa-apk) Cleartext Storage of Sensitive Information * [CWE-319]
+insecurebankv2-apk) Relative Path Traversal * [CWE-073](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-73-in-android-
+application-ovaa-apk) External Control of File Name or Path * [CWE-088](https:/
+/quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-88-in-
+android-application-vuldroid-apk) Improper Neutralization of Argument
+Delimiters in a Command * [CWE-089](https://quark-engine.readthedocs.io/en/
+latest/quark_script.html#detect-cwe-89-in-android-application-androgoat-apk)
+Improper Neutralization of Special Elements used in an SQL Command ('SQL
+Injection') * [CWE-094](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-94-in-android-application-ovaa-apk) Improper
+Control of Generation of Code ('Code Injection') * [CWE-295](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-295-in-android-
+application-insecureshop-apk) Improper Certificate Validation * [CWE-312]
 (https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-
-319-in-android-application-ovaa-apk) Cleartext Transmission of Sensitive
-Information * [CWE-327](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-327-in-android-application-injuredandroid-apk) Use
-of a Broken or Risky Cryptographic Algorithm * [CWE-328](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-328-in-android-
-application-allsafe-apk) Use of Weak Hash * [CWE-338](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-338-in-android-
-application-pivva-apk) Use of Cryptographically Weak Pseudo-Random Number
-Generator (PRNG) * [CWE-489](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-489-in-android-application-allsafe-apk-androgoat-
-apk-pivaa-apk) Active Debug Code * [CWE-532](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-532-in-android-
-application-dvba-apk) Insertion of Sensitive Information into Log File * [CWE-
-749](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-
-cwe-749-in-android-application-mstg-android-java-apk) Exposed Dangerous Method
-or Function * [CWE-780](https://quark-engine.readthedocs.io/en/latest/
-quark_script.html#detect-cwe-780-in-android-application-mstg-android-java-apk)
-Use of RSA Algorithm without OAEP * [CWE-798](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-798-in-android-
-application-ovaa-apk) Use of Hard-coded Credentials * [CWE-921](https://quark-
-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-921-in-android-
-application-ovaa-apk) Storage of Sensitive Data in a Mechanism without Access
-Control * [CWE-926](https://quark-engine.readthedocs.io/en/latest/
+312-in-android-application-ovaa-apk) Cleartext Storage of Sensitive Information
+* [CWE-319](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-319-in-android-application-ovaa-apk) Cleartext
+Transmission of Sensitive Information * [CWE-327](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-327-in-android-
+application-injuredandroid-apk) Use of a Broken or Risky Cryptographic
+Algorithm * [CWE-328](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-328-in-android-application-allsafe-apk) Use of
+Weak Hash * [CWE-338](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-338-in-android-application-pivva-apk) Use of
+Cryptographically Weak Pseudo-Random Number Generator (PRNG) * [CWE-489](https:
+//quark-engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-489-in-
+android-application-allsafe-apk-androgoat-apk-pivaa-apk) Active Debug Code *
+[CWE-532](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-532-in-android-application-dvba-apk) Insertion of
+Sensitive Information into Log File * [CWE-749](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-749-in-android-
+application-mstg-android-java-apk) Exposed Dangerous Method or Function * [CWE-
+780](https://quark-engine.readthedocs.io/en/latest/quark_script.html#detect-
+cwe-780-in-android-application-mstg-android-java-apk) Use of RSA Algorithm
+without OAEP * [CWE-798](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-798-in-android-application-ovaa-apk) Use of Hard-
+coded Credentials * [CWE-921](https://quark-engine.readthedocs.io/en/latest/
+quark_script.html#detect-cwe-921-in-android-application-ovaa-apk) Storage of
+Sensitive Data in a Mechanism without Access Control * [CWE-925](https://quark-
+engine.readthedocs.io/en/latest/quark_script.html#detect-cwe-925-in-android-
+application-insecurebankv2-androgoat) Improper Verification of Intent by
+Broadcast Receiver * [CWE-926](https://quark-engine.readthedocs.io/en/latest/
 quark_script.html#detect-cwe-926-in-android-application-dvba-apk) Improper
 Export of Android Application Components # Quick Start In this section, we will
 show how to detect CWE-798 with Quark Script. ### Step 1: Environments
 Requirements * Quark requires Python 3.8 or above. ### Step 2: Install Quark
 Engine * Install Quark Engine by running: ```bash $ pip3 install -U quark-
 engine ``` ### Step 3: Prepare Quark Script, Detection Rule and the Sample File
 1. Get the CWE-798 Quark Script and the detection rule [here](https://quark-
```

### Comparing `quark-engine-23.4.1/quark_engine.egg-info/SOURCES.txt` & `quark-engine-23.5.1/quark_engine.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -49,12 +49,8 @@
 quark/webreport/generate.py
 quark/webreport/genrule_report_layout.html
 quark_engine.egg-info/PKG-INFO
 quark_engine.egg-info/SOURCES.txt
 quark_engine.egg-info/dependency_links.txt
 quark_engine.egg-info/entry_points.txt
 quark_engine.egg-info/requires.txt
-quark_engine.egg-info/top_level.txt
-tests/__init__.py
-tests/conftest.py
-tests/test_freshquark.py
-tests/test_report.py
+quark_engine.egg-info/top_level.txt
```

### Comparing `quark-engine-23.4.1/setup.py` & `quark-engine-23.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     version=__version__,
     author="YuShiang Dang, ShengFeng Lu, KunYu Chen",
     author_email="pulorsok@gmail.com",
     description="An Obfuscation-Neglect Android Malware Scoring System",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/quark-engine/quark-engine",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=("tests",)),
     package_data={
         "quark.core.axmlreader": ["axml_definition"],
         "quark.webreport": [
             "analysis_report_layout.html",
             "genrule_report_layout.html"
         ],
         "quark.script.frida": [
```

