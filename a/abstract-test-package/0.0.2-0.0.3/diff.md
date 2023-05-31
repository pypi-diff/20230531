# Comparing `tmp/abstract_test_package-0.0.2.tar.gz` & `tmp/abstract_test_package-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_test_package-0.0.2.tar", last modified: Wed May 31 01:01:47 2023, max compression
+gzip compressed data, was "abstract_test_package-0.0.3.tar", last modified: Wed May 31 01:08:37 2023, max compression
```

## Comparing `abstract_test_package-0.0.2.tar` & `abstract_test_package-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2203 2023-05-30 02:32:36.000000 abstract_test_package-0.0.2/README.md
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-30 03:02:55.000000 abstract_test_package-0.0.2/pyproject.toml
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/setup.cfg
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1243 2023-05-31 01:01:28.000000 abstract_test_package-0.0.2/setup.py
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:01:47.164842 abstract_test_package-0.0.2/src/
-drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:01:47.168841 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/PKG-INFO
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      229 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/SOURCES.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/dependency_links.txt
--rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:01:47.000000 abstract_test_package-0.0.2/src/abstract_test_package.egg-info/top_level.txt
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2203 2023-05-30 02:32:36.000000 abstract_test_package-0.0.3/README.md
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       85 2023-05-30 03:02:55.000000 abstract_test_package-0.0.3/pyproject.toml
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)       38 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/setup.cfg
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     1071 2023-05-31 01:07:54.000000 abstract_test_package-0.0.3/setup.py
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:08:37.603542 abstract_test_package-0.0.3/src/
+drwxrwxr-x   0 hmmm      (1000) hmmm      (1000)        0 2023-05-31 01:08:37.607542 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)     2953 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/PKG-INFO
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)      229 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 hmmm      (1000) hmmm      (1000)        1 2023-05-31 01:08:37.000000 abstract_test_package-0.0.3/src/abstract_test_package.egg-info/top_level.txt
```

### Comparing `abstract_test_package-0.0.2/PKG-INFO` & `abstract_test_package-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_test_package
-Version: 0.0.2
+Version: 0.0.3
 Summary: abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.
 Home-page: https://github.com/AbstractEndeavors/abstract_test_package
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_test_package-0.0.2/README.md` & `abstract_test_package-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `abstract_test_package-0.0.2/setup.py` & `abstract_test_package-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-from setuptools import setup, find_packages
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_test_package',
-    version='0.0.2',
+    version='0.0.3',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_test_package',
-    packages=find_packages(where="src"),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
-    install_requires=[
-        # Add your project's requirements here, e.g.,
-        # 'numpy>=1.22.0',
-        # 'pandas>=1.3.0',
-    ],
-
 )
```

### Comparing `abstract_test_package-0.0.2/src/abstract_test_package.egg-info/PKG-INFO` & `abstract_test_package-0.0.3/src/abstract_test_package.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-test-package
-Version: 0.0.2
+Version: 0.0.3
 Summary: abstract_test_package is a Python package that facilitates testing with abstract scenarios. Utilizing PyTest, it offers extra utilities to streamline the creation and execution of abstract tests.
 Home-page: https://github.com/AbstractEndeavors/abstract_test_package
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

