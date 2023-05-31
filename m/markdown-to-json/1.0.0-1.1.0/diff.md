# Comparing `tmp/markdown-to-json-1.0.0.tar.gz` & `tmp/markdown-to-json-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-to-json-1.0.0.tar", last modified: Thu Dec 10 21:01:11 2015, max compression, from Unix
+gzip compressed data, was "markdown-to-json-1.1.0.tar", last modified: Wed May 31 19:21:27 2023, max compression
```

## Comparing `markdown-to-json-1.0.0.tar` & `markdown-to-json-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json/
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json.egg-info/
--rw-r--r--   0 njvack     (503) staff       (20)      233 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/PKG-INFO
--rw-r--r--   0 njvack     (503) staff       (20)       59 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/setup.cfg
--rwxr-xr-x   0 njvack     (503) staff       (20)     1006 2015-12-10 20:27:50.000000 markdown-to-json-1.0.0/setup.py
--rw-r--r--   0 njvack     (503) staff       (20)        1 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json.egg-info/dependency_links.txt
--rw-r--r--   0 njvack     (503) staff       (20)       73 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json.egg-info/entry_points.txt
--rw-r--r--   0 njvack     (503) staff       (20)      233 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json.egg-info/PKG-INFO
--rw-r--r--   0 njvack     (503) staff       (20)      748 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json.egg-info/SOURCES.txt
--rw-r--r--   0 njvack     (503) staff       (20)       17 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json.egg-info/top_level.txt
--rw-r--r--   0 njvack     (503) staff       (20)      108 2015-12-08 17:16:56.000000 markdown-to-json-1.0.0/markdown_to_json/__init__.py
--rw-r--r--   0 njvack     (503) staff       (20)      249 2015-12-10 20:55:55.000000 markdown-to-json-1.0.0/markdown_to_json/_metadata.py
--rw-r--r--   0 njvack     (503) staff       (20)     4510 2015-12-09 21:43:47.000000 markdown-to-json-1.0.0/markdown_to_json/markdown_to_json.py
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json/scripts/
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/
--rw-r--r--   0 njvack     (503) staff       (20)        0 2015-12-04 21:17:03.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/__init__.py
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/CommonMark/
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/docopt/
-drwxr-xr-x   0 njvack     (503) staff       (20)        0 2015-12-10 21:01:11.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/ordereddict/
--rw-r--r--   0 njvack     (503) staff       (20)      134 2015-12-10 20:34:19.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/ordereddict/__init__.py
--rw-------   0 njvack     (503) staff       (20)      226 2015-12-04 21:47:04.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/ordereddict/._ordereddict.py
--rw-------   0 njvack     (503) staff       (20)     4221 2015-12-04 21:47:04.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/ordereddict/ordereddict.py
--rw-r--r--   0 njvack     (503) staff       (20)       62 2015-12-10 20:29:03.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/docopt/__init__.py
--rw-r--r--   0 njvack     (503) staff       (20)    19784 2015-12-04 21:46:48.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/docopt/docopt.py
--rw-r--r--   0 njvack     (503) staff       (20)      240 2015-12-04 21:17:03.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/CommonMark/__init__.py
--rwxr-xr-x   0 njvack     (503) staff       (20)    55784 2015-12-04 21:17:03.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/CommonMark/CommonMark.py
--rwxr-xr-x   0 njvack     (503) staff       (20)    63763 2015-12-10 20:38:30.000000 markdown-to-json-1.0.0/markdown_to_json/vendor/CommonMark/entitytrans.py
--rw-r--r--   0 njvack     (503) staff       (20)        0 2015-12-07 17:37:21.000000 markdown-to-json-1.0.0/markdown_to_json/scripts/__init__.py
--rwxr-xr-x   0 njvack     (503) staff       (20)     2351 2015-12-10 20:36:08.000000 markdown-to-json-1.0.0/markdown_to_json/scripts/md_to_json.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.898553 markdown-to-json-1.1.0/
+-rw-r--r--   0 njvack     (501) staff       (20)     1118 2023-05-31 19:20:38.000000 markdown-to-json-1.1.0/LICENSE
+-rw-r--r--   0 njvack     (501) staff       (20)      199 2023-05-31 19:21:27.898439 markdown-to-json-1.1.0/PKG-INFO
+-rw-r--r--   0 njvack     (501) staff       (20)     2966 2015-12-10 21:14:04.000000 markdown-to-json-1.1.0/README.md
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.895036 markdown-to-json-1.1.0/markdown_to_json/
+-rw-r--r--   0 njvack     (501) staff       (20)      108 2015-12-08 17:16:56.000000 markdown-to-json-1.1.0/markdown_to_json/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)      410 2023-05-31 19:20:57.000000 markdown-to-json-1.1.0/markdown_to_json/_metadata.py
+-rw-r--r--   0 njvack     (501) staff       (20)     4488 2023-05-31 19:20:48.000000 markdown-to-json-1.1.0/markdown_to_json/markdown_to_json.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.895746 markdown-to-json-1.1.0/markdown_to_json/scripts/
+-rw-r--r--   0 njvack     (501) staff       (20)        0 2015-12-07 17:37:21.000000 markdown-to-json-1.1.0/markdown_to_json/scripts/__init__.py
+-rwxr-xr-x   0 njvack     (501) staff       (20)     2536 2023-05-31 19:20:52.000000 markdown-to-json-1.1.0/markdown_to_json/scripts/md_to_json.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.895845 markdown-to-json-1.1.0/markdown_to_json/vendor/
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.896876 markdown-to-json-1.1.0/markdown_to_json/vendor/CommonMark/
+-rwxr-xr-x   0 njvack     (501) staff       (20)    55764 2023-05-31 19:19:24.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/CommonMark/CommonMark.py
+-rw-r--r--   0 njvack     (501) staff       (20)      240 2015-12-04 21:17:03.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/CommonMark/__init__.py
+-rwxr-xr-x   0 njvack     (501) staff       (20)    63763 2015-12-10 20:38:30.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/CommonMark/entitytrans.py
+-rw-r--r--   0 njvack     (501) staff       (20)        0 2015-12-04 21:17:03.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/__init__.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.897585 markdown-to-json-1.1.0/markdown_to_json/vendor/docopt/
+-rw-r--r--   0 njvack     (501) staff       (20)       62 2015-12-10 20:29:03.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/docopt/__init__.py
+-rw-r--r--   0 njvack     (501) staff       (20)    19784 2015-12-04 21:46:48.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/docopt/docopt.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.898080 markdown-to-json-1.1.0/markdown_to_json/vendor/ordereddict/
+-rw-r--r--   0 njvack     (501) staff       (20)      134 2015-12-10 20:34:19.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/ordereddict/__init__.py
+-rw-------   0 njvack     (501) staff       (20)     4221 2015-12-04 21:47:04.000000 markdown-to-json-1.1.0/markdown_to_json/vendor/ordereddict/ordereddict.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.895555 markdown-to-json-1.1.0/markdown_to_json.egg-info/
+-rw-r--r--   0 njvack     (501) staff       (20)      199 2023-05-31 19:21:27.000000 markdown-to-json-1.1.0/markdown_to_json.egg-info/PKG-INFO
+-rw-r--r--   0 njvack     (501) staff       (20)      786 2023-05-31 19:21:27.000000 markdown-to-json-1.1.0/markdown_to_json.egg-info/SOURCES.txt
+-rw-r--r--   0 njvack     (501) staff       (20)        1 2023-05-31 19:21:27.000000 markdown-to-json-1.1.0/markdown_to_json.egg-info/dependency_links.txt
+-rw-r--r--   0 njvack     (501) staff       (20)       72 2023-05-31 19:21:27.000000 markdown-to-json-1.1.0/markdown_to_json.egg-info/entry_points.txt
+-rw-r--r--   0 njvack     (501) staff       (20)       17 2023-05-31 19:21:27.000000 markdown-to-json-1.1.0/markdown_to_json.egg-info/top_level.txt
+-rw-r--r--   0 njvack     (501) staff       (20)       38 2023-05-31 19:21:27.898620 markdown-to-json-1.1.0/setup.cfg
+-rwxr-xr-x   0 njvack     (501) staff       (20)     1006 2015-12-10 20:27:50.000000 markdown-to-json-1.1.0/setup.py
+drwxr-xr-x   0 njvack     (501) staff       (20)        0 2023-05-31 19:21:27.898285 markdown-to-json-1.1.0/tests/
+-rw-r--r--   0 njvack     (501) staff       (20)      727 2023-05-31 19:20:42.000000 markdown-to-json-1.1.0/tests/test_lists.py
```

### Comparing `markdown-to-json-1.0.0/setup.py` & `markdown-to-json-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `markdown-to-json-1.0.0/markdown_to_json.egg-info/SOURCES.txt` & `markdown-to-json-1.1.0/markdown_to_json.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+README.md
 setup.py
 markdown_to_json/__init__.py
 markdown_to_json/_metadata.py
 markdown_to_json/markdown_to_json.py
 markdown_to_json.egg-info/PKG-INFO
 markdown_to_json.egg-info/SOURCES.txt
 markdown_to_json.egg-info/dependency_links.txt
@@ -12,8 +14,9 @@
 markdown_to_json/vendor/__init__.py
 markdown_to_json/vendor/CommonMark/CommonMark.py
 markdown_to_json/vendor/CommonMark/__init__.py
 markdown_to_json/vendor/CommonMark/entitytrans.py
 markdown_to_json/vendor/docopt/__init__.py
 markdown_to_json/vendor/docopt/docopt.py
 markdown_to_json/vendor/ordereddict/__init__.py
-markdown_to_json/vendor/ordereddict/ordereddict.py
+markdown_to_json/vendor/ordereddict/ordereddict.py
+tests/test_lists.py
```

### Comparing `markdown-to-json-1.0.0/markdown_to_json/markdown_to_json.py` & `markdown-to-json-1.1.0/markdown_to_json/markdown_to_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Part of the markdown_to_json package
 # Written by Nate Vack <njvack@freshforever.net>
-# Copyright 2015 Board of Regents of the University of Wisconsin System
+# Copyright 2023 Board of Regents of the University of Wisconsin System
 
 from __future__ import unicode_literals, absolute_import
 
 from functools import reduce
 import operator
 
 from .vendor.ordereddict import OrderedDict
```

### Comparing `markdown-to-json-1.0.0/markdown_to_json/vendor/ordereddict/ordereddict.py` & `markdown-to-json-1.1.0/markdown_to_json/vendor/ordereddict/ordereddict.py`

 * *Files identical despite different names*

### Comparing `markdown-to-json-1.0.0/markdown_to_json/vendor/docopt/docopt.py` & `markdown-to-json-1.1.0/markdown_to_json/vendor/docopt/docopt.py`

 * *Files identical despite different names*

### Comparing `markdown-to-json-1.0.0/markdown_to_json/vendor/CommonMark/CommonMark.py` & `markdown-to-json-1.1.0/markdown_to_json/vendor/CommonMark/CommonMark.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from warnings import warn
 
 # if python3 use html.parser and urllib.parse, else use HTMLParser and urllib
 if sys.version_info >= (3, 0):
     import urllib.parse
     if sys.version_info >= (3, 4):
         import html.parser
-        HTMLunescape = html.parser.HTMLParser().unescape
+        HTMLunescape = html.unescape
     else:
         from .entitytrans import _unescape
         HTMLunescape = _unescape
     HTMLquote = urllib.parse.quote
     HTMLunquote = urllib.parse.unquote
     URLparse = urllib.parse.urlparse
 else:
```

### Comparing `markdown-to-json-1.0.0/markdown_to_json/vendor/CommonMark/entitytrans.py` & `markdown-to-json-1.1.0/markdown_to_json/vendor/CommonMark/entitytrans.py`

 * *Files identical despite different names*

### Comparing `markdown-to-json-1.0.0/markdown_to_json/scripts/md_to_json.py` & `markdown-to-json-1.1.0/markdown_to_json/scripts/md_to_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Part of the markdown_to_json package
+# Written by Nate Vack <njvack@freshforever.net>
+# Copyright 2023 Board of Regents of the University of Wisconsin System
+
 """Translate markdown into JSON.
 
 Usage:
   md_to_json [options] <markdown_file>
   md_to_json -h | --help
 
 Options:
```

