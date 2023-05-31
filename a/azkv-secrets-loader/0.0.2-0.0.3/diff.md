# Comparing `tmp/azkv-secrets-loader-0.0.2.tar.gz` & `tmp/azkv-secrets-loader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azkv-secrets-loader-0.0.2.tar", last modified: Tue May 30 21:38:56 2023, max compression
+gzip compressed data, was "azkv-secrets-loader-0.0.3.tar", last modified: Wed May 31 14:18:06 2023, max compression
```

## Comparing `azkv-secrets-loader-0.0.2.tar` & `azkv-secrets-loader-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 21:38:56.009380 azkv-secrets-loader-0.0.2/
--rw-rw-rw-   0        0        0      558 2023-05-30 21:38:56.009380 azkv-secrets-loader-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 16:51:04.000000 azkv-secrets-loader-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 21:38:56.008617 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/
--rw-rw-rw-   0        0        0      558 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 21:38:55.000000 azkv-secrets-loader-0.0.2/azkv_secrets_loader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 21:38:56.009380 azkv-secrets-loader-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-05-30 21:38:43.000000 azkv-secrets-loader-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:18:05.995729 azkv-secrets-loader-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 14:18:05.991729 azkv-secrets-loader-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:18:05.991729 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 14:18:05.000000 azkv-secrets-loader-0.0.3/azkv_secrets_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:18:05.991729 azkv-secrets-loader-0.0.3/secrets_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/secrets_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/secrets_loader/secrets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:18:05.995729 azkv-secrets-loader-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-31 14:17:50.000000 azkv-secrets-loader-0.0.3/setup.py
```

### Comparing `azkv-secrets-loader-0.0.2/setup.py` & `azkv-secrets-loader-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-VERSION = '0.0.2'
-DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
-LONG_DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
-
-# Setting up
-setup(
-    name="azkv-secrets-loader",
-    version=VERSION,
-    author="Richard",
-    author_email="<rich_swainson@hotmail.co.uk>",
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
-    install_requires=[
-        'azure-identity' ,
-        'azure-keyvault-secrets',
-        'azure-core'
-    ],
-    keywords=['azure', 'api', 'keyvault'],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+VERSION = '0.0.3'
+DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
+LONG_DESCRIPTION = 'A package for loading Azure Key Vault Secrets.'
+
+# Setting up
+setup(
+    name="azkv-secrets-loader",
+    version=VERSION,
+    author="Richard",
+    author_email="<rich_swainson@hotmail.co.uk>",
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    install_requires=[
+        'azure-identity' ,
+        'azure-keyvault-secrets',
+        'azure-core'
+    ],
+    keywords=['azure', 'api', 'keyvault'],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
 )
```

