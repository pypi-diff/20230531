# Comparing `tmp/cmind-1.2.2.tar.gz` & `tmp/cmind-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.2.2.tar", last modified: Tue May 30 19:25:32 2023, max compression
+gzip compressed data, was "cmind-1.3.0.tar", last modified: Wed May 31 18:35:57 2023, max compression
```

## Comparing `cmind-1.2.2.tar` & `cmind-1.3.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6057 2023-05-30 19:25:32.316357 cmind-1.2.2/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5127 2023-05-30 19:25:20.000000 cmind-1.2.2/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    46002 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    24428 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9326 2023-05-26 16:24:59.000000 cmind-1.2.2/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.296357 cmind-1.2.2/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.316357 cmind-1.2.2/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    31060 2023-05-30 19:25:20.000000 cmind-1.2.2/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.2.2/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-30 19:25:32.306357 cmind-1.2.2/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6057 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-25 12:15:08.000000 cmind-1.2.2/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-30 19:25:32.000000 cmind-1.2.2/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-30 19:25:32.316357 cmind-1.2.2/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-05-25 12:13:31.000000 cmind-1.2.2/setup.py
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.571146 cmind-1.3.0/
+-rw-rw-r--   0 ck        (1001) ck        (1001)    10174 2023-05-25 09:39:44.000000 cmind-1.3.0/LICENSE.CK.md
+-rw-rw-r--   0 ck        (1001) ck        (1001)    10174 2023-05-25 09:39:44.000000 cmind-1.3.0/LICENSE.md
+-rw-rw-r--   0 ck        (1001) ck        (1001)     5531 2023-05-31 18:35:57.571146 cmind-1.3.0/PKG-INFO
+-rw-rw-r--   0 ck        (1001) ck        (1001)     5127 2023-05-31 18:35:42.000000 cmind-1.3.0/README.md
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.563146 cmind-1.3.0/cmind/
+-rw-rw-r--   0 ck        (1001) ck        (1001)      136 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/__init__.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)       35 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/__main__.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     4908 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/artifact.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)    46874 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/automation.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     4213 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/cli.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     3285 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/config.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)    24606 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/core.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     9326 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/index.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     2046 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/net.py
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.567146 cmind-1.3.0/cmind/repo/
+-rw-rw-r--   0 ck        (1001) ck        (1001)      491 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/README.md
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.559146 cmind-1.3.0/cmind/repo/automation/
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.567146 cmind-1.3.0/cmind/repo/automation/automation/
+-rw-rw-r--   0 ck        (1001) ck        (1001)     2647 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/repo/automation/automation/README.md
+-rw-rw-r--   0 ck        (1001) ck        (1001)      289 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/automation/_cm.json
+-rw-rw-r--   0 ck        (1001) ck        (1001)     3799 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/automation/module.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     1518 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/automation/module_dummy.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     8772 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/automation/module_misc.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)      310 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/automation/template_list_of_automations.md
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.567146 cmind-1.3.0/cmind/repo/automation/ck/
+-rw-rw-r--   0 ck        (1001) ck        (1001)      984 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/repo/automation/ck/README.md
+-rw-rw-r--   0 ck        (1001) ck        (1001)      325 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/ck/_cm.json
+-rw-rw-r--   0 ck        (1001) ck        (1001)     1015 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/ck/module.py
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.567146 cmind-1.3.0/cmind/repo/automation/core/
+-rw-rw-r--   0 ck        (1001) ck        (1001)      996 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/repo/automation/core/README.md
+-rw-rw-r--   0 ck        (1001) ck        (1001)      302 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/core/_cm.json
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.567146 cmind-1.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-rw-r--   0 ck        (1001) ck        (1001)        0 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)      220 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)     1008 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/core/module.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)      220 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/core/module_misc.py
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.571146 cmind-1.3.0/cmind/repo/automation/repo/
+-rw-rw-r--   0 ck        (1001) ck        (1001)     9508 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/repo/automation/repo/README.md
+-rw-rw-r--   0 ck        (1001) ck        (1001)      377 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/automation/repo/_cm.json
+-rw-rw-r--   0 ck        (1001) ck        (1001)    31060 2023-05-31 18:35:42.000000 cmind-1.3.0/cmind/repo/automation/repo/module.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)       71 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo/cmr.yaml
+-rw-rw-r--   0 ck        (1001) ck        (1001)     1978 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repo.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)    18709 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/repos.py
+-rw-rw-r--   0 ck        (1001) ck        (1001)    41400 2023-05-25 09:39:44.000000 cmind-1.3.0/cmind/utils.py
+drwxrwxr-x   0 ck        (1001) ck        (1001)        0 2023-05-31 18:35:57.567146 cmind-1.3.0/cmind.egg-info/
+-rw-rw-r--   0 ck        (1001) ck        (1001)     5531 2023-05-31 18:35:57.000000 cmind-1.3.0/cmind.egg-info/PKG-INFO
+-rw-rw-r--   0 ck        (1001) ck        (1001)     1247 2023-05-31 18:35:57.000000 cmind-1.3.0/cmind.egg-info/SOURCES.txt
+-rw-rw-r--   0 ck        (1001) ck        (1001)        1 2023-05-31 18:35:57.000000 cmind-1.3.0/cmind.egg-info/dependency_links.txt
+-rw-rw-r--   0 ck        (1001) ck        (1001)       60 2023-05-31 18:35:57.000000 cmind-1.3.0/cmind.egg-info/entry_points.txt
+-rw-rw-r--   0 ck        (1001) ck        (1001)        1 2023-05-25 09:40:48.000000 cmind-1.3.0/cmind.egg-info/not-zip-safe
+-rw-rw-r--   0 ck        (1001) ck        (1001)       16 2023-05-31 18:35:57.000000 cmind-1.3.0/cmind.egg-info/requires.txt
+-rw-rw-r--   0 ck        (1001) ck        (1001)        6 2023-05-31 18:35:57.000000 cmind-1.3.0/cmind.egg-info/top_level.txt
+-rw-rw-r--   0 ck        (1001) ck        (1001)       38 2023-05-31 18:35:57.571146 cmind-1.3.0/setup.cfg
+-rw-rw-r--   0 ck        (1001) ck        (1001)     2668 2023-05-25 09:39:44.000000 cmind-1.3.0/setup.py
```

### Comparing `cmind-1.2.2/PKG-INFO` & `cmind-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,71 @@
-Metadata-Version: 2.1
-Name: cmind
-Version: 1.2.2
-Summary: cmind
-Home-page: https://github.com/mlcommons/ck/tree/master/cm
-Author: Grigori Fursin
-Author-email: grigori@octoml.ai
-License: Apache 2.0
-Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
-        [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
-        [![Downloads](https://pepy.tech/badge/cmind/month)](https://pepy.tech/project/cmind)
-        [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
-        
-        [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
-        [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
-        
-        ### About
-        
-        [Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
-        is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
-        It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
-        when reproducing experiments from more than 150 research papers and validating them in the real world - 
-        there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
-        on any platform with any software, hardware, and data.
-        
-        CM is being developed by the [public MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md) 
-        as a simple, intuitive, technology-agnostic, and English-like scripting language that provides
-        a universal interface to any software project and transforms it into a [database of portable and reusable CM scripts]( https://github.com/mlcommons/ck/tree/master/cm-mlops/script )
-        in a transparent and non-intrusive way.
-        
-        CM is powered by Python, JSON and/or YAML meta descriptions, and a unified CLI.
-        Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
-        unified README files and synthesize unified containers with a common API.
-        It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
-        while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
-        
-        CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
-        to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-        connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
-        and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
-        (cost, performance, power consumption, accuracy, etc).
-        
-        See a few real-world examples of using the CM scripting language:
-        - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
-        - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
-        - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
-        - [Auto-generated Docker containers to run and reproduce MLPerf inference benchmark](cm-mlops/script/app-mlperf-inference/dockerfiles/retinanet)
-        
-        
-        ### Documentation and the Getting Started Guide
-        
-        [Table of contents](https://github.com/mlcommons/ck/tree/master/docs/README.md)
-        
-        ### Collaborative development
-        
-        This open-source technology is being developed by the open
-        [MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
-        led by [Grigori Fursin](https://cKnowledge.org/gfursin) and
-        [Arjun Suresh](https://www.linkedin.com/in/arjunsuresh):
-        
-        * Join our [public Discord server](https://discord.gg/JjWNWXKxwT).
-        * Join our [public conf-calls](https://docs.google.com/document/d/1zMNK1m_LhWm6jimZK6YE05hu4VH9usdbKJ3nBy-ZPAw).
-        * Check our [news](docs/news.md).
-        * Check our [presentation](https://doi.org/10.5281/zenodo.7871070) and [Forbes article](https://www.forbes.com/sites/karlfreund/2023/04/05/nvidia-performance-trounces-all-competitors-who-have-the-guts-to-submit-to-mlperf-inference-30/?sh=3c38d2866676) about our development plans.
-        * Read about our [CK concept (previous version before MLCommons)](https://arxiv.org/abs/2011.01149).
-        
-        ### Copyright
-        
-        2021-2023 [MLCommons](https://mlcommons.org)
-        
-        ### License
-        
-        [Apache 2.0](LICENSE.md)
-        
-        ### Acknowledgments
-        
-        This project is currently supported by [MLCommons](https://mlcommons.org), [cTuning foundation](https://cTuning.org),
-        [cKnowledge](https://cKnowledge.org) and [individual contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md).
-        We thank [HiPEAC](https://hipeac.net) and [OctoML](https://octoml.ai) for sponsoring initial development.
-        
-Keywords: collective mind,cmind,cdatabase,cmeta,automation,reusability,meta,JSON,YAML,python
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+[![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
+[![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
+[![Downloads](https://pepy.tech/badge/cmind/month)](https://pepy.tech/project/cmind)
+[![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
+
+[![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
+[![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
+
+### About
+
+[Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
+is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
+It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
+when reproducing experiments from more than 150 research papers and validating them in the real world - 
+there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
+on any platform with any software, hardware, and data.
+
+CM is being developed by the [public MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md) 
+as a simple, intuitive, technology-agnostic, and English-like scripting language that provides
+a universal interface to any software project and transforms it into a [database of portable and reusable CM scripts]( https://github.com/mlcommons/ck/tree/master/cm-mlops/script )
+in a transparent and non-intrusive way.
+
+CM is powered by Python, JSON and/or YAML meta descriptions, and a unified CLI.
+Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
+unified README files and synthesize unified containers with a common API.
+It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
+while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
+
+CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
+to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
+connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
+(cost, performance, power consumption, accuracy, etc).
+
+See a few real-world examples of using the CM scripting language:
+- [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
+- [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
+- [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
+- [Auto-generated Docker containers to run and reproduce MLPerf inference benchmark](cm-mlops/script/app-mlperf-inference/dockerfiles/retinanet)
+
+
+### Documentation and the Getting Started Guide
+
+[Table of contents](https://github.com/mlcommons/ck/tree/master/docs/README.md)
+
+### Collaborative development
+
+This open-source technology is being developed by the open
+[MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
+led by [Grigori Fursin](https://cKnowledge.org/gfursin) and
+[Arjun Suresh](https://www.linkedin.com/in/arjunsuresh):
+
+* Join our [public Discord server](https://discord.gg/JjWNWXKxwT).
+* Join our [public conf-calls](https://docs.google.com/document/d/1zMNK1m_LhWm6jimZK6YE05hu4VH9usdbKJ3nBy-ZPAw).
+* Check our [news](docs/news.md).
+* Check our [presentation](https://doi.org/10.5281/zenodo.7871070) and [Forbes article](https://www.forbes.com/sites/karlfreund/2023/04/05/nvidia-performance-trounces-all-competitors-who-have-the-guts-to-submit-to-mlperf-inference-30/?sh=3c38d2866676) about our development plans.
+* Read about our [CK concept (previous version before MLCommons)](https://arxiv.org/abs/2011.01149).
+
+### Copyright
+
+2021-2023 [MLCommons](https://mlcommons.org)
+
+### License
+
+[Apache 2.0](LICENSE.md)
+
+### Acknowledgments
+
+This project is currently supported by [MLCommons](https://mlcommons.org), [cTuning foundation](https://cTuning.org),
+[cKnowledge](https://cKnowledge.org) and [individual contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md).
+We thank [HiPEAC](https://hipeac.net) and [OctoML](https://octoml.ai) for sponsoring initial development.
```

### Comparing `cmind-1.2.2/README.md` & `cmind-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: cmind
+Version: 1.3.0
+Summary: cmind
+Home-page: https://github.com/mlcommons/ck/tree/master/cm
+Author: Grigori Fursin
+Author-email: grigori@octoml.ai
+License: Apache 2.0
+Keywords: collective mind,cmind,cdatabase,cmeta,automation,reusability,meta,JSON,YAML,python
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE.CK.md
+License-File: LICENSE.md
+
 [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
 [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
 [![Downloads](https://pepy.tech/badge/cmind/month)](https://pepy.tech/project/cmind)
 [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
 
 [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
 [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
@@ -65,7 +79,9 @@
 [Apache 2.0](LICENSE.md)
 
 ### Acknowledgments
 
 This project is currently supported by [MLCommons](https://mlcommons.org), [cTuning foundation](https://cTuning.org),
 [cKnowledge](https://cKnowledge.org) and [individual contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md).
 We thank [HiPEAC](https://hipeac.net) and [OctoML](https://octoml.ai) for sponsoring initial development.
+
+
```

### Comparing `cmind-1.2.2/cmind/artifact.py` & `cmind-1.3.0/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/automation.py` & `cmind-1.3.0/cmind/automation.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,14 +392,15 @@
             parsed_artifact (list): prepared in CM CLI or CM access function
                                       [ (artifact alias, artifact UID) ] or
                                       [ (artifact alias, artifact UID), (artifact repo alias, artifact repo UID) ]
 
             meta (dict): meta description of this artifact
 
             (tags) (string or list): tags to be added to meta
+            (new_tags) (string or list): new tags to be added to meta (the same as tags)
             (yaml) (bool): if True, record YAML instead of JSON
 
         Returns: 
             (CM return dict):
 
             * return (int): return code == 0 if no error and >0 if error
             * (error) (str): error string if return>0
@@ -479,17 +480,28 @@
 
         if meta.get('alias','')=='': meta['alias']=artifact_obj[0]
         if meta.get('uid','')=='': meta['uid']=artifact_obj[1]
         if meta.get('automation_alias','')=='': meta['automation_alias']=automation_name[0]
         if meta.get('automation_uid','')=='': meta['automation_uid']=automation_name[1]
 
         existing_tags = meta.get('tags',[])
-        if len(tags)>0: 
-            existing_tags += tags
-        meta['tags'] = utils.filter_tags(existing_tags)
+
+        new_tags_list = []
+        if i.get('new_tags','')!='':
+            new_tags_list = i['new_tags'].split(',')
+
+        if len(tags)>0:
+            new_tags_list += tags    
+
+        if len(new_tags_list)>0: 
+            for xtag in new_tags_list:
+                if xtag!='' and xtag not in existing_tags:
+                    existing_tags.append(xtag)
+
+            meta['tags'] = existing_tags
 
         # Record meta
         if i.get('yaml', False):
             r = utils.save_yaml(meta_path_yaml, meta=meta)
         else:
             r = utils.save_json(meta_path_json, meta=meta)
         if r['return']>0: return r
@@ -966,14 +978,16 @@
                                       [ (artifact alias, artifact UID) ] or
                                       [ (artifact alias, artifact UID), (artifact repo alias, artifact repo UID) ]
 
             parsed_artifacts (list): prepared in CM CLI or CM access function - 1st entry has a new artifact name and repository:
                                       [ (artifact alias, artifact UID) ] or
                                       [ (artifact alias, artifact UID), (artifact repo alias, artifact repo UID) ]
 
+            new_tags (string): add new tags (separated by comma) to new artifacts
+        
         Returns: 
             (CM return dict):
 
             * return (int): return code == 0 if no error and >0 if error
             * (error) (str): error string if return>0
 
             * list (list): list of copied CM artifacts
@@ -1026,14 +1040,19 @@
             elif len(target_repo_list) >1:
                 return {'return':1, 'error':'more than 1 target repo found "{}"'.format(target_artifact_repo)}
 
             target_artifact_repo_obj = target_repo_list[0]
             target_repo_path = os.path.abspath(target_artifact_repo_obj.path_with_prefix)
 
         # Updating artifacts
+        new_tags_list = []
+        if i.get('new_tags','')!='':
+            new_tags_list = i['new_tags'].split(',')
+
+        
         for artifact in lst:
 
             artifact_path = os.path.abspath(artifact.path)
 
             artifact_meta = artifact.original_meta
 
             artifact_alias = artifact_meta.get('alias','')
@@ -1055,14 +1074,20 @@
             new_artifact_path = os.path.join(target_repo_path, artifact_automation, new_name) if target_repo_path is not None \
                 else os.path.join(artifact_automation_dir, new_name)
 
             if target_artifact_obj_alias != '' and artifact_alias.lower() != target_artifact_obj_alias.lower():
                 artifact_meta['alias']=target_artifact_obj_alias
 
             artifact_meta['uid']=target_artifact_obj_uid
+            if len(new_tags_list)>0:
+                xtags = artifact_meta.get('tags',[])
+                for xtag in new_tags_list:
+                    if xtag!='' and xtag not in xtags:
+                        xtags.append(xtag)
+                artifact_meta['tags'] = xtags
 
             artifact.path = new_artifact_path
 
             # Copy
             if artifact_path != new_artifact_path:
                 if console:
                     print ('* Copying "{}" to'.format(artifact_path))
```

### Comparing `cmind-1.2.2/cmind/cli.py` & `cmind-1.3.0/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/config.py` & `cmind-1.3.0/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/core.py` & `cmind-1.3.0/cmind/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
         # Logging
         self.logger = None
         self.log = []
 
         # Index
         self.index = None
 
-        self.use_index = False
-        if os.environ.get(self.cfg['env_index'],'').strip().lower() in ['yes','on','true']:
-            self.use_index = True
+        self.use_index = True
+        if os.environ.get(self.cfg['env_index'],'').strip().lower() in ['no','off','false']:
+            self.use_index = False
 
     ############################################################
     def error(self, r):
         """
         If r['return']>0: print CM error and raise error if in debugging mode
 
         Args:
@@ -297,14 +297,18 @@
         use_common_automation = True if i.get('common',False) else False
 
         automation_lst = []
         use_any_action = False
 
         artifact = i.get('artifact','').strip()
         artifacts = i.get('artifacts',[]) # Only if more than 1 artifact
+        
+        # Check artifact names
+        if artifact == '.' or '.' in artifacts:
+            return {'return':1, 'error':'forbidden artifact name "."'}
 
         # Check if automation is "." - then attempt to detect repo, automation and artifact from the current directory
         if automation == '.':
             r = self.access({'action':'detect',
                              'automation':'repo,55c3e27e8a140e48'})
             if r['return']>0: return r
 
@@ -420,21 +424,29 @@
                 elif len(automation_lst)>1:
                     return {'return':2, 'error':'ambiguity because several automations were found for {}'.format(auto_name)}
 
                 # Report an error if a repo is specified for a given automation action but it's not found there
                 if len(automation_lst)==0 and auto_repo is not None:
                     return {'return':3, 'error':'automation was not found in a specified repo {}'.format(auto_repo)}
 
+        # Convert action into function (substitute internal words)
+        original_action = action
+        action = action.replace('-','_')
+
+        if action in self.cfg['action_substitutions']:
+            action = self.cfg['action_substitutions'][action]
+
+        
         # Check if common automation and --help
         if (use_common_automation or automation=='') and cm_help:
             return print_action_help(self.common_automation, 
                                      self.common_automation, 
                                      'common',
                                      action,
-                                     action)
+                                     original_action)
 
         # If no automation was found we do not force common automation, check if should fail or continue
         if not use_common_automation and len(automation_lst)==0:
             if self.cfg['fail_if_automation_not_found']:
                 # Quit with error
                 if automation=='':
                     return {'return':4, 'error':'automation was not specified'}
@@ -455,21 +467,14 @@
                             'uid':'bbeb15d8f0a944a4'
                           }
 
         # Finalize automation class initialization
         initialized_automation = loaded_automation_class(self, automation_full_path)
         initialized_automation.meta = automation_meta
 
-        # Convert action into function (substitute internal words)
-        original_action = action
-        action = action.replace('-','_')
-
-        if action in self.cfg['action_substitutions']:
-            action = self.cfg['action_substitutions'][action]
-
         # Check action in a class when importing
         if use_any_action:
             action = 'any'
 
         print_automation = automation_meta.get('alias','') + ',' + automation_meta.get('uid','')
         initialized_automation.artfact = print_automation
```

### Comparing `cmind-1.2.2/cmind/index.py` & `cmind-1.3.0/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/net.py` & `cmind-1.3.0/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/automation/README.md` & `cmind-1.3.0/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/automation/module.py` & `cmind-1.3.0/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.3.0/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/automation/module_misc.py` & `cmind-1.3.0/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/ck/README.md` & `cmind-1.3.0/cmind/repo/automation/ck/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/ck/module.py` & `cmind-1.3.0/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/core/README.md` & `cmind-1.3.0/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/core/module.py` & `cmind-1.3.0/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/repo/README.md` & `cmind-1.3.0/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo/automation/repo/module.py` & `cmind-1.3.0/cmind/repo/automation/repo/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repo.py` & `cmind-1.3.0/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/repos.py` & `cmind-1.3.0/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind/utils.py` & `cmind-1.3.0/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-1.2.2/cmind.egg-info/PKG-INFO` & `cmind-1.3.0/cmind.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,87 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.2.2
+Version: 1.3.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: grigori@octoml.ai
 License: Apache 2.0
-Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
-        [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
-        [![Downloads](https://pepy.tech/badge/cmind/month)](https://pepy.tech/project/cmind)
-        [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
-        
-        [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
-        [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
-        
-        ### About
-        
-        [Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
-        is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
-        It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
-        when reproducing experiments from more than 150 research papers and validating them in the real world - 
-        there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
-        on any platform with any software, hardware, and data.
-        
-        CM is being developed by the [public MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md) 
-        as a simple, intuitive, technology-agnostic, and English-like scripting language that provides
-        a universal interface to any software project and transforms it into a [database of portable and reusable CM scripts]( https://github.com/mlcommons/ck/tree/master/cm-mlops/script )
-        in a transparent and non-intrusive way.
-        
-        CM is powered by Python, JSON and/or YAML meta descriptions, and a unified CLI.
-        Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
-        unified README files and synthesize unified containers with a common API.
-        It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
-        while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
-        
-        CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
-        to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
-        connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
-        and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
-        (cost, performance, power consumption, accuracy, etc).
-        
-        See a few real-world examples of using the CM scripting language:
-        - [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
-        - [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
-        - [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
-        - [Auto-generated Docker containers to run and reproduce MLPerf inference benchmark](cm-mlops/script/app-mlperf-inference/dockerfiles/retinanet)
-        
-        
-        ### Documentation and the Getting Started Guide
-        
-        [Table of contents](https://github.com/mlcommons/ck/tree/master/docs/README.md)
-        
-        ### Collaborative development
-        
-        This open-source technology is being developed by the open
-        [MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
-        led by [Grigori Fursin](https://cKnowledge.org/gfursin) and
-        [Arjun Suresh](https://www.linkedin.com/in/arjunsuresh):
-        
-        * Join our [public Discord server](https://discord.gg/JjWNWXKxwT).
-        * Join our [public conf-calls](https://docs.google.com/document/d/1zMNK1m_LhWm6jimZK6YE05hu4VH9usdbKJ3nBy-ZPAw).
-        * Check our [news](docs/news.md).
-        * Check our [presentation](https://doi.org/10.5281/zenodo.7871070) and [Forbes article](https://www.forbes.com/sites/karlfreund/2023/04/05/nvidia-performance-trounces-all-competitors-who-have-the-guts-to-submit-to-mlperf-inference-30/?sh=3c38d2866676) about our development plans.
-        * Read about our [CK concept (previous version before MLCommons)](https://arxiv.org/abs/2011.01149).
-        
-        ### Copyright
-        
-        2021-2023 [MLCommons](https://mlcommons.org)
-        
-        ### License
-        
-        [Apache 2.0](LICENSE.md)
-        
-        ### Acknowledgments
-        
-        This project is currently supported by [MLCommons](https://mlcommons.org), [cTuning foundation](https://cTuning.org),
-        [cKnowledge](https://cKnowledge.org) and [individual contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md).
-        We thank [HiPEAC](https://hipeac.net) and [OctoML](https://octoml.ai) for sponsoring initial development.
-        
 Keywords: collective mind,cmind,cdatabase,cmeta,automation,reusability,meta,JSON,YAML,python
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.CK.md
+License-File: LICENSE.md
+
+[![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
+[![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
+[![Downloads](https://pepy.tech/badge/cmind/month)](https://pepy.tech/project/cmind)
+[![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
+
+[![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
+[![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
+
+### About
+
+[Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
+is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
+It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
+when reproducing experiments from more than 150 research papers and validating them in the real world - 
+there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
+on any platform with any software, hardware, and data.
+
+CM is being developed by the [public MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md) 
+as a simple, intuitive, technology-agnostic, and English-like scripting language that provides
+a universal interface to any software project and transforms it into a [database of portable and reusable CM scripts]( https://github.com/mlcommons/ck/tree/master/cm-mlops/script )
+in a transparent and non-intrusive way.
+
+CM is powered by Python, JSON and/or YAML meta descriptions, and a unified CLI.
+Is helps to solve the "dependency hell" for ML and AI systems while automatically generating 
+unified README files and synthesize unified containers with a common API.
+It is also used to automate [reproducibility initiatives and artifact evaluation at AI, ML and Systems conferences](https://cTuning.org/ae)
+while reducing all the tedious, manual, repetitive, and ad-hoc efforts to reproduce research projects and validate them in production.
+
+CM powers the [Collective Knowledge platform (MLCommons CK playground)](https://access.cKnowledge.org)
+to aggregate [reproducible experiments](https://access.cknowledge.org/playground/?action=experiments),
+connect academia and industry to [organize reproducibility, replicability and optimization challenges]( https://github.com/mlcommons/ck/tree/master/cm-mlops/challenge ),
+and help developers and users select Pareto-optimal end-to-end applications and systems based on their requirements and constraints
+(cost, performance, power consumption, accuracy, etc).
+
+See a few real-world examples of using the CM scripting language:
+- [README to reproduce published IPOL'22 paper](cm-mlops/script/app-ipol-reproducibility-2022-439)
+- [README to reproduce MLPerf RetinaNet inference benchmark at Student Cluster Competition'22](docs/tutorials/sc22-scc-mlperf.md)
+- [Auto-generated READMEs to reproduce official MLPerf BERT inference benchmark v3.0 submission with a model from the Hugging Face Zoo](https://github.com/mlcommons/submissions_inference_3.0/tree/main/open/cTuning/code/huggingface-bert/README.md)
+- [Auto-generated Docker containers to run and reproduce MLPerf inference benchmark](cm-mlops/script/app-mlperf-inference/dockerfiles/retinanet)
+
+
+### Documentation and the Getting Started Guide
+
+[Table of contents](https://github.com/mlcommons/ck/tree/master/docs/README.md)
+
+### Collaborative development
+
+This open-source technology is being developed by the open
+[MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
+led by [Grigori Fursin](https://cKnowledge.org/gfursin) and
+[Arjun Suresh](https://www.linkedin.com/in/arjunsuresh):
+
+* Join our [public Discord server](https://discord.gg/JjWNWXKxwT).
+* Join our [public conf-calls](https://docs.google.com/document/d/1zMNK1m_LhWm6jimZK6YE05hu4VH9usdbKJ3nBy-ZPAw).
+* Check our [news](docs/news.md).
+* Check our [presentation](https://doi.org/10.5281/zenodo.7871070) and [Forbes article](https://www.forbes.com/sites/karlfreund/2023/04/05/nvidia-performance-trounces-all-competitors-who-have-the-guts-to-submit-to-mlperf-inference-30/?sh=3c38d2866676) about our development plans.
+* Read about our [CK concept (previous version before MLCommons)](https://arxiv.org/abs/2011.01149).
+
+### Copyright
+
+2021-2023 [MLCommons](https://mlcommons.org)
+
+### License
+
+[Apache 2.0](LICENSE.md)
+
+### Acknowledgments
+
+This project is currently supported by [MLCommons](https://mlcommons.org), [cTuning foundation](https://cTuning.org),
+[cKnowledge](https://cKnowledge.org) and [individual contributors](https://github.com/mlcommons/ck/blob/master/CONTRIBUTING.md).
+We thank [HiPEAC](https://hipeac.net) and [OctoML](https://octoml.ai) for sponsoring initial development.
+
+
```

### Comparing `cmind-1.2.2/cmind.egg-info/SOURCES.txt` & `cmind-1.3.0/cmind.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE.CK.md
+LICENSE.md
 README.md
 setup.py
 cmind/__init__.py
 cmind/__main__.py
 cmind/artifact.py
 cmind/automation.py
 cmind/cli.py
```

### Comparing `cmind-1.2.2/setup.py` & `cmind-1.3.0/setup.py`

 * *Files identical despite different names*

