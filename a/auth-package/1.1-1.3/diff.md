# Comparing `tmp/auth_package-1.1.tar.gz` & `tmp/auth_package-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auth_package-1.1.tar", last modified: Wed May 31 05:07:40 2023, max compression
+gzip compressed data, was "auth_package-1.3.tar", last modified: Wed May 31 07:13:46 2023, max compression
```

## Comparing `auth_package-1.1.tar` & `auth_package-1.3.tar`

### file list

```diff
@@ -1,8 +1,16 @@
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 05:07:40.000000 auth_package-1.1/
--rw-r--r--   0 raminzamani   (501) staff       (20)     1002 2023-05-31 05:07:40.000000 auth_package-1.1/PKG-INFO
--rw-r--r--   0 raminzamani   (501) staff       (20)     1862 2023-05-31 05:07:21.000000 auth_package-1.1/setup.py
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 05:07:40.000000 auth_package-1.1/auth_package/
--rw-r--r--   0 raminzamani   (501) staff       (20)     1793 2023-05-31 05:04:37.000000 auth_package-1.1/auth_package/user.py
--rw-r--r--   0 raminzamani   (501) staff       (20)     2938 2023-05-31 05:03:43.000000 auth_package-1.1/auth_package/permission.py
--rw-r--r--   0 raminzamani   (501) staff       (20)      233 2023-05-29 19:39:45.000000 auth_package-1.1/auth_package/__init__.py
--rw-r--r--   0 raminzamani   (501) staff       (20)       39 2023-05-29 19:53:39.000000 auth_package-1.1/setup.cfg
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:13:46.668066 auth_package-1.3/
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1061 2023-05-29 19:53:56.000000 auth_package-1.3/LICENSE.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)      989 2023-05-31 07:13:46.668159 auth_package-1.3/PKG-INFO
+-rw-r--r--   0 raminzamani   (501) staff       (20)      704 2023-05-31 06:59:59.000000 auth_package-1.3/README.md
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:13:46.666840 auth_package-1.3/auth_package/
+-rw-r--r--   0 raminzamani   (501) staff       (20)      233 2023-05-29 19:39:45.000000 auth_package-1.3/auth_package/__init__.py
+-rw-r--r--   0 raminzamani   (501) staff       (20)     2938 2023-05-31 05:03:43.000000 auth_package-1.3/auth_package/permission.py
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1793 2023-05-31 05:04:37.000000 auth_package-1.3/auth_package/user.py
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:13:46.667920 auth_package-1.3/auth_package.egg-info/
+-rw-r--r--   0 raminzamani   (501) staff       (20)      989 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/PKG-INFO
+-rw-r--r--   0 raminzamani   (501) staff       (20)      292 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/SOURCES.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)        1 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/dependency_links.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)        9 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/requires.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)       13 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/top_level.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)       79 2023-05-31 07:13:46.668531 auth_package-1.3/setup.cfg
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1862 2023-05-31 07:11:59.000000 auth_package-1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `auth_package-1.1/PKG-INFO` & `auth_package-1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: auth_package
-Version: 1.1
+Version: 1.3
 Summary: Auth package for authentication with microservices
 Home-page: https://www.ramzamani.com/
+Download-URL: https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.3.tar.gz
 Author: Ramin Zamanighiri
 Author-email: zamaniramin549@gmail.com
 License: mit
-Download-URL: https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.1.tar.gz
-Description: UNKNOWN
 Keywords: microservices,Auth package,API
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE.txt
```

### Comparing `auth_package-1.1/setup.py` & `auth_package-1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'auth_package',         # How you named your package folder (MyLib)
   packages = ['auth_package'],   # Chose the same as "name"
-  version = '1.1',      # Start with a small number and increase it with every change you make
+  version = '1.3',      # Start with a small number and increase it with every change you make
   license='mit',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Auth package for authentication with microservices',   # Give a short description about your library
   author = 'Ramin Zamanighiri',                   # Type in your name
   author_email = 'zamaniramin549@gmail.com',      # Type in your E-Mail
   url = 'https://www.ramzamani.com/',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.3.tar.gz',    # I explain this later on
   keywords = ['microservices', 'Auth package', 'API'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

### Comparing `auth_package-1.1/auth_package/user.py` & `auth_package-1.3/auth_package/user.py`

 * *Files identical despite different names*

### Comparing `auth_package-1.1/auth_package/permission.py` & `auth_package-1.3/auth_package/permission.py`

 * *Files identical despite different names*

