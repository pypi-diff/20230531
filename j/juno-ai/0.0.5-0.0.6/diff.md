# Comparing `tmp/juno-ai-0.0.5.tar.gz` & `tmp/juno-ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juno-ai-0.0.5.tar", last modified: Fri May 26 06:48:40 2023, max compression
+gzip compressed data, was "juno-ai-0.0.6.tar", last modified: Wed May 31 03:47:19 2023, max compression
```

## Comparing `juno-ai-0.0.5.tar` & `juno-ai-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-26 06:48:40.432955 juno-ai-0.0.5/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-05-26 06:48:40.432608 juno-ai-0.0.5/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1938 2023-05-26 06:36:52.000000 juno-ai-0.0.5/README.md
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-26 06:48:40.430465 juno-ai-0.0.5/juno/
--rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.5/juno/__init__.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1002 2023-05-24 08:38:40.000000 juno-ai-0.0.5/juno/agent_injection.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.5/juno/client_setup.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1916 2023-05-24 08:38:40.000000 juno-ai-0.0.5/juno/event_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     2723 2023-05-24 08:38:40.000000 juno-ai-0.0.5/juno/juno.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1984 2023-05-11 01:35:57.000000 juno-ai-0.0.5/juno/magic.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.5/juno/output_parser.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)    14035 2023-05-26 06:26:51.000000 juno-ai-0.0.5/juno/prompting_javascript.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)     4685 2023-04-26 23:26:15.000000 juno-ai-0.0.5/juno/serialize_context.py
--rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-04-26 23:26:15.000000 juno-ai-0.0.5/juno/version.py
-drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-26 06:48:40.432228 juno-ai-0.0.5/juno_ai.egg-info/
--rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-05-26 06:48:40.000000 juno-ai-0.0.5/juno_ai.egg-info/PKG-INFO
--rw-r--r--   0 alexirobbins   (501) staff       (20)      379 2023-05-26 06:48:40.000000 juno-ai-0.0.5/juno_ai.egg-info/SOURCES.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-05-26 06:48:40.000000 juno-ai-0.0.5/juno_ai.egg-info/dependency_links.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       53 2023-05-26 06:48:40.000000 juno-ai-0.0.5/juno_ai.egg-info/requires.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-05-26 06:48:40.000000 juno-ai-0.0.5/juno_ai.egg-info/top_level.txt
--rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-05-26 06:48:40.433041 juno-ai-0.0.5/setup.cfg
--rw-r--r--   0 alexirobbins   (501) staff       (20)     1248 2023-05-26 06:46:54.000000 juno-ai-0.0.5/setup.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.941022 juno-ai-0.0.6/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-05-31 03:47:19.940720 juno-ai-0.0.6/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1938 2023-05-26 07:12:21.000000 juno-ai-0.0.6/README.md
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.937719 juno-ai-0.0.6/juno/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       58 2023-04-09 05:43:26.000000 juno-ai-0.0.6/juno/__init__.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1002 2023-05-24 08:38:40.000000 juno-ai-0.0.6/juno/agent_injection.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1253 2023-04-16 22:35:57.000000 juno-ai-0.0.6/juno/client_setup.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1916 2023-05-26 07:12:21.000000 juno-ai-0.0.6/juno/event_javascript.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.938329 juno-ai-0.0.6/juno/js/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    15888 2023-05-26 06:26:51.000000 juno-ai-0.0.6/juno/js/juno.min.js
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     2723 2023-05-24 08:38:40.000000 juno-ai-0.0.6/juno/juno.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1984 2023-05-11 01:35:57.000000 juno-ai-0.0.6/juno/magic.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      873 2023-03-31 21:04:15.000000 juno-ai-0.0.6/juno/output_parser.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)    14035 2023-05-26 06:26:51.000000 juno-ai-0.0.6/juno/prompting_javascript.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     4685 2023-04-26 23:26:15.000000 juno-ai-0.0.6/juno/serialize_context.py
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      473 2023-05-26 07:12:21.000000 juno-ai-0.0.6/juno/version.py
+drwxr-xr-x   0 alexirobbins   (501) staff       (20)        0 2023-05-31 03:47:19.940336 juno-ai-0.0.6/juno_ai.egg-info/
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      648 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/PKG-INFO
+-rw-r--r--   0 alexirobbins   (501) staff       (20)      399 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        1 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       53 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/requires.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)        5 2023-05-31 03:47:19.000000 juno-ai-0.0.6/juno_ai.egg-info/top_level.txt
+-rw-r--r--   0 alexirobbins   (501) staff       (20)       38 2023-05-31 03:47:19.941100 juno-ai-0.0.6/setup.cfg
+-rw-r--r--   0 alexirobbins   (501) staff       (20)     1322 2023-05-31 03:46:36.000000 juno-ai-0.0.6/setup.py
```

### Comparing `juno-ai-0.0.5/PKG-INFO` & `juno-ai-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.5/README.md` & `juno-ai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/agent_injection.py` & `juno-ai-0.0.6/juno/agent_injection.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/client_setup.py` & `juno-ai-0.0.6/juno/client_setup.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/event_javascript.py` & `juno-ai-0.0.6/juno/event_javascript.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/juno.py` & `juno-ai-0.0.6/juno/juno.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/magic.py` & `juno-ai-0.0.6/juno/magic.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/output_parser.py` & `juno-ai-0.0.6/juno/output_parser.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/prompting_javascript.py` & `juno-ai-0.0.6/juno/prompting_javascript.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno/serialize_context.py` & `juno-ai-0.0.6/juno/serialize_context.py`

 * *Files identical despite different names*

### Comparing `juno-ai-0.0.5/juno_ai.egg-info/PKG-INFO` & `juno-ai-0.0.6/juno_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juno-ai
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/alexi/juno
 Author: juno
 Author-email: hellojunoai@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: IPython
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `juno-ai-0.0.5/setup.py` & `juno-ai-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 # exec(open(read('juno/version.py')).read())
 print('packages:', [package for package in find_packages()
                 if package.startswith('juno')])
 setup(
     name='juno-ai', 
     # version=__version__, 
-    version='0.0.5',
+    version='0.0.6',
     packages=[package for package in find_packages()
                 if package.startswith('juno')], 
+    package_data={'': ['js/juno.min.js']},
+    include_package_data=True,
     long_description='Juno AI Assistant for Jupyter Notebook',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Framework :: IPython',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Topic :: Multimedia :: Graphics',
```

