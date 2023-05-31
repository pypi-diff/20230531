# Comparing `tmp/abstract_utilities_test-0.0.1.tar.gz` & `tmp/abstract_utilities_test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_utilities_test-0.0.1.tar", last modified: Wed May 31 00:15:57 2023, max compression
+gzip compressed data, was "abstract_utilities_test-0.0.2.tar", last modified: Wed May 31 00:19:08 2023, max compression
```

## Comparing `abstract_utilities_test-0.0.1.tar` & `abstract_utilities_test-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:15:57.465118 abstract_utilities_test-0.0.1/
--rw-rw-r--   0 root         (0) root         (0)     1075 2023-05-30 21:24:22.000000 abstract_utilities_test-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 00:15:57.465118 abstract_utilities_test-0.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       56 2023-05-30 21:24:22.000000 abstract_utilities_test-0.0.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       86 2023-05-30 21:24:22.000000 abstract_utilities_test-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 00:15:57.465118 abstract_utilities_test-0.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1284 2023-05-30 21:24:22.000000 abstract_utilities_test-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:15:57.461118 abstract_utilities_test-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:15:57.465118 abstract_utilities_test-0.0.1/src/abstract_utilities_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 00:15:57.000000 abstract_utilities_test-0.0.1/src/abstract_utilities_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      299 2023-05-31 00:15:57.000000 abstract_utilities_test-0.0.1/src/abstract_utilities_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 00:15:57.000000 abstract_utilities_test-0.0.1/src/abstract_utilities_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-31 00:15:57.000000 abstract_utilities_test-0.0.1/src/abstract_utilities_test.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 00:15:57.000000 abstract_utilities_test-0.0.1/src/abstract_utilities_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:19:08.786957 abstract_utilities_test-0.0.2/
+-rw-rw-r--   0 root         (0) root         (0)     1075 2023-05-30 21:24:22.000000 abstract_utilities_test-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 00:19:08.786957 abstract_utilities_test-0.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       56 2023-05-30 21:24:22.000000 abstract_utilities_test-0.0.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)       86 2023-05-30 21:24:22.000000 abstract_utilities_test-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 00:19:08.786957 abstract_utilities_test-0.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1288 2023-05-31 00:18:45.000000 abstract_utilities_test-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:19:08.782957 abstract_utilities_test-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 00:19:08.786957 abstract_utilities_test-0.0.2/src/abstract_utilities_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 00:19:08.000000 abstract_utilities_test-0.0.2/src/abstract_utilities_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      299 2023-05-31 00:19:08.000000 abstract_utilities_test-0.0.2/src/abstract_utilities_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 00:19:08.000000 abstract_utilities_test-0.0.2/src/abstract_utilities_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-31 00:19:08.000000 abstract_utilities_test-0.0.2/src/abstract_utilities_test.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 00:19:08.000000 abstract_utilities_test-0.0.2/src/abstract_utilities_test.egg-info/top_level.txt
```

### Comparing `abstract_utilities_test-0.0.1/LICENSE` & `abstract_utilities_test-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abstract_utilities_test-0.0.1/PKG-INFO` & `abstract_utilities_test-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_utilities_test
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract_utilities_test is a Python package.
 Home-page: https://github.com/AbstractEndeavors/abstract_package_test/abstract_utilities_test
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_utilities_test-0.0.1/setup.py` & `abstract_utilities_test-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='abstract_utilities_test',
-    version='0.0.1',
+    version='0.0.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_utilities_test is a Python package.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_package_test/abstract_utilities_test',
     packages=find_packages(where="src"),
@@ -28,10 +28,10 @@
     python_requires=">=3.6",
     install_requires=[
         # Add your project's requirements here, e.g.,
         # 'numpy>=1.22.0',
         # 'pandas>=1.3.0',
     ],
     entry_points={
-        'console_scripts': ["abstract_utilities_test=abstract_utilities_test.main:main"]
+        'console_scripts': ["abstract_utilities_test=abstract_utilities_test.src.main:main"]
     },
 )
```

### Comparing `abstract_utilities_test-0.0.1/src/abstract_utilities_test.egg-info/PKG-INFO` & `abstract_utilities_test-0.0.2/src/abstract_utilities_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-utilities-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract_utilities_test is a Python package.
 Home-page: https://github.com/AbstractEndeavors/abstract_package_test/abstract_utilities_test
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

