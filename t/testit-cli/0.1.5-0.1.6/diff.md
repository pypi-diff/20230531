# Comparing `tmp/testit-cli-0.1.5.tar.gz` & `tmp/testit-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-cli-0.1.5.tar", last modified: Thu May 25 13:41:30 2023, max compression
+gzip compressed data, was "testit-cli-0.1.6.tar", last modified: Wed May 31 12:34:23 2023, max compression
```

## Comparing `testit-cli-0.1.5.tar` & `testit-cli-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.878831 testit-cli-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 13:41:16.000000 testit-cli-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-25 13:41:30.878831 testit-cli-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-25 13:41:16.000000 testit-cli-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:41:30.878831 testit-cli-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 13:41:16.000000 testit-cli-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.874830 testit-cli-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.874830 testit-cli-0.1.5/src/testit_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.878831 testit-cli-0.1.5/src/testit_cli/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/models/testrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-25 13:41:16.000000 testit-cli-0.1.5/src/testit_cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:41:30.878831 testit-cli-0.1.5/src/testit_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 13:41:30.000000 testit-cli-0.1.5/src/testit_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:34:23.934960 testit-cli-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 12:34:11.000000 testit-cli-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 12:34:23.934960 testit-cli-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 12:34:11.000000 testit-cli-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:34:23.934960 testit-cli-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 12:34:11.000000 testit-cli-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:34:23.930961 testit-cli-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:34:23.934960 testit-cli-0.1.6/src/testit_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:34:23.934960 testit-cli-0.1.6/src/testit_cli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/models/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/models/testrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-31 12:34:11.000000 testit-cli-0.1.6/src/testit_cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:34:23.934960 testit-cli-0.1.6/src/testit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 12:34:23.000000 testit-cli-0.1.6/src/testit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-31 12:34:23.000000 testit-cli-0.1.6/src/testit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:34:23.000000 testit-cli-0.1.6/src/testit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 12:34:23.000000 testit-cli-0.1.6/src/testit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 12:34:23.000000 testit-cli-0.1.6/src/testit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 12:34:23.000000 testit-cli-0.1.6/src/testit_cli.egg-info/top_level.txt
```

### Comparing `testit-cli-0.1.5/LICENSE` & `testit-cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/PKG-INFO` & `testit-cli-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-cli-0.1.5/setup.py` & `testit-cli-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-cli',
-    version='0.1.5',
+    version='0.1.6',
     description='This tool is the command line wrapper of Test IT allowing you to upload the test results in real time '
                 'to Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit/',
     author='Integration team',
     author_email='integrations@testit.software',
@@ -17,14 +17,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_cli'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['testit-api-client>=3,<4', 'validators', 'tqdm'],
+    install_requires=['testit-api-client>=3.1.1,<4', 'validators', 'tqdm'],
     entry_points={
         'console_scripts': [
             'testit = testit_cli.__main__:console_main'
         ]
     }
 )
```

### Comparing `testit-cli-0.1.5/src/testit_cli/__main__.py` & `testit-cli-0.1.6/src/testit_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/apiclient.py` & `testit-cli-0.1.6/src/testit_cli/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/args_parser.py` & `testit-cli-0.1.6/src/testit_cli/args_parser.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/configurator.py` & `testit-cli-0.1.6/src/testit_cli/configurator.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/converter.py` & `testit-cli-0.1.6/src/testit_cli/converter.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/importer.py` & `testit-cli-0.1.6/src/testit_cli/importer.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/models/testcase.py` & `testit-cli-0.1.6/src/testit_cli/models/testcase.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/parser.py` & `testit-cli-0.1.6/src/testit_cli/parser.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli/service.py` & `testit-cli-0.1.6/src/testit_cli/service.py`

 * *Files identical despite different names*

### Comparing `testit-cli-0.1.5/src/testit_cli.egg-info/PKG-INFO` & `testit-cli-0.1.6/src/testit_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-cli-0.1.5/src/testit_cli.egg-info/SOURCES.txt` & `testit-cli-0.1.6/src/testit_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

