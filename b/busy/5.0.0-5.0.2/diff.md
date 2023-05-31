# Comparing `tmp/busy-5.0.0.tar.gz` & `tmp/busy-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-5.0.0.tar", last modified: Wed May 31 06:34:19 2023, max compression
+gzip compressed data, was "busy-5.0.2.tar", last modified: Wed May 31 18:58:18 2023, max compression
```

## Comparing `busy-5.0.0.tar` & `busy-5.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.196485 busy-5.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-31 06:33:57.000000 busy-5.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22558 2023-05-31 06:34:19.196485 busy-5.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    22313 2023-05-31 06:33:57.000000 busy-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.187485 busy-5.0.0/busy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-31 06:33:57.000000 busy-5.0.0/busy/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.192485 busy-5.0.0/busy/command/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/activate_command.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/add_command.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/base_command.py
--rw-rw-rw-   0 root         (0) root         (0)     6843 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/command.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/curses_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/defer_command.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/delete_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/drop_and_pop_command.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/edit_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/finish_command.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/list_command.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/queues_command.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/resource_command.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/show_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/switch_command.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/tags_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3551 2023-05-31 06:33:57.000000 busy-5.0.0/busy/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.192485 busy-5.0.0/busy/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.193485 busy-5.0.0/busy/model/collection/
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/done_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/plan_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/skip_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/todo_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.193485 busy-5.0.0/busy/storage/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-31 06:33:57.000000 busy-5.0.0/busy/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-05-31 06:33:57.000000 busy-5.0.0/busy/storage/file_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.194485 busy-5.0.0/busy/ui/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6423 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/curses_ui.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/shell_ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.195485 busy-5.0.0/busy/ui/tcl_ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/tcl_ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/tcl_ui/edit_task_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/tcl_ui/get_item_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.196485 busy-5.0.0/busy/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/date_util.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/python_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/selector.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.188485 busy-5.0.0/busy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22558 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1383 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-05-31 06:33:57.000000 busy-5.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 06:34:19.196485 busy-5.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-05-31 06:33:57.000000 busy-5.0.0/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.203659 busy-5.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-31 18:57:57.000000 busy-5.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-05-31 18:58:18.203659 busy-5.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2023-05-31 18:57:57.000000 busy-5.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.193659 busy-5.0.2/busy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-31 18:57:57.000000 busy-5.0.2/busy/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.198659 busy-5.0.2/busy/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/activate_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/add_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/base_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     6843 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/curses_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/defer_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/delete_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/drop_and_pop_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/edit_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/finish_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/list_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/queues_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/resource_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/show_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/switch_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-31 18:57:57.000000 busy-5.0.2/busy/command/tags_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2023-05-31 18:57:57.000000 busy-5.0.2/busy/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.199659 busy-5.0.2/busy/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.200659 busy-5.0.2/busy/model/collection/
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/done_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/plan_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/skip_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/collection/todo_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-05-31 18:57:57.000000 busy-5.0.2/busy/model/item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.200659 busy-5.0.2/busy/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-31 18:57:57.000000 busy-5.0.2/busy/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-05-31 18:57:57.000000 busy-5.0.2/busy/storage/file_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.201659 busy-5.0.2/busy/ui/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6423 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/curses_ui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/shell_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.202659 busy-5.0.2/busy/ui/tcl_ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/tcl_ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/tcl_ui/edit_task_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/tcl_ui/get_item_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2023-05-31 18:57:57.000000 busy-5.0.2/busy/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.203659 busy-5.0.2/busy/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/python_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-05-31 18:57:57.000000 busy-5.0.2/busy/util/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:58:18.195659 busy-5.0.2/busy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-31 18:58:18.000000 busy-5.0.2/busy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-05-31 18:57:57.000000 busy-5.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 18:58:18.203659 busy-5.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-05-31 18:57:57.000000 busy-5.0.2/version
```

### Comparing `busy-5.0.0/LICENSE` & `busy-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/PKG-INFO` & `busy-5.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 2.1
-Name: busy
-Version: 5.0.0
-Summary: Personal time management system
-Author-email: Francis Potter <busy@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Busy
 ====
 
-**Note: Busy 4 uses a different data model from previous versions. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
+Personal time management for techies
+------------------------------------
+
+tl;dr:
+
+```bash
+pipx install busy
+```
+
+```bash
+busy
+```
+
+**Note: Busy versions 5.0 and later use a different data model from versions 3 and before. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
 
 _Using Busy? [Contact us!](mailto:busy@steampunkwizard.ca)_
 
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
@@ -34,15 +37,14 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-tl;dr: `pipx install busy`
 
 You'll need a terminal emulator to access a command or shell prompt. Examples include:
 
 - iTerm2 or Terminal on MacOS
 - Gnome Terminal or XTerm on Linux
 - CMD on Windows
 - Terminator on all platforms
@@ -60,14 +62,16 @@
 Once Python and PIP are installed, type:
 
 ```
 pip3 install pipx
 pipx install busy
 ```
 
+To upgrade it later:
+
 ```
 pipx upgrade busy
 ```
 
 Overview
 --------
```

### Comparing `busy-5.0.0/README.md` & `busy-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,34 @@
+Metadata-Version: 2.1
+Name: busy
+Version: 5.0.2
+Summary: Personal time management for techies
+Author-email: Francis Potter <busy@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.6.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Busy
 ====
 
-**Note: Busy 4 uses a different data model from previous versions. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
+Personal time management for techies
+------------------------------------
+
+tl;dr:
+
+```bash
+pipx install busy
+```
+
+```bash
+busy
+```
+
+**Note: Busy versions 5.0 and later use a different data model from versions 3 and before. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
 
 _Using Busy? [Contact us!](mailto:busy@steampunkwizard.ca)_
 
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
@@ -24,15 +47,14 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-tl;dr: `pipx install busy`
 
 You'll need a terminal emulator to access a command or shell prompt. Examples include:
 
 - iTerm2 or Terminal on MacOS
 - Gnome Terminal or XTerm on Linux
 - CMD on Windows
 - Terminator on all platforms
@@ -50,14 +72,16 @@
 Once Python and PIP are installed, type:
 
 ```
 pip3 install pipx
 pipx install busy
 ```
 
+To upgrade it later:
+
 ```
 pipx upgrade busy
 ```
 
 Overview
 --------
```

### Comparing `busy-5.0.0/busy/command/activate_command.py` & `busy-5.0.2/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/add_command.py` & `busy-5.0.2/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/command.py` & `busy-5.0.2/busy/command/command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/defer_command.py` & `busy-5.0.2/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/delete_command.py` & `busy-5.0.2/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/drop_and_pop_command.py` & `busy-5.0.2/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/edit_command.py` & `busy-5.0.2/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/finish_command.py` & `busy-5.0.2/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/list_command.py` & `busy-5.0.2/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/command/switch_command.py` & `busy-5.0.2/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/handler.py` & `busy-5.0.2/busy/handler.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/model/collection/__init__.py` & `busy-5.0.2/busy/model/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/model/item.py` & `busy-5.0.2/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/storage/file_storage.py` & `busy-5.0.2/busy/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/ui/curses_ui.py` & `busy-5.0.2/busy/ui/curses_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/ui/shell_ui.py` & `busy-5.0.2/busy/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/ui/tcl_ui/edit_task_widget.py` & `busy-5.0.2/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/ui/tcl_ui/get_item_widget.py` & `busy-5.0.2/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/ui/ui.py` & `busy-5.0.2/busy/ui/ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/util/class_family.py` & `busy-5.0.2/busy/util/class_family.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/util/date_util.py` & `busy-5.0.2/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/util/selector.py` & `busy-5.0.2/busy/util/selector.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy/util/super_wrapper.py` & `busy-5.0.2/busy/util/super_wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/busy.egg-info/PKG-INFO` & `busy-5.0.2/busy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.0.0
-Summary: Personal time management system
+Version: 5.0.2
+Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Busy
 ====
 
-**Note: Busy 4 uses a different data model from previous versions. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
+Personal time management for techies
+------------------------------------
+
+tl;dr:
+
+```bash
+pipx install busy
+```
+
+```bash
+busy
+```
+
+**Note: Busy versions 5.0 and later use a different data model from versions 3 and before. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
 
 _Using Busy? [Contact us!](mailto:busy@steampunkwizard.ca)_
 
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
@@ -34,15 +47,14 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-tl;dr: `pipx install busy`
 
 You'll need a terminal emulator to access a command or shell prompt. Examples include:
 
 - iTerm2 or Terminal on MacOS
 - Gnome Terminal or XTerm on Linux
 - CMD on Windows
 - Terminator on all platforms
@@ -60,14 +72,16 @@
 Once Python and PIP are installed, type:
 
 ```
 pip3 install pipx
 pipx install busy
 ```
 
+To upgrade it later:
+
 ```
 pipx upgrade busy
 ```
 
 Overview
 --------
```

### Comparing `busy-5.0.0/busy.egg-info/SOURCES.txt` & `busy-5.0.2/busy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `busy-5.0.0/pyproject.toml` & `busy-5.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "busy"
 authors = [
     {name = "Francis Potter", email = "busy@steampunkwizard.ca"}
 ]
-description = "Personal time management system"
+description = "Personal time management for techies"
 readme = "README.md"
 requires-python = ">=3.6.5"
 license = {text = "MIT"}
 dependencies = [
     "platformdirs >=3.2.0",
     "wizlib >=0.2.2",
     "windows-curses; platform_system=='Windows'"
```

