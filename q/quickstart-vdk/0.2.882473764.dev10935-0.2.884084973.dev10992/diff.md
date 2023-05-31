# Comparing `tmp/quickstart-vdk-0.2.882473764.dev10935.tar.gz` & `tmp/quickstart-vdk-0.2.884084973.dev10992.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.882473764.dev10935.tar", last modified: Tue May 30 04:22:19 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.884084973.dev10992.tar", last modified: Wed May 31 04:21:45 2023, max compression
```

## Comparing `quickstart-vdk-0.2.882473764.dev10935.tar` & `quickstart-vdk-0.2.884084973.dev10992.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 04:22:19.955433 quickstart-vdk-0.2.882473764.dev10935/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-30 04:22:19.955433 quickstart-vdk-0.2.882473764.dev10935/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-30 04:19:33.000000 quickstart-vdk-0.2.882473764.dev10935/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 04:22:19.955433 quickstart-vdk-0.2.882473764.dev10935/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-30 04:22:19.000000 quickstart-vdk-0.2.882473764.dev10935/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-30 04:22:19.000000 quickstart-vdk-0.2.882473764.dev10935/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 04:22:19.000000 quickstart-vdk-0.2.882473764.dev10935/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-30 04:22:19.000000 quickstart-vdk-0.2.882473764.dev10935/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-30 04:22:19.000000 quickstart-vdk-0.2.882473764.dev10935/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 04:22:19.955433 quickstart-vdk-0.2.882473764.dev10935/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-30 04:22:10.000000 quickstart-vdk-0.2.882473764.dev10935/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 04:22:19.955433 quickstart-vdk-0.2.882473764.dev10935/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-30 04:19:33.000000 quickstart-vdk-0.2.882473764.dev10935/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:45.787757 quickstart-vdk-0.2.884084973.dev10992/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-31 04:21:45.787757 quickstart-vdk-0.2.884084973.dev10992/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-31 04:19:01.000000 quickstart-vdk-0.2.884084973.dev10992/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:45.787757 quickstart-vdk-0.2.884084973.dev10992/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-31 04:21:45.000000 quickstart-vdk-0.2.884084973.dev10992/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-31 04:21:45.000000 quickstart-vdk-0.2.884084973.dev10992/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 04:21:45.000000 quickstart-vdk-0.2.884084973.dev10992/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-31 04:21:45.000000 quickstart-vdk-0.2.884084973.dev10992/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-31 04:21:45.000000 quickstart-vdk-0.2.884084973.dev10992/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 04:21:45.787757 quickstart-vdk-0.2.884084973.dev10992/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-31 04:21:35.000000 quickstart-vdk-0.2.884084973.dev10992/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:45.787757 quickstart-vdk-0.2.884084973.dev10992/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-31 04:19:01.000000 quickstart-vdk-0.2.884084973.dev10992/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.882473764.dev10935/PKG-INFO` & `quickstart-vdk-0.2.884084973.dev10992/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.882473764.dev10935
+Version: 0.2.884084973.dev10992
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.882473764.dev10935/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.884084973.dev10992/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.882473764.dev10935
+Version: 0.2.884084973.dev10992
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.882473764.dev10935/setup.py` & `quickstart-vdk-0.2.884084973.dev10992/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.882473764.dev10935"
+__version__ = "0.2.884084973.dev10992"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

