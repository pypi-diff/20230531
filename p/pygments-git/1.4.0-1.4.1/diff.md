# Comparing `tmp/pygments_git-1.4.0.tar.gz` & `tmp/pygments_git-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments_git-1.4.0.tar", last modified: Wed May 24 10:37:39 2023, max compression
+gzip compressed data, was "pygments_git-1.4.1.tar", last modified: Wed May 31 14:50:02 2023, max compression
```

## Comparing `pygments_git-1.4.0.tar` & `pygments_git-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.409635 pygments_git-1.4.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)      635 2023-05-24 10:37:37.000000 pygments_git-1.4.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.4.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.4.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-24 10:37:39.409699 pygments_git-1.4.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-04-10 17:30:19.000000 pygments_git-1.4.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.4.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1809 2023-05-24 10:37:39.410003 pygments_git-1.4.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.407634 pygments_git-1.4.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.408620 pygments_git-1.4.0/src/pygments_git/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    13568 2023-05-24 10:36:44.000000 pygments_git-1.4.0/src/pygments_git/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.4.0/src/pygments_git/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.409406 pygments_git-1.4.0/src/pygments_git.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/entry_points.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-05-24 10:37:39.000000 pygments_git-1.4.0/src/pygments_git.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-24 10:37:39.409525 pygments_git-1.4.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    10328 2023-05-24 10:36:44.000000 pygments_git-1.4.0/tests/test_pygments_git.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.883620 pygments_git-1.4.1/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      764 2023-05-31 14:49:57.000000 pygments_git-1.4.1/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-04-01 11:07:54.000000 pygments_git-1.4.1/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-01 11:04:32.000000 pygments_git-1.4.1/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-31 14:50:02.883677 pygments_git-1.4.1/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     3444 2023-04-10 17:30:19.000000 pygments_git-1.4.1/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-04-01 13:54:14.000000 pygments_git-1.4.1/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1809 2023-05-31 14:50:02.883982 pygments_git-1.4.1/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.881513 pygments_git-1.4.1/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.882567 pygments_git-1.4.1/src/pygments_git/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13581 2023-05-31 14:19:57.000000 pygments_git-1.4.1/src/pygments_git/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-01 11:04:33.000000 pygments_git-1.4.1/src/pygments_git/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.883394 pygments_git-1.4.1/src/pygments_git.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     4594 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      432 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      322 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/entry_points.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        9 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       13 2023-05-31 14:50:02.000000 pygments_git-1.4.1/src/pygments_git.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-31 14:50:02.883514 pygments_git-1.4.1/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    10528 2023-05-31 14:19:57.000000 pygments_git-1.4.1/tests/test_pygments_git.py
```

### Comparing `pygments_git-1.4.0/CHANGELOG.rst` & `pygments_git-1.4.1/CHANGELOG.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.4.1 (2023-05-31)
+------------------
+
+* Fix ``git-conflict-markers`` highlighting of non-marker lines that use marker symbols.
+
 1.4.0 (2023-05-24)
 ------------------
 
 * Support hint, error, and fatal lines in ``git-console``.
 
 * Fix ``commit`` lines and support ``Merge:`` lines in ``git-console``.
```

### Comparing `pygments_git-1.4.0/LICENSE` & `pygments_git-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments_git-1.4.0/PKG-INFO` & `pygments_git-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments_git
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `pygments_git-1.4.0/README.rst` & `pygments_git-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pygments_git-1.4.0/setup.cfg` & `pygments_git-1.4.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygments_git
-version = 1.4.0
+version = 1.4.1
 description = Pygments lexers for Git output and files.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/pygments-git
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
```

### Comparing `pygments_git-1.4.0/src/pygments_git/__init__.py` & `pygments_git-1.4.1/src/pygments_git/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     name = "Git Conflict Markers"
     aliases = ("git-conflict-markers",)
     flags = re.MULTILINE
 
     tokens = {
         "root": [
             (
-                r"^(<{7})( )?(.+)?$",
+                r"^(<{7})(?:( )(.+))?$",
                 bygroups(  # type: ignore [no-untyped-call]
                     Punctuation.Marker, Text, Name.Label
                 ),
             ),
             (
                 r"""(?x)
                     ^
@@ -126,21 +126,21 @@
                     Number.Hex,
                     Text,
                     Name.Label,
                     Text,
                 ),
             ),
             (
-                r"^(\|{7})( )?(.*)$",
+                r"^(\|{7})(?:( )(.*))?$",
                 bygroups(  # type: ignore [no-untyped-call]
                     Punctuation.Marker, Text, Name.Label
                 ),
             ),
             (
-                r"^(={7})( )?(.*)$",
+                r"^(={7})(?:( )(.*))?$",
                 bygroups(  # type: ignore [no-untyped-call]
                     Punctuation.Marker, Text, Name.Label
                 ),
             ),
             (
                 r"""(?x)
                     ^
@@ -153,15 +153,15 @@
                     $
                 """,
                 bygroups(  # type: ignore [no-untyped-call]
                     Punctuation.Marker, Text, Number.Hex, Text, Name.Label, Text
                 ),
             ),
             (
-                r"^(>{7})(\ )?(.*)?$",
+                r"^(>{7})(?:( )(.*))?$",
                 bygroups(  # type: ignore [no-untyped-call]
                     Punctuation.Marker, Text, Name.Label
                 ),
             ),
             (r".*\n", Text),
         ]
     }
```

### Comparing `pygments_git-1.4.0/src/pygments_git.egg-info/PKG-INFO` & `pygments_git-1.4.1/src/pygments_git.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygments-git
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pygments lexers for Git output and files.
 Home-page: https://github.com/adamchainz/pygments-git
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/pygments-git/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
```

### Comparing `pygments_git-1.4.0/tests/test_pygments_git.py` & `pygments_git-1.4.1/tests/test_pygments_git.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,14 +171,26 @@
 
 
 def test_git_conflict_markers(golden_file):
     golden_file.check(
         "test_git_conflict_markers",
         "git-conflict-markers",
         """\
+        This is a heading
+        =================
+
+        another heading
+        <<<<<<<<<<<<<<<
+
+        another heading
+        |||||||||||||||
+
+        another heading
+        >>>>>>>>>>>>>>>
+
         <<<<<<< HEAD
         red
         ||||||| parent of 09fb2fb (Make it blue)
         yellow
         =======
         blue
         >>>>>>> 09fb2fb (Make it blue)
```

