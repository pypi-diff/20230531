# Comparing `tmp/sinyi_datateam_utils-0.1.4.tar.gz` & `tmp/sinyi_datateam_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinyi_datateam_utils-0.1.4.tar", last modified: Tue Feb 14 07:40:30 2023, max compression
+gzip compressed data, was "sinyi_datateam_utils-0.1.5.tar", last modified: Wed May 31 06:17:07 2023, max compression
```

## Comparing `sinyi_datateam_utils-0.1.4.tar` & `sinyi_datateam_utils-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-02-14 07:40:30.445531 sinyi_datateam_utils-0.1.4/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-02-14 07:40:30.445531 sinyi_datateam_utils-0.1.4/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.4/README.md
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-02-14 07:40:30.445531 sinyi_datateam_utils-0.1.4/setup.cfg
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-02-14 07:23:06.000000 sinyi_datateam_utils-0.1.4/setup.py
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-02-14 07:40:30.441531 sinyi_datateam_utils-0.1.4/sinyi_datateam_utils.egg-info/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-02-14 07:40:30.000000 sinyi_datateam_utils-0.1.4/sinyi_datateam_utils.egg-info/PKG-INFO
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-02-14 07:40:30.000000 sinyi_datateam_utils-0.1.4/sinyi_datateam_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-02-14 07:40:30.000000 sinyi_datateam_utils-0.1.4/sinyi_datateam_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-02-14 07:40:30.000000 sinyi_datateam_utils-0.1.4/sinyi_datateam_utils.egg-info/requires.txt
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-02-14 07:40:30.000000 sinyi_datateam_utils-0.1.4/sinyi_datateam_utils.egg-info/top_level.txt
-drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-02-14 07:40:30.445531 sinyi_datateam_utils-0.1.4/sinyi_utils/
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.4/sinyi_utils/__init__.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.4/sinyi_utils/db_connector.py
--rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3885 2023-02-14 03:38:42.000000 sinyi_datateam_utils-0.1.4/sinyi_utils/format_tool.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2180 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.5/README.md
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       38 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/setup.cfg
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      646 2023-05-31 06:16:49.000000 sinyi_datateam_utils-0.1.5/setup.py
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-05-31 06:17:07.512218 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2406 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)      316 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        1 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       83 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/requires.txt
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)       12 2023-05-31 06:17:07.000000 sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/top_level.txt
+drwxrwxr-x   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2023-05-31 06:17:07.516218 sinyi_datateam_utils-0.1.5/sinyi_utils/
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)        0 2022-12-06 02:44:18.000000 sinyi_datateam_utils-0.1.5/sinyi_utils/__init__.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     2634 2022-12-16 02:49:49.000000 sinyi_datateam_utils-0.1.5/sinyi_utils/db_connector.py
+-rw-rw-r--   0 Lable360PrdVMuser  (1000) Lable360PrdVMuser  (1000)     3906 2023-05-31 06:15:07.000000 sinyi_datateam_utils-0.1.5/sinyi_utils/format_tool.py
```

### Comparing `sinyi_datateam_utils-0.1.4/PKG-INFO` & `sinyi_datateam_utils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi_datateam_utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.4/README.md` & `sinyi_datateam_utils-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.4/setup.py` & `sinyi_datateam_utils-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="sinyi_datateam_utils",
-    version="0.1.4",
+    version="0.1.5",
     author="sinyidatateam",
     author_email="me30@sinyi.com.tw",
     packages=["sinyi_utils"],
     description="Utilities for data analysis",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils",
```

### Comparing `sinyi_datateam_utils-0.1.4/sinyi_datateam_utils.egg-info/PKG-INFO` & `sinyi_datateam_utils-0.1.5/sinyi_datateam_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinyi-datateam-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utilities for data analysis
 Home-page: https://SinyiDataTeam@dev.azure.com/SinyiDataTeam/Label360/_git/sinyi_utils
 Author: sinyidatateam
 Author-email: me30@sinyi.com.tw
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sinyi_datateam_utils-0.1.4/sinyi_utils/db_connector.py` & `sinyi_datateam_utils-0.1.5/sinyi_utils/db_connector.py`

 * *Files identical despite different names*

### Comparing `sinyi_datateam_utils-0.1.4/sinyi_utils/format_tool.py` & `sinyi_datateam_utils-0.1.5/sinyi_utils/format_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 credential = EnvironmentCredential()
 client = SecretClient(vault_url,credential=credential)
 
 
 def roc_era_to_ad(roc_era):
     roc_era = roc_era.replace('-',"").replace(" ","").replace('_',"")
     if roc_era: 
-        if len(roc_era) == 7 :
+        if len(roc_era) == 6 or len(roc_era) == 7 :
             year = roc_era[:-4]
             year = str(int(year)+1911)
             return year+roc_era[-4:]
         else:
             return None
 
 class AESCrypto:
```

