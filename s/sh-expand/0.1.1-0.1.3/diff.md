# Comparing `tmp/sh_expand-0.1.1-py3-none-any.whl.zip` & `tmp/sh_expand-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 7246 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-May-31 15:28 sh_expand/__init__.py
--rw-r--r--  2.0 unx    17340 b- defN 23-May-31 15:28 sh_expand/expand.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-31 15:28 sh_expand-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2034 b- defN 23-May-31 15:28 sh_expand-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 15:28 sh_expand-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-31 15:28 sh_expand-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      548 b- defN 23-May-31 15:28 sh_expand-0.1.1.dist-info/RECORD
-7 files, 21097 bytes uncompressed, 6274 bytes compressed:  70.3%
+Zip file size: 10534 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 19:27 sh_expand/__init__.py
+-rw-r--r--  2.0 unx     8459 b- defN 23-May-31 19:27 sh_expand/env_vars_util.py
+-rw-r--r--  2.0 unx    17321 b- defN 23-May-31 19:27 sh_expand/expand.py
+-rw-r--r--  2.0 unx      366 b- defN 23-May-31 19:27 sh_expand/util.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-31 19:28 sh_expand-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2034 b- defN 23-May-31 19:28 sh_expand-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 19:28 sh_expand-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-31 19:28 sh_expand-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      704 b- defN 23-May-31 19:28 sh_expand-0.1.3.dist-info/RECORD
+9 files, 30059 bytes uncompressed, 9324 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: sh_expand/__init__.py
 Comment: 
 
+Filename: sh_expand/env_vars_util.py
+Comment: 
+
 Filename: sh_expand/expand.py
 Comment: 
 
-Filename: sh_expand-0.1.1.dist-info/LICENSE
+Filename: sh_expand/util.py
+Comment: 
+
+Filename: sh_expand-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: sh_expand-0.1.1.dist-info/METADATA
+Filename: sh_expand-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: sh_expand-0.1.1.dist-info/WHEEL
+Filename: sh_expand-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: sh_expand-0.1.1.dist-info/top_level.txt
+Filename: sh_expand-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sh_expand-0.1.1.dist-info/RECORD
+Filename: sh_expand-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sh_expand/expand.py

```diff
@@ -1,19 +1,17 @@
 import copy
-import logging
 
 from shasta.ast_node import *
 
+from sh_expand.util import log
+
 ################################################################################
 # SAFE EXPANSION ANALYSIS
 ################################################################################
 
-def log(msg: str):
-    logging.info(f'Expansion: {msg}')
-
 ## This contains all necessary state of the expansion
 class ExpansionState:
     variables: dict
     def __init__(self, variables: dict):
         self.variables = variables
 
     def __repr__(self):
@@ -241,15 +239,15 @@
     _type, value = exp_state.variables.get(varname, [None, None])
     return value
 
 ## This function checks if the -u flag is set
 def is_u_set(exp_state: ExpansionState):
     value = lookup_variable_inner_unsafe('-', exp_state)
     # log(f'Previous set status is: {value}')
-    return "u" in value
+    return value is not None and "u" in value
 
 
 def invalidate_variable(var, reason, exp_state):
     exp_state.variables[var] = [None, InvalidVariable(var, reason)]
     return exp_state
```

## Comparing `sh_expand-0.1.1.dist-info/LICENSE` & `sh_expand-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sh_expand-0.1.1.dist-info/METADATA` & `sh_expand-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh-expand
-Version: 0.1.1
+Version: 0.1.3
 Summary: A library for expanding shell ASTs
 Author-email: Michael Greenberg <michael@greenberg.science>, Konstantinos Kallas <konstantinos.kallas@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 The PaSh Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

