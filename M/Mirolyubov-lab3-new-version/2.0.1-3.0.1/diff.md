# Comparing `tmp/Mirolyubov_lab3_new_version-2.0.1.tar.gz` & `tmp/Mirolyubov_lab3_new_version-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mirolyubov_lab3_new_version-2.0.1.tar", last modified: Wed May 31 12:44:34 2023, max compression
+gzip compressed data, was "Mirolyubov_lab3_new_version-3.0.1.tar", last modified: Wed May 31 12:54:30 2023, max compression
```

## Comparing `Mirolyubov_lab3_new_version-2.0.1.tar` & `Mirolyubov_lab3_new_version-3.0.1.tar`

### file list

```diff
@@ -1,9 +1,16 @@
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:44:34.192063 Mirolyubov_lab3_new_version-2.0.1/
-drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:44:34.192063 Mirolyubov_lab3_new_version-2.0.1/Mirolyubov_lab3_new_version.egg-info/
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-05-31 12:44:34.000000 Mirolyubov_lab3_new_version-2.0.1/Mirolyubov_lab3_new_version.egg-info/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      212 2023-05-31 12:44:34.000000 Mirolyubov_lab3_new_version-2.0.1/Mirolyubov_lab3_new_version.egg-info/SOURCES.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-31 12:44:34.000000 Mirolyubov_lab3_new_version-2.0.1/Mirolyubov_lab3_new_version.egg-info/dependency_links.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-31 12:44:34.000000 Mirolyubov_lab3_new_version-2.0.1/Mirolyubov_lab3_new_version.egg-info/top_level.txt
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-05-31 12:44:34.192063 Mirolyubov_lab3_new_version-2.0.1/PKG-INFO
--rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-31 12:44:34.192063 Mirolyubov_lab3_new_version-2.0.1/setup.cfg
--rw-rw-r--   0 ilya      (1000) ilya      (1000)      299 2023-05-31 12:42:26.000000 Mirolyubov_lab3_new_version-2.0.1/setup.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       54 2023-05-30 21:19:09.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/CONSTANTS.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       94 2023-05-30 21:19:09.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/__init__.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      323 2023-05-30 21:19:09.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/factory.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7825 2023-05-31 12:52:02.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/json_serializer.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     9776 2023-05-31 12:52:02.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/packing.py
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)     7999 2023-05-31 12:52:02.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version/xml_serializer.py
+drwxrwxr-x   0 ilya      (1000) ilya      (1000)        0 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      464 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)        1 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       28 2023-05-31 12:54:30.000000 Mirolyubov_lab3_new_version-3.0.1/Mirolyubov_lab3_new_version.egg-info/top_level.txt
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      171 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/PKG-INFO
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)       38 2023-05-31 12:54:30.433338 Mirolyubov_lab3_new_version-3.0.1/setup.cfg
+-rw-rw-r--   0 ilya      (1000) ilya      (1000)      315 2023-05-31 12:54:18.000000 Mirolyubov_lab3_new_version-3.0.1/setup.py
```

