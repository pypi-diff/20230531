# Comparing `tmp/iris_pex_embedded_python-2.3.0.tar.gz` & `tmp/iris_pex_embedded_python-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.3.0.tar", last modified: Wed May 31 14:34:51 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.3.1.tar", last modified: Wed May 31 16:24:12 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.3.0.tar` & `iris_pex_embedded_python-2.3.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.772402 iris_pex_embedded_python-2.3.0/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.0/LICENSE
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 14:34:51.771507 iris_pex_embedded_python-2.3.0/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49099 2023-05-31 14:32:55.000000 iris_pex_embedded_python-2.3.0/README.md
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.0/pyproject.toml
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-05-31 14:34:51.772743 iris_pex_embedded_python-2.3.0/setup.cfg
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2074 2023-05-31 14:34:08.000000 iris_pex_embedded_python-2.3.0/setup.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.709708 iris_pex_embedded_python-2.3.0/src/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.708904 iris_pex_embedded_python-2.3.0/src/grongier/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.718681 iris_pex_embedded_python-2.3.0/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.758587 iris_pex_embedded_python-2.3.0/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/__main__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5491 2023-05-31 11:56:27.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_cli.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     6762 2023-05-31 12:39:39.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.769143 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      878 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       43 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.201367 iris_pex_embedded_python-2.3.1/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.1/LICENSE
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 16:24:12.200313 iris_pex_embedded_python-2.3.1/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49099 2023-05-31 14:32:55.000000 iris_pex_embedded_python-2.3.1/README.md
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.1/pyproject.toml
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-05-31 16:24:12.201732 iris_pex_embedded_python-2.3.1/setup.cfg
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2295 2023-05-31 16:23:50.000000 iris_pex_embedded_python-2.3.1/setup.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.142758 iris_pex_embedded_python-2.3.1/src/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.141596 iris_pex_embedded_python-2.3.1/src/grongier/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.151296 iris_pex_embedded_python-2.3.1/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.186260 iris_pex_embedded_python-2.3.1/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/__main__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5491 2023-05-31 11:56:27.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_cli.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8057 2023-05-31 15:44:03.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.198356 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      933 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       47 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/entry_points.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       43 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.3.0/LICENSE` & `iris_pex_embedded_python-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/PKG-INFO` & `iris_pex_embedded_python-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.3.0
+Version: 2.3.1
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.3.0/README.md` & `iris_pex_embedded_python-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/setup.py` & `iris_pex_embedded_python-2.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.3.0',
+        version='2.3.1',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
@@ -49,13 +49,19 @@
         packages=['grongier.pex','grongier.iris'],
         include_package_data=True,
         python_requires='>=3.6',
         install_requires=[
             "dacite>=1.6.0",
             "xmltodict>=0.12.0",
             "irissqlcli"
-        ]
+        ],
+        entry_points={
+            'console_scripts': [
+                # create an iop command that point to the main of the grongier.pex package
+                'iop = grongier.pex._cli:main',
+            ],
+        }
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_cli.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_cli.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.3.1/src/grongier/pex/_utils.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.3.0
+Version: 2.3.1
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 src/grongier/pex/_pickle_message.py
 src/grongier/pex/_private_session_duplex.py
 src/grongier/pex/_private_session_process.py
 src/grongier/pex/_utils.py
 src/iris_pex_embedded_python.egg-info/PKG-INFO
 src/iris_pex_embedded_python.egg-info/SOURCES.txt
 src/iris_pex_embedded_python.egg-info/dependency_links.txt
+src/iris_pex_embedded_python.egg-info/entry_points.txt
 src/iris_pex_embedded_python.egg-info/requires.txt
 src/iris_pex_embedded_python.egg-info/top_level.txt
```

