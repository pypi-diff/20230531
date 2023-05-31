# Comparing `tmp/OpaAi-0.2.1.tar.gz` & `tmp/OpaAi-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpaAi-0.2.1.tar", last modified: Wed May 31 11:29:08 2023, max compression
+gzip compressed data, was "OpaAi-1.0.tar", last modified: Wed May 31 11:18:08 2023, max compression
```

## Comparing `OpaAi-0.2.1.tar` & `OpaAi-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 11:29:08.939530 OpaAi-0.2.1/
--rw-rw-rw-   0        0        0     1090 2023-05-31 11:10:33.000000 OpaAi-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2393 2023-05-31 11:29:08.938531 OpaAi-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-05-31 09:33:16.000000 OpaAi-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 11:29:08.939530 OpaAi-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      886 2023-05-31 11:28:42.000000 OpaAi-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:29:08.910353 OpaAi-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 11:29:08.936538 OpaAi-0.2.1/src/OpaAi.egg-info/
--rw-rw-rw-   0        0        0     2393 2023-05-31 11:29:08.000000 OpaAi-0.2.1/src/OpaAi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-31 11:29:08.000000 OpaAi-0.2.1/src/OpaAi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 11:29:08.000000 OpaAi-0.2.1/src/OpaAi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 11:29:08.000000 OpaAi-0.2.1/src/OpaAi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 11:18:08.521929 OpaAi-1.0/
+-rw-rw-rw-   0        0        0     1090 2023-05-31 11:10:33.000000 OpaAi-1.0/LICENSE
+-rw-rw-rw-   0        0        0     2391 2023-05-31 11:18:08.520901 OpaAi-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-05-31 09:33:16.000000 OpaAi-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 11:18:08.521929 OpaAi-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-05-30 19:20:48.000000 OpaAi-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 11:18:08.493002 OpaAi-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 11:18:08.517850 OpaAi-1.0/src/OpaAi.egg-info/
+-rw-rw-rw-   0        0        0     2391 2023-05-31 11:18:08.000000 OpaAi-1.0/src/OpaAi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-05-31 11:18:08.000000 OpaAi-1.0/src/OpaAi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 11:18:08.000000 OpaAi-1.0/src/OpaAi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 11:18:08.000000 OpaAi-1.0/src/OpaAi.egg-info/top_level.txt
```

### Comparing `OpaAi-0.2.1/LICENSE` & `OpaAi-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpaAi-0.2.1/PKG-INFO` & `OpaAi-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpaAi
-Version: 0.2.1
+Version: 1.0
 Summary: Ai Library for developer Ahmed Al-Awadi
 Home-page: https://github.com/Ahmed-alawadi/OPsAi
 Author: AHMED AL-AWADI
 Author-email: dev.ahmed.alawadi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OpaAi Version: 0.2.1 Summary: Ai Library for
+Metadata-Version: 2.1 Name: OpaAi Version: 1.0 Summary: Ai Library for
 developer Ahmed Al-Awadi Home-page: https://github.com/Ahmed-alawadi/OPsAi
 Author: AHMED AL-AWADI Author-email: dev.ahmed.alawadi@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                               ****** OpsAi ******
                  ***** Python library for AI programs . *****
```

### Comparing `OpaAi-0.2.1/README.md` & `OpaAi-1.0/README.md`

 * *Files identical despite different names*

### Comparing `OpaAi-0.2.1/setup.py` & `OpaAi-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 f.write('requests')
 
 with open('requirements.txt', 'r') as fr:
     requires = fr.read().split('\n')
 
 setuptools.setup(
     name='OpaAi',
-    version='0.2.1',
+    version='1.0',
     author='AHMED AL-AWADI',
     author_email='dev.ahmed.alawadi@gmail.com',
     description='Ai Library for developer Ahmed Al-Awadi',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Ahmed-alawadi/OPsAi',
     classifiers=[
```

### Comparing `OpaAi-0.2.1/src/OpaAi.egg-info/PKG-INFO` & `OpaAi-1.0/src/OpaAi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpaAi
-Version: 0.2.1
+Version: 1.0
 Summary: Ai Library for developer Ahmed Al-Awadi
 Home-page: https://github.com/Ahmed-alawadi/OPsAi
 Author: AHMED AL-AWADI
 Author-email: dev.ahmed.alawadi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OpaAi Version: 0.2.1 Summary: Ai Library for
+Metadata-Version: 2.1 Name: OpaAi Version: 1.0 Summary: Ai Library for
 developer Ahmed Al-Awadi Home-page: https://github.com/Ahmed-alawadi/OPsAi
 Author: AHMED AL-AWADI Author-email: dev.ahmed.alawadi@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
                               ****** OpsAi ******
                  ***** Python library for AI programs . *****
```

