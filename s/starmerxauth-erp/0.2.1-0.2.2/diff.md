# Comparing `tmp/starmerxauth_erp-0.2.1.tar.gz` & `tmp/starmerxauth_erp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/yf/pippackage/starmerxauth_erp/dist/tmpnlvthybt/starmerxauth_erp-0.2.1.tar", last modified: Wed Jun 15 06:01:51 2022, max compression
+gzip compressed data, was "/home/yf/pippackage/starmerxauth_erp/dist/tmp7nwgiutn/starmerxauth_erp-0.2.2.tar", last modified: Wed May 31 07:37:33 2023, max compression
```

## Comparing `starmerxauth_erp-0.2.1.tar` & `starmerxauth_erp-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/
--rw-rw-r--   0 yf        (1000) yf        (1000)     1053 2022-04-08 06:58:25.000000 starmerxauth_erp-0.2.1/LICENSE
--rw-rw-r--   0 yf        (1000) yf        (1000)      436 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/PKG-INFO
--rw-rw-rw-   0 yf        (1000) yf        (1000)       28 2022-04-28 03:03:21.000000 starmerxauth_erp-0.2.1/README.md
--rw-rw-r--   0 yf        (1000) yf        (1000)       85 2022-04-08 06:37:48.000000 starmerxauth_erp-0.2.1/pyproject.toml
--rw-rw-r--   0 yf        (1000) yf        (1000)      554 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/setup.cfg
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/src/
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp/
--rw-rw-r--   0 yf        (1000) yf        (1000)       26 2021-02-03 07:45:13.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp/__init__.py
--rw-rw-r--   0 yf        (1000) yf        (1000)     3055 2022-06-15 05:59:46.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp/middleware.py
-drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp.egg-info/
--rw-rw-r--   0 yf        (1000) yf        (1000)      436 2022-06-15 06:01:50.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp.egg-info/PKG-INFO
--rw-rw-r--   0 yf        (1000) yf        (1000)      329 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp.egg-info/SOURCES.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)        1 2022-06-15 06:01:50.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp.egg-info/dependency_links.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)       31 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp.egg-info/requires.txt
--rw-rw-r--   0 yf        (1000) yf        (1000)       17 2022-06-15 06:01:51.000000 starmerxauth_erp-0.2.1/src/starmerxauth_erp.egg-info/top_level.txt
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/
+-rw-rw-r--   0 yf        (1000) yf        (1000)     1053 2022-04-08 06:58:25.000000 starmerxauth_erp-0.2.2/LICENSE
+-rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/PKG-INFO
+-rw-rw-rw-   0 yf        (1000) yf        (1000)       28 2022-04-28 03:03:21.000000 starmerxauth_erp-0.2.2/README.md
+-rw-rw-r--   0 yf        (1000) yf        (1000)       85 2022-04-08 06:37:48.000000 starmerxauth_erp-0.2.2/pyproject.toml
+-rw-rw-r--   0 yf        (1000) yf        (1000)      554 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/setup.cfg
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp/
+-rw-rw-r--   0 yf        (1000) yf        (1000)       26 2021-02-03 07:45:13.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp/__init__.py
+-rw-rw-r--   0 yf        (1000) yf        (1000)     3055 2022-06-15 05:59:46.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp/middleware.py
+drwxrwxr-x   0 yf        (1000) yf        (1000)        0 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/
+-rw-rw-r--   0 yf        (1000) yf        (1000)      436 2023-05-31 07:37:32.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/PKG-INFO
+-rw-rw-r--   0 yf        (1000) yf        (1000)      329 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/SOURCES.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)        1 2023-05-31 07:37:32.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/dependency_links.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)       31 2023-05-31 07:37:32.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/requires.txt
+-rw-rw-r--   0 yf        (1000) yf        (1000)       17 2023-05-31 07:37:33.000000 starmerxauth_erp-0.2.2/src/starmerxauth_erp.egg-info/top_level.txt
```

### Comparing `starmerxauth_erp-0.2.1/LICENSE` & `starmerxauth_erp-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starmerxauth_erp-0.2.1/setup.cfg` & `starmerxauth_erp-0.2.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = starmerxauth_erp
-version = 0.2.1
+version = 0.2.2
 author = yang
 author_email = yangjuan@starmerx.com
 description = starmerx verify jwt in erp
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python
@@ -13,16 +13,16 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=2.7
 install_requires = 
-	PyJWT == 1.7.1
-	cryptography == 2.7
+	PyJWT >= 1.7.1
+	cryptography >= 2.7
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `starmerxauth_erp-0.2.1/src/starmerxauth_erp/middleware.py` & `starmerxauth_erp-0.2.2/src/starmerxauth_erp/middleware.py`

 * *Files identical despite different names*

