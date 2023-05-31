# Comparing `tmp/pyndjs-0.0.3.tar.gz` & `tmp/pyndjs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyndjs-0.0.3.tar", last modified: Thu Feb  9 01:11:52 2023, max compression
+gzip compressed data, was "pyndjs-0.0.4.tar", last modified: Wed May 31 07:07:33 2023, max compression
```

## Comparing `pyndjs-0.0.3.tar` & `pyndjs-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-09 01:11:52.000000 pyndjs-0.0.3/
--rw-rw-rw-   0        0        0      192 2023-02-09 01:11:52.000000 pyndjs-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-09 01:11:52.000000 pyndjs-0.0.3/pyndjs/
--rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.3/pyndjs/__init__.py
--rw-rw-rw-   0        0        0     6111 2023-02-09 01:10:26.000000 pyndjs-0.0.3/pyndjs/pyndjs.py
-drwxrwxrwx   0        0        0        0 2023-02-09 01:11:52.000000 pyndjs-0.0.3/pyndjs.egg-info/
--rw-rw-rw-   0        0        0      192 2023-02-09 01:11:52.000000 pyndjs-0.0.3/pyndjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-02-09 01:11:52.000000 pyndjs-0.0.3/pyndjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-09 01:11:52.000000 pyndjs-0.0.3/pyndjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-02-09 01:11:52.000000 pyndjs-0.0.3/pyndjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-09 01:11:52.000000 pyndjs-0.0.3/pyndjs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-09 01:11:52.000000 pyndjs-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      275 2023-02-09 01:11:37.000000 pyndjs-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:07:33.795314 pyndjs-0.0.4/
+-rw-rw-rw-   0        0        0       72 2023-05-31 07:07:33.794314 pyndjs-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 07:07:33.788206 pyndjs-0.0.4/pyndjs/
+-rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.4/pyndjs/__init__.py
+-rw-rw-rw-   0        0        0     6111 2023-02-09 01:10:26.000000 pyndjs-0.0.4/pyndjs/pyndjs.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:07:33.793314 pyndjs-0.0.4/pyndjs.egg-info/
+-rw-rw-rw-   0        0        0       72 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 07:07:33.000000 pyndjs-0.0.4/pyndjs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:07:33.795314 pyndjs-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      275 2023-05-31 07:06:54.000000 pyndjs-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyndjs-0.0.3/pyndjs/pyndjs.py` & `pyndjs-0.0.4/pyndjs/pyndjs.py`

 * *Files identical despite different names*

