# Comparing `tmp/openi-beta-0.0.2.tar.gz` & `tmp/openi-beta-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.2.tar", last modified: Tue May 30 10:32:59 2023, max compression
+gzip compressed data, was "openi-beta-0.0.3.tar", last modified: Wed May 31 07:09:27 2023, max compression
```

## Comparing `openi-beta-0.0.2.tar` & `openi-beta-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-30 10:32:59.550487 openi-beta-0.0.2/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2636 2023-05-30 10:32:59.550201 openi-beta-0.0.2/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     2006 2023-05-30 10:27:22.000000 openi-beta-0.0.2/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-05-30 10:32:59.550570 openi-beta-0.0.2/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1090 2023-05-30 10:32:51.000000 openi-beta-0.0.2/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-30 10:32:59.547016 openi-beta-0.0.2/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-30 10:32:59.547472 openi-beta-0.0.2/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       47 2023-05-29 10:23:59.000000 openi-beta-0.0.2/src/openi/__init__.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-30 10:32:59.548060 openi-beta-0.0.2/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.2/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10676 2023-05-30 10:27:38.000000 openi-beta-0.0.2/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-30 10:32:59.549016 openi-beta-0.0.2/src/openi/modelarts/
--rw-r--r--   0 jochen10518   (501) staff       (20)       24 2023-05-30 09:14:40.000000 openi-beta-0.0.2/src/openi/modelarts/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     4555 2023-05-30 09:11:58.000000 openi-beta-0.0.2/src/openi/modelarts/helper.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     2113 2023-05-30 09:14:41.000000 openi-beta-0.0.2/src/openi/modelarts/modelarts.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-30 10:32:59.549975 openi-beta-0.0.2/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2636 2023-05-30 10:32:59.000000 openi-beta-0.0.2/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      383 2023-05-30 10:32:59.000000 openi-beta-0.0.2/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-05-30 10:32:59.000000 openi-beta-0.0.2/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       43 2023-05-30 10:32:59.000000 openi-beta-0.0.2/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-05-30 10:32:59.000000 openi-beta-0.0.2/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.167158 openi-beta-0.0.3/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2636 2023-05-31 07:09:27.167010 openi-beta-0.0.3/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2006 2023-05-30 10:27:22.000000 openi-beta-0.0.3/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-05-31 07:09:27.167200 openi-beta-0.0.3/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1043 2023-05-31 07:09:25.000000 openi-beta-0.0.3/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.163954 openi-beta-0.0.3/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.164444 openi-beta-0.0.3/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       47 2023-05-29 10:23:59.000000 openi-beta-0.0.3/src/openi/__init__.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.165249 openi-beta-0.0.3/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.3/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    10676 2023-05-30 10:27:38.000000 openi-beta-0.0.3/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.165930 openi-beta-0.0.3/src/openi/modelarts/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       24 2023-05-30 09:14:40.000000 openi-beta-0.0.3/src/openi/modelarts/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     4555 2023-05-31 07:07:02.000000 openi-beta-0.0.3/src/openi/modelarts/helper.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1669 2023-05-31 07:07:04.000000 openi-beta-0.0.3/src/openi/modelarts/modelarts.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-05-31 07:09:27.166769 openi-beta-0.0.3/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2636 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      383 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       43 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-05-31 07:09:27.000000 openi-beta-0.0.3/src/openi_beta.egg-info/top_level.txt
```

### Comparing `openi-beta-0.0.2/PKG-INFO` & `openi-beta-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.2
+Version: 0.0.3
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.0.2/README.md` & `openi-beta-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.2/setup.py` & `openi-beta-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # python setup.py sdist bdist_wheel  
-# twine upload --repository testpypi dist/*    
-#twine upload dist/*    
+# twine upload dist/*    
 
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.2',
+    version='0.0.3',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
```

### Comparing `openi-beta-0.0.2/src/openi/dataset/dataset.py` & `openi-beta-0.0.3/src/openi/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.2/src/openi/modelarts/helper.py` & `openi-beta-0.0.3/src/openi/modelarts/helper.py`

 * *Files identical despite different names*

### Comparing `openi-beta-0.0.2/src/openi/modelarts/modelarts.py` & `openi-beta-0.0.3/src/openi/modelarts/modelarts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 import emoji
 
 def env_check():
     try:
         import moxing as mox
+        print(f'{emoji.emojize(":thumbs_up:")} enviornment check pass: Modelarts enviornment checked')
+        return True
     except:
         print(f'{emoji.emojize(":cross_mark:")} enviornment check failed: 请在启智平台NPU集群上运行该代码')
+        return False
 
 def openi_dataset_to_Env(data_url, data_dir):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} pass Modelarts check')
-        from .helper import openi_dataset_to_Env
-        openi_dataset_to_Env(data_url, data_dir)
+        from .helper import openi_dataset_to_Env as func
+        func(data_url, data_dir)
 
 def openi_multidataset_to_env(multi_data_url, data_dir):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} Modelarts check')
-        from .helper import openi_dataset_to_Env
-        openi_multidataset_to_env(multi_data_url, data_dir)
+        from .helper import openi_dataset_to_Env as func
+        func(multi_data_url, data_dir)
 
 def pretrain_to_env(pretrain_url, pretrain_dir):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} Modelarts check')
-        from .helper import openi_dataset_to_Env
-        pretrain_to_env(pretrain_url, pretrain_dir)
+        from .helper import openi_dataset_to_Env as func
+        func(pretrain_url, pretrain_dir)
 
 def env_to_openi(train_dir, train_url):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} Modelarts check')
-        from .helper import openi_dataset_to_Env
-        env_to_openi(train_dir, train_url)
+        from .helper import openi_dataset_to_Env as func
+        func(train_dir, train_url)
 
 def obs_copy_file(obs_file_url, file_url):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} Modelarts check')
-        from .helper import openi_dataset_to_Env
-        obs_copy_file(obs_file_url, file_url)
+        from .helper import openi_dataset_to_Env as func
+        func(obs_file_url, file_url)
     
 def obs_copy_folder(folder_dir, obs_folder_url):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} Modelarts check')
-        from .helper import openi_dataset_to_Env
-        obs_copy_folder(folder_dir, obs_folder_url)
+        from .helper import openi_dataset_to_Env as func
+        func(folder_dir, obs_folder_url)
 
 def c2net_multidataset_to_env(multi_data_url, data_dir):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} Modelarts check')
-        from .helper import openi_dataset_to_Env
-        c2net_multidataset_to_env(multi_data_url, data_dir)
+        from .helper import openi_dataset_to_Env as func
+        func(multi_data_url, data_dir)
 
 def EnvToOpenIEpochEnd(train_dir, obs_train_url):
     if env_check():
-        print(f'{emoji.emojize(":circle_mark:")} Modelarts check')
-        from .helper import openi_dataset_to_Env
-        EnvToOpenIEpochEnd(train_dir, obs_train_url)
+        from .helper import openi_dataset_to_Env as func
+        func(train_dir, obs_train_url)
```

### Comparing `openi-beta-0.0.2/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.0.3/src/openi_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.2
+Version: 0.0.3
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

