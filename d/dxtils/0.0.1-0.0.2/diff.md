# Comparing `tmp/dxtils-0.0.1.tar.gz` & `tmp/dxtils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxtils-0.0.1.tar", last modified: Wed May 31 18:09:15 2023, max compression
+gzip compressed data, was "dxtils-0.0.2.tar", last modified: Wed May 31 18:32:09 2023, max compression
```

## Comparing `dxtils-0.0.1.tar` & `dxtils-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 18:09:15.832323 dxtils-0.0.1/
--rw-rw-rw-   0        0        0      169 2023-05-31 18:09:15.828325 dxtils-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-05-31 18:05:29.000000 dxtils-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 18:09:15.771326 dxtils-0.0.1/dxtils/
--rw-rw-rw-   0        0        0     1143 2023-05-31 18:02:04.000000 dxtils-0.0.1/dxtils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:09:15.823328 dxtils-0.0.1/dxtils.egg-info/
--rw-rw-rw-   0        0        0      169 2023-05-31 18:09:14.000000 dxtils-0.0.1/dxtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-05-31 18:09:15.000000 dxtils-0.0.1/dxtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 18:09:14.000000 dxtils-0.0.1/dxtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 18:09:14.000000 dxtils-0.0.1/dxtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-05-31 18:05:14.000000 dxtils-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 18:09:15.833421 dxtils-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 18:32:09.001939 dxtils-0.0.2/
+-rw-rw-rw-   0        0        0      169 2023-05-31 18:32:08.994448 dxtils-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2023-05-31 18:05:29.000000 dxtils-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 18:32:08.935978 dxtils-0.0.2/dxtils/
+-rw-rw-rw-   0        0        0     1454 2023-05-31 18:30:30.000000 dxtils-0.0.2/dxtils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:32:08.987936 dxtils-0.0.2/dxtils.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-05-31 18:32:07.000000 dxtils-0.0.2/dxtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-05-31 18:32:08.000000 dxtils-0.0.2/dxtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 18:32:07.000000 dxtils-0.0.2/dxtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 18:32:07.000000 dxtils-0.0.2/dxtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      277 2023-05-31 18:30:36.000000 dxtils-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 18:32:09.002935 dxtils-0.0.2/setup.cfg
```

