# Comparing `tmp/configwizard-1.0.1.tar.gz` & `tmp/configwizard-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configwizard-1.0.1.tar", last modified: Wed May 31 02:26:37 2023, max compression
+gzip compressed data, was "configwizard-1.0.2.tar", last modified: Wed May 31 02:35:06 2023, max compression
```

## Comparing `configwizard-1.0.1.tar` & `configwizard-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 02:26:37.397322 configwizard-1.0.1/
--rw-rw-rw-   0        0        0     2261 2023-05-31 02:26:37.396322 configwizard-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1749 2023-05-31 02:08:00.000000 configwizard-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 02:26:37.395322 configwizard-1.0.1/configwizard.egg-info/
--rw-rw-rw-   0        0        0     2261 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 02:26:37.397322 configwizard-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-05-31 02:25:54.000000 configwizard-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:35:06.722111 configwizard-1.0.2/
+-rw-rw-rw-   0        0        0     2240 2023-05-31 02:35:06.721112 configwizard-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1728 2023-05-31 02:34:45.000000 configwizard-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 02:35:06.720111 configwizard-1.0.2/configwizard.egg-info/
+-rw-rw-rw-   0        0        0     2240 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 02:35:06.000000 configwizard-1.0.2/configwizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 02:35:06.722111 configwizard-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-05-31 02:35:02.000000 configwizard-1.0.2/setup.py
```

### Comparing `configwizard-1.0.1/PKG-INFO` & `configwizard-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for handling configuration files
 Home-page: https://github.com/LapisPhoenix/Py-Config-Handler
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11.3
 Description-Content-Type: text/markdown
 
-# pyconfighandler
+# configwizard
 
-pyconfighandler is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
+configwizard is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
 
 ## Installation
 
-You can install pyconfighandler using pip:
+You can install configwizard using pip:
 
 ```bash
-pip install pyconfighandler
+pip install configwizard
 ```
 
 ## Usage
-Here's an example of how to use pyconfighandler:
+Here's an example of how to use configwizard:
 
 ```python
-from pyconfighandler import Config
+from configwizard import Config
 
 # Create a new configuration file
 config = Config('config', 'json')
 
 # Add content to the configuration file
 config.add_content({'key': 'value'})
 
@@ -51,15 +51,15 @@
 config.destroy_config()
 ```
 
 In the example above, we create a Config instance with a file name of 'config' and a file type of 'json'. We then add content to the configuration file using the add_content method and retrieve the contents using the get_content method. We update the contents with new values using the update_content method and finally destroy the configuration file with the destroy_config method.
 
 ## Supported File Types
 
-pyconfighandler supports the following file types for configuration files:
+configwizard supports the following file types for configuration files:
 
 - JSON (.json)
 - TOML (.toml)
 
 When creating a Config instance, make sure to provide the appropriate file type.
 
 ## License
```

### Comparing `configwizard-1.0.1/README.md` & `configwizard-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# pyconfighandler
+# configwizard
 
-pyconfighandler is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
+configwizard is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
 
 ## Installation
 
-You can install pyconfighandler using pip:
+You can install configwizard using pip:
 
 ```bash
-pip install pyconfighandler
+pip install configwizard
 ```
 
 ## Usage
-Here's an example of how to use pyconfighandler:
+Here's an example of how to use configwizard:
 
 ```python
-from pyconfighandler import Config
+from configwizard import Config
 
 # Create a new configuration file
 config = Config('config', 'json')
 
 # Add content to the configuration file
 config.add_content({'key': 'value'})
 
@@ -37,15 +37,15 @@
 config.destroy_config()
 ```
 
 In the example above, we create a Config instance with a file name of 'config' and a file type of 'json'. We then add content to the configuration file using the add_content method and retrieve the contents using the get_content method. We update the contents with new values using the update_content method and finally destroy the configuration file with the destroy_config method.
 
 ## Supported File Types
 
-pyconfighandler supports the following file types for configuration files:
+configwizard supports the following file types for configuration files:
 
 - JSON (.json)
 - TOML (.toml)
 
 When creating a Config instance, make sure to provide the appropriate file type.
 
 ## License
```

### Comparing `configwizard-1.0.1/configwizard.egg-info/PKG-INFO` & `configwizard-1.0.2/configwizard.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for handling configuration files
 Home-page: https://github.com/LapisPhoenix/Py-Config-Handler
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11.3
 Description-Content-Type: text/markdown
 
-# pyconfighandler
+# configwizard
 
-pyconfighandler is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
+configwizard is a Python package for handling configuration files. It provides a `Config` class that allows you to easily create, read, update, and delete configuration files in different formats such as JSON and TOML.
 
 ## Installation
 
-You can install pyconfighandler using pip:
+You can install configwizard using pip:
 
 ```bash
-pip install pyconfighandler
+pip install configwizard
 ```
 
 ## Usage
-Here's an example of how to use pyconfighandler:
+Here's an example of how to use configwizard:
 
 ```python
-from pyconfighandler import Config
+from configwizard import Config
 
 # Create a new configuration file
 config = Config('config', 'json')
 
 # Add content to the configuration file
 config.add_content({'key': 'value'})
 
@@ -51,15 +51,15 @@
 config.destroy_config()
 ```
 
 In the example above, we create a Config instance with a file name of 'config' and a file type of 'json'. We then add content to the configuration file using the add_content method and retrieve the contents using the get_content method. We update the contents with new values using the update_content method and finally destroy the configuration file with the destroy_config method.
 
 ## Supported File Types
 
-pyconfighandler supports the following file types for configuration files:
+configwizard supports the following file types for configuration files:
 
 - JSON (.json)
 - TOML (.toml)
 
 When creating a Config instance, make sure to provide the appropriate file type.
 
 ## License
```

### Comparing `configwizard-1.0.1/setup.py` & `configwizard-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="configwizard",
-    version="1.0.1",
+    version="1.0.2",
     author="Lapis Pheonix",
     description="A package for handling configuration files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LapisPhoenix/Py-Config-Handler",
     packages=find_packages(),
     classifiers=[
```

