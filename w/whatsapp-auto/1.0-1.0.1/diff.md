# Comparing `tmp/whatsapp_auto-1.0.tar.gz` & `tmp/whatsapp_auto-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_auto-1.0.tar", last modified: Wed May 31 17:06:28 2023, max compression
+gzip compressed data, was "whatsapp_auto-1.0.1.tar", last modified: Wed May 31 17:30:18 2023, max compression
```

## Comparing `whatsapp_auto-1.0.tar` & `whatsapp_auto-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 17:06:28.367473 whatsapp_auto-1.0/
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 17:06:28.363585 whatsapp_auto-1.0/.github/
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 17:06:28.364806 whatsapp_auto-1.0/.github/workflows/
--rw-r--r--   0 anish      (501) staff       (20)     1152 2023-05-31 16:42:21.000000 whatsapp_auto-1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 anish      (501) staff       (20)     1062 2023-01-27 15:51:21.000000 whatsapp_auto-1.0/LICENSE
--rw-r--r--   0 anish      (501) staff       (20)      665 2023-05-31 17:06:28.367231 whatsapp_auto-1.0/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)       94 2023-05-31 16:45:41.000000 whatsapp_auto-1.0/README.md
--rw-r--r--   0 anish      (501) staff       (20)      734 2023-05-31 17:05:29.000000 whatsapp_auto-1.0/pyproject.toml
--rw-r--r--   0 anish      (501) staff       (20)       38 2023-05-31 17:06:28.367534 whatsapp_auto-1.0/setup.cfg
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 17:06:28.365814 whatsapp_auto-1.0/whatsapp_auto/
--rw-r--r--   0 anish      (501) staff       (20)       24 2023-01-27 13:35:12.000000 whatsapp_auto-1.0/whatsapp_auto/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)      377 2023-01-27 13:30:00.000000 whatsapp_auto-1.0/whatsapp_auto/exception.py
--rw-r--r--   0 anish      (501) staff       (20)     7814 2023-05-31 17:06:08.000000 whatsapp_auto-1.0/whatsapp_auto/main.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 17:06:28.366910 whatsapp_auto-1.0/whatsapp_auto.egg-info/
--rw-r--r--   0 anish      (501) staff       (20)      665 2023-05-31 17:06:28.000000 whatsapp_auto-1.0/whatsapp_auto.egg-info/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)      328 2023-05-31 17:06:28.000000 whatsapp_auto-1.0/whatsapp_auto.egg-info/SOURCES.txt
--rw-r--r--   0 anish      (501) staff       (20)        1 2023-05-31 17:06:28.000000 whatsapp_auto-1.0/whatsapp_auto.egg-info/dependency_links.txt
--rw-r--r--   0 anish      (501) staff       (20)       33 2023-05-31 17:06:28.000000 whatsapp_auto-1.0/whatsapp_auto.egg-info/requires.txt
--rw-r--r--   0 anish      (501) staff       (20)       14 2023-05-31 17:06:28.000000 whatsapp_auto-1.0/whatsapp_auto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:30:18.788097 whatsapp_auto-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:30:18.784097 whatsapp_auto-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:30:18.784097 whatsapp_auto-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-31 17:30:05.000000 whatsapp_auto-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 17:30:05.000000 whatsapp_auto-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-31 17:30:18.784097 whatsapp_auto-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 17:30:05.000000 whatsapp_auto-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 17:30:05.000000 whatsapp_auto-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:30:18.788097 whatsapp_auto-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:30:18.784097 whatsapp_auto-1.0.1/whatsapp_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 17:30:05.000000 whatsapp_auto-1.0.1/whatsapp_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-31 17:30:05.000000 whatsapp_auto-1.0.1/whatsapp_auto/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-05-31 17:30:05.000000 whatsapp_auto-1.0.1/whatsapp_auto/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:30:18.784097 whatsapp_auto-1.0.1/whatsapp_auto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-31 17:30:18.000000 whatsapp_auto-1.0.1/whatsapp_auto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-31 17:30:18.000000 whatsapp_auto-1.0.1/whatsapp_auto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:30:18.000000 whatsapp_auto-1.0.1/whatsapp_auto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 17:30:18.000000 whatsapp_auto-1.0.1/whatsapp_auto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 17:30:18.000000 whatsapp_auto-1.0.1/whatsapp_auto.egg-info/top_level.txt
```

### Comparing `whatsapp_auto-1.0/.github/workflows/python-publish.yml` & `whatsapp_auto-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `whatsapp_auto-1.0/LICENSE` & `whatsapp_auto-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp_auto-1.0/PKG-INFO` & `whatsapp_auto-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: whatsapp_auto
-Version: 1.0
-Summary: It is a Simple and Powerful WhatsApp Automation Library with many useful Features
+Version: 1.0.1
+Summary: Hides Your Ip address in https requests
 Author-email: Anish <anishshakthivelnadar@gmail.com>
-Project-URL: Homepage, https://github.com/Anish0612/whatsapp.git
-Project-URL: Bug Tracker, https://github.com/Anish0612/whatsapp.git/issues
+Project-URL: Homepage, https://github.com/Anish0612/whatsapp-auto
+Project-URL: Bug Tracker, https://github.com/Anish0612/whatsapp-auto/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whatsapp_auto-1.0/whatsapp_auto/main.py` & `whatsapp_auto-1.0.1/whatsapp_auto/main.py`

 * *Files identical despite different names*

