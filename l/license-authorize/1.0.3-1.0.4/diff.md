# Comparing `tmp/license_authorize-1.0.3.tar.gz` & `tmp/license_authorize-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\license_authorize-1.0.3.tar", last modified: Wed May 31 07:25:03 2023, max compression
+gzip compressed data, was "dist\license_authorize-1.0.4.tar", last modified: Wed May 31 08:04:06 2023, max compression
```

## Comparing `license_authorize-1.0.3.tar` & `license_authorize-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:25:03.342274 license_authorize-1.0.3/
--rw-rw-rw-   0        0        0     1405 2023-05-31 07:25:03.341274 license_authorize-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-05-19 09:47:18.000000 license_authorize-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 07:25:03.332274 license_authorize-1.0.3/license_authorize/
--rw-rw-rw-   0        0        0      226 2023-05-19 06:53:07.000000 license_authorize-1.0.3/license_authorize/__init__.py
--rw-rw-rw-   0        0        0     3381 2023-05-31 07:14:43.000000 license_authorize-1.0.3/license_authorize/_core.py
--rw-rw-rw-   0        0        0      877 2023-05-19 10:12:48.000000 license_authorize-1.0.3/license_authorize/decode.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:25:03.339274 license_authorize-1.0.3/license_authorize.egg-info/
--rw-rw-rw-   0        0        0     1405 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 07:25:03.342274 license_authorize-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2236 2023-05-31 07:22:35.000000 license_authorize-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:04:06.412997 license_authorize-1.0.4/
+-rw-rw-rw-   0        0        0     1405 2023-05-31 08:04:06.411999 license_authorize-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-05-19 09:47:18.000000 license_authorize-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 08:04:06.397996 license_authorize-1.0.4/license_authorize/
+-rw-rw-rw-   0        0        0      226 2023-05-19 06:53:07.000000 license_authorize-1.0.4/license_authorize/__init__.py
+-rw-rw-rw-   0        0        0     3381 2023-05-31 07:14:43.000000 license_authorize-1.0.4/license_authorize/_core.py
+-rw-rw-rw-   0        0        0      877 2023-05-19 10:12:48.000000 license_authorize-1.0.4/license_authorize/decode.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:04:06.410997 license_authorize-1.0.4/license_authorize.egg-info/
+-rw-rw-rw-   0        0        0     1405 2023-05-31 08:04:06.000000 license_authorize-1.0.4/license_authorize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-31 08:04:06.000000 license_authorize-1.0.4/license_authorize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 08:04:06.000000 license_authorize-1.0.4/license_authorize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 08:04:06.000000 license_authorize-1.0.4/license_authorize.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-31 08:04:06.000000 license_authorize-1.0.4/license_authorize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 08:04:06.412997 license_authorize-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2236 2023-05-31 08:03:07.000000 license_authorize-1.0.4/setup.py
```

### Comparing `license_authorize-1.0.3/PKG-INFO` & `license_authorize-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license_authorize
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tools for license authorize in windows
 Home-page: https://github.com/gisfanmachel/licenseAuthorize
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this program is for lincense authorize
```

### Comparing `license_authorize-1.0.3/license_authorize/_core.py` & `license_authorize-1.0.4/license_authorize/_core.py`

 * *Files identical despite different names*

### Comparing `license_authorize-1.0.3/license_authorize/decode.py` & `license_authorize-1.0.4/license_authorize/decode.py`

 * *Files identical despite different names*

### Comparing `license_authorize-1.0.3/license_authorize.egg-info/PKG-INFO` & `license_authorize-1.0.4/license_authorize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-authorize
-Version: 1.0.3
+Version: 1.0.4
 Summary: A tools for license authorize in windows
 Home-page: https://github.com/gisfanmachel/licenseAuthorize
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this program is for lincense authorize
```

### Comparing `license_authorize-1.0.3/setup.py` & `license_authorize-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     # name="license_authorize",  # Required 项目名称
     name="license_authorize",  # Required 项目名称
-    version="1.0.3",  # Required 发布版本号
+    version="1.0.4",  # Required 发布版本号
     description="A tools for license authorize in windows",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/licenseAuthorize",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

