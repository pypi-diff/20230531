# Comparing `tmp/novapy-0.1.tar.gz` & `tmp/novapy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novapy-0.1.tar", last modified: Wed May 31 20:21:58 2023, max compression
+gzip compressed data, was "novapy-0.1.1.tar", last modified: Wed May 31 20:24:59 2023, max compression
```

## Comparing `novapy-0.1.tar` & `novapy-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 20:21:58.924432 novapy-0.1/
--rw-rw-rw-   0        0        0       51 2023-05-31 20:21:58.923418 novapy-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 20:21:58.921469 novapy-0.1/novapy.egg-info/
--rw-rw-rw-   0        0        0       51 2023-05-31 20:21:58.000000 novapy-0.1/novapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-31 20:21:58.000000 novapy-0.1/novapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 20:21:58.000000 novapy-0.1/novapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-31 20:21:58.000000 novapy-0.1/novapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 20:21:58.000000 novapy-0.1/novapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 20:21:58.924432 novapy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      360 2023-05-31 20:21:46.000000 novapy-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:24:59.814935 novapy-0.1.1/
+-rw-rw-rw-   0        0        0       53 2023-05-31 20:24:59.814435 novapy-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 20:24:59.812435 novapy-0.1.1/novapy.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-05-31 20:24:59.000000 novapy-0.1.1/novapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-31 20:24:59.000000 novapy-0.1.1/novapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:24:59.000000 novapy-0.1.1/novapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-31 20:24:59.000000 novapy-0.1.1/novapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 20:24:59.000000 novapy-0.1.1/novapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:24:59.815435 novapy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-05-31 20:24:57.000000 novapy-0.1.1/setup.py
```

