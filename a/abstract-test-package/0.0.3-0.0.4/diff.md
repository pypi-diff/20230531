# Comparing `tmp/abstract_test_package-0.0.3.tar.gz` & `tmp/abstract_test_package-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_test_package-0.0.3.tar", last modified: Wed May 31 01:08:37 2023, max compression
+gzip compressed data, was "abstract_test_package-0.0.4.tar", last modified: Wed May 31 01:27:33 2023, max compression
```

## Comparing `abstract_test_package-0.0.3.tar` & `abstract_test_package-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2203 2023-05-30 02:32:36.000000 abstract_test_package-0.0.3/README.md
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-30 03:02:55.000000 abstract_test_package-0.0.3/pyproject.toml
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/setup.cfg
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1071 2023-05-31 01:07:54.000000 abstract_test_package-0.0.3/setup.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:08:37.603542 abstract_test_package-0.0.3/src/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      229 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/SOURCES.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/dependency_links.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 01:27:33.629205 abstract_test_package-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-05-31 01:27:33.629205 abstract_test_package-0.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2203 2023-05-30 02:32:36.000000 abstract_test_package-0.0.4/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-30 03:02:55.000000 abstract_test_package-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 01:27:33.629205 abstract_test_package-0.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1071 2023-05-31 01:26:46.000000 abstract_test_package-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 01:27:33.625205 abstract_test_package-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 01:27:33.629205 abstract_test_package-0.0.4/src/abstract_test_package/
+-rw-rw-r--   0 root         (0) root         (0)       56 2023-05-31 01:22:08.000000 abstract_test_package-0.0.4/src/abstract_test_package/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1297 2023-05-31 01:22:08.000000 abstract_test_package-0.0.4/src/abstract_test_package/main.py
+-rw-rw-r--   0 root         (0) root         (0)      828 2023-05-31 01:22:08.000000 abstract_test_package-0.0.4/src/abstract_test_package/test.py
+-rw-rw-r--   0 root         (0) root         (0)      903 2023-05-31 01:22:08.000000 abstract_test_package-0.0.4/src/abstract_test_package/test_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 01:27:33.629205 abstract_test_package-0.0.4/src/abstract_test_package.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     2953 2023-05-31 01:27:33.000000 abstract_test_package-0.0.4/src/abstract_test_package.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      376 2023-05-31 01:27:33.000000 abstract_test_package-0.0.4/src/abstract_test_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-31 01:27:33.000000 abstract_test_package-0.0.4/src/abstract_test_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-05-31 01:27:33.000000 abstract_test_package-0.0.4/src/abstract_test_package.egg-info/top_level.txt
```

### Comparing `abstract_test_package-0.0.3/PKG-INFO` & `abstract_test_package-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_test_package
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.
 Home-page: https://github.com/AbstractEndeavors/abstract_test_package
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_test_package-0.0.3/README.md` & `abstract_test_package-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `abstract_test_package-0.0.3/setup.py` & `abstract_test_package-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_test_package',
-    version='0.0.3',
+    version='0.0.4',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_test_package',
     classifiers=[
```

### Comparing `abstract_test_package-0.0.3/src/abstract_test_package.egg-info/PKG-INFO` & `abstract_test_package-0.0.4/src/abstract_test_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-test-package
-Version: 0.0.3
+Version: 0.0.4
 Summary: abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.
 Home-page: https://github.com/AbstractEndeavors/abstract_test_package
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

