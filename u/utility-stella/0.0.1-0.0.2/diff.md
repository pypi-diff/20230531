# Comparing `tmp/utility_stella-0.0.1.tar.gz` & `tmp/utility_stella-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utility_stella-0.0.1.tar", last modified: Wed May 31 15:43:53 2023, max compression
+gzip compressed data, was "utility_stella-0.0.2.tar", last modified: Wed May 31 16:37:20 2023, max compression
```

## Comparing `utility_stella-0.0.1.tar` & `utility_stella-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 15:43:53.567719 utility_stella-0.0.1/
--rw-rw-rw-   0        0        0     1077 2023-04-18 15:56:29.000000 utility_stella-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-05-31 15:43:53.565714 utility_stella-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-05-31 15:36:34.000000 utility_stella-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 15:43:53.569712 utility_stella-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1060 2023-05-31 15:30:00.000000 utility_stella-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 15:43:53.554044 utility_stella-0.0.1/utility_stella/
--rw-rw-rw-   0        0        0       56 2023-05-31 15:39:29.000000 utility_stella-0.0.1/utility_stella/__init__.py
--rw-rw-rw-   0        0        0      250 2023-05-31 15:35:29.000000 utility_stella-0.0.1/utility_stella/__main__.py
--rw-rw-rw-   0        0        0      929 2023-04-21 10:08:49.000000 utility_stella-0.0.1/utility_stella/log_config.py
-drwxrwxrwx   0        0        0        0 2023-05-31 15:43:53.563668 utility_stella-0.0.1/utility_stella.egg-info/
--rw-rw-rw-   0        0        0      946 2023-05-31 15:43:53.000000 utility_stella-0.0.1/utility_stella.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-31 15:43:53.000000 utility_stella-0.0.1/utility_stella.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 15:43:53.000000 utility_stella-0.0.1/utility_stella.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 15:43:53.000000 utility_stella-0.0.1/utility_stella.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 15:43:53.000000 utility_stella-0.0.1/utility_stella.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 16:37:20.911862 utility_stella-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 15:56:29.000000 utility_stella-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      953 2023-05-31 16:37:20.910862 utility_stella-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-05-31 15:44:31.000000 utility_stella-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 16:37:20.911862 utility_stella-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2023-05-31 16:32:11.000000 utility_stella-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:37:20.901705 utility_stella-0.0.2/utility_stella/
+-rw-rw-rw-   0        0        0       44 2023-05-31 16:28:44.000000 utility_stella-0.0.2/utility_stella/__init__.py
+-rw-rw-rw-   0        0        0      250 2023-05-31 15:35:29.000000 utility_stella-0.0.2/utility_stella/__main__.py
+-rw-rw-rw-   0        0        0      929 2023-04-21 10:08:49.000000 utility_stella-0.0.2/utility_stella/log_config.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:37:20.909908 utility_stella-0.0.2/utility_stella.egg-info/
+-rw-rw-rw-   0        0        0      953 2023-05-31 16:37:20.000000 utility_stella-0.0.2/utility_stella.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-31 16:37:20.000000 utility_stella-0.0.2/utility_stella.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 16:37:20.000000 utility_stella-0.0.2/utility_stella.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 16:37:20.000000 utility_stella-0.0.2/utility_stella.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 16:37:20.000000 utility_stella-0.0.2/utility_stella.egg-info/top_level.txt
```

### Comparing `utility_stella-0.0.1/LICENSE.txt` & `utility_stella-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `utility_stella-0.0.1/PKG-INFO` & `utility_stella-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utility_stella
-Version: 0.0.1
+Version: 0.0.2
 Summary: utility per progetto stella 
 Home-page: UNKNOWN
 Author: Jorge figueroa
 Author-email: atientas0412@gmail.com
 License: MIT
 Keywords: utility_stella
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ##https://codigofacilito.com/cursos/taller-modulos-paquetes-python
 
 ## provando un paquete
 python -m utility_stella
-python setup.py sdist
+python setup.py sdist       
 
 
 ##pip install pip --upgrade  DA ERRORE
 pip install twine
 twine upload dist/*
 https://pypi.org/account/login/
```

### Comparing `utility_stella-0.0.1/setup.py` & `utility_stella-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path  # > 3.6
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'utility per progetto stella '
 PACKAGE_NAME = 'utility_stella'
 AUTHOR = 'Jorge figueroa'
 EMAIL = 'atientas0412@gmail.com'
 #GITHUB_URL = 'https://github.com/JorgeFigueroa/codigofacilito_package'
 
 setup(
```

### Comparing `utility_stella-0.0.1/utility_stella/log_config.py` & `utility_stella-0.0.2/utility_stella/log_config.py`

 * *Files identical despite different names*

### Comparing `utility_stella-0.0.1/utility_stella.egg-info/PKG-INFO` & `utility_stella-0.0.2/utility_stella.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utility-stella
-Version: 0.0.1
+Version: 0.0.2
 Summary: utility per progetto stella 
 Home-page: UNKNOWN
 Author: Jorge figueroa
 Author-email: atientas0412@gmail.com
 License: MIT
 Keywords: utility_stella
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ##https://codigofacilito.com/cursos/taller-modulos-paquetes-python
 
 ## provando un paquete
 python -m utility_stella
-python setup.py sdist
+python setup.py sdist       
 
 
 ##pip install pip --upgrade  DA ERRORE
 pip install twine
 twine upload dist/*
 https://pypi.org/account/login/
```

