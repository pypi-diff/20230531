# Comparing `tmp/AeholdSerializer-0.2.1.tar.gz` & `tmp/AeholdSerializer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AeholdSerializer-0.2.1.tar", last modified: Wed May 31 11:03:32 2023, max compression
+gzip compressed data, was "AeholdSerializer-0.2.2.tar", last modified: Wed May 31 12:29:55 2023, max compression
```

## Comparing `AeholdSerializer-0.2.1.tar` & `AeholdSerializer-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 aehold    (1000) aehold    (1000)        0 2023-05-31 11:03:32.647603 AeholdSerializer-0.2.1/
-drwxrwxr-x   0 aehold    (1000) aehold    (1000)        0 2023-05-31 11:03:32.647603 AeholdSerializer-0.2.1/AeholdSerializer.egg-info/
--rw-rw-r--   0 aehold    (1000) aehold    (1000)      118 2023-05-31 11:03:32.000000 AeholdSerializer-0.2.1/AeholdSerializer.egg-info/PKG-INFO
--rw-rw-r--   0 aehold    (1000) aehold    (1000)      211 2023-05-31 11:03:32.000000 AeholdSerializer-0.2.1/AeholdSerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 aehold    (1000) aehold    (1000)        1 2023-05-31 11:03:32.000000 AeholdSerializer-0.2.1/AeholdSerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 aehold    (1000) aehold    (1000)       43 2023-05-31 11:03:32.000000 AeholdSerializer-0.2.1/AeholdSerializer.egg-info/entry_points.txt
--rw-rw-r--   0 aehold    (1000) aehold    (1000)        1 2023-05-31 11:03:32.000000 AeholdSerializer-0.2.1/AeholdSerializer.egg-info/top_level.txt
--rw-rw-r--   0 aehold    (1000) aehold    (1000)      118 2023-05-31 11:03:32.647603 AeholdSerializer-0.2.1/PKG-INFO
--rw-rw-r--   0 aehold    (1000) aehold    (1000)       38 2023-05-31 11:03:32.647603 AeholdSerializer-0.2.1/setup.cfg
--rw-rw-r--   0 aehold    (1000) aehold    (1000)      324 2023-05-31 11:03:18.000000 AeholdSerializer-0.2.1/setup.py
+drwxrwxr-x   0 aehold    (1000) aehold    (1000)        0 2023-05-31 12:29:55.713378 AeholdSerializer-0.2.2/
+drwxrwxr-x   0 aehold    (1000) aehold    (1000)        0 2023-05-31 12:29:55.713378 AeholdSerializer-0.2.2/AeholdSerializer.egg-info/
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)      118 2023-05-31 12:29:55.000000 AeholdSerializer-0.2.2/AeholdSerializer.egg-info/PKG-INFO
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)      211 2023-05-31 12:29:55.000000 AeholdSerializer-0.2.2/AeholdSerializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)        1 2023-05-31 12:29:55.000000 AeholdSerializer-0.2.2/AeholdSerializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)       53 2023-05-31 12:29:55.000000 AeholdSerializer-0.2.2/AeholdSerializer.egg-info/entry_points.txt
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)        1 2023-05-31 12:29:55.000000 AeholdSerializer-0.2.2/AeholdSerializer.egg-info/top_level.txt
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)      118 2023-05-31 12:29:55.713378 AeholdSerializer-0.2.2/PKG-INFO
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)       38 2023-05-31 12:29:55.713378 AeholdSerializer-0.2.2/setup.cfg
+-rw-rw-r--   0 aehold    (1000) aehold    (1000)      354 2023-05-31 12:29:36.000000 AeholdSerializer-0.2.2/setup.py
```

