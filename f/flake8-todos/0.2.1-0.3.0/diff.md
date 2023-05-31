# Comparing `tmp/flake8-todos-0.2.1.tar.gz` & `tmp/flake8-todos-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-todos-0.2.1.tar", last modified: Sat Nov 19 17:59:07 2022, max compression
+gzip compressed data, was "flake8-todos-0.3.0.tar", last modified: Wed May 31 12:03:22 2023, max compression
```

## Comparing `flake8-todos-0.2.1.tar` & `flake8-todos-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       60 2022-11-10 09:21:26.735329 flake8-todos-0.2.1/.gitignore
--rw-r--r--   0        0        0     1556 2022-11-10 09:17:55.265847 flake8-todos-0.2.1/LICENSE
--rw-r--r--   0        0        0     1993 2022-11-10 09:17:55.265847 flake8-todos-0.2.1/README.md
--rw-r--r--   0        0        0      330 2022-11-19 17:58:46.817697 flake8-todos-0.2.1/flake8_todos/__init__.py
--rw-r--r--   0        0        0     1589 2022-11-10 09:57:59.557304 flake8-todos-0.2.1/flake8_todos/_checker.py
--rw-r--r--   0        0        0      121 2022-11-10 09:57:59.557304 flake8-todos-0.2.1/flake8_todos/_constants.py
--rw-r--r--   0        0        0      792 2022-11-10 09:57:59.557304 flake8-todos-0.2.1/flake8_todos/_error.py
--rw-r--r--   0        0        0     6750 2022-11-19 17:58:33.585723 flake8-todos-0.2.1/flake8_todos/_rules.py
--rw-r--r--   0        0        0      986 2022-11-10 09:57:59.557304 flake8-todos-0.2.1/flake8_todos/_token.py
--rw-r--r--   0        0        0     1309 2022-11-10 09:57:59.557304 flake8-todos-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      120 2022-11-10 09:19:07.236990 flake8-todos-0.2.1/setup.cfg
--rw-r--r--   0        0        0        0 2022-11-10 09:17:55.265847 flake8-todos-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     4511 2022-11-19 17:58:33.585723 flake8-todos-0.2.1/tests/test_checker.py
--rw-r--r--   0        0        0      551 2022-11-10 09:57:59.557304 flake8-todos-0.2.1/tests/test_token.py
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 flake8-todos-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       60 2022-11-10 09:21:26.735329 flake8-todos-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1556 2022-11-10 09:17:55.265847 flake8-todos-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1993 2022-11-10 09:17:55.265847 flake8-todos-0.3.0/README.md
+-rw-r--r--   0        0        0      330 2023-05-31 12:02:44.117663 flake8-todos-0.3.0/flake8_todos/__init__.py
+-rw-r--r--   0        0        0     1589 2022-11-10 09:57:59.557304 flake8-todos-0.3.0/flake8_todos/_checker.py
+-rw-r--r--   0        0        0      121 2022-11-10 09:57:59.557304 flake8-todos-0.3.0/flake8_todos/_constants.py
+-rw-r--r--   0        0        0      792 2022-11-10 09:57:59.557304 flake8-todos-0.3.0/flake8_todos/_error.py
+-rw-r--r--   0        0        0     6863 2023-05-31 12:02:06.326055 flake8-todos-0.3.0/flake8_todos/_rules.py
+-rw-r--r--   0        0        0      986 2022-11-10 09:57:59.557304 flake8-todos-0.3.0/flake8_todos/_token.py
+-rw-r--r--   0        0        0     1309 2022-11-10 09:57:59.557304 flake8-todos-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2022-11-10 09:19:07.236990 flake8-todos-0.3.0/setup.cfg
+-rw-r--r--   0        0        0        0 2022-11-10 09:17:55.265847 flake8-todos-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     4579 2023-05-31 12:02:06.326055 flake8-todos-0.3.0/tests/test_checker.py
+-rw-r--r--   0        0        0      551 2022-11-10 09:57:59.557304 flake8-todos-0.3.0/tests/test_token.py
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 flake8-todos-0.3.0/PKG-INFO
```

### Comparing `flake8-todos-0.2.1/LICENSE` & `flake8-todos-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-todos-0.2.1/README.md` & `flake8-todos-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8-todos-0.2.1/flake8_todos/_checker.py` & `flake8-todos-0.3.0/flake8_todos/_checker.py`

 * *Files identical despite different names*

### Comparing `flake8-todos-0.2.1/flake8_todos/_error.py` & `flake8-todos-0.3.0/flake8_todos/_error.py`

 * *Files identical despite different names*

### Comparing `flake8-todos-0.2.1/flake8_todos/_rules.py` & `flake8-todos-0.3.0/flake8_todos/_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,20 @@
             return True
 
         body = token.string[match.end():].strip()
         body = body.split(':', maxsplit=1)[0]
         if not body:
             return False
         # check brackets format
-        if body[0] != '(' or body[-1] != ')':
-            return False
-        return bool(body[1:-1].strip())
+        if body[0] == '(' and body[-1] == ')':
+            return bool(body[1:-1].strip())
+        # check alternative format using @
+        if body[0] == '@':
+            return bool(body[1:].strip())
+        return False
 
 
 @register_rule
 class MissedLinkRule(BaseRule):
     code = 3
     text = 'add link on issue into TODO'
```

### Comparing `flake8-todos-0.2.1/flake8_todos/_token.py` & `flake8-todos-0.3.0/flake8_todos/_token.py`

 * *Files identical despite different names*

### Comparing `flake8-todos-0.2.1/pyproject.toml` & `flake8-todos-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-todos-0.2.1/tests/test_checker.py` & `flake8-todos-0.3.0/tests/test_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,18 @@
     [
         (rules.BadTagRule,          True,   '1 # TODO: i am ok'),
         (rules.BadTagRule,          False,  '1 # FIXME: inline'),
         (rules.BadTagRule,          False,  '# BUG: block'),
         (rules.BadTagRule,          False,  '1 # BUG: inline again'),
         (rules.BadTagRule,          False,  '1 # BUG: inline again'),
         (rules.MissedAuthorRule,    True,   '1 # TODO(author): i am ok'),
+        (rules.MissedAuthorRule,    True,   '1 # TODO@author: i am ok'),
         (rules.MissedAuthorRule,    False,  '1 # TODO: missed author'),
         (rules.MissedAuthorRule,    False,  '1 # TODO(   ): empty brackets'),
-        (rules.MissedAuthorRule,    False,  '1 # TODO(   ): empty brackets'),
+        (rules.MissedAuthorRule,    False,  '1 # TODO@: missed author'),
         (rules.MissedAuthorRule,    False,  '1 # TODO[name]: wrong brackets'),
         (rules.MissedColonRule,     True,   '1 # TODO(author): i am ok'),
         (rules.MissedColonRule,     True,   '1 # TODO: i am also ok'),
         (rules.MissedColonRule,     False,  '1 # TODO(author) missed colon'),
         (rules.MissedColonRule,     False,  '1 # TODO missed author and colon'),
         (rules.MissedColonRule,     False,  '1 # TODO(author) not the right place :)'),
         (rules.MissedTextRule,      True,   '1 # TODO(author): i am ok'),
```

### Comparing `flake8-todos-0.2.1/tests/test_token.py` & `flake8-todos-0.3.0/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `flake8-todos-0.2.1/PKG-INFO` & `flake8-todos-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-todos
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python linter to check TODO comments for consistency and best practice.
 Home-page: https://github.com/orsinium-labs/flake8-todos
 License: BSD 3-Clause
 Keywords: flake8 flake8-plugin linter styleguide code quality
 Author: Gram
 Author-email: gram@orsinium.dev
 Requires-Python: >=3.8
```

