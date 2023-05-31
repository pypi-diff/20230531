# Comparing `tmp/manot-0.8.2.tar.gz` & `tmp/manot-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manot-0.8.2.tar", last modified: Wed May 31 09:05:59 2023, max compression
+gzip compressed data, was "manot-0.8.3.tar", last modified: Wed May 31 11:11:15 2023, max compression
```

## Comparing `manot-0.8.2.tar` & `manot-0.8.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 09:05:59.908314 manot-0.8.2/
--rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.2/LICENSE
--rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-05-31 09:05:59.908314 manot-0.8.2/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)     6135 2023-04-20 08:48:59.000000 manot-0.8.2/README.md
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 09:05:59.908314 manot-0.8.2/manot.egg-info/
--rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-05-31 09:05:59.000000 manot-0.8.2/manot.egg-info/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-05-31 09:05:59.000000 manot-0.8.2/manot.egg-info/SOURCES.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-05-31 09:05:59.000000 manot-0.8.2/manot.egg-info/dependency_links.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-05-31 09:05:59.000000 manot-0.8.2/manot.egg-info/requires.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-05-31 09:05:59.000000 manot-0.8.2/manot.egg-info/top_level.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-05-31 09:05:17.000000 manot-0.8.2/pyproject.toml
--rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-05-31 09:05:59.908314 manot-0.8.2/setup.cfg
--rw-rw-r--   0 armen     (1000) armen     (1000)      816 2023-05-31 08:55:53.000000 manot-0.8.2/setup.py
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 09:05:59.908314 manot-0.8.2/src/
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 09:05:59.908314 manot-0.8.2/src/manot/
--rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.2/src/manot/__init__.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.2/src/manot/logger.py
--rw-rw-r--   0 armen     (1000) armen     (1000)    12035 2023-05-31 08:26:04.000000 manot-0.8.2/src/manot/manot.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     4890 2023-04-17 14:43:30.000000 manot-0.8.2/src/manot/upload_manager.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.3/LICENSE
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-05-31 11:11:14.999904 manot-0.8.3/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)     6135 2023-05-31 09:09:00.000000 manot-0.8.3/README.md
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/manot.egg-info/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/SOURCES.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/dependency_links.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/requires.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/top_level.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-05-31 11:11:07.000000 manot-0.8.3/pyproject.toml
+-rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-05-31 11:11:14.999904 manot-0.8.3/setup.cfg
+-rw-rw-r--   0 armen     (1000) armen     (1000)      816 2023-05-31 11:11:07.000000 manot-0.8.3/setup.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/src/
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/src/manot/
+-rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.3/src/manot/__init__.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.3/src/manot/logger.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)    12035 2023-05-31 10:48:45.000000 manot-0.8.3/src/manot/manot.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     4890 2023-05-31 09:09:00.000000 manot-0.8.3/src/manot/upload_manager.py
```

### Comparing `manot-0.8.2/LICENSE` & `manot-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manot-0.8.2/PKG-INFO` & `manot-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.8.2
+Version: 0.8.3
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
```

### Comparing `manot-0.8.2/README.md` & `manot-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `manot-0.8.2/manot.egg-info/PKG-INFO` & `manot-0.8.3/manot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.8.2
+Version: 0.8.3
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
```

### Comparing `manot-0.8.2/pyproject.toml` & `manot-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "manot"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
     { name = "manot", email = "engineering@manot.ai" },
 ]
 license = {text = "MIT"}
 description = "manot AI is a model observability platform to monitor computer vision performance in real-time."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `manot-0.8.2/setup.py` & `manot-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name='manot',
-    version='0.8.2',
+    version='0.8.3',
     description='The manot SDK is a wrapper on top of our API to make it easier to work with our model performance monitoring system. Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data, classes and model. Once the project is set up you will be able to use the insight method to extract outliers that manot has detected on the new unstructured data that the performance of the model is evaluated on.',
     author='manot',
     author_email='engineering@manot.ai',
     url='https://www.manot.ai',
     packages=['manot'],
     package_dir={'manot': 'src/manot'},
     project_urls={
```

### Comparing `manot-0.8.2/src/manot/logger.py` & `manot-0.8.3/src/manot/logger.py`

 * *Files identical despite different names*

### Comparing `manot-0.8.2/src/manot/manot.py` & `manot-0.8.3/src/manot/manot.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         try:
             response = requests.post(url=url, data=json.dumps(arguments), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             log.info("Setup process is being prepared to be started.")
             progress_result = self.__check_progress(self.get_setup, response.json()["id"])
             if progress_result:
                 if progress_result['status'] == "finished":
                     log.info("Setup process has successfully finished.")
                 elif progress_result['status'] == "failure":
                     log.error(f'There is problem setup process with id {response.json()["id"]}.')
@@ -124,15 +124,15 @@
 
         try:
             response = requests.post(url=url, data=json.dumps(data), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             log.info("Insight process is being prepared to be started.")
             progress_result = self.__check_progress(self.get_insight, response.json()["id"])
             if progress_result:
                 if progress_result['status'] == "finished":
                     log.info("Insight process has successfully finished.")
                 elif progress_result['status'] == "failure":
                     log.error(f'There is problem insight process with id {response.json()["id"]}.')
@@ -165,15 +165,15 @@
         }
         try:
             response = requests.post(url=url, data=json.dumps(data), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
-        if response.status_code == 202:
+        if response.status_code == 201:
             log.info("Insight process is being prepared to be started.")
             progress_result = self.__check_progress(self.get_insight, response.json()["id"])
             if progress_result:
                 if progress_result['status'] == "finished":
                     log.info("Insight process has successfully finished.")
                 elif progress_result['status'] == "failure":
                     log.error(f'There is problem insight process with id {response.json()["id"]}.')
```

### Comparing `manot-0.8.2/src/manot/upload_manager.py` & `manot-0.8.3/src/manot/upload_manager.py`

 * *Files identical despite different names*

