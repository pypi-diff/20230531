# Comparing `tmp/mathtranslate-2.3.3.tar.gz` & `tmp/mathtranslate-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.3.3.tar", last modified: Mon May 29 16:27:35 2023, max compression
+gzip compressed data, was "mathtranslate-2.3.4.tar", last modified: Tue May 30 08:16:46 2023, max compression
```

## Comparing `mathtranslate-2.3.3.tar` & `mathtranslate-2.3.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-29 16:27:35.000000 mathtranslate-2.3.3/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-29 16:27:35.000000 mathtranslate-2.3.3/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:27:35.000000 mathtranslate-2.3.3/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 16:27:35.000000 mathtranslate-2.3.3/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 16:27:35.000000 mathtranslate-2.3.3/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 16:27:35.000000 mathtranslate-2.3.3/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:27:35.833403 mathtranslate-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-29 16:27:14.000000 mathtranslate-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-30 08:16:46.000000 mathtranslate-2.3.4/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-30 08:16:46.000000 mathtranslate-2.3.4/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:16:46.000000 mathtranslate-2.3.4/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 08:16:46.000000 mathtranslate-2.3.4/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 08:16:46.000000 mathtranslate-2.3.4/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 08:16:46.000000 mathtranslate-2.3.4/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:16:46.143761 mathtranslate-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-30 08:16:21.000000 mathtranslate-2.3.4/setup.py
```

### Comparing `mathtranslate-2.3.3/LICENSE` & `mathtranslate-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/PKG-INFO` & `mathtranslate-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.3.3
+Version: 2.3.4
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.3 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.4 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.3.3/README.md` & `mathtranslate-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/cache.py` & `mathtranslate-2.3.4/mathtranslate/cache.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/config.py` & `mathtranslate-2.3.4/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/encoding.py` & `mathtranslate-2.3.4/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/process_file.py` & `mathtranslate-2.3.4/mathtranslate/process_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,18 +19,19 @@
         if result is None:
             break
         begin, end = result.span()
         match = result.group(1)
         filename = os.path.join(dirname, match)
         if os.path.exists(f'{filename}.tex'):
             filename = f'{filename}.tex'
-        print('filename', filename)
+        print('merging', filename)
         assert os.path.exists(filename)
         encoding = get_file_encoding(filename)
         new_content = open(filename, encoding=encoding).read()
+        new_content = remove_tex_comments(new_content)
         content = content[:begin] + new_content + content[end:]
     print(content, file=open(path, "w", encoding='utf-8'))
 
 
 def add_bbl(tex):
     '''
     for replace \bibliography commands by the corresponding bbl file
```

### Comparing `mathtranslate-2.3.3/mathtranslate/process_latex.py` & `mathtranslate-2.3.4/mathtranslate/process_latex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/process_text.py` & `mathtranslate-2.3.4/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencent.py` & `mathtranslate-2.3.4/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.3.4/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/translate.py` & `mathtranslate-2.3.4/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/translate_arxiv.py` & `mathtranslate-2.3.4/mathtranslate/translate_arxiv.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/translate_tex.py` & `mathtranslate-2.3.4/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/upload_overleaf.py` & `mathtranslate-2.3.4/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate/utils.py` & `mathtranslate-2.3.4/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.3.4/mathtranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.3.3
+Version: 2.3.4
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.3 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.4 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.3.3/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.3.4/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.3/setup.py` & `mathtranslate-2.3.4/setup.py`

 * *Files identical despite different names*

