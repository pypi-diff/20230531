# Comparing `tmp/pygraphviz-1.8rc1.zip` & `tmp/pygraphviz-1.9.zip`

## zipinfo {}

```diff
@@ -1,73 +1,73 @@
-Zip file size: 120107 bytes, number of entries: 71
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/examples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/pygraphviz/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/pygraphviz.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/doc/
--rw-rw-r--  2.0 unx     4386 b- defN 22-Jan-09 22:54 pygraphviz-1.8rc1/INSTALL.txt
--rw-rw-r--  2.0 unx     1621 b- defN 21-Jan-15 09:57 pygraphviz-1.8rc1/LICENSE
--rw-rw-r--  2.0 unx      359 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/MANIFEST.in
--rw-rw-r--  2.0 unx     2318 b- defN 21-Jan-02 07:37 pygraphviz-1.8rc1/pystrings.swg
--rw-rw-r--  2.0 unx       38 b- defN 22-Jan-14 16:46 pygraphviz-1.8rc1/setup.cfg
--rw-rw-r--  2.0 unx     2816 b- defN 22-Jan-14 16:46 pygraphviz-1.8rc1/PKG-INFO
--rw-rw-r--  2.0 unx     3715 b- defN 21-Dec-26 14:03 pygraphviz-1.8rc1/setup.py
--rw-rw-r--  2.0 unx     1509 b- defN 21-Dec-26 13:11 pygraphviz-1.8rc1/README.rst
--rw-rw-r--  2.0 unx      419 b- defN 21-Jan-02 07:55 pygraphviz-1.8rc1/Makefile
--rw-rw-r--  2.0 unx    20236 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/examples/miles_dat.txt.gz
--rw-rw-r--  2.0 unx      801 b- defN 21-Jan-02 07:43 pygraphviz-1.8rc1/examples/skip_utf8_encoding.py
--rw-rw-r--  2.0 unx      961 b- defN 21-Jan-02 07:43 pygraphviz-1.8rc1/examples/plot_star.py
--rw-rw-r--  2.0 unx      695 b- defN 21-Jan-02 07:43 pygraphviz-1.8rc1/examples/plot_attributes.py
--rw-rw-r--  2.0 unx     3075 b- defN 21-Jan-02 07:43 pygraphviz-1.8rc1/examples/plot_miles.py
--rw-rw-r--  2.0 unx     1236 b- defN 21-Jan-02 07:43 pygraphviz-1.8rc1/examples/skip_django_simple.py
--rw-rw-r--  2.0 unx      452 b- defN 21-Jan-02 07:43 pygraphviz-1.8rc1/examples/plot_subgraph.py
--rw-rw-r--  2.0 unx      693 b- defN 21-Jan-02 07:43 pygraphviz-1.8rc1/examples/plot_simple.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/pygraphviz/tests/
--rw-rw-r--  2.0 unx   188417 b- defN 21-Jan-16 15:05 pygraphviz-1.8rc1/pygraphviz/graphviz_wrap.c
--rw-rw-r--  2.0 unx     8977 b- defN 21-Jan-16 15:05 pygraphviz-1.8rc1/pygraphviz/graphviz.i
--rw-rw-r--  2.0 unx     2775 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/scraper.py
--rw-rw-r--  2.0 unx      590 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/testing.py
--rw-rw-r--  2.0 unx     6930 b- defN 21-Dec-26 14:07 pygraphviz-1.8rc1/pygraphviz/graphviz.py
--rw-rw-r--  2.0 unx    69722 b- defN 22-Jan-09 21:57 pygraphviz-1.8rc1/pygraphviz/agraph.py
--rw-rw-r--  2.0 unx      858 b- defN 22-Jan-14 16:26 pygraphviz-1.8rc1/pygraphviz/__init__.py
--rw-rw-r--  2.0 unx     2707 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_attribute_defaults.py
--rw-rw-r--  2.0 unx      974 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_subgraph.py
--rw-rw-r--  2.0 unx     1058 b- defN 21-Jan-02 07:42 pygraphviz-1.8rc1/pygraphviz/tests/test_readwrite.py
--rw-rw-r--  2.0 unx      933 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_unicode.py
--rw-rw-r--  2.0 unx     4489 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_drawing.py
--rw-rw-r--  2.0 unx      925 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_string.py
--rw-rw-r--  2.0 unx      253 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_close.py
--rw-rw-r--  2.0 unx     1022 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_scraper.py
--rw-rw-r--  2.0 unx      645 b- defN 22-Jan-09 20:07 pygraphviz-1.8rc1/pygraphviz/tests/test_repr_mimebundle.py
--rw-rw-r--  2.0 unx     1964 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_edge_attributes.py
--rw-rw-r--  2.0 unx    16665 b- defN 21-Dec-26 13:11 pygraphviz-1.8rc1/pygraphviz/tests/test_graph.py
--rw-rw-r--  2.0 unx     2069 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_html.py
--rw-rw-r--  2.0 unx      880 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_clear.py
--rw-rw-r--  2.0 unx        0 b- defN 21-Jan-02 07:42 pygraphviz-1.8rc1/pygraphviz/tests/__init__.py
--rw-rw-r--  2.0 unx     1487 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/pygraphviz/tests/test_node_attributes.py
--rw-rw-r--  2.0 unx     3270 b- defN 21-Jan-15 09:57 pygraphviz-1.8rc1/pygraphviz/tests/test_layout.py
--rw-rw-r--  2.0 unx       11 b- defN 22-Jan-14 16:46 pygraphviz-1.8rc1/pygraphviz.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Jan-14 16:46 pygraphviz-1.8rc1/pygraphviz.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     1655 b- defN 22-Jan-14 16:46 pygraphviz-1.8rc1/pygraphviz.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx     2816 b- defN 22-Jan-14 16:46 pygraphviz-1.8rc1/pygraphviz.egg-info/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/doc/source/
--rw-rw-r--  2.0 unx     4327 b- defN 20-Dec-16 18:20 pygraphviz-1.8rc1/doc/Makefile
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/doc/source/reference/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jan-14 16:46 pygraphviz-1.8rc1/doc/source/_templates/
--rw-rw-r--  2.0 unx     2765 b- defN 21-Jan-15 09:57 pygraphviz-1.8rc1/doc/source/tutorial.rst
--rw-rw-r--  2.0 unx     4386 b- defN 22-Jan-09 22:54 pygraphviz-1.8rc1/doc/source/install.rst
--rw-rw-r--  2.0 unx       36 b- defN 22-Jan-11 22:12 pygraphviz-1.8rc1/doc/source/contribute.rst
--rw-rw-r--  2.0 unx     4541 b- defN 22-Jan-09 20:07 pygraphviz-1.8rc1/doc/source/conf.py
--rw-rw-r--  2.0 unx      264 b- defN 22-Jan-11 22:12 pygraphviz-1.8rc1/doc/source/index.rst
--rw-rw-r--  2.0 unx      155 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/doc/source/reference/history.rst
--rw-rw-r--  2.0 unx      728 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/doc/source/reference/credits.rst
--rw-rw-r--  2.0 unx      283 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/doc/source/reference/related.rst
--rw-rw-r--  2.0 unx     2121 b- defN 21-Jan-18 17:41 pygraphviz-1.8rc1/doc/source/reference/faq.rst
--rw-rw-r--  2.0 unx      138 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/doc/source/reference/agraph.rst
--rw-rw-r--  2.0 unx     2416 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/doc/source/reference/api_notes.rst
--rw-rw-r--  2.0 unx     5829 b- defN 22-Jan-14 16:24 pygraphviz-1.8rc1/doc/source/reference/news.rst
--rw-rw-r--  2.0 unx      160 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/doc/source/reference/index.rst
--rw-rw-r--  2.0 unx     2955 b- defN 20-Dec-16 18:14 pygraphviz-1.8rc1/doc/source/reference/legal.rst
--rw-rw-r--  2.0 unx      315 b- defN 21-Feb-01 14:28 pygraphviz-1.8rc1/doc/source/_templates/layout.html
--rw-rw-r--  2.0 unx      331 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/doc/source/_templates/dev_banner.html
--rw-rw-r--  2.0 unx      351 b- defN 21-Jan-04 12:03 pygraphviz-1.8rc1/doc/source/_templates/eol_banner.html
-71 files, 399524 bytes uncompressed, 108677 bytes compressed:  72.8%
+Zip file size: 119946 bytes, number of entries: 71
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/examples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/pygraphviz/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/pygraphviz.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/doc/
+-rw-rw-r--  2.0 unx     4386 b- defN 22-Jan-09 22:54 pygraphviz-1.9/INSTALL.txt
+-rw-rw-r--  2.0 unx     1621 b- defN 22-Feb-09 09:59 pygraphviz-1.9/LICENSE
+-rw-rw-r--  2.0 unx      359 b- defN 20-Dec-16 18:14 pygraphviz-1.9/MANIFEST.in
+-rw-rw-r--  2.0 unx     2318 b- defN 21-Jan-02 07:37 pygraphviz-1.9/pystrings.swg
+-rw-rw-r--  2.0 unx       38 b- defN 22-Feb-09 10:14 pygraphviz-1.9/setup.cfg
+-rw-rw-r--  2.0 unx     2813 b- defN 22-Feb-09 10:14 pygraphviz-1.9/PKG-INFO
+-rw-rw-r--  2.0 unx     3715 b- defN 22-Feb-09 09:15 pygraphviz-1.9/setup.py
+-rw-rw-r--  2.0 unx     1509 b- defN 22-Feb-09 09:59 pygraphviz-1.9/README.rst
+-rw-rw-r--  2.0 unx      419 b- defN 21-Jan-02 07:55 pygraphviz-1.9/Makefile
+-rw-rw-r--  2.0 unx    20236 b- defN 20-Dec-16 18:14 pygraphviz-1.9/examples/miles_dat.txt.gz
+-rw-rw-r--  2.0 unx      801 b- defN 21-Jan-02 07:43 pygraphviz-1.9/examples/skip_utf8_encoding.py
+-rw-rw-r--  2.0 unx      961 b- defN 21-Jan-02 07:43 pygraphviz-1.9/examples/plot_star.py
+-rw-rw-r--  2.0 unx      695 b- defN 21-Jan-02 07:43 pygraphviz-1.9/examples/plot_attributes.py
+-rw-rw-r--  2.0 unx     3075 b- defN 21-Jan-02 07:43 pygraphviz-1.9/examples/plot_miles.py
+-rw-rw-r--  2.0 unx     1236 b- defN 21-Jan-02 07:43 pygraphviz-1.9/examples/skip_django_simple.py
+-rw-rw-r--  2.0 unx      452 b- defN 21-Jan-02 07:43 pygraphviz-1.9/examples/plot_subgraph.py
+-rw-rw-r--  2.0 unx      693 b- defN 21-Jan-02 07:43 pygraphviz-1.9/examples/plot_simple.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/pygraphviz/tests/
+-rw-rw-r--  2.0 unx   188417 b- defN 21-Jan-16 15:05 pygraphviz-1.9/pygraphviz/graphviz_wrap.c
+-rw-rw-r--  2.0 unx     8977 b- defN 21-Jan-16 15:05 pygraphviz-1.9/pygraphviz/graphviz.i
+-rw-rw-r--  2.0 unx     2775 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/scraper.py
+-rw-rw-r--  2.0 unx      590 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/testing.py
+-rw-rw-r--  2.0 unx     6930 b- defN 21-Dec-26 14:07 pygraphviz-1.9/pygraphviz/graphviz.py
+-rw-rw-r--  2.0 unx    69768 b- defN 22-Feb-09 09:15 pygraphviz-1.9/pygraphviz/agraph.py
+-rw-rw-r--  2.0 unx      855 b- defN 22-Feb-09 09:30 pygraphviz-1.9/pygraphviz/__init__.py
+-rw-rw-r--  2.0 unx     2707 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_attribute_defaults.py
+-rw-rw-r--  2.0 unx      974 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_subgraph.py
+-rw-rw-r--  2.0 unx     1058 b- defN 21-Jan-02 07:42 pygraphviz-1.9/pygraphviz/tests/test_readwrite.py
+-rw-rw-r--  2.0 unx      933 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_unicode.py
+-rw-rw-r--  2.0 unx     4489 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_drawing.py
+-rw-rw-r--  2.0 unx      925 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_string.py
+-rw-rw-r--  2.0 unx      253 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_close.py
+-rw-rw-r--  2.0 unx     1022 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_scraper.py
+-rw-rw-r--  2.0 unx      645 b- defN 22-Jan-09 20:07 pygraphviz-1.9/pygraphviz/tests/test_repr_mimebundle.py
+-rw-rw-r--  2.0 unx     1964 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_edge_attributes.py
+-rw-rw-r--  2.0 unx    16665 b- defN 21-Dec-26 13:11 pygraphviz-1.9/pygraphviz/tests/test_graph.py
+-rw-rw-r--  2.0 unx     2069 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_html.py
+-rw-rw-r--  2.0 unx      880 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_clear.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Jan-02 07:42 pygraphviz-1.9/pygraphviz/tests/__init__.py
+-rw-rw-r--  2.0 unx     1487 b- defN 21-Jan-04 12:03 pygraphviz-1.9/pygraphviz/tests/test_node_attributes.py
+-rw-rw-r--  2.0 unx     3364 b- defN 22-Feb-09 09:15 pygraphviz-1.9/pygraphviz/tests/test_layout.py
+-rw-rw-r--  2.0 unx       11 b- defN 22-Feb-09 10:14 pygraphviz-1.9/pygraphviz.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Feb-09 10:14 pygraphviz-1.9/pygraphviz.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     1655 b- defN 22-Feb-09 10:14 pygraphviz-1.9/pygraphviz.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx     2813 b- defN 22-Feb-09 10:14 pygraphviz-1.9/pygraphviz.egg-info/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/doc/source/
+-rw-rw-r--  2.0 unx     4327 b- defN 20-Dec-16 18:20 pygraphviz-1.9/doc/Makefile
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/doc/source/reference/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Feb-09 10:14 pygraphviz-1.9/doc/source/_templates/
+-rw-rw-r--  2.0 unx     2766 b- defN 22-Feb-09 09:15 pygraphviz-1.9/doc/source/tutorial.rst
+-rw-rw-r--  2.0 unx     4386 b- defN 22-Jan-09 22:54 pygraphviz-1.9/doc/source/install.rst
+-rw-rw-r--  2.0 unx       36 b- defN 22-Jan-11 22:12 pygraphviz-1.9/doc/source/contribute.rst
+-rw-rw-r--  2.0 unx     4541 b- defN 22-Jan-09 20:07 pygraphviz-1.9/doc/source/conf.py
+-rw-rw-r--  2.0 unx      264 b- defN 22-Jan-11 22:12 pygraphviz-1.9/doc/source/index.rst
+-rw-rw-r--  2.0 unx      155 b- defN 20-Dec-16 18:14 pygraphviz-1.9/doc/source/reference/history.rst
+-rw-rw-r--  2.0 unx      728 b- defN 20-Dec-16 18:14 pygraphviz-1.9/doc/source/reference/credits.rst
+-rw-rw-r--  2.0 unx      283 b- defN 20-Dec-16 18:14 pygraphviz-1.9/doc/source/reference/related.rst
+-rw-rw-r--  2.0 unx     2121 b- defN 21-Jan-18 17:41 pygraphviz-1.9/doc/source/reference/faq.rst
+-rw-rw-r--  2.0 unx      138 b- defN 20-Dec-16 18:14 pygraphviz-1.9/doc/source/reference/agraph.rst
+-rw-rw-r--  2.0 unx     2416 b- defN 20-Dec-16 18:14 pygraphviz-1.9/doc/source/reference/api_notes.rst
+-rw-rw-r--  2.0 unx     6015 b- defN 22-Feb-09 09:23 pygraphviz-1.9/doc/source/reference/news.rst
+-rw-rw-r--  2.0 unx      160 b- defN 20-Dec-16 18:14 pygraphviz-1.9/doc/source/reference/index.rst
+-rw-rw-r--  2.0 unx     2955 b- defN 20-Dec-16 18:14 pygraphviz-1.9/doc/source/reference/legal.rst
+-rw-rw-r--  2.0 unx      225 b- defN 22-Feb-09 09:29 pygraphviz-1.9/doc/source/_templates/layout.html
+-rw-rw-r--  2.0 unx      331 b- defN 21-Jan-04 12:03 pygraphviz-1.9/doc/source/_templates/dev_banner.html
+-rw-rw-r--  2.0 unx      351 b- defN 21-Jan-04 12:03 pygraphviz-1.9/doc/source/_templates/eol_banner.html
+71 files, 399752 bytes uncompressed, 108942 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -1,214 +1,214 @@
-Filename: pygraphviz-1.8rc1/
+Filename: pygraphviz-1.9/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/
+Filename: pygraphviz-1.9/examples/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/
+Filename: pygraphviz-1.9/pygraphviz/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz.egg-info/
+Filename: pygraphviz-1.9/pygraphviz.egg-info/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/
+Filename: pygraphviz-1.9/doc/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/INSTALL.txt
+Filename: pygraphviz-1.9/INSTALL.txt
 Comment: 
 
-Filename: pygraphviz-1.8rc1/LICENSE
+Filename: pygraphviz-1.9/LICENSE
 Comment: 
 
-Filename: pygraphviz-1.8rc1/MANIFEST.in
+Filename: pygraphviz-1.9/MANIFEST.in
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pystrings.swg
+Filename: pygraphviz-1.9/pystrings.swg
 Comment: 
 
-Filename: pygraphviz-1.8rc1/setup.cfg
+Filename: pygraphviz-1.9/setup.cfg
 Comment: 
 
-Filename: pygraphviz-1.8rc1/PKG-INFO
+Filename: pygraphviz-1.9/PKG-INFO
 Comment: 
 
-Filename: pygraphviz-1.8rc1/setup.py
+Filename: pygraphviz-1.9/setup.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/README.rst
+Filename: pygraphviz-1.9/README.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/Makefile
+Filename: pygraphviz-1.9/Makefile
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/miles_dat.txt.gz
+Filename: pygraphviz-1.9/examples/miles_dat.txt.gz
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/skip_utf8_encoding.py
+Filename: pygraphviz-1.9/examples/skip_utf8_encoding.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/plot_star.py
+Filename: pygraphviz-1.9/examples/plot_star.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/plot_attributes.py
+Filename: pygraphviz-1.9/examples/plot_attributes.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/plot_miles.py
+Filename: pygraphviz-1.9/examples/plot_miles.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/skip_django_simple.py
+Filename: pygraphviz-1.9/examples/skip_django_simple.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/plot_subgraph.py
+Filename: pygraphviz-1.9/examples/plot_subgraph.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/examples/plot_simple.py
+Filename: pygraphviz-1.9/examples/plot_simple.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/
+Filename: pygraphviz-1.9/pygraphviz/tests/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/graphviz_wrap.c
+Filename: pygraphviz-1.9/pygraphviz/graphviz_wrap.c
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/graphviz.i
+Filename: pygraphviz-1.9/pygraphviz/graphviz.i
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/scraper.py
+Filename: pygraphviz-1.9/pygraphviz/scraper.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/testing.py
+Filename: pygraphviz-1.9/pygraphviz/testing.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/graphviz.py
+Filename: pygraphviz-1.9/pygraphviz/graphviz.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/agraph.py
+Filename: pygraphviz-1.9/pygraphviz/agraph.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/__init__.py
+Filename: pygraphviz-1.9/pygraphviz/__init__.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_attribute_defaults.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_attribute_defaults.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_subgraph.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_subgraph.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_readwrite.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_readwrite.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_unicode.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_unicode.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_drawing.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_drawing.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_string.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_string.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_close.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_close.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_scraper.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_scraper.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_repr_mimebundle.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_repr_mimebundle.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_edge_attributes.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_edge_attributes.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_graph.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_graph.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_html.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_html.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_clear.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_clear.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/__init__.py
+Filename: pygraphviz-1.9/pygraphviz/tests/__init__.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_node_attributes.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_node_attributes.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz/tests/test_layout.py
+Filename: pygraphviz-1.9/pygraphviz/tests/test_layout.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz.egg-info/top_level.txt
+Filename: pygraphviz-1.9/pygraphviz.egg-info/top_level.txt
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz.egg-info/dependency_links.txt
+Filename: pygraphviz-1.9/pygraphviz.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz.egg-info/SOURCES.txt
+Filename: pygraphviz-1.9/pygraphviz.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pygraphviz-1.8rc1/pygraphviz.egg-info/PKG-INFO
+Filename: pygraphviz-1.9/pygraphviz.egg-info/PKG-INFO
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/
+Filename: pygraphviz-1.9/doc/source/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/Makefile
+Filename: pygraphviz-1.9/doc/Makefile
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/
+Filename: pygraphviz-1.9/doc/source/reference/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/_templates/
+Filename: pygraphviz-1.9/doc/source/_templates/
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/tutorial.rst
+Filename: pygraphviz-1.9/doc/source/tutorial.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/install.rst
+Filename: pygraphviz-1.9/doc/source/install.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/contribute.rst
+Filename: pygraphviz-1.9/doc/source/contribute.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/conf.py
+Filename: pygraphviz-1.9/doc/source/conf.py
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/index.rst
+Filename: pygraphviz-1.9/doc/source/index.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/history.rst
+Filename: pygraphviz-1.9/doc/source/reference/history.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/credits.rst
+Filename: pygraphviz-1.9/doc/source/reference/credits.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/related.rst
+Filename: pygraphviz-1.9/doc/source/reference/related.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/faq.rst
+Filename: pygraphviz-1.9/doc/source/reference/faq.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/agraph.rst
+Filename: pygraphviz-1.9/doc/source/reference/agraph.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/api_notes.rst
+Filename: pygraphviz-1.9/doc/source/reference/api_notes.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/news.rst
+Filename: pygraphviz-1.9/doc/source/reference/news.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/index.rst
+Filename: pygraphviz-1.9/doc/source/reference/index.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/reference/legal.rst
+Filename: pygraphviz-1.9/doc/source/reference/legal.rst
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/_templates/layout.html
+Filename: pygraphviz-1.9/doc/source/_templates/layout.html
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/_templates/dev_banner.html
+Filename: pygraphviz-1.9/doc/source/_templates/dev_banner.html
 Comment: 
 
-Filename: pygraphviz-1.8rc1/doc/source/_templates/eol_banner.html
+Filename: pygraphviz-1.9/doc/source/_templates/eol_banner.html
 Comment: 
 
 Zip file comment:
```

## Comparing `pygraphviz-1.8rc1/INSTALL.txt` & `pygraphviz-1.9/INSTALL.txt`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/LICENSE` & `pygraphviz-1.9/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2004-2021 by
+Copyright (C) 2004-2022 by
 Aric Hagberg <hagberg@lanl.gov>
 Dan Schult <dschult@colgate.edu>
 Manos Renieris, http://www.cs.brown.edu/~er/
 Distributed with BSD license.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
```

## Comparing `pygraphviz-1.8rc1/pystrings.swg` & `pygraphviz-1.9/pystrings.swg`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/PKG-INFO` & `pygraphviz-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygraphviz
-Version: 1.8rc1
+Version: 1.9
 Summary: Python interface to Graphviz
 Home-page: http://pygraphviz.github.io
 Author: Aric Hagberg
 Author-email: aric.hagberg@gmail.com
 License: BSD
 Download-URL: https://pypi.python.org/pypi/pygraphviz
 Keywords: Networks,Graph Visualization,network,graph,graph drawing
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 PyGraphviz
 ==========
 
 .. image:: https://github.com/pygraphviz/pygraphviz/workflows/test/badge.svg?branch=main
   :target: https://github.com/pygraphviz/pygraphviz/actions?query=workflow%3Atest+branch%3Amain
@@ -74,13 +74,13 @@
 Please see `INSTALL.txt` for details.
 
 License
 -------
 
 Released under the 3-Clause BSD license (see ``LICENSE``)::
 
-  Copyright (C) 2006-2021 PyGraphviz Developers
+  Copyright (C) 2006-2022 PyGraphviz Developers
   Aric Hagberg <aric.hagberg@gmail.gov>
   Dan Schult <dschult@colgate.edu>
   Manos Renieris
```

## Comparing `pygraphviz-1.8rc1/setup.py` & `pygraphviz-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,10 +101,10 @@
         download_url=download_url,
         classifiers=classifiers,
         packages=packages,
         data_files=data,
         ext_modules=extension,
         package_data=package_data,
         include_package_data=True,
-        python_requires=">=3.7",
+        python_requires=">=3.8",
         tests_require=["pytest"],
     )
```

## Comparing `pygraphviz-1.8rc1/README.rst` & `pygraphviz-1.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -42,11 +42,11 @@
 Please see `INSTALL.txt` for details.
 
 License
 -------
 
 Released under the 3-Clause BSD license (see ``LICENSE``)::
 
-  Copyright (C) 2006-2021 PyGraphviz Developers
+  Copyright (C) 2006-2022 PyGraphviz Developers
   Aric Hagberg <aric.hagberg@gmail.gov>
   Dan Schult <dschult@colgate.edu>
   Manos Renieris
```

## Comparing `pygraphviz-1.8rc1/examples/miles_dat.txt.gz` & `pygraphviz-1.9/examples/miles_dat.txt.gz`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/examples/skip_utf8_encoding.py` & `pygraphviz-1.9/examples/skip_utf8_encoding.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/examples/plot_star.py` & `pygraphviz-1.9/examples/plot_star.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/examples/plot_attributes.py` & `pygraphviz-1.9/examples/plot_attributes.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/examples/plot_miles.py` & `pygraphviz-1.9/examples/plot_miles.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/examples/skip_django_simple.py` & `pygraphviz-1.9/examples/skip_django_simple.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/examples/plot_simple.py` & `pygraphviz-1.9/examples/plot_simple.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/graphviz_wrap.c` & `pygraphviz-1.9/pygraphviz/graphviz_wrap.c`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/graphviz.i` & `pygraphviz-1.9/pygraphviz/graphviz.i`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/scraper.py` & `pygraphviz-1.9/pygraphviz/scraper.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/testing.py` & `pygraphviz-1.9/pygraphviz/testing.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/graphviz.py` & `pygraphviz-1.9/pygraphviz/graphviz.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/agraph.py` & `pygraphviz-1.9/pygraphviz/agraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1326,31 +1326,33 @@
         fh.seek(0)
         self.read(fh)
         fh.close()
         return self
 
     def _get_prog(self, prog):
         # private: get path of graphviz program
-        progs = [
+        progs = {
             "neato",
             "dot",
             "twopi",
             "circo",
             "fdp",
             "nop",
+            "osage",
+            "patchwork",
             "gc",
             "acyclic",
             "gvpr",
             "gvcolor",
             "ccomps",
             "sccmap",
             "tred",
             "sfdp",
             "unflatten",
-        ]
+        }
         if prog not in progs:
             raise ValueError(f"Program {prog} is not one of: {', '.join(progs)}.")
 
         try:  # user must pick one of the graphviz programs...
             runprog = self._which(prog)
         except:
             raise ValueError(f"Program {prog} not found in path.")
```

## Comparing `pygraphviz-1.8rc1/pygraphviz/__init__.py` & `pygraphviz-1.9/pygraphviz/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     import os
 
     for path in os.environ["PATH"].split(os.pathsep):
         if "graphviz" in path.lower() and os.path.exists(path):
             os.add_dll_directory(path)
 
 
-__version__ = "1.8rc1"
+__version__ = "1.9"
 
 from .agraph import AGraph, Node, Edge, Attribute, ItemAttribute, DotError
 
 __all__ = ["AGraph", "Node", "Edge", "Attribute", "ItemAttribute", "DotError"]
 
 from . import testing
```

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_attribute_defaults.py` & `pygraphviz-1.9/pygraphviz/tests/test_attribute_defaults.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_subgraph.py` & `pygraphviz-1.9/pygraphviz/tests/test_subgraph.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_readwrite.py` & `pygraphviz-1.9/pygraphviz/tests/test_readwrite.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_unicode.py` & `pygraphviz-1.9/pygraphviz/tests/test_unicode.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_drawing.py` & `pygraphviz-1.9/pygraphviz/tests/test_drawing.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_string.py` & `pygraphviz-1.9/pygraphviz/tests/test_string.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_scraper.py` & `pygraphviz-1.9/pygraphviz/tests/test_scraper.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_repr_mimebundle.py` & `pygraphviz-1.9/pygraphviz/tests/test_repr_mimebundle.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_edge_attributes.py` & `pygraphviz-1.9/pygraphviz/tests/test_edge_attributes.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_graph.py` & `pygraphviz-1.9/pygraphviz/tests/test_graph.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_html.py` & `pygraphviz-1.9/pygraphviz/tests/test_html.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_clear.py` & `pygraphviz-1.9/pygraphviz/tests/test_clear.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz/tests/test_node_attributes.py` & `pygraphviz-1.9/pygraphviz/tests/test_node_attributes.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz.egg-info/SOURCES.txt` & `pygraphviz-1.9/pygraphviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/pygraphviz.egg-info/PKG-INFO` & `pygraphviz-1.9/pygraphviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygraphviz
-Version: 1.8rc1
+Version: 1.9
 Summary: Python interface to Graphviz
 Home-page: http://pygraphviz.github.io
 Author: Aric Hagberg
 Author-email: aric.hagberg@gmail.com
 License: BSD
 Download-URL: https://pypi.python.org/pypi/pygraphviz
 Keywords: Networks,Graph Visualization,network,graph,graph drawing
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
 
 PyGraphviz
 ==========
 
 .. image:: https://github.com/pygraphviz/pygraphviz/workflows/test/badge.svg?branch=main
   :target: https://github.com/pygraphviz/pygraphviz/actions?query=workflow%3Atest+branch%3Amain
@@ -74,13 +74,13 @@
 Please see `INSTALL.txt` for details.
 
 License
 -------
 
 Released under the 3-Clause BSD license (see ``LICENSE``)::
 
-  Copyright (C) 2006-2021 PyGraphviz Developers
+  Copyright (C) 2006-2022 PyGraphviz Developers
   Aric Hagberg <aric.hagberg@gmail.gov>
   Dan Schult <dschult@colgate.edu>
   Manos Renieris
```

## Comparing `pygraphviz-1.8rc1/doc/Makefile` & `pygraphviz-1.9/doc/Makefile`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/doc/source/tutorial.rst` & `pygraphviz-1.9/doc/source/tutorial.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 >>> G = pgv.AGraph(strict=False, directed=True)
 
 You may specify a dot format file to be read on initialization:
 
 >>> G = pgv.AGraph("Petersen.dot")  # doctest: +SKIP
 
-Other options for intializing a graph are using a string,
+Other options for initializing a graph are using a string,
 
 >>> G = pgv.AGraph("graph {1 - 2}")
 
 using a dict of dicts,
 
 >>> d = {"1": {"2": None}, "2": {"1": None, "3": None}, "3": {"2": None}}
 >>> A = pgv.AGraph(d)
```

## Comparing `pygraphviz-1.8rc1/doc/source/install.rst` & `pygraphviz-1.9/doc/source/install.rst`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/doc/source/conf.py` & `pygraphviz-1.9/doc/source/conf.py`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/doc/source/reference/credits.rst` & `pygraphviz-1.9/doc/source/reference/credits.rst`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/doc/source/reference/faq.rst` & `pygraphviz-1.9/doc/source/reference/faq.rst`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/doc/source/reference/api_notes.rst` & `pygraphviz-1.9/doc/source/reference/api_notes.rst`

 * *Files identical despite different names*

## Comparing `pygraphviz-1.8rc1/doc/source/reference/news.rst` & `pygraphviz-1.9/doc/source/reference/news.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 ..  -*- coding: utf-8 -*-
 
 News
 ==== 
 
-pygraphviz-1.8 (draft)
-----------------------
+pygraphviz-1.9
+--------------
 
-Release date: 
+Release date: 9 February 2022
 
  - Drop Python 3.7 support
  - Add Python 3.10 support
+ - Add osage and patchwork to progs list
  - Add IPython rich display hook to AGraph class
  - Add contributor guide
  - Fixed directed nature of AGraph.copy()
  - Minor documentation and code fixes
 
+pygraphviz-1.8
+--------------
+
+Release date: 20 January 2022
+
+This release was pulled because the install was broken with pip 22 and python 3.7.
+
 pygraphviz-1.7
 --------------
 
 Release date: 1 February 2021
 
  - Drop Python 3.6 support
  - Add Python 3.9 support
```

## Comparing `pygraphviz-1.8rc1/doc/source/reference/legal.rst` & `pygraphviz-1.9/doc/source/reference/legal.rst`

 * *Files identical despite different names*

