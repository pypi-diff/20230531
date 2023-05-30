# Comparing `tmp/cellmaps_generate_hierarchy-0.1.0a4.tar.gz` & `tmp/cellmaps_generate_hierarchy-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a4.tar", last modified: Tue May 30 21:18:55 2023, max compression
+gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a5.tar", last modified: Tue May 30 23:33:02 2023, max compression
```

## Comparing `cellmaps_generate_hierarchy-0.1.0a4.tar` & `cellmaps_generate_hierarchy-0.1.0a5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.078205 cellmaps_generate_hierarchy-0.1.0a4/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a4/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 21:18:55.078354 cellmaps_generate_hierarchy-0.1.0a4/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4203 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.069113 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/
--rw-r--r--   0 churas     (504) staff       (20)      325 2023-05-30 21:18:21.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     5400 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    17254 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/hierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     3764 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/ppi.py
--rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.070350 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1429 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       56 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.075042 cellmaps_generate_hierarchy-0.1.0a4/docs/
--rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.064921 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.064990 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.075788 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/cellmaps_generate_hierarchy.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      410 2023-05-30 21:18:55.078837 cellmaps_generate_hierarchy-0.1.0a4/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2310 2023-05-25 23:23:13.000000 cellmaps_generate_hierarchy-0.1.0a4/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.077257 cellmaps_generate_hierarchy-0.1.0a4/tests/
--rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.078023 cellmaps_generate_hierarchy-0.1.0a4/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/data/fake_4_node_coembedding.tsv
--rw-r--r--   0 churas     (504) staff       (20)       30 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/data/hidef_output.edges
--rw-r--r--   0 churas     (504) staff       (20)       62 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/data/hidef_output.nodes
--rw-r--r--   0 churas     (504) staff       (20)     9132 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cdapshierarchygenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmapsgeneratehierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cosinesimilarityppigenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_integration_cellmaps_generate_hierarchy.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.292047 cellmaps_generate_hierarchy-0.1.0a5/
+-rw-r--r--   0 churas     (504) staff       (20)      160 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a5/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 23:33:02.292175 cellmaps_generate_hierarchy-0.1.0a5/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4203 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a5/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.282418 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/
+-rw-r--r--   0 churas     (504) staff       (20)      325 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     5391 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    17184 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/hierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     3764 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/ppi.py
+-rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.284170 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1429 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       56 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-30 23:33:02.000000 cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.288662 cellmaps_generate_hierarchy-0.1.0a5/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.277776 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.277860 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.289471 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/cellmaps_generate_hierarchy.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      410 2023-05-30 23:33:02.292610 cellmaps_generate_hierarchy-0.1.0a5/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2310 2023-05-25 23:23:13.000000 cellmaps_generate_hierarchy-0.1.0a5/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.290914 cellmaps_generate_hierarchy-0.1.0a5/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 23:33:02.291865 cellmaps_generate_hierarchy-0.1.0a5/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/data/fake_4_node_coembedding.tsv
+-rw-r--r--   0 churas     (504) staff       (20)       30 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/data/hidef_output.edges
+-rw-r--r--   0 churas     (504) staff       (20)       62 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/data/hidef_output.nodes
+-rw-r--r--   0 churas     (504) staff       (20)    10675 2023-05-30 23:32:46.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cdapshierarchygenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmapsgeneratehierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_cosinesimilarityppigenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a5/tests/test_integration_cellmaps_generate_hierarchy.py
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/CONTRIBUTING.rst` & `cellmaps_generate_hierarchy-0.1.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/LICENSE` & `cellmaps_generate_hierarchy-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_generate_hierarchy
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Clara Hu
 Author-email: mhu@ucsd.edu
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/README.rst` & `cellmaps_generate_hierarchy-0.1.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     theargs.version = cellmaps_generate_hierarchy.__version__
 
     try:
         logutils.setup_cmd_logging(theargs)
         provenance = ProvenanceUtil()
         ppigen = CosineSimilarityPPIGenerator(embeddingdir=theargs.coembedding_dir)
 
-        hiergen = CDAPSHiDeFHierarchyGenerator(author=cellmaps_generate_hierarchy.__author__,
+        hiergen = CDAPSHiDeFHierarchyGenerator(author='cellmaps_generate_hierarchy',
                                                version=cellmaps_generate_hierarchy.__version__,
                                                provenance_utils=provenance)
         return CellmapsGenerateHierarchy(outdir=theargs.outdir,
                                          inputdir=theargs.coembedding_dir,
                                          ppigen=ppigen,
                                          hiergen=hiergen,
                                          input_data_dict=theargs.__dict__,
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/hierarchy.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import csv
 import logging
 import subprocess
 from datetime import date
 import ndex2
 import cdapsutil
+import cellmaps_generate_hierarchy
 from cellmaps_utils import constants
 from cellmaps_utils.provenance import ProvenanceUtil
 from cellmaps_generate_hierarchy.exceptions import CellmapsGenerateHierarchyError
 
 logger = logging.getLogger(__name__)
 
 
@@ -17,16 +18,16 @@
     """
     Base class for generating hierarchy
     that is output in CX format following
     CDAPS style
     """
     def __init__(self,
                  provenance_utils=ProvenanceUtil(),
-                 author=None,
-                 version=None):
+                 author='cellmaps_generate_hierarchy',
+                 version=cellmaps_generate_hierarchy.__version__):
         """
         Constructor
         """
         self._provenance_utils = provenance_utils
         self._author = author
         self._version = version
         self._generated_dataset_ids = []
@@ -66,17 +67,17 @@
     NODE_CX_KEY_NAME = 'nodeAttributesAsCX2'
 
     ATTR_DEC_NAME = 'attributeDeclarations'
 
     PERSISTENCE_COL_NAME = 'HiDeF_persistence'
 
     def __init__(self, hidef_cmd='hidef_finder.py',
-                 provenance_utils=None,
-                 author=None,
-                 version=None):
+                 provenance_utils=ProvenanceUtil(),
+                 author='cellmaps_generate_hierarchy',
+                 version=cellmaps_generate_hierarchy.__version__):
         """
         Constructor
         """
         super().__init__(provenance_utils=provenance_utils,
                          author=author,
                          version=version)
         self._hidef_cmd = hidef_cmd
@@ -329,16 +330,16 @@
                 largest_network = net
 
                 # register edgelist file with fairscape
                 data_dict = {'name': os.path.basename(dest_path) +
                              ' PPI id edgelist file',
                              'description': 'PPI id edgelist file',
                              'data-format': 'tsv',
-                             'author': self._author,
-                             'version': self._version,
+                             'author': str(self._author),
+                             'version': str(self._version),
                              'date-published': date.today().strftime('%m-%d-%Y')}
                 dataset_id = self._provenance_utils.register_dataset(os.path.dirname(dest_path),
                                                                      source_file=dest_path,
                                                                      data_dict=data_dict)
                 self._generated_dataset_ids.append(dataset_id)
 
         logger.debug('Largest network name: ' + largest_network.get_name())
@@ -346,32 +347,30 @@
 
     def _register_hidef_output_files(self, outdir):
         """
         Register <HIDEF_PREFIX>.nodes and <HIDEF_PREFIX>.edges
         and <HIDEF_PREFIX>.weaver files with FAIRSCAPE
 
         """
-        nodesfile = os.path.join(outdir,
-                                 CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX + '.nodes')
-        edgesfile = os.path.join(outdir,
-                                 CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX + '.edges')
-        weaverfile = os.path.join(outdir,
-                                 CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX + '.weaver')
-        for hidef_file in [('nodes', 'tsv', nodesfile),
-                           ('edges', 'tsv', edgesfile),
-                           ('weaver', 'npy', weaverfile)]:
-            data_dict = {'name': os.path.basename(hidef_file[2]) +
+
+        for hidef_file in [('nodes', 'tsv'),
+                           ('edges', 'tsv'),
+                           ('weaver', 'npy')]:
+            outfile = os.path.join(outdir,
+                                   CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX +
+                                   '.' + hidef_file[0])
+            data_dict = {'name': os.path.basename(outfile) +
                          ' HiDeF output ' + hidef_file[0] + ' file',
                          'description': ' HiDeF output ' + hidef_file[0] + ' file',
                          'data-format': hidef_file[1],
-                         'author': self._author,
-                         'version': self._version,
+                         'author': str(self._author),
+                         'version': str(self._version),
                          'date-published': date.today().strftime('%m-%d-%Y')}
-            dataset_id = self._provenance_utils.register_dataset(os.path.dirname(hidef_file[2]),
-                                                                 source_file=hidef_file[2],
+            dataset_id = self._provenance_utils.register_dataset(os.path.dirname(outfile),
+                                                                 source_file=outfile,
                                                                  data_dict=data_dict)
             self._generated_dataset_ids.append(dataset_id)
 
     def get_hierarchy(self, networks):
         """
         Runs HiDeF to generate hierarchy and registers resulting output
         files with FAIRSCAPE. To do this the method generates edgelist
@@ -420,16 +419,16 @@
                 self.convert_hidef_output_to_cdaps(out_stream, outdir)
 
             # register cdaps json file with fairscape
             data_dict = {'name': os.path.basename(cdaps_out_file) +
                          ' CDAPS output JSON file',
                          'description': 'CDAPS output JSON file',
                          'data-format': 'json',
-                         'author': self._author,
-                         'version': self._version,
+                         'author': str(self._author),
+                         'version': str(self._version),
                          'date-published': date.today().strftime('%m-%d-%Y')}
             dataset_id = self._provenance_utils.register_dataset(os.path.dirname(cdaps_out_file),
                                                                  source_file=cdaps_out_file,
                                                                  data_dict=data_dict)
             self._generated_dataset_ids.append(dataset_id)
 
             cd = cdapsutil.CommunityDetection(runner=cdapsutil.ExternalResultsRunner())
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/ppi.py` & `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/ppi.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/runner.py` & `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-generate-hierarchy
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Clara Hu
 Author-email: mhu@ucsd.edu
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/SOURCES.txt` & `cellmaps_generate_hierarchy-0.1.0a5/cellmaps_generate_hierarchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/Makefile` & `cellmaps_generate_hierarchy-0.1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/cellmaps_generate_hierarchy.rst` & `cellmaps_generate_hierarchy-0.1.0a5/docs/cellmaps_generate_hierarchy.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/conf.py` & `cellmaps_generate_hierarchy-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/index.rst` & `cellmaps_generate_hierarchy-0.1.0a5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/installation.rst` & `cellmaps_generate_hierarchy-0.1.0a5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/make.bat` & `cellmaps_generate_hierarchy-0.1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/newrelease.rst` & `cellmaps_generate_hierarchy-0.1.0a5/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/pypircfile.rst` & `cellmaps_generate_hierarchy-0.1.0a5/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/usage.rst` & `cellmaps_generate_hierarchy-0.1.0a5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/docs/versioningscheme.rst` & `cellmaps_generate_hierarchy-0.1.0a5/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/setup.py` & `cellmaps_generate_hierarchy-0.1.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/tests/data/fake_4_node_coembedding.tsv` & `cellmaps_generate_hierarchy-0.1.0a5/tests/data/fake_4_node_coembedding.tsv`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/tests/test_cdapshierarchygenerator.py` & `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cdapshierarchygenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import unittest
 from unittest.mock import MagicMock
 import json
 import ndex2
 from io import StringIO
 
 from cellmaps_utils import constants
+import cellmaps_generate_hierarchy
 from cellmaps_generate_hierarchy.hierarchy import CDAPSHiDeFHierarchyGenerator
 from cellmaps_generate_hierarchy.hierarchy import CXHierarchyGenerator
 
 
 class TestCDAPSHierarchyGenerator(unittest.TestCase):
     """Tests for `CDAPSHierarchyGenerator`."""
 
@@ -192,12 +193,38 @@
                                                       source_file=two_edge_net_file +
                                                       CDAPSHiDeFHierarchyGenerator.EDGELIST_TSV,
                                                       data_dict=data_dict)
             self.assertEqual(2, mockprov.register_dataset.call_count)
         finally:
             shutil.rmtree(temp_dir)
 
+    def test_register_hidef_output_files(self):
+        temp_dir = tempfile.mkdtemp()
+        try:
+            mockprov = MagicMock()
+            mockprov.register_dataset = MagicMock()
+            mockprov.register_dataset.side_effect = ['X', 'Y', 'Z']
+            gen = CDAPSHiDeFHierarchyGenerator(provenance_utils=mockprov)
+            gen._register_hidef_output_files(temp_dir)
+            self.assertEqual(['X', 'Y', 'Z'], gen.get_generated_dataset_ids())
+
+            data_dict = {'name': CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX +
+                         '.nodes HiDeF output nodes file',
+                         'description': ' HiDeF output nodes file',
+                         'data-format': 'tsv',
+                         'author': 'cellmaps_generate_hierarchy',
+                         'version': cellmaps_generate_hierarchy.__version__,
+                         'date-published': date.today().strftime('%m-%d-%Y')}
+            mockprov.register_dataset.assert_any_call(temp_dir,
+                                                      source_file=os.path.join(temp_dir,
+                                                                               CDAPSHiDeFHierarchyGenerator.HIDEF_OUT_PREFIX +
+                                                                               '.nodes'),
+                                                      data_dict=data_dict)
+            self.assertEqual(3, mockprov.register_dataset.call_count)
+        finally:
+            shutil.rmtree(temp_dir)
+
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmaps_generate_hierarchycmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmapsgeneratehierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cellmapsgeneratehierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/tests/test_cosinesimilarityppigenerator.py` & `cellmaps_generate_hierarchy-0.1.0a5/tests/test_cosinesimilarityppigenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a4/tests/test_integration_cellmaps_generate_hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a5/tests/test_integration_cellmaps_generate_hierarchy.py`

 * *Files identical despite different names*

