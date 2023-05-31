# Comparing `tmp/wkt_scraper-1.0.0.tar.gz` & `tmp/wkt_scraper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wkt_scraper-1.0.0.tar", last modified: Fri Dec 13 21:44:35 2019, max compression
+gzip compressed data, was "wkt_scraper-1.0.1.tar", last modified: Wed May 31 20:12:06 2023, max compression
```

## Comparing `wkt_scraper-1.0.0.tar` & `wkt_scraper-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 fatih     (1000) fatih     (1000)        0 2019-12-13 21:44:35.000000 wkt_scraper-1.0.0/
--rw-r--r--   0 fatih     (1000) fatih     (1000)       18 2019-12-12 21:49:53.000000 wkt_scraper-1.0.0/MANIFEST.in
--rw-r--r--   0 fatih     (1000) fatih     (1000)      802 2019-12-13 21:44:35.000000 wkt_scraper-1.0.0/PKG-INFO
--rw-r--r--   0 fatih     (1000) fatih     (1000)      276 2019-12-13 21:14:54.000000 wkt_scraper-1.0.0/README.md
-drwxr-xr-x   0 fatih     (1000) fatih     (1000)        0 2019-12-13 21:44:35.000000 wkt_scraper-1.0.0/scraper/
--rw-r--r--   0 fatih     (1000) fatih     (1000)       29 2019-12-13 16:55:00.000000 wkt_scraper-1.0.0/scraper/__init__.py
--rw-r--r--   0 fatih     (1000) fatih     (1000)     8730 2019-12-13 20:55:37.000000 wkt_scraper-1.0.0/scraper/scraper.py
--rw-r--r--   0 fatih     (1000) fatih     (1000)       38 2019-12-13 21:44:35.000000 wkt_scraper-1.0.0/setup.cfg
--rw-r--r--   0 fatih     (1000) fatih     (1000)      759 2019-12-13 21:43:30.000000 wkt_scraper-1.0.0/setup.py
-drwxr-xr-x   0 fatih     (1000) fatih     (1000)        0 2019-12-13 21:44:35.000000 wkt_scraper-1.0.0/wkt_scraper.egg-info/
--rw-r--r--   0 fatih     (1000) fatih     (1000)      802 2019-12-13 21:44:34.000000 wkt_scraper-1.0.0/wkt_scraper.egg-info/PKG-INFO
--rw-r--r--   0 fatih     (1000) fatih     (1000)      243 2019-12-13 21:44:34.000000 wkt_scraper-1.0.0/wkt_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 fatih     (1000) fatih     (1000)        1 2019-12-13 21:44:34.000000 wkt_scraper-1.0.0/wkt_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 fatih     (1000) fatih     (1000)       21 2019-12-13 21:44:34.000000 wkt_scraper-1.0.0/wkt_scraper.egg-info/requires.txt
--rw-r--r--   0 fatih     (1000) fatih     (1000)        8 2019-12-13 21:44:34.000000 wkt_scraper-1.0.0/wkt_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-05-31 20:12:06.054674 wkt_scraper-1.0.1/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1068 2023-05-27 22:07:08.000000 wkt_scraper-1.0.1/LICENSE
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       18 2023-05-27 22:07:08.000000 wkt_scraper-1.0.1/MANIFEST.in
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1089 2023-05-31 20:12:06.054674 wkt_scraper-1.0.1/PKG-INFO
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      568 2023-05-31 20:06:46.000000 wkt_scraper-1.0.1/README.md
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-05-31 20:12:06.050674 wkt_scraper-1.0.1/scraper/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       29 2023-05-27 22:07:08.000000 wkt_scraper-1.0.1/scraper/__init__.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1051 2023-05-31 14:00:56.000000 wkt_scraper-1.0.1/scraper/language.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)    14094 2023-05-31 19:50:14.000000 wkt_scraper-1.0.1/scraper/scraper.py
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       38 2023-05-31 20:12:06.054674 wkt_scraper-1.0.1/setup.cfg
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      811 2023-05-31 20:09:34.000000 wkt_scraper-1.0.1/setup.py
+drwxrwxr-x   0 fatih     (1000) fatih     (1000)        0 2023-05-31 20:12:06.050674 wkt_scraper-1.0.1/wkt_scraper.egg-info/
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)     1089 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)      271 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)        1 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)       24 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/requires.txt
+-rw-rw-r--   0 fatih     (1000) fatih     (1000)        8 2023-05-31 20:12:06.000000 wkt_scraper-1.0.1/wkt_scraper.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wkt_scraper-1.0.0/PKG-INFO` & `wkt_scraper-1.0.1/wkt_scraper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
-Name: wkt_scraper
-Version: 1.0.0
-Summary: Parse word information from Wiktionary
+Name: wkt-scraper
+Version: 1.0.1
+Summary: Parse word information from Wiktionary. Currently only English and Turkish are supported.
 Home-page: https://github.com/fatih-akgul/wkt_scraper
 Author: Fatih Akgul
 Author-email: akguls@gmail.com
 License: MIT
-Description: # Wiktionary Scraper
-        Wiktionary Scraper is a basic scraper implementation to get word data from Wiktionary for a given word and language.  
-        
-        ## Installation
-        You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
-            pip install wkt_scraper
-        
 Keywords: wiktionary scraper parser
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Wiktionary Scraper
+Wiktionary Scraper is a basic scraper implementation to get word data from Wiktionary for a given word and language.  
+
+## Installation
+You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
+    
+    pip install wkt_scraper
+
+In python code, to look up the word "complicated" from English to English:
+
+    from scraper import Scraper
+    response = Scraper('en', 'en').scrape('complicated')
+
+Currently only English and Turkish are supported. 
+Supporting more languages will require additional work and testing.
```

### Comparing `wkt_scraper-1.0.0/setup.py` & `wkt_scraper-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='wkt_scraper',
-    version='1.0.0',
-    description='Parse word information from Wiktionary',
+    version='1.0.1',
+    description='Parse word information from Wiktionary. Currently only English and Turkish are supported.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='wiktionary scraper parser',
     author='Fatih Akgul',
     author_email='akguls@gmail.com',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.11',
     ],
-    packages=('scraper', ),
+    packages=['scraper', ],
     include_package_data=True,
     url='https://github.com/fatih-akgul/wkt_scraper',
-    install_requires=['bs4', 'requests', 'iso-639'],
+    install_requires=['beautifulsoup4', 'requests'],
 )
```

### Comparing `wkt_scraper-1.0.0/wkt_scraper.egg-info/PKG-INFO` & `wkt_scraper-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 Metadata-Version: 2.1
-Name: wkt-scraper
-Version: 1.0.0
-Summary: Parse word information from Wiktionary
+Name: wkt_scraper
+Version: 1.0.1
+Summary: Parse word information from Wiktionary. Currently only English and Turkish are supported.
 Home-page: https://github.com/fatih-akgul/wkt_scraper
 Author: Fatih Akgul
 Author-email: akguls@gmail.com
 License: MIT
-Description: # Wiktionary Scraper
-        Wiktionary Scraper is a basic scraper implementation to get word data from Wiktionary for a given word and language.  
-        
-        ## Installation
-        You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
-            pip install wkt_scraper
-        
 Keywords: wiktionary scraper parser
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Wiktionary Scraper
+Wiktionary Scraper is a basic scraper implementation to get word data from Wiktionary for a given word and language.  
+
+## Installation
+You can install the Wiktionary Scraper from [PyPI](https://pypi.org/project/wkt_scraper/):
+    
+    pip install wkt_scraper
+
+In python code, to look up the word "complicated" from English to English:
+
+    from scraper import Scraper
+    response = Scraper('en', 'en').scrape('complicated')
+
+Currently only English and Turkish are supported. 
+Supporting more languages will require additional work and testing.
```

