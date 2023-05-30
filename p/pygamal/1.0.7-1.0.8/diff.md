# Comparing `tmp/pygamal-1.0.7.tar.gz` & `tmp/pygamal-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamal-1.0.7.tar", last modified: Mon May 29 16:24:47 2023, max compression
+gzip compressed data, was "pygamal-1.0.8.tar", last modified: Tue May 30 22:23:49 2023, max compression
```

## Comparing `pygamal-1.0.7.tar` & `pygamal-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 16:24:47.993203 pygamal-1.0.7/
--rw-rw-rw-   0        0        0      861 2023-05-29 16:24:47.993203 pygamal-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 16:24:47.983279 pygamal-1.0.7/pygamal/
--rw-rw-rw-   0        0        0       22 2023-05-28 00:15:11.000000 pygamal-1.0.7/pygamal/__init__.py
--rw-rw-rw-   0        0        0     4308 2023-05-27 23:24:32.000000 pygamal-1.0.7/pygamal/pygamal.py
-drwxrwxrwx   0        0        0        0 2023-05-29 16:24:47.993203 pygamal-1.0.7/pygamal.egg-info/
--rw-rw-rw-   0        0        0      861 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 16:24:47.993203 pygamal-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-05-29 16:19:54.000000 pygamal-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:23:49.914464 pygamal-1.0.8/
+-rw-rw-rw-   0        0        0      861 2023-05-30 22:23:49.914464 pygamal-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 22:23:49.876420 pygamal-1.0.8/pygamal/
+-rw-rw-rw-   0        0        0       22 2023-05-28 00:15:11.000000 pygamal-1.0.8/pygamal/__init__.py
+-rw-rw-rw-   0        0        0     4649 2023-05-30 22:22:35.000000 pygamal-1.0.8/pygamal/pygamal.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:23:49.914464 pygamal-1.0.8/pygamal.egg-info/
+-rw-rw-rw-   0        0        0      861 2023-05-30 22:23:49.000000 pygamal-1.0.8/pygamal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-30 22:23:49.000000 pygamal-1.0.8/pygamal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 22:23:49.000000 pygamal-1.0.8/pygamal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-30 22:23:49.000000 pygamal-1.0.8/pygamal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 22:23:49.000000 pygamal-1.0.8/pygamal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 22:23:49.914464 pygamal-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-05-30 22:21:14.000000 pygamal-1.0.8/setup.py
```

### Comparing `pygamal-1.0.7/PKG-INFO` & `pygamal-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 1.0.7
+Version: 1.0.8
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pygamal-1.0.7/pygamal/pygamal.py` & `pygamal-1.0.8/pygamal/pygamal.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 gen_keys:
     Generate the global g, e keys from the secret key and p
      
 gen_keys_FAST:
     Generate the global g, e keys from the secret key and p
     Faster
 
+gen_keys_FASTEST:
+    Generate the global g, e keys from the secret key and p
+    FASTEST
+
 gen_c1:
     generate cypher msg 1
 
 gen_x_key:
     generate x_key used for decrypting
 
 encrypt:
@@ -143,14 +147,22 @@
     """
     Generate the global g, e keys from the secret key and p
     Uses faster algorithm to find primitive roots
     """
     g, e = ElGamal_c.gen_keys_FAST(p, secret)
     return g, e
 
+def gen_keys_FASTEST(p:int, secret:int):
+    """
+    Generate the global g, e keys from the secret key and p
+    Uses THE FASTEST algorithm to find primitive roots
+    """
+    g, e = ElGamal_c.gen_keys_FASTEST(p, secret)
+    return g, e
+
 def gen_c1(g, secret, p) -> int:
     """
     Generate the first cipher message from g, secret and p
     """
     return ElGamal_c.gen_c1(g, secret, p)
 
 def gen_x_key(c1, secret, p) -> int:
```

### Comparing `pygamal-1.0.7/pygamal.egg-info/PKG-INFO` & `pygamal-1.0.8/pygamal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 1.0.7
+Version: 1.0.8
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pygamal-1.0.7/setup.py` & `pygamal-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 """
 This module have been made for the project of discret math CSC281 at ksu university.
 The project supervisor is Aqil Alazimi. LinkedIn: https://www.linkedin.com/in/aqil-azmi-20903960/
 The project repo is: https://github.com/Wouze/csc281-project
 """
 
 setup(name="pygamal",
-      version="1.0.7",
+      version="1.0.8",
       author="Wouze (Mohammad)",
       author_email="m7mdwats1@hotmail.com",
       description="This module is for csc281 encryption project ",
       long_description_content_type="text/markdown",
       long_description=long_description,
       url='https://github.com/Wouze/csc281-project',
       keywords=['python', 'c', 'primitive root', 'encryption', 'algamal', 'prime'],
-      install_requires=["ElGamal-c==2.0.1"],
+      install_requires=["ElGamal-c==2.0.2"],
       classifiers=[
             "Development Status :: 1 - Planning",
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3",
             "Operating System :: Unix",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
```

