# Comparing `tmp/zq-config-0.1.0.tar.gz` & `tmp/zq-config-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-config-0.1.0.tar", last modified: Sun Apr 23 07:01:24 2023, max compression
+gzip compressed data, was "zq-config-0.1.1.tar", last modified: Wed May 31 09:30:32 2023, max compression
```

## Comparing `zq-config-0.1.0.tar` & `zq-config-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-04-23 07:01:24.948767 zq-config-0.1.0/
--rw-r--r--   0 test      (1000) test      (1001)     1081 2023-04-21 06:48:00.000000 zq-config-0.1.0/LICENSE.txt
--rw-r--r--   0 test      (1000) test      (1001)     2992 2023-04-23 07:01:24.948767 zq-config-0.1.0/PKG-INFO
--rw-r--r--   0 test      (1000) test      (1001)      511 2023-04-21 07:12:13.000000 zq-config-0.1.0/README.md
--rw-r--r--   0 test      (1000) test      (1001)     4115 2023-04-21 06:53:54.000000 zq-config-0.1.0/pyproject.toml
--rw-r--r--   0 test      (1000) test      (1001)       38 2023-04-23 07:01:24.948767 zq-config-0.1.0/setup.cfg
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-04-23 07:01:24.945434 zq-config-0.1.0/tests/
--rw-r--r--   0 test      (1000) test      (1001)      667 2023-04-21 08:09:21.000000 zq-config-0.1.0/tests/test_simple.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-04-23 07:01:24.945434 zq-config-0.1.0/zq_config/
--rw-r--r--   0 test      (1000) test      (1001)        0 2023-04-21 09:34:13.000000 zq-config-0.1.0/zq_config/__init__.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-04-23 07:01:24.945434 zq-config-0.1.0/zq_config/backends/
--rw-r--r--   0 test      (1000) test      (1001)      398 2023-04-21 09:39:10.000000 zq-config-0.1.0/zq_config/backends/__init__.py
--rw-r--r--   0 test      (1000) test      (1001)      200 2023-04-21 09:34:28.000000 zq-config-0.1.0/zq_config/backends/backend_registry.py
--rw-r--r--   0 test      (1000) test      (1001)      334 2023-04-21 06:10:24.000000 zq-config-0.1.0/zq_config/backends/nacos.py
--rw-r--r--   0 test      (1000) test      (1001)     1305 2023-04-21 09:42:14.000000 zq-config-0.1.0/zq_config/zq_configs.py
-drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-04-23 07:01:24.945434 zq-config-0.1.0/zq_config.egg-info/
--rw-r--r--   0 test      (1000) test      (1001)     2992 2023-04-23 07:01:24.000000 zq-config-0.1.0/zq_config.egg-info/PKG-INFO
--rw-r--r--   0 test      (1000) test      (1001)      401 2023-04-23 07:01:24.000000 zq-config-0.1.0/zq_config.egg-info/SOURCES.txt
--rw-r--r--   0 test      (1000) test      (1001)        1 2023-04-23 07:01:24.000000 zq-config-0.1.0/zq_config.egg-info/dependency_links.txt
--rw-r--r--   0 test      (1000) test      (1001)       39 2023-04-23 07:01:24.000000 zq-config-0.1.0/zq_config.egg-info/entry_points.txt
--rw-r--r--   0 test      (1000) test      (1001)       50 2023-04-23 07:01:24.000000 zq-config-0.1.0/zq_config.egg-info/requires.txt
--rw-r--r--   0 test      (1000) test      (1001)       10 2023-04-23 07:01:24.000000 zq-config-0.1.0/zq_config.egg-info/top_level.txt
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-05-31 09:30:32.323280 zq-config-0.1.1/
+-rw-r--r--   0 test      (1000) test      (1001)     1081 2023-04-21 06:48:00.000000 zq-config-0.1.1/LICENSE.txt
+-rw-r--r--   0 test      (1000) test      (1001)     2992 2023-05-31 09:30:32.323280 zq-config-0.1.1/PKG-INFO
+-rw-r--r--   0 test      (1000) test      (1001)      511 2023-04-21 07:12:13.000000 zq-config-0.1.1/README.md
+-rw-r--r--   0 test      (1000) test      (1001)     4132 2023-05-31 09:19:36.000000 zq-config-0.1.1/pyproject.toml
+-rw-r--r--   0 test      (1000) test      (1001)       38 2023-05-31 09:30:32.323280 zq-config-0.1.1/setup.cfg
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-05-31 09:30:32.316614 zq-config-0.1.1/tests/
+-rw-r--r--   0 test      (1000) test      (1001)      667 2023-04-21 08:09:21.000000 zq-config-0.1.1/tests/test_simple.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-05-31 09:30:32.316614 zq-config-0.1.1/zq_config/
+-rw-r--r--   0 test      (1000) test      (1001)        0 2023-04-21 09:34:13.000000 zq-config-0.1.1/zq_config/__init__.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-05-31 09:30:32.323280 zq-config-0.1.1/zq_config/backends/
+-rw-r--r--   0 test      (1000) test      (1001)      398 2023-04-21 09:39:10.000000 zq-config-0.1.1/zq_config/backends/__init__.py
+-rw-r--r--   0 test      (1000) test      (1001)      200 2023-04-21 09:34:28.000000 zq-config-0.1.1/zq_config/backends/backend_registry.py
+-rw-r--r--   0 test      (1000) test      (1001)      365 2023-05-31 09:27:28.000000 zq-config-0.1.1/zq_config/backends/nacos.py
+-rw-r--r--   0 test      (1000) test      (1001)     1305 2023-04-21 09:42:14.000000 zq-config-0.1.1/zq_config/zq_configs.py
+drwxr-xr-x   0 test      (1000) test      (1001)        0 2023-05-31 09:30:32.319947 zq-config-0.1.1/zq_config.egg-info/
+-rw-r--r--   0 test      (1000) test      (1001)     2992 2023-05-31 09:30:32.000000 zq-config-0.1.1/zq_config.egg-info/PKG-INFO
+-rw-r--r--   0 test      (1000) test      (1001)      401 2023-05-31 09:30:32.000000 zq-config-0.1.1/zq_config.egg-info/SOURCES.txt
+-rw-r--r--   0 test      (1000) test      (1001)        1 2023-05-31 09:30:32.000000 zq-config-0.1.1/zq_config.egg-info/dependency_links.txt
+-rw-r--r--   0 test      (1000) test      (1001)       39 2023-05-31 09:30:32.000000 zq-config-0.1.1/zq_config.egg-info/entry_points.txt
+-rw-r--r--   0 test      (1000) test      (1001)       49 2023-05-31 09:30:32.000000 zq-config-0.1.1/zq_config.egg-info/requires.txt
+-rw-r--r--   0 test      (1000) test      (1001)       10 2023-05-31 09:30:32.000000 zq-config-0.1.1/zq_config.egg-info/top_level.txt
```

### Comparing `zq-config-0.1.0/LICENSE.txt` & `zq-config-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.0/PKG-INFO` & `zq-config-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-config
-Version: 0.1.0
+Version: 0.1.1
 Summary: zq-config is wrapper for config centers such as nacos
 Author-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 Maintainer-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `zq-config-0.1.0/pyproject.toml` & `zq-config-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zq-config"
-version = "0.1.0"
+version = "0.1.1"
 description = "zq-config is wrapper for config centers such as nacos"
 readme = "README.md"
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
@@ -54,15 +54,16 @@
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
-  "peppercorn"
+  # "peppercorn",
+  "ttl-cache"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `zq-config-0.1.0/tests/test_simple.py` & `zq-config-0.1.1/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.0/zq_config/zq_configs.py` & `zq-config-0.1.1/zq_config/zq_configs.py`

 * *Files identical despite different names*

### Comparing `zq-config-0.1.0/zq_config.egg-info/PKG-INFO` & `zq-config-0.1.1/zq_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-config
-Version: 0.1.0
+Version: 0.1.1
 Summary: zq-config is wrapper for config centers such as nacos
 Author-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 Maintainer-email: Tianyue Ren <rentianyue-jk@360shuke.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

