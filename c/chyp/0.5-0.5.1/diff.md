# Comparing `tmp/chyp-0.5.tar.gz` & `tmp/chyp-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.5.tar", last modified: Wed May 31 16:11:52 2023, max compression
+gzip compressed data, was "chyp-0.5.1.tar", last modified: Wed May 31 16:16:07 2023, max compression
```

## Comparing `chyp-0.5.tar` & `chyp-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.5/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16186 2023-05-31 16:11:52.552710 chyp-0.5/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15651 2023-05-24 08:31:14.000000 chyp-0.5/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.5/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.5/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    17564 2023-05-31 13:33:25.000000 chyp-0.5/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.5/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2537 2023-05-22 22:22:46.000000 chyp-0.5/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4911 2023-05-22 22:22:48.000000 chyp-0.5/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.5/chyp/gui/colors.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.5/chyp/gui/completion.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4774 2023-05-22 22:23:00.000000 chyp-0.5/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11344 2023-05-31 12:57:08.000000 chyp-0.5/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-05-22 22:23:06.000000 chyp-0.5/chyp/gui/errorlist.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     8146 2023-05-31 13:34:32.000000 chyp-0.5/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1281 2023-05-29 12:07:27.000000 chyp-0.5/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3307 2023-05-24 08:35:35.000000 chyp-0.5/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    13424 2023-05-22 22:23:18.000000 chyp-0.5/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10786 2023-05-23 21:40:13.000000 chyp-0.5/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.5/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16896 2023-05-31 13:47:17.000000 chyp-0.5/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.5/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1806 2023-05-31 13:58:50.000000 chyp-0.5/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.5/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5504 2023-05-31 14:43:38.000000 chyp-0.5/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     6018 2023-05-23 23:17:32.000000 chyp-0.5/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:11:52.552710 chyp-0.5/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16186 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      630 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-31 16:11:52.000000 chyp-0.5/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.5/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-31 16:11:52.552710 chyp-0.5/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1059 2023-05-31 16:10:54.000000 chyp-0.5/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.586484 chyp-0.5.1/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.5.1/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-31 16:16:07.586484 chyp-0.5.1/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    15651 2023-05-24 08:31:14.000000 chyp-0.5.1/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.582484 chyp-0.5.1/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.5.1/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.5.1/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    17564 2023-05-31 13:33:25.000000 chyp-0.5.1/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.586484 chyp-0.5.1/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.5.1/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2537 2023-05-22 22:22:46.000000 chyp-0.5.1/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4911 2023-05-22 22:22:48.000000 chyp-0.5.1/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.5.1/chyp/gui/colors.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.5.1/chyp/gui/completion.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4774 2023-05-22 22:23:00.000000 chyp-0.5.1/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11344 2023-05-31 12:57:08.000000 chyp-0.5.1/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-05-22 22:23:06.000000 chyp-0.5.1/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     8146 2023-05-31 13:34:32.000000 chyp-0.5.1/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1281 2023-05-29 12:07:27.000000 chyp-0.5.1/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3307 2023-05-24 08:35:35.000000 chyp-0.5.1/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    13424 2023-05-22 22:23:18.000000 chyp-0.5.1/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10786 2023-05-23 21:40:13.000000 chyp-0.5.1/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.5.1/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16896 2023-05-31 13:47:17.000000 chyp-0.5.1/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.5.1/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1806 2023-05-31 13:58:50.000000 chyp-0.5.1/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.5.1/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5504 2023-05-31 14:43:38.000000 chyp-0.5.1/chyp/state.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.586484 chyp-0.5.1/chyp/tactic/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     6140 2023-05-31 14:22:39.000000 chyp-0.5.1/chyp/tactic/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1678 2023-05-31 13:45:24.000000 chyp-0.5.1/chyp/tactic/ruletac.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1551 2023-05-31 14:54:32.000000 chyp-0.5.1/chyp/tactic/simptac.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     6018 2023-05-23 23:17:32.000000 chyp-0.5.1/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-31 16:16:07.582484 chyp-0.5.1/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      700 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-31 16:16:07.000000 chyp-0.5.1/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.5.1/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-31 16:16:07.586484 chyp-0.5.1/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1076 2023-05-31 16:15:09.000000 chyp-0.5.1/setup.py
```

### Comparing `chyp-0.5/LICENSE` & `chyp-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.5/PKG-INFO` & `chyp-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.5
+Version: 0.5.1
 Summary: An interactive theorem prover for string diagrams
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.5/README.md` & `chyp-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/__init__.py` & `chyp-0.5.1/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/__main__.py` & `chyp-0.5.1/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/graph.py` & `chyp-0.5.1/chyp/graph.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/__init__.py` & `chyp-0.5.1/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/app.py` & `chyp-0.5.1/chyp/gui/app.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/codeview.py` & `chyp-0.5.1/chyp/gui/codeview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/colors.py` & `chyp-0.5.1/chyp/gui/colors.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/completion.py` & `chyp-0.5.1/chyp/gui/completion.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/document.py` & `chyp-0.5.1/chyp/gui/document.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/editor.py` & `chyp-0.5.1/chyp/gui/editor.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/errorlist.py` & `chyp-0.5.1/chyp/gui/errorlist.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/graphscene.py` & `chyp-0.5.1/chyp/gui/graphscene.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/graphview.py` & `chyp-0.5.1/chyp/gui/graphview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/highlighter.py` & `chyp-0.5.1/chyp/gui/highlighter.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/gui/mainwindow.py` & `chyp-0.5.1/chyp/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/layout.py` & `chyp-0.5.1/chyp/layout.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/matcher.py` & `chyp-0.5.1/chyp/matcher.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/parser.py` & `chyp-0.5.1/chyp/parser.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/rewrite.py` & `chyp-0.5.1/chyp/rewrite.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/rule.py` & `chyp-0.5.1/chyp/rule.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/scraps.py` & `chyp-0.5.1/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/state.py` & `chyp-0.5.1/chyp/state.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp/term.py` & `chyp-0.5.1/chyp/term.py`

 * *Files identical despite different names*

### Comparing `chyp-0.5/chyp.egg-info/PKG-INFO` & `chyp-0.5.1/chyp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.5
+Version: 0.5.1
 Summary: An interactive theorem prover for string diagrams
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.5/setup.py` & `chyp-0.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.5",
+    version="0.5.1",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for string diagrams",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
@@ -22,14 +22,14 @@
     },
     license="Apache2",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    packages=["chyp", "chyp.gui"],
+    packages=["chyp", "chyp.gui", "chyp.tactic"],
     package_data={'': ['*.svg']},
     data_files=data_files,
     install_requires=["PySide6>=6.4.3", "lark>=1.1.5", "cvxpy>=1.3.1"],
     python_requires=">=3.7",
     entry_points={'console_scripts': 'chyp=chyp.gui.app:main'},
 )
```

