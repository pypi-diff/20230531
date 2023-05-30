# Comparing `tmp/mkdocs-walt-0.0.3.dev0.tar.gz` & `tmp/mkdocs-walt-0.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-walt-0.0.3.dev0.tar", last modified: Tue May 30 20:55:44 2023, max compression
+gzip compressed data, was "mkdocs-walt-0.0.4.dev0.tar", last modified: Tue May 30 22:08:10 2023, max compression
```

## Comparing `mkdocs-walt-0.0.3.dev0.tar` & `mkdocs-walt-0.0.4.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 20:55:44.172957 mkdocs-walt-0.0.3.dev0/
--rw-r--r--   0 sue        (501) staff       (20)      145 2023-05-30 20:37:51.000000 mkdocs-walt-0.0.3.dev0/MANIFEST.in
--rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-30 20:55:44.172839 mkdocs-walt-0.0.3.dev0/PKG-INFO
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 20:55:44.172003 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/
--rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-30 20:55:44.000000 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      366 2023-05-30 20:55:44.000000 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/SOURCES.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-30 20:55:44.000000 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/dependency_links.txt
--rw-r--r--   0 sue        (501) staff       (20)       28 2023-05-30 20:55:44.000000 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/entry_points.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/not-zip-safe
--rw-r--r--   0 sue        (501) staff       (20)        7 2023-05-30 20:55:44.000000 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/requires.txt
--rw-r--r--   0 sue        (501) staff       (20)        5 2023-05-30 20:55:44.000000 mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/top_level.txt
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-30 20:55:44.172991 mkdocs-walt-0.0.3.dev0/setup.cfg
--rw-r--r--   0 sue        (501) staff       (20)     1241 2023-05-30 20:55:19.000000 mkdocs-walt-0.0.3.dev0/setup.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 20:55:44.172690 mkdocs-walt-0.0.3.dev0/walt/
--rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.0.3.dev0/walt/__init__.py
--rw-r--r--   0 sue        (501) staff       (20)     2035 2023-05-30 17:08:24.000000 mkdocs-walt-0.0.3.dev0/walt/base.html
--rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.0.3.dev0/walt/main.html
--rw-r--r--   0 sue        (501) staff       (20)      153 2023-05-30 15:30:45.000000 mkdocs-walt-0.0.3.dev0/walt/mkdocs_theme.yml
--rw-r--r--   0 sue        (501) staff       (20)     5628 2023-05-30 19:55:41.000000 mkdocs-walt-0.0.3.dev0/walt/styles.css
--rw-r--r--   0 sue        (501) staff       (20)      423 2023-05-30 20:14:49.000000 mkdocs-walt-0.0.3.dev0/walt/writ.html
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 22:08:10.901172 mkdocs-walt-0.0.4.dev0/
+-rw-r--r--   0 sue        (501) staff       (20)      145 2023-05-30 20:37:51.000000 mkdocs-walt-0.0.4.dev0/MANIFEST.in
+-rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-30 22:08:10.901067 mkdocs-walt-0.0.4.dev0/PKG-INFO
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 22:08:10.900210 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/
+-rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      366 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/SOURCES.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/dependency_links.txt
+-rw-r--r--   0 sue        (501) staff       (20)       28 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/entry_points.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/not-zip-safe
+-rw-r--r--   0 sue        (501) staff       (20)        7 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/requires.txt
+-rw-r--r--   0 sue        (501) staff       (20)        5 2023-05-30 22:08:10.000000 mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/top_level.txt
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-30 22:08:10.901202 mkdocs-walt-0.0.4.dev0/setup.cfg
+-rw-r--r--   0 sue        (501) staff       (20)     1241 2023-05-30 21:01:40.000000 mkdocs-walt-0.0.4.dev0/setup.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-30 22:08:10.900905 mkdocs-walt-0.0.4.dev0/walt/
+-rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.0.4.dev0/walt/__init__.py
+-rw-r--r--   0 sue        (501) staff       (20)     2035 2023-05-30 17:08:24.000000 mkdocs-walt-0.0.4.dev0/walt/base.html
+-rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.0.4.dev0/walt/main.html
+-rw-r--r--   0 sue        (501) staff       (20)      150 2023-05-30 22:04:56.000000 mkdocs-walt-0.0.4.dev0/walt/mkdocs_theme.yml
+-rw-r--r--   0 sue        (501) staff       (20)     5628 2023-05-30 22:02:26.000000 mkdocs-walt-0.0.4.dev0/walt/styles.css
+-rw-r--r--   0 sue        (501) staff       (20)      423 2023-05-30 20:14:49.000000 mkdocs-walt-0.0.4.dev0/walt/writ.html
```

### Comparing `mkdocs-walt-0.0.3.dev0/PKG-INFO` & `mkdocs-walt-0.0.4.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-walt
-Version: 0.0.3.dev0
+Version: 0.0.4.dev0
 Summary: A minimal theme for MkDocs
 Home-page: https://github.com/codesue/walt
 Author: Suzen Fylke
 Author-email: codesue@users.noreply.github.com
 License: GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `mkdocs-walt-0.0.3.dev0/mkdocs_walt.egg-info/PKG-INFO` & `mkdocs-walt-0.0.4.dev0/mkdocs_walt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-walt
-Version: 0.0.3.dev0
+Version: 0.0.4.dev0
 Summary: A minimal theme for MkDocs
 Home-page: https://github.com/codesue/walt
 Author: Suzen Fylke
 Author-email: codesue@users.noreply.github.com
 License: GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `mkdocs-walt-0.0.3.dev0/setup.py` & `mkdocs-walt-0.0.4.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3-dev'
+VERSION = '0.0.4-dev'
 
 LONG_DESCRIPTION = '''
 # mkdocs-walt: a minimal documentation theme for MkDocs
 
 Walt is a minimal documentation theme that is best suited for single page websites.
 
 ## Installation
```

### Comparing `mkdocs-walt-0.0.3.dev0/walt/base.html` & `mkdocs-walt-0.0.4.dev0/walt/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-walt-0.0.3.dev0/walt/styles.css` & `mkdocs-walt-0.0.4.dev0/walt/styles.css`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
   -moz-osx-font-smoothing: grayscale;
 }
 
 /* Layout */
 
 html, body {
   height: 100%;
-  color: var(--text-color);
-  background-color: var(--background-color);
+  color: var(--color-text);
+  background-color: var(--color-background);
   font-family: var(--font-family);
   font-size: var(--font-size);
   line-height: var(--line-height);
 }
 
 html {
   overflow-y: auto;
```

