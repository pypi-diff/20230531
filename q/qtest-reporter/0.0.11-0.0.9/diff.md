# Comparing `tmp/qtest_reporter-0.0.11.tar.gz` & `tmp/qtest_reporter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtest_reporter-0.0.11.tar", last modified: Wed May 31 08:47:38 2023, max compression
+gzip compressed data, was "qtest_reporter-0.0.9.tar", last modified: Mon May 22 10:57:32 2023, max compression
```

## Comparing `qtest_reporter-0.0.11.tar` & `qtest_reporter-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-31 08:47:38.916418 qtest_reporter-0.0.11/
--rw-r--r--   0 vzyhmund   (501) staff       (20)    35148 2023-05-04 16:40:04.000000 qtest_reporter-0.0.11/LICENSE
--rw-r--r--   0 vzyhmund   (501) staff       (20)      811 2023-05-31 08:47:38.916255 qtest_reporter-0.0.11/PKG-INFO
--rw-r--r--   0 vzyhmund   (501) staff       (20)      148 2023-05-08 08:28:42.000000 qtest_reporter-0.0.11/README.md
--rw-r--r--   0 vzyhmund   (501) staff       (20)      758 2023-05-31 08:47:12.000000 qtest_reporter-0.0.11/pyproject.toml
--rw-r--r--   0 vzyhmund   (501) staff       (20)       38 2023-05-31 08:47:38.916471 qtest_reporter-0.0.11/setup.cfg
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-31 08:47:38.909917 qtest_reporter-0.0.11/src/
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-31 08:47:38.912127 qtest_reporter-0.0.11/src/qtest_reporter/
--rw-r--r--   0 vzyhmund   (501) staff       (20)       98 2023-05-31 08:47:19.000000 qtest_reporter-0.0.11/src/qtest_reporter/__init__.py
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-31 08:47:38.915912 qtest_reporter-0.0.11/src/qtest_reporter/api/
--rw-r--r--   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:24:57.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/__init__.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     1668 2023-05-08 12:28:27.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/login.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     3162 2023-05-08 12:28:35.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/project.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    12284 2023-05-08 12:28:40.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/test_case.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    11564 2023-05-08 12:28:52.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/test_cycle.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     9787 2023-05-26 11:55:24.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/test_log.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    12856 2023-05-08 12:29:32.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/test_run.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)    11672 2023-05-19 17:35:39.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/test_suite.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)     1489 2023-05-08 12:29:56.000000 qtest_reporter-0.0.11/src/qtest_reporter/api/user_profile.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      337 2023-05-04 16:26:28.000000 qtest_reporter-0.0.11/src/qtest_reporter/logger.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      376 2023-05-18 11:56:17.000000 qtest_reporter-0.0.11/src/qtest_reporter/qtest.py
--rw-r--r--   0 vzyhmund   (501) staff       (20)      421 2023-04-25 12:22:26.000000 qtest_reporter-0.0.11/src/qtest_reporter/requester.py
-drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-31 08:47:38.913104 qtest_reporter-0.0.11/src/qtest_reporter.egg-info/
--rw-r--r--   0 vzyhmund   (501) staff       (20)      811 2023-05-31 08:47:38.000000 qtest_reporter-0.0.11/src/qtest_reporter.egg-info/PKG-INFO
--rw-r--r--   0 vzyhmund   (501) staff       (20)      681 2023-05-31 08:47:38.000000 qtest_reporter-0.0.11/src/qtest_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 vzyhmund   (501) staff       (20)        1 2023-05-31 08:47:38.000000 qtest_reporter-0.0.11/src/qtest_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 vzyhmund   (501) staff       (20)       17 2023-05-31 08:47:38.000000 qtest_reporter-0.0.11/src/qtest_reporter.egg-info/requires.txt
--rw-r--r--   0 vzyhmund   (501) staff       (20)       15 2023-05-31 08:47:38.000000 qtest_reporter-0.0.11/src/qtest_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-22 10:57:32.538002 qtest_reporter-0.0.9/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    35148 2023-05-04 16:40:04.000000 qtest_reporter-0.0.9/LICENSE
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-22 10:57:32.537849 qtest_reporter-0.0.9/PKG-INFO
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      148 2023-05-08 08:28:42.000000 qtest_reporter-0.0.9/README.md
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      757 2023-05-22 10:56:20.000000 qtest_reporter-0.0.9/pyproject.toml
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       38 2023-05-22 10:57:32.538068 qtest_reporter-0.0.9/setup.cfg
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-22 10:57:32.530089 qtest_reporter-0.0.9/src/
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-22 10:57:32.533008 qtest_reporter-0.0.9/src/qtest_reporter/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       97 2023-05-22 10:56:33.000000 qtest_reporter-0.0.9/src/qtest_reporter/__init__.py
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-22 10:57:32.537471 qtest_reporter-0.0.9/src/qtest_reporter/api/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)        0 2023-05-08 12:24:57.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/__init__.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     1668 2023-05-08 12:28:27.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/login.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     3162 2023-05-08 12:28:35.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/project.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    12284 2023-05-08 12:28:40.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/test_case.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    11564 2023-05-08 12:28:52.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/test_cycle.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     9787 2023-05-08 12:29:06.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/test_log.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    12856 2023-05-08 12:29:32.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/test_run.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)    11672 2023-05-19 17:35:39.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/test_suite.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)     1489 2023-05-08 12:29:56.000000 qtest_reporter-0.0.9/src/qtest_reporter/api/user_profile.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      337 2023-05-04 16:26:28.000000 qtest_reporter-0.0.9/src/qtest_reporter/logger.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      376 2023-05-18 11:56:17.000000 qtest_reporter-0.0.9/src/qtest_reporter/qtest.py
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      421 2023-04-25 12:22:26.000000 qtest_reporter-0.0.9/src/qtest_reporter/requester.py
+drwxr-xr-x   0 vzyhmund   (501) staff       (20)        0 2023-05-22 10:57:32.534364 qtest_reporter-0.0.9/src/qtest_reporter.egg-info/
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      810 2023-05-22 10:57:32.000000 qtest_reporter-0.0.9/src/qtest_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 vzyhmund   (501) staff       (20)      681 2023-05-22 10:57:32.000000 qtest_reporter-0.0.9/src/qtest_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)        1 2023-05-22 10:57:32.000000 qtest_reporter-0.0.9/src/qtest_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       17 2023-05-22 10:57:32.000000 qtest_reporter-0.0.9/src/qtest_reporter.egg-info/requires.txt
+-rw-r--r--   0 vzyhmund   (501) staff       (20)       15 2023-05-22 10:57:32.000000 qtest_reporter-0.0.9/src/qtest_reporter.egg-info/top_level.txt
```

### Comparing `qtest_reporter-0.0.11/LICENSE` & `qtest_reporter-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/PKG-INFO` & `qtest_reporter-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtest_reporter
-Version: 0.0.11
+Version: 0.0.9
 Summary: qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool.
 Author-email: Volodymyr Zyhmund <volodymyr.romanovych@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `qtest_reporter-0.0.11/pyproject.toml` & `qtest_reporter-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qtest_reporter"
-version = "0.0.11"
+version = "0.0.9"
 authors = [
   { name="Volodymyr Zyhmund", email="volodymyr.romanovych@gmail.com" },
 ]
 description = "qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -17,9 +17,9 @@
     "License :: Freeware",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
     "Natural Language :: English",
     "Topic :: Software Development :: Testing",
 ]
 dependencies = [
-    "requests>=2.31.0"
+    "requests==2.29.0"
 ]
```

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/login.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/login.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/project.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/project.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/test_case.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/test_case.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/test_cycle.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/test_cycle.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/test_log.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             self,
             projectId: int,  # ID of the project
             testRunId: int,  # ID of the Test Run
             status: str,     # Status, as in qTest project's Field Settings, of test log. 601 => Passed, 602 => Failed, 603 => Skipped
             note: str = None # Execution note included with the test log
             ):
         """To submit test result of a manual Test Run"""
-        status_id = 601 if status == "passed" else 602 if status == "failed" else 603 if status == "skipped" else 603
+        status_id = 601 if status == "Passed" else 602 if status == "Failed" else 603 if status == "Skipped" else 603
         parentSuiteId = Test_Run(self).get_test_run_by_id(projectId=projectId, testRunId=testRunId)['resopnse']['parentId']
         test_runs = Test_Run(self).get_test_runs(projectId=projectId, parentSuiteId=parentSuiteId)['resopnse']['items']
 
         for test_run in test_runs:
             if test_run['id'] == testRunId: testCaseId = test_run['testCaseId']
             for _ in test_run['properties']:
                 if test_run['id'] == testRunId: test_run_name = test_run['name']
```

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/test_run.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/test_run.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/test_suite.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/test_suite.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter/api/user_profile.py` & `qtest_reporter-0.0.9/src/qtest_reporter/api/user_profile.py`

 * *Files identical despite different names*

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter.egg-info/PKG-INFO` & `qtest_reporter-0.0.9/src/qtest_reporter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtest-reporter
-Version: 0.0.11
+Version: 0.0.9
 Summary: qtest_reporter is a tool that allows you to easily report the results of your automated testing to qTest test management tool.
 Author-email: Volodymyr Zyhmund <volodymyr.romanovych@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `qtest_reporter-0.0.11/src/qtest_reporter.egg-info/SOURCES.txt` & `qtest_reporter-0.0.9/src/qtest_reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

