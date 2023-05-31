# Comparing `tmp/configwizard-1.0.2.tar.gz` & `tmp/configwizard-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configwizard-1.0.2.tar", last modified: Wed May 31 02:35:06 2023, max compression
+gzip compressed data, was "configwizard-1.0.3.tar", last modified: Wed May 31 06:08:51 2023, max compression
```

## Comparing `configwizard-1.0.2.tar` & `configwizard-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 02:35:06.722111 configwizard-1.0.2/
--rw-rw-rw-   0        0        0     2240 2023-05-31 02:35:06.721112 configwizard-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1728 2023-05-31 02:34:45.000000 configwizard-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 02:35:06.720111 configwizard-1.0.2/configwizard.egg-info/
--rw-rw-rw-   0        0        0     2240 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 02:35:06.722111 configwizard-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-05-31 02:35:02.000000 configwizard-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:08:51.899325 configwizard-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-05-31 03:53:07.000000 configwizard-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2291 2023-05-31 06:08:51.898324 configwizard-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1761 2023-05-31 05:54:33.000000 configwizard-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 06:08:51.892325 configwizard-1.0.3/Wizard/
+-rw-rw-rw-   0        0        0     7817 2023-05-31 05:55:17.000000 configwizard-1.0.3/Wizard/ConfigHandler.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 04:30:13.000000 configwizard-1.0.3/Wizard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:08:51.898324 configwizard-1.0.3/configwizard.egg-info/
+-rw-rw-rw-   0        0        0     2291 2023-05-31 06:08:51.000000 configwizard-1.0.3/configwizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-31 06:08:51.000000 configwizard-1.0.3/configwizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 06:08:51.000000 configwizard-1.0.3/configwizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 06:08:51.000000 configwizard-1.0.3/configwizard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 06:08:51.000000 configwizard-1.0.3/configwizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 06:08:51.899325 configwizard-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-05-31 06:08:35.000000 configwizard-1.0.3/setup.py
```

### Comparing `configwizard-1.0.2/PKG-INFO` & `configwizard-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for handling configuration files
-Home-page: https://github.com/LapisPhoenix/Py-Config-Handler
+Home-page: https://github.com/LapisPhoenix/ConfigWizard
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11.3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # configwizard
 
 configwizard is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
 
+# [Changelog](./Changelog.md)
+
 ## Installation
 
 You can install configwizard using pip:
 
 ```bash
 pip install configwizard
 ```
```

### Comparing `configwizard-1.0.2/README.md` & `configwizard-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # configwizard
 
 configwizard is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
 
+# [Changelog](./Changelog.md)
+
 ## Installation
 
 You can install configwizard using pip:
 
 ```bash
 pip install configwizard
 ```
```

### Comparing `configwizard-1.0.2/configwizard.egg-info/PKG-INFO` & `configwizard-1.0.3/configwizard.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for handling configuration files
-Home-page: https://github.com/LapisPhoenix/Py-Config-Handler
+Home-page: https://github.com/LapisPhoenix/ConfigWizard
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11.3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # configwizard
 
 configwizard is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
 
+# [Changelog](./Changelog.md)
+
 ## Installation
 
 You can install configwizard using pip:
 
 ```bash
 pip install configwizard
 ```
```

### Comparing `configwizard-1.0.2/setup.py` & `configwizard-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("../ConfigWizard/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="configwizard",
-    version="1.0.2",
+    version="1.0.3",
     author="Lapis Pheonix",
     description="A package for handling configuration files",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/LapisPhoenix/Py-Config-Handler",
+    url="https://github.com/LapisPhoenix/ConfigWizard",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
```

