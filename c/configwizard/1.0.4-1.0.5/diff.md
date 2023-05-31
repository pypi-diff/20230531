# Comparing `tmp/configwizard-1.0.4.tar.gz` & `tmp/configwizard-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configwizard-1.0.4.tar", last modified: Wed May 31 06:45:10 2023, max compression
+gzip compressed data, was "configwizard-1.0.5.tar", last modified: Wed May 31 06:48:24 2023, max compression
```

## Comparing `configwizard-1.0.4.tar` & `configwizard-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 06:45:10.439741 configwizard-1.0.4/
--rw-rw-rw-   0        0        0     1083 2023-05-31 03:53:07.000000 configwizard-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2345 2023-05-31 06:45:10.438774 configwizard-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1815 2023-05-31 06:43:24.000000 configwizard-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 06:45:10.432746 configwizard-1.0.4/configwizard/
--rw-rw-rw-   0        0        0     9265 2023-05-31 06:41:20.000000 configwizard-1.0.4/configwizard/ConfigHandler.py
--rw-rw-rw-   0        0        0        0 2023-05-31 04:30:13.000000 configwizard-1.0.4/configwizard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:45:10.437766 configwizard-1.0.4/configwizard.egg-info/
--rw-rw-rw-   0        0        0     2345 2023-05-31 06:45:10.000000 configwizard-1.0.4/configwizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-31 06:45:10.000000 configwizard-1.0.4/configwizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 06:45:10.000000 configwizard-1.0.4/configwizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 06:45:10.000000 configwizard-1.0.4/configwizard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-31 06:45:10.000000 configwizard-1.0.4/configwizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 06:45:10.439741 configwizard-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-05-31 06:19:19.000000 configwizard-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:48:24.965733 configwizard-1.0.5/
+-rw-rw-rw-   0        0        0     1083 2023-05-31 03:53:07.000000 configwizard-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2368 2023-05-31 06:48:24.965733 configwizard-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1838 2023-05-31 06:47:53.000000 configwizard-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 06:48:24.928285 configwizard-1.0.5/configwizard/
+-rw-rw-rw-   0        0        0     9265 2023-05-31 06:41:20.000000 configwizard-1.0.5/configwizard/ConfigHandler.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 04:30:13.000000 configwizard-1.0.5/configwizard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:48:24.964746 configwizard-1.0.5/configwizard.egg-info/
+-rw-rw-rw-   0        0        0     2368 2023-05-31 06:48:24.000000 configwizard-1.0.5/configwizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-31 06:48:24.000000 configwizard-1.0.5/configwizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 06:48:24.000000 configwizard-1.0.5/configwizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 06:48:24.000000 configwizard-1.0.5/configwizard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 06:48:24.000000 configwizard-1.0.5/configwizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 06:48:24.966732 configwizard-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-05-31 06:48:07.000000 configwizard-1.0.5/setup.py
```

### Comparing `configwizard-1.0.4/LICENSE` & `configwizard-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `configwizard-1.0.4/PKG-INFO` & `configwizard-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for handling configuration files
 Home-page: https://github.com/LapisPhoenix/ConfigWizard
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,21 +27,21 @@
 pip install configwizard
 ```
 
 ## Usage
 Here's an example of how to use configwizard:
 
 ```python
-from configwizard import Config
+from configwizard import ConfigHandler
 
 # Create a new configuration file
-config = Config('config', 'json')
+config = ConfigHandler.Config('config', 'json')
 
 # Add content to the configuration file
-config._add_content({'key': 'value'})
+config.update_content({'key': 'value'})
 
 # Get the contents of the configuration file
 contents = config.get_content()
 print(contents)  # Output: {'key': 'value'}
 
 # Update the contents of the configuration file
 config.update_content({'key2': 'value2'})
```

### Comparing `configwizard-1.0.4/README.md` & `configwizard-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 pip install configwizard
 ```
 
 ## Usage
 Here's an example of how to use configwizard:
 
 ```python
-from configwizard import Config
+from configwizard import ConfigHandler
 
 # Create a new configuration file
-config = Config('config', 'json')
+config = ConfigHandler.Config('config', 'json')
 
 # Add content to the configuration file
-config._add_content({'key': 'value'})
+config.update_content({'key': 'value'})
 
 # Get the contents of the configuration file
 contents = config.get_content()
 print(contents)  # Output: {'key': 'value'}
 
 # Update the contents of the configuration file
 config.update_content({'key2': 'value2'})
```

### Comparing `configwizard-1.0.4/configwizard/ConfigHandler.py` & `configwizard-1.0.5/configwizard/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `configwizard-1.0.4/configwizard.egg-info/PKG-INFO` & `configwizard-1.0.5/configwizard.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for handling configuration files
 Home-page: https://github.com/LapisPhoenix/ConfigWizard
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,21 +27,21 @@
 pip install configwizard
 ```
 
 ## Usage
 Here's an example of how to use configwizard:
 
 ```python
-from configwizard import Config
+from configwizard import ConfigHandler
 
 # Create a new configuration file
-config = Config('config', 'json')
+config = ConfigHandler.Config('config', 'json')
 
 # Add content to the configuration file
-config._add_content({'key': 'value'})
+config.update_content({'key': 'value'})
 
 # Get the contents of the configuration file
 contents = config.get_content()
 print(contents)  # Output: {'key': 'value'}
 
 # Update the contents of the configuration file
 config.update_content({'key2': 'value2'})
```

### Comparing `configwizard-1.0.4/setup.py` & `configwizard-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("../ConfigWizard/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="configwizard",
-    version="1.0.4",
+    version="1.0.5",
     author="Lapis Pheonix",
     description="A package for handling configuration files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LapisPhoenix/ConfigWizard",
     packages=find_packages(),
     classifiers=[
```

