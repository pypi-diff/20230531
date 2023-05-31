# Comparing `tmp/wordlexord-0.0.1.tar.gz` & `tmp/wordlexord-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordlexord-0.0.1.tar", last modified: Tue May 30 20:56:42 2023, max compression
+gzip compressed data, was "wordlexord-0.0.2.tar", last modified: Wed May 31 08:32:04 2023, max compression
```

## Comparing `wordlexord-0.0.1.tar` & `wordlexord-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lindy     (1000) lindy     (1000)        0 2023-05-30 20:56:42.525708 wordlexord-0.0.1/
--rw-rw-r--   0 lindy     (1000) lindy     (1000)     1066 2023-04-15 20:15:55.000000 wordlexord-0.0.1/LICENSE
--rw-rw-r--   0 lindy     (1000) lindy     (1000)     2044 2023-05-30 20:56:42.525708 wordlexord-0.0.1/PKG-INFO
--rw-rw-r--   0 lindy     (1000) lindy     (1000)     1235 2023-04-18 19:57:20.000000 wordlexord-0.0.1/README.md
--rw-rw-r--   0 lindy     (1000) lindy     (1000)      665 2023-05-30 20:47:31.000000 wordlexord-0.0.1/pyproject.toml
--rw-rw-r--   0 lindy     (1000) lindy     (1000)       38 2023-05-30 20:56:42.525708 wordlexord-0.0.1/setup.cfg
--rw-rw-r--   0 lindy     (1000) lindy     (1000)      847 2023-05-30 20:55:23.000000 wordlexord-0.0.1/setup.py
-drwxrwxr-x   0 lindy     (1000) lindy     (1000)        0 2023-05-30 20:56:42.525708 wordlexord-0.0.1/word_lexord/
--rw-rw-r--   0 lindy     (1000) lindy     (1000)      395 2023-04-18 19:35:52.000000 wordlexord-0.0.1/word_lexord/__init__.py
--rw-rw-r--   0 lindy     (1000) lindy     (1000)     1188 2023-04-18 19:35:52.000000 wordlexord-0.0.1/word_lexord/__main__.py
--rw-rw-r--   0 lindy     (1000) lindy     (1000)     4825 2023-05-30 20:36:38.000000 wordlexord-0.0.1/word_lexord/base.py
--rw-rw-r--   0 lindy     (1000) lindy     (1000)      400 2023-04-18 19:35:52.000000 wordlexord-0.0.1/word_lexord/lang.py
-drwxrwxr-x   0 lindy     (1000) lindy     (1000)        0 2023-05-30 20:56:42.525708 wordlexord-0.0.1/wordlexord.egg-info/
--rw-rw-r--   0 lindy     (1000) lindy     (1000)     2044 2023-05-30 20:56:42.000000 wordlexord-0.0.1/wordlexord.egg-info/PKG-INFO
--rw-rw-r--   0 lindy     (1000) lindy     (1000)      265 2023-05-30 20:56:42.000000 wordlexord-0.0.1/wordlexord.egg-info/SOURCES.txt
--rw-rw-r--   0 lindy     (1000) lindy     (1000)        1 2023-05-30 20:56:42.000000 wordlexord-0.0.1/wordlexord.egg-info/dependency_links.txt
--rw-rw-r--   0 lindy     (1000) lindy     (1000)       12 2023-05-30 20:56:42.000000 wordlexord-0.0.1/wordlexord.egg-info/top_level.txt
+drwxrwxr-x   0 lindy     (1000) lindy     (1000)        0 2023-05-31 08:32:04.448155 wordlexord-0.0.2/
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)     1066 2023-04-15 20:15:55.000000 wordlexord-0.0.2/LICENSE
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)     4961 2023-05-31 08:32:04.448155 wordlexord-0.0.2/PKG-INFO
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)     4152 2023-05-31 08:28:35.000000 wordlexord-0.0.2/README.md
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)      665 2023-05-31 08:31:17.000000 wordlexord-0.0.2/pyproject.toml
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)       38 2023-05-31 08:32:04.448155 wordlexord-0.0.2/setup.cfg
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)      847 2023-05-31 08:31:21.000000 wordlexord-0.0.2/setup.py
+drwxrwxr-x   0 lindy     (1000) lindy     (1000)        0 2023-05-31 08:32:04.448155 wordlexord-0.0.2/word_lexord/
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)      434 2023-05-31 08:23:26.000000 wordlexord-0.0.2/word_lexord/__init__.py
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)     1188 2023-04-18 19:35:52.000000 wordlexord-0.0.2/word_lexord/__main__.py
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)     4825 2023-05-30 20:36:38.000000 wordlexord-0.0.2/word_lexord/base.py
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)      400 2023-04-18 19:35:52.000000 wordlexord-0.0.2/word_lexord/lang.py
+drwxrwxr-x   0 lindy     (1000) lindy     (1000)        0 2023-05-31 08:32:04.448155 wordlexord-0.0.2/wordlexord.egg-info/
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)     4961 2023-05-31 08:32:04.000000 wordlexord-0.0.2/wordlexord.egg-info/PKG-INFO
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)      265 2023-05-31 08:32:04.000000 wordlexord-0.0.2/wordlexord.egg-info/SOURCES.txt
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)        1 2023-05-31 08:32:04.000000 wordlexord-0.0.2/wordlexord.egg-info/dependency_links.txt
+-rw-rw-r--   0 lindy     (1000) lindy     (1000)       12 2023-05-31 08:32:04.000000 wordlexord-0.0.2/wordlexord.egg-info/top_level.txt
```

### Comparing `wordlexord-0.0.1/LICENSE` & `wordlexord-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wordlexord-0.0.1/pyproject.toml` & `wordlexord-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wordlexord"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Aleksej Kosolapov", email="kakaporuqee@gmail.com" },
 ]
 description = "This is a python package for having fun with words ordered by length and then lexicographically"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `wordlexord-0.0.1/setup.py` & `wordlexord-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='wordlexord',
-    version='0.0.1',
+    version='0.0.2',
     description='This is a python package for having fun with words ordered by length and then lexicographically',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Aleksej Kosolapov',
     author_email='kakaporuqee@gmail.com',
```

### Comparing `wordlexord-0.0.1/word_lexord/__main__.py` & `wordlexord-0.0.2/word_lexord/__main__.py`

 * *Files identical despite different names*

### Comparing `wordlexord-0.0.1/word_lexord/base.py` & `wordlexord-0.0.2/word_lexord/base.py`

 * *Files identical despite different names*

