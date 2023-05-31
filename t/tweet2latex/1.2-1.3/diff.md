# Comparing `tmp/tweet2latex-1.2.tar.gz` & `tmp/tweet2latex-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweet2latex-1.2.tar", last modified: Tue Dec 21 23:15:10 2021, max compression
+gzip compressed data, was "tweet2latex-1.3.tar", last modified: Wed May 31 19:09:28 2023, max compression
```

## Comparing `tweet2latex-1.2.tar` & `tweet2latex-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 wilx      (1000) wilx      (1000)        0 2021-12-21 23:15:10.496175 tweet2latex-1.2/
--rw-rw-r--   0 wilx      (1000) wilx      (1000)     1077 2021-12-19 22:13:44.000000 tweet2latex-1.2/LICENSE
--rw-rw-r--   0 wilx      (1000) wilx      (1000)        0 2020-06-07 13:05:04.000000 tweet2latex-1.2/MANIFEST.in
--rw-rw-r--   0 wilx      (1000) wilx      (1000)     4014 2021-12-21 23:15:10.496175 tweet2latex-1.2/PKG-INFO
--rw-rw-r--   0 wilx      (1000) wilx      (1000)     3316 2021-12-21 20:39:16.000000 tweet2latex-1.2/README.md
--rw-rw-r--   0 wilx      (1000) wilx      (1000)      104 2021-12-21 20:51:11.000000 tweet2latex-1.2/pyproject.toml
--rw-rw-r--   0 wilx      (1000) wilx      (1000)       38 2021-12-21 23:15:10.496175 tweet2latex-1.2/setup.cfg
--rw-rw-r--   0 wilx      (1000) wilx      (1000)     1085 2021-12-21 23:14:03.000000 tweet2latex-1.2/setup.py
-drwxrwxr-x   0 wilx      (1000) wilx      (1000)        0 2021-12-21 23:15:10.496175 tweet2latex-1.2/tweet2latex.egg-info/
--rw-rw-r--   0 wilx      (1000) wilx      (1000)     4014 2021-12-21 23:15:10.000000 tweet2latex-1.2/tweet2latex.egg-info/PKG-INFO
--rw-rw-r--   0 wilx      (1000) wilx      (1000)      278 2021-12-21 23:15:10.000000 tweet2latex-1.2/tweet2latex.egg-info/SOURCES.txt
--rw-rw-r--   0 wilx      (1000) wilx      (1000)        1 2021-12-21 23:15:10.000000 tweet2latex-1.2/tweet2latex.egg-info/dependency_links.txt
--rw-rw-r--   0 wilx      (1000) wilx      (1000)      104 2021-12-21 20:22:07.000000 tweet2latex-1.2/tweet2latex.egg-info/pyproject.toml
--rw-rw-r--   0 wilx      (1000) wilx      (1000)       22 2021-12-21 23:15:10.000000 tweet2latex-1.2/tweet2latex.egg-info/requires.txt
--rw-rw-r--   0 wilx      (1000) wilx      (1000)        1 2021-12-21 23:15:10.000000 tweet2latex-1.2/tweet2latex.egg-info/top_level.txt
--rwxrwxr-x   0 wilx      (1000) wilx      (1000)    15191 2020-06-06 16:49:11.000000 tweet2latex-1.2/tweet2latex.py
+drwxrwxr-x   0 wilx      (1000) wilx      (1000)        0 2023-05-31 19:09:28.959057 tweet2latex-1.3/
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)     1077 2021-12-19 22:13:44.000000 tweet2latex-1.3/LICENSE
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)        0 2020-06-07 13:05:04.000000 tweet2latex-1.3/MANIFEST.in
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)     3977 2023-05-31 19:09:28.959057 tweet2latex-1.3/PKG-INFO
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)     3316 2021-12-21 20:39:16.000000 tweet2latex-1.3/README.md
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)      104 2021-12-21 20:51:11.000000 tweet2latex-1.3/pyproject.toml
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)       38 2023-05-31 19:09:28.959057 tweet2latex-1.3/setup.cfg
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)     1085 2023-05-31 18:29:01.000000 tweet2latex-1.3/setup.py
+drwxrwxr-x   0 wilx      (1000) wilx      (1000)        0 2023-05-31 19:09:28.958057 tweet2latex-1.3/tweet2latex.egg-info/
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)     3977 2023-05-31 19:09:28.000000 tweet2latex-1.3/tweet2latex.egg-info/PKG-INFO
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)      278 2023-05-31 19:09:28.000000 tweet2latex-1.3/tweet2latex.egg-info/SOURCES.txt
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)        1 2023-05-31 19:09:28.000000 tweet2latex-1.3/tweet2latex.egg-info/dependency_links.txt
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)      104 2021-12-21 20:22:07.000000 tweet2latex-1.3/tweet2latex.egg-info/pyproject.toml
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)       22 2023-05-31 19:09:28.000000 tweet2latex-1.3/tweet2latex.egg-info/requires.txt
+-rw-rw-r--   0 wilx      (1000) wilx      (1000)        1 2023-05-31 19:09:28.000000 tweet2latex-1.3/tweet2latex.egg-info/top_level.txt
+-rwxrwxr-x   0 wilx      (1000) wilx      (1000)    15191 2020-06-06 16:49:11.000000 tweet2latex-1.3/tweet2latex.py
```

### Comparing `tweet2latex-1.2/LICENSE` & `tweet2latex-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tweet2latex-1.2/PKG-INFO` & `tweet2latex-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tweet2latex
-Version: 1.2
+Version: 1.3
 Summary: Utility to retrieve tweets and format them into LaTeX fragments.
 Home-page: https://github.com/wilx/tweet2latex/
 Author: Václav Haisman
 Author-email: vhaisman+tweet2latex@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
@@ -80,9 +78,7 @@
     \sffamily%
 }{\end{tcolorbox}}
 ```
 
 The `tweet2latex.py` utility also downloads user image and linked images and
 puts them in the working directory so that resulting document can use them.
 
-
-
```

### Comparing `tweet2latex-1.2/README.md` & `tweet2latex-1.3/README.md`

 * *Files identical despite different names*

### Comparing `tweet2latex-1.2/setup.py` & `tweet2latex-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 print("packages: %s"%setuptools.find_packages("."))
 
 setuptools.setup(
     name='tweet2latex',
-    version='1.2',
+    version='1.3',
     scripts=['tweet2latex.py'],
     author="Václav Haisman",
     author_email="vhaisman+tweet2latex@gmail.com",
     description="Utility to retrieve tweets and format them into LaTeX fragments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wilx/tweet2latex/",
```

### Comparing `tweet2latex-1.2/tweet2latex.egg-info/PKG-INFO` & `tweet2latex-1.3/tweet2latex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tweet2latex
-Version: 1.2
+Version: 1.3
 Summary: Utility to retrieve tweets and format them into LaTeX fragments.
 Home-page: https://github.com/wilx/tweet2latex/
 Author: Václav Haisman
 Author-email: vhaisman+tweet2latex@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
@@ -80,9 +78,7 @@
     \sffamily%
 }{\end{tcolorbox}}
 ```
 
 The `tweet2latex.py` utility also downloads user image and linked images and
 puts them in the working directory so that resulting document can use them.
 
-
-
```

### Comparing `tweet2latex-1.2/tweet2latex.py` & `tweet2latex-1.3/tweet2latex.py`

 * *Files identical despite different names*

