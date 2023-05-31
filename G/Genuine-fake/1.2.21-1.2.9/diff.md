# Comparing `tmp/Genuine-fake-1.2.21.tar.gz` & `tmp/Genuine-fake-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Genuine-fake-1.2.21.tar", last modified: Wed May 31 13:29:18 2023, max compression
+gzip compressed data, was "dist\Genuine-fake-1.2.9.tar", last modified: Sun Oct 11 12:38:50 2020, max compression
```

## Comparing `Genuine-fake-1.2.21.tar` & `Genuine-fake-1.2.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 andilejaden   (501) staff       (20)        0 2023-05-31 13:29:18.064320 Genuine-fake-1.2.21/
-drwxr-xr-x   0 andilejaden   (501) staff       (20)        0 2023-05-31 13:29:18.062461 Genuine-fake-1.2.21/Genuine_fake.egg-info/
--rw-r--r--   0 andilejaden   (501) staff       (20)     3130 2023-05-31 13:29:18.000000 Genuine-fake-1.2.21/Genuine_fake.egg-info/PKG-INFO
--rw-r--r--   0 andilejaden   (501) staff       (20)      261 2023-05-31 13:29:18.000000 Genuine-fake-1.2.21/Genuine_fake.egg-info/SOURCES.txt
--rw-r--r--   0 andilejaden   (501) staff       (20)        1 2023-05-31 13:29:18.000000 Genuine-fake-1.2.21/Genuine_fake.egg-info/dependency_links.txt
--rw-r--r--   0 andilejaden   (501) staff       (20)        8 2023-05-31 13:29:18.000000 Genuine-fake-1.2.21/Genuine_fake.egg-info/top_level.txt
--rw-r--r--   0 andilejaden   (501) staff       (20)     1094 2023-05-30 16:26:29.000000 Genuine-fake-1.2.21/LICENSE
--rw-r--r--   0 andilejaden   (501) staff       (20)       23 2023-05-30 16:26:29.000000 Genuine-fake-1.2.21/MANIFEST.in
--rw-r--r--   0 andilejaden   (501) staff       (20)     3130 2023-05-31 13:29:18.064114 Genuine-fake-1.2.21/PKG-INFO
--rw-r--r--   0 andilejaden   (501) staff       (20)     2775 2023-05-30 16:26:29.000000 Genuine-fake-1.2.21/README.md
-drwxr-xr-x   0 andilejaden   (501) staff       (20)        0 2023-05-31 13:29:18.063706 Genuine-fake-1.2.21/genuine/
--rw-r--r--   0 andilejaden   (501) staff       (20)      211 2023-05-31 13:22:07.000000 Genuine-fake-1.2.21/genuine/__init__.py
--rw-r--r--   0 andilejaden   (501) staff       (20)    31489 2023-05-30 16:26:29.000000 Genuine-fake-1.2.21/genuine/data_list.py
--rw-r--r--   0 andilejaden   (501) staff       (20)    15849 2023-05-30 16:26:29.000000 Genuine-fake-1.2.21/genuine/data_list.txt
--rw-r--r--   0 andilejaden   (501) staff       (20)    14160 2023-05-30 23:50:40.000000 Genuine-fake-1.2.21/genuine/fake.py
--rw-r--r--   0 andilejaden   (501) staff       (20)       38 2023-05-31 13:29:18.064372 Genuine-fake-1.2.21/setup.cfg
--rw-r--r--   0 andilejaden   (501) staff       (20)      871 2023-05-31 13:27:20.000000 Genuine-fake-1.2.21/setup.py
+drwxrwxrwx   0        0        0        0 2020-10-11 12:38:50.186443 Genuine-fake-1.2.9/
+drwxrwxrwx   0        0        0        0 2020-10-11 12:38:49.728422 Genuine-fake-1.2.9/Genuine_fake.egg-info/
+-rw-rw-rw-   0        0        0     3725 2020-10-11 12:38:47.000000 Genuine-fake-1.2.9/Genuine_fake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2020-10-11 12:38:47.000000 Genuine-fake-1.2.9/Genuine_fake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-10-11 12:38:47.000000 Genuine-fake-1.2.9/Genuine_fake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2020-10-11 12:38:47.000000 Genuine-fake-1.2.9/Genuine_fake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       23 2020-01-10 06:01:40.000000 Genuine-fake-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3725 2020-10-11 12:38:50.185442 Genuine-fake-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2566 2020-09-26 21:35:45.000000 Genuine-fake-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2020-10-11 12:38:50.181443 Genuine-fake-1.2.9/genuine/
+-rw-rw-rw-   0        0        0      187 2020-09-26 18:27:52.000000 Genuine-fake-1.2.9/genuine/__init__.py
+-rw-rw-rw-   0        0        0    34949 2020-10-11 12:12:39.000000 Genuine-fake-1.2.9/genuine/data_list.py
+-rw-rw-rw-   0        0        0    15849 2019-12-20 08:14:44.000000 Genuine-fake-1.2.9/genuine/data_list.txt
+-rw-rw-rw-   0        0        0     6565 2020-10-02 02:05:23.000000 Genuine-fake-1.2.9/genuine/fake.py
+-rw-rw-rw-   0        0        0       42 2020-10-11 12:38:50.188442 Genuine-fake-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      869 2020-10-11 12:24:22.000000 Genuine-fake-1.2.9/setup.py
```

### Comparing `Genuine-fake-1.2.21/genuine/data_list.txt` & `Genuine-fake-1.2.9/genuine/data_list.txt`

 * *Files identical despite different names*

### Comparing `Genuine-fake-1.2.21/setup.py` & `Genuine-fake-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="Genuine-fake",
-    version="1.2.21",
+    version="1.2.9",
     description="Get genuine data for your testing requirements.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/xeroxzen/genuine-fake",
     author="Andile Jaden Mbele",
     author_email="andilembele020@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.8",
     ],
     packages=["genuine"],
     include_package_data=True,
     # install_requires=[],
 )
```

