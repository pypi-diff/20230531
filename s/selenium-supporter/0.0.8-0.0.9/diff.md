# Comparing `tmp/selenium-supporter-0.0.8.tar.gz` & `tmp/selenium-supporter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-supporter-0.0.8.tar", last modified: Tue May 30 01:05:18 2023, max compression
+gzip compressed data, was "selenium-supporter-0.0.9.tar", last modified: Tue May 30 01:14:54 2023, max compression
```

## Comparing `selenium-supporter-0.0.8.tar` & `selenium-supporter-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 01:05:18.083646 selenium-supporter-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1939 2023-05-30 01:05:18.083646 selenium-supporter-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1675 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 01:05:18.082646 selenium-supporter-0.0.8/selenium_supporter/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9181 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter/drivers.py
--rw-r--r--   0 root         (0) root         (0)     9924 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 01:05:18.083646 selenium-supporter-0.0.8/selenium_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1939 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/selenium_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 01:05:18.083646 selenium-supporter-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-05-30 01:05:17.000000 selenium-supporter-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 01:14:54.004928 selenium-supporter-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-30 01:14:54.004928 selenium-supporter-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 01:14:54.002928 selenium-supporter-0.0.9/selenium_supporter/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9181 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter/drivers.py
+-rw-r--r--   0 root         (0) root         (0)     9924 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 01:14:54.004928 selenium-supporter-0.0.9/selenium_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/selenium_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 01:14:54.004928 selenium-supporter-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-05-30 01:14:53.000000 selenium-supporter-0.0.9/setup.py
```

### Comparing `selenium-supporter-0.0.8/PKG-INFO` & `selenium-supporter-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `selenium-supporter-0.0.8/README.md` & `selenium-supporter-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.8/selenium_supporter/drivers.py` & `selenium-supporter-0.0.9/selenium_supporter/drivers.py`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.8/selenium_supporter/utils.py` & `selenium-supporter-0.0.9/selenium_supporter/utils.py`

 * *Files identical despite different names*

### Comparing `selenium-supporter-0.0.8/selenium_supporter.egg-info/PKG-INFO` & `selenium-supporter-0.0.9/selenium_supporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-supporter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Selenium supporter
 Home-page: https://github.com/automatethem/selenium-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `selenium-supporter-0.0.8/setup.py` & `selenium-supporter-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='selenium-supporter',
-	version='0.0.8',
+	version='0.0.9',
 	description='Selenium supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/selenium-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

