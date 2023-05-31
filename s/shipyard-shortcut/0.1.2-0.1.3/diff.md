# Comparing `tmp/shipyard_shortcut-0.1.2.tar.gz` & `tmp/shipyard_shortcut-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_shortcut-0.1.2.tar", max compression
+gzip compressed data, was "shipyard_shortcut-0.1.3.tar", max compression
```

## Comparing `shipyard_shortcut-0.1.2.tar` & `shipyard_shortcut-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3722 2023-05-30 13:23:10.342632 shipyard_shortcut-0.1.2/README.md
--rw-r--r--   0        0        0      618 2023-05-30 13:25:43.735912 shipyard_shortcut-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       93 2023-05-25 13:51:48.292105 shipyard_shortcut-0.1.2/shipyard_shortcut/__init__.py
--rw-r--r--   0        0        0      904 2023-05-30 13:21:53.620981 shipyard_shortcut-0.1.2/shipyard_shortcut/cli/add_comment.py
--rw-r--r--   0        0        0     1985 2023-05-25 13:51:48.292792 shipyard_shortcut-0.1.2/shipyard_shortcut/cli/create_ticket.py
--rw-r--r--   0        0        0     2185 2023-05-25 13:51:48.293295 shipyard_shortcut-0.1.2/shipyard_shortcut/cli/edit_ticket.py
--rw-r--r--   0        0        0      781 2023-05-25 13:51:48.293489 shipyard_shortcut-0.1.2/shipyard_shortcut/error_handler.py
--rw-r--r--   0        0        0     8379 2023-05-30 13:23:10.337976 shipyard_shortcut-0.1.2/shipyard_shortcut/shortcut.py
--rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 shipyard_shortcut-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3722 2023-05-30 18:58:34.287577 shipyard_shortcut-0.1.3/README.md
+-rw-r--r--   0        0        0      618 2023-05-31 14:52:48.338216 shipyard_shortcut-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-25 13:51:48.292105 shipyard_shortcut-0.1.3/shipyard_shortcut/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-31 14:51:51.960163 shipyard_shortcut-0.1.3/shipyard_shortcut/cli/add_comment.py
+-rw-r--r--   0        0        0     1845 2023-05-31 14:52:07.017963 shipyard_shortcut-0.1.3/shipyard_shortcut/cli/create_ticket.py
+-rw-r--r--   0        0        0     2042 2023-05-31 14:52:26.048179 shipyard_shortcut-0.1.3/shipyard_shortcut/cli/edit_ticket.py
+-rw-r--r--   0        0        0      781 2023-05-25 13:51:48.293489 shipyard_shortcut-0.1.3/shipyard_shortcut/error_handler.py
+-rw-r--r--   0        0        0     8379 2023-05-30 18:58:34.288905 shipyard_shortcut-0.1.3/shipyard_shortcut/shortcut.py
+-rw-r--r--   0        0        0     4273 1970-01-01 00:00:00.000000 shipyard_shortcut-0.1.3/PKG-INFO
```

### Comparing `shipyard_shortcut-0.1.2/README.md` & `shipyard_shortcut-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_shortcut-0.1.2/pyproject.toml` & `shipyard_shortcut-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-shortcut"
-version = "0.1.2"
+version = "0.1.3"
 description = "A local client for connecting and working with the shortcut app"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_shortcut"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `shipyard_shortcut-0.1.2/shipyard_shortcut/cli/add_comment.py` & `shipyard_shortcut-0.1.3/shipyard_shortcut/cli/add_comment.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--access-token", dest="access_token", required=True)
     parser.add_argument("--story-id", dest="story_id", required=True)
     parser.add_argument("--comment", dest="comment", required=True)
-    parser.add_argument("--verbose", dest="verbose", default=False, action="store_true")
     return parser.parse_args()
 
 
 def main():
     args = get_args()
-    shortcut = ShortcutClient(access_token=args.access_token, verbose=args.verbose)
+    shortcut = ShortcutClient(access_token=args.access_token)
 
     try:
         shortcut.add_comment(story_id=args.story_id, comment=args.comment)
     except Exception as error:
         shortcut.logger.error(error)
         handle_error(shortcut, error)
     else:
```

### Comparing `shipyard_shortcut-0.1.2/shipyard_shortcut/cli/create_ticket.py` & `shipyard_shortcut-0.1.3/shipyard_shortcut/cli/create_ticket.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,23 @@
     parser.add_argument('--story-name', dest='story_name', required=True)
     parser.add_argument('--workflow-state-id', dest='workflow_state_id', required=True)
     parser.add_argument('--description', dest='description', required=False, default=None)
     parser.add_argument('--story-type', dest='story_type', choices=['feature', 'bug', 'chore'], required=True)
     parser.add_argument('--labels', dest='labels', required=False, default=None)
     parser.add_argument('--deadline', dest='deadline', required=False, default=None)
     parser.add_argument('--tasks', dest='tasks', required=False, default=None)
-    parser.add_argument("--verbose", dest="verbose", default=False, action="store_true")
 
     return parser.parse_args()
 
 
 def main():
     args = get_args()
     args_dict = vars(args)
-    shortcut = ShortcutClient(access_token=args.access_token, verbose=args.verbose)
+    shortcut = ShortcutClient(access_token=args.access_token)
     args_dict.pop('access_token')
-    args_dict.pop('verbose')
 
     if args_dict['labels']:
         labels = args_dict['labels'].split(',')
         args_dict['labels'] = [{"name": label} for label in labels]
     if args_dict['tasks']:
         tasks = args_dict['tasks'].split(',')
         args_dict['tasks'] = [{"description": task} for task in tasks]
```

### Comparing `shipyard_shortcut-0.1.2/shipyard_shortcut/cli/edit_ticket.py` & `shipyard_shortcut-0.1.3/shipyard_shortcut/cli/edit_ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,29 @@
 from shipyard_shortcut import ShortcutClient
 from shipyard_shortcut.error_handler import handle_error
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--access-token", dest="access_token", required=True)
     parser.add_argument('--story-id', dest='story_id', required=True)
-    parser.add_argument('--story-name', dest='story_name', required=False, default=None)
+    parser.add_argument('--story-name', dest='name', required=False, default=None)
     parser.add_argument('--workflow-state-id', dest='workflow_state_id', required=False, default=None)
     parser.add_argument('--description', dest='description', required=False, default=None)
-    parser.add_argument('--story-type', dest='story_type', choices=['feature', 'bug', 'chore'], required=True)
+    parser.add_argument('--story-type', dest='story_type', choices=['feature', 'bug', 'chore',''], required=False)
     parser.add_argument('--labels', dest='labels', required=False, default=None)
     parser.add_argument('--deadline', dest='deadline', required=False, default=None)
     parser.add_argument('--tasks', dest='tasks', required=False, default=None)
-    parser.add_argument('--verbose', dest='verbose', default=False, action='store_true')
     return parser.parse_args()
 
 
 def main():
     args = get_args()
     args_dict = vars(args)
-    shortcut = ShortcutClient(access_token=args.access_token, verbose=args.verbose)
+    shortcut = ShortcutClient(access_token=args.access_token)
     args_dict.pop('access_token')
-    args_dict.pop('verbose')
-
     tasks = None
     if args_dict['labels']:
         labels = args_dict['labels'].split(',')
         args_dict['labels'] = [{"name": label} for label in labels]
 
     if args_dict['tasks']:
         tasks = args_dict['tasks'].split(',')
```

### Comparing `shipyard_shortcut-0.1.2/shipyard_shortcut/error_handler.py` & `shipyard_shortcut-0.1.3/shipyard_shortcut/error_handler.py`

 * *Files identical despite different names*

### Comparing `shipyard_shortcut-0.1.2/shipyard_shortcut/shortcut.py` & `shipyard_shortcut-0.1.3/shipyard_shortcut/shortcut.py`

 * *Files identical despite different names*

### Comparing `shipyard_shortcut-0.1.2/PKG-INFO` & `shipyard_shortcut-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-shortcut
-Version: 0.1.2
+Version: 0.1.3
 Summary: A local client for connecting and working with the shortcut app
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

