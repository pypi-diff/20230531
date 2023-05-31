# Comparing `tmp/abstract_test_package-0.0.1.tar.gz` & `tmp/abstract_test_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_test_package-0.0.1.tar", last modified: Tue May 30 03:41:05 2023, max compression
+gzip compressed data, was "abstract_test_package-0.0.2.tar", last modified: Wed May 31 01:01:47 2023, max compression
```

## Comparing `abstract_test_package-0.0.1.tar` & `abstract_test_package-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-30 03:41:05.192396 abstract_test_package-0.0.1/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-30 03:41:05.192396 abstract_test_package-0.0.1/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2203 2023-05-30 02:32:36.000000 abstract_test_package-0.0.1/README.md
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-30 03:02:55.000000 abstract_test_package-0.0.1/pyproject.toml
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-30 03:41:05.192396 abstract_test_package-0.0.1/setup.cfg
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1241 2023-05-30 03:36:45.000000 abstract_test_package-0.0.1/setup.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-30 03:41:05.188396 abstract_test_package-0.0.1/src/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-30 03:41:05.188396 abstract_test_package-0.0.1/src/abstract_test_package.egg-info/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-30 03:41:05.000000 abstract_test_package-0.0.1/src/abstract_test_package.egg-info/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      281 2023-05-30 03:41:05.000000 abstract_test_package-0.0.1/src/abstract_test_package.egg-info/SOURCES.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-30 03:41:05.000000 abstract_test_package-0.0.1/src/abstract_test_package.egg-info/dependency_links.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       74 2023-05-30 03:41:05.000000 abstract_test_package-0.0.1/src/abstract_test_package.egg-info/entry_points.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-30 03:41:05.000000 abstract_test_package-0.0.1/src/abstract_test_package.egg-info/top_level.txt
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2203 2023-05-30 02:32:36.000000 abstract_test_package-0.0.2/README.md
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-30 03:02:55.000000 abstract_test_package-0.0.2/pyproject.toml
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/setup.cfg
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1243 2023-05-31 01:01:28.000000 abstract_test_package-0.0.2/setup.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:01:47.164842 abstract_test_package-0.0.2/src/
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      229 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/top_level.txt
```

### Comparing `abstract_test_package-0.0.1/PKG-INFO` & `abstract_test_package-0.0.2/src/abstract_test_package.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract_test_package
-Version: 0.0.1
+Name: abstract-test-package
+Version: 0.0.2
 Summary: abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.
 Home-page: https://github.com/AbstractEndeavors/abstract_test_package
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_test_package-0.0.1/README.md` & `abstract_test_package-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `abstract_test_package-0.0.1/setup.py` & `abstract_test_package-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from setuptools import setup, find_packages
-
-setup(
+from time import time
+import setuptools
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+setuptools.setup(
     name='abstract_test_package',
-    version='0.0.1',
+    version='0.0.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_test_package',
     packages=find_packages(where="src"),
@@ -21,13 +24,9 @@
     package_dir={"": "src"},
     python_requires=">=3.6",
     install_requires=[
         # Add your project's requirements here, e.g.,
         # 'numpy>=1.22.0',
         # 'pandas>=1.3.0',
     ],
-    entry_points={
-        'console_scripts': [
-            'abstract_test_package=abstract_test_package.main:main',
-        ],
-    },
+
 )
```

### Comparing `abstract_test_package-0.0.1/src/abstract_test_package.egg-info/PKG-INFO` & `abstract_test_package-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abstract-test-package
-Version: 0.0.1
+Name: abstract_test_package
+Version: 0.0.2
 Summary: abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.
 Home-page: https://github.com/AbstractEndeavors/abstract_test_package
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

