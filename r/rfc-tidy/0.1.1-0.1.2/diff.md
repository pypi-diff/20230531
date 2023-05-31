# Comparing `tmp/rfc-tidy-0.1.1.tar.gz` & `tmp/rfc-tidy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc-tidy-0.1.1.tar", last modified: Tue Apr  5 04:00:14 2022, max compression
+gzip compressed data, was "rfc-tidy-0.1.2.tar", last modified: Wed May 31 16:04:06 2023, max compression
```

## Comparing `rfc-tidy-0.1.1.tar` & `rfc-tidy-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2022-04-05 04:00:14.193841 rfc-tidy-0.1.1/
--rw-r--r--   0 martin    (1000) martin    (1000)     1071 2022-03-28 06:41:05.000000 rfc-tidy-0.1.1/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)     1102 2022-04-05 04:00:14.193841 rfc-tidy-0.1.1/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      603 2022-04-01 04:26:45.000000 rfc-tidy-0.1.1/README.md
--rwxr-xr-x   0 martin    (1000) martin    (1000)     4517 2022-04-01 04:46:16.000000 rfc-tidy-0.1.1/rfc-tidy
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2022-04-05 04:00:14.193841 rfc-tidy-0.1.1/rfc_tidy.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     1102 2022-04-05 04:00:13.000000 rfc-tidy-0.1.1/rfc_tidy.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      163 2022-04-05 04:00:14.000000 rfc-tidy-0.1.1/rfc_tidy.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2022-04-05 04:00:13.000000 rfc-tidy-0.1.1/rfc_tidy.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2022-04-05 04:00:14.000000 rfc-tidy-0.1.1/rfc_tidy.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2022-04-05 04:00:14.193841 rfc-tidy-0.1.1/setup.cfg
--rwxr-xr-x   0 martin    (1000) martin    (1000)      854 2022-04-05 03:59:40.000000 rfc-tidy-0.1.1/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-31 16:04:06.141684 rfc-tidy-0.1.2/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1071 2023-05-31 15:40:23.000000 rfc-tidy-0.1.2/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)     1283 2023-05-31 16:04:06.141684 rfc-tidy-0.1.2/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      630 2023-05-31 15:45:31.000000 rfc-tidy-0.1.2/README.md
+-rw-r--r--   0 martin    (1000) martin    (1000)      645 2023-05-31 16:03:58.000000 rfc-tidy-0.1.2/pyproject.toml
+-rwxr-xr-x   0 martin    (1000) martin    (1000)     4525 2023-05-31 15:43:29.000000 rfc-tidy-0.1.2/rfc-tidy
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-05-31 16:04:06.141684 rfc-tidy-0.1.2/rfc_tidy.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1283 2023-05-31 16:04:06.000000 rfc-tidy-0.1.2/rfc_tidy.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      178 2023-05-31 16:04:06.000000 rfc-tidy-0.1.2/rfc_tidy.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-05-31 16:04:06.000000 rfc-tidy-0.1.2/rfc_tidy.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-05-31 16:04:06.000000 rfc-tidy-0.1.2/rfc_tidy.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-05-31 16:04:06.141684 rfc-tidy-0.1.2/setup.cfg
+-rwxr-xr-x   0 martin    (1000) martin    (1000)     1043 2023-05-31 15:46:19.000000 rfc-tidy-0.1.2/setup.py
```

### Comparing `rfc-tidy-0.1.1/LICENSE` & `rfc-tidy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rfc-tidy-0.1.1/PKG-INFO` & `rfc-tidy-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: rfc-tidy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cleanup RFC XML
 Home-page: https://github.com/martinthomson/rfc-tidy
 Author: Martin Thomson
-Author-email: mt@lowentropy.net
+Author-email: Martin Thomson <mt@lowentropy.net>
 License: MIT
-Keywords: rfc ietf xml
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/martinthomson/rfc-tidy
+Project-URL: Bug Tracker, https://github.com/martinthomson/rfc-tidy/issues
+Keywords: rfc,ietf,xml
 Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Requires-Python: >=3.6
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rfc-tidy
 
 A simple tool that cleans up RFC XML.
 
@@ -42,8 +43,8 @@
 Removes extraneous XML, comments, and whitespace.
 
 Indents elements consistently.
 
 Replaces non-ASCII characters in text with XML numeric entities so that you
 don't miss them.
 
-
+Sorts attributes by name.
```

### Comparing `rfc-tidy-0.1.1/README.md` & `rfc-tidy-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,7 +23,9 @@
 
 Removes extraneous XML, comments, and whitespace.
 
 Indents elements consistently.
 
 Replaces non-ASCII characters in text with XML numeric entities so that you
 don't miss them.
+
+Sorts attributes by name.
```

### Comparing `rfc-tidy-0.1.1/rfc-tidy` & `rfc-tidy-0.1.2/rfc-tidy`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
         self.tags.append(tag)
         if not Tidy.inline(tag):
             self.nesting = self.nesting + 1
             print("  " * self.nesting, end="")
 
         print(f"<{tag}", end="")
-        for name, value in attributes.items():
+        for name, value in sorted(attributes.items()):
             print(f" {name}={quoteattr(value)}", end="")
 
         self.state = "open"
         self.nl = False
 
     def endElement(self, tag):
         self.flush(self.tags.pop())
```

### Comparing `rfc-tidy-0.1.1/rfc_tidy.egg-info/PKG-INFO` & `rfc-tidy-0.1.2/rfc_tidy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: rfc-tidy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cleanup RFC XML
 Home-page: https://github.com/martinthomson/rfc-tidy
 Author: Martin Thomson
-Author-email: mt@lowentropy.net
+Author-email: Martin Thomson <mt@lowentropy.net>
 License: MIT
-Keywords: rfc ietf xml
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/martinthomson/rfc-tidy
+Project-URL: Bug Tracker, https://github.com/martinthomson/rfc-tidy/issues
+Keywords: rfc,ietf,xml
 Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Requires-Python: >=3.6
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rfc-tidy
 
 A simple tool that cleans up RFC XML.
 
@@ -42,8 +43,8 @@
 Removes extraneous XML, comments, and whitespace.
 
 Indents elements consistently.
 
 Replaces non-ASCII characters in text with XML numeric entities so that you
 don't miss them.
 
-
+Sorts attributes by name.
```

