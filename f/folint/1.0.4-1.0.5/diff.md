# Comparing `tmp/folint-1.0.4.tar.gz` & `tmp/folint-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folint-1.0.4.tar", last modified: Fri May  5 05:34:37 2023, max compression
+gzip compressed data, was "folint-1.0.5.tar", last modified: Wed May 31 10:37:40 2023, max compression
```

## Comparing `folint-1.0.4.tar` & `folint-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/
--rw-r--r--   0 sva       (1000) sva       (1001)    35149 2022-12-23 19:15:30.000000 folint-1.0.4/LICENSE
--rw-r--r--   0 sva       (1000) sva       (1001)       50 2022-12-23 19:15:30.000000 folint-1.0.4/MANIFEST.in
--rw-r--r--   0 sva       (1000) sva       (1001)     2891 2023-05-05 05:34:37.443359 folint-1.0.4/PKG-INFO
--rw-r--r--   0 sva       (1000) sva       (1001)     2341 2023-04-13 06:56:56.000000 folint-1.0.4/README.md
-drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/folint/
--rw-r--r--   0 sva       (1000) sva       (1001)    10309 2023-05-05 05:21:40.000000 folint-1.0.4/folint/SCA.py
--rw-r--r--   0 sva       (1000) sva       (1001)       14 2022-12-23 19:15:30.000000 folint-1.0.4/folint/__init__.py
-drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/folint/ast_engine/
--rw-r--r--   0 sva       (1000) sva       (1001)       34 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/Annotate.py
--rw-r--r--   0 sva       (1000) sva       (1001)       36 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/Assignments.py
--rw-r--r--   0 sva       (1000) sva       (1001)    16941 2023-05-05 05:21:40.000000 folint-1.0.4/folint/ast_engine/Expression.py
--rw-r--r--   0 sva       (1000) sva       (1001)    11004 2023-04-20 07:12:10.000000 folint-1.0.4/folint/ast_engine/Parse.py
--rw-r--r--   0 sva       (1000) sva       (1001)       34 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/Simplify.py
--rw-r--r--   0 sva       (1000) sva       (1001)       82 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/__init__.py
--rw-r--r--   0 sva       (1000) sva       (1001)       30 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/utils.py
-drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/folint.egg-info/
--rw-r--r--   0 sva       (1000) sva       (1001)     2891 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/PKG-INFO
--rw-r--r--   0 sva       (1000) sva       (1001)      462 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/SOURCES.txt
--rw-r--r--   0 sva       (1000) sva       (1001)        1 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/dependency_links.txt
--rw-r--r--   0 sva       (1000) sva       (1001)       43 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/entry_points.txt
--rw-r--r--   0 sva       (1000) sva       (1001)       41 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/requires.txt
--rw-r--r--   0 sva       (1000) sva       (1001)        7 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/top_level.txt
--rw-r--r--   0 sva       (1000) sva       (1001)       38 2023-05-05 05:34:37.443359 folint-1.0.4/setup.cfg
--rw-r--r--   0 sva       (1000) sva       (1001)     1041 2023-05-05 05:33:45.000000 folint-1.0.4/setup.py
+drwxrwxr-x   0 pcarbonn  (1000) pcarbonn  (1000)        0 2023-05-31 10:37:40.655351 folint-1.0.5/
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)    35149 2023-03-05 18:02:48.000000 folint-1.0.5/LICENSE
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       50 2023-03-05 18:02:48.000000 folint-1.0.5/MANIFEST.in
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)     2928 2023-05-31 10:37:40.655351 folint-1.0.5/PKG-INFO
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)     2341 2023-04-25 09:53:04.000000 folint-1.0.5/README.md
+drwxrwxr-x   0 pcarbonn  (1000) pcarbonn  (1000)        0 2023-05-31 10:37:40.655351 folint-1.0.5/folint/
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)    10309 2023-05-02 18:57:55.000000 folint-1.0.5/folint/SCA.py
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       14 2023-03-05 18:02:48.000000 folint-1.0.5/folint/__init__.py
+drwxrwxr-x   0 pcarbonn  (1000) pcarbonn  (1000)        0 2023-05-31 10:37:40.655351 folint-1.0.5/folint/ast_engine/
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       34 2023-04-03 12:20:21.000000 folint-1.0.5/folint/ast_engine/Annotate.py
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       36 2023-04-03 12:20:21.000000 folint-1.0.5/folint/ast_engine/Assignments.py
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)    16941 2023-05-02 18:57:55.000000 folint-1.0.5/folint/ast_engine/Expression.py
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)    11004 2023-04-25 09:53:04.000000 folint-1.0.5/folint/ast_engine/Parse.py
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       34 2023-04-03 12:20:21.000000 folint-1.0.5/folint/ast_engine/Simplify.py
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       82 2023-03-05 18:02:48.000000 folint-1.0.5/folint/ast_engine/__init__.py
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       30 2023-04-03 12:20:21.000000 folint-1.0.5/folint/ast_engine/utils.py
+drwxrwxr-x   0 pcarbonn  (1000) pcarbonn  (1000)        0 2023-05-31 10:37:40.655351 folint-1.0.5/folint.egg-info/
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)     2928 2023-05-31 10:37:40.000000 folint-1.0.5/folint.egg-info/PKG-INFO
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)      462 2023-05-31 10:37:40.000000 folint-1.0.5/folint.egg-info/SOURCES.txt
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)        1 2023-05-31 10:37:40.000000 folint-1.0.5/folint.egg-info/dependency_links.txt
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       44 2023-05-31 10:37:40.000000 folint-1.0.5/folint.egg-info/entry_points.txt
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       19 2023-05-31 10:37:40.000000 folint-1.0.5/folint.egg-info/requires.txt
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)        7 2023-05-31 10:37:40.000000 folint-1.0.5/folint.egg-info/top_level.txt
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)       38 2023-05-31 10:37:40.655351 folint-1.0.5/setup.cfg
+-rw-rw-r--   0 pcarbonn  (1000) pcarbonn  (1000)     1010 2023-05-31 10:36:27.000000 folint-1.0.5/setup.py
```

### Comparing `folint-1.0.4/LICENSE` & `folint-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `folint-1.0.4/PKG-INFO` & `folint-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: folint
-Version: 1.0.4
+Version: 1.0.5
 Summary: Linter for FO-dot, used in the IDP-Z3 system
 Home-page: https://gitlab.com/EAVISE/sva/folint
 Author: vadevesi
 Author-email: s.vandevelde@kuleuven.be
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Quality Assurance
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -93,7 +95,9 @@
 * Wrong number of arguments for predicate/function
 * Wrong number of arguments for `model_check` or using unknown block names
 * Checking if types are defined in voc or struct
 * Checking totality of functions
 * Checking for duplicate entries in interpretations
 * Checking corretness of entries in interpretations
 * Other minor linting such as "no double spaces", "spaces around connectives", ...
+
+
```

### Comparing `folint-1.0.4/README.md` & `folint-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `folint-1.0.4/folint/SCA.py` & `folint-1.0.5/folint/SCA.py`

 * *Files identical despite different names*

### Comparing `folint-1.0.4/folint/ast_engine/Expression.py` & `folint-1.0.5/folint/ast_engine/Expression.py`

 * *Files identical despite different names*

### Comparing `folint-1.0.4/folint/ast_engine/Parse.py` & `folint-1.0.5/folint/ast_engine/Parse.py`

 * *Files identical despite different names*

### Comparing `folint-1.0.4/folint.egg-info/PKG-INFO` & `folint-1.0.5/folint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: folint
-Version: 1.0.4
+Version: 1.0.5
 Summary: Linter for FO-dot, used in the IDP-Z3 system
 Home-page: https://gitlab.com/EAVISE/sva/folint
 Author: vadevesi
 Author-email: s.vandevelde@kuleuven.be
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Quality Assurance
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -93,7 +95,9 @@
 * Wrong number of arguments for predicate/function
 * Wrong number of arguments for `model_check` or using unknown block names
 * Checking if types are defined in voc or struct
 * Checking totality of functions
 * Checking for duplicate entries in interpretations
 * Checking corretness of entries in interpretations
 * Other minor linting such as "no double spaces", "spaces around connectives", ...
+
+
```

### Comparing `folint-1.0.4/setup.py` & `folint-1.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="folint",
-    version="1.0.4",
+    version="1.0.5",
     description="Linter for FO-dot, used in the IDP-Z3 system",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/EAVISE/sva/folint",
     author="vadevesi",
     author_email="s.vandevelde@kuleuven.be",
     classifiers=[
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development :: Quality Assurance'
       ],
     packages=find_packages(),
-    install_requires=["textX", "z3-solver", "click", "idp_engine==0.10.2"],
+    install_requires=["idp_engine>=0.10.9"],
     entry_points={
       'console_scripts': ['folint=folint.SCA:main']
     }
 )
```

