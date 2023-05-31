# Comparing `tmp/busy-3.4.6.tar.gz` & `tmp/busy-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-3.4.6.tar", last modified: Mon Apr 10 09:59:09 2023, max compression
+gzip compressed data, was "busy-5.0.0.tar", last modified: Wed May 31 06:34:19 2023, max compression
```

## Comparing `busy-3.4.6.tar` & `busy-5.0.0.tar`

### file list

```diff
@@ -1,108 +1,64 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.589567 busy-3.4.6/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-30 16:53:52.000000 busy-3.4.6/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)    20450 2023-04-10 09:59:09.589068 busy-3.4.6/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)    20205 2023-04-10 09:55:35.000000 busy-3.4.6/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.530556 busy-3.4.6/busy/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       66 2023-03-30 16:53:52.000000 busy-3.4.6/busy/__main__.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.548988 busy-3.4.6/busy/command/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1872 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/activate_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      825 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/add_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      245 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/base_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     8907 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      279 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/curses_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1643 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/defer_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      981 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/delete_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/drop_and_pop_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1309 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/edit_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1908 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/finish_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      681 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/list_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      212 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/queues_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      254 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/resource_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      950 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/switch_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      196 2023-03-30 16:53:52.000000 busy-3.4.6/busy/command/tags_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)      476 2023-04-10 09:34:40.000000 busy-3.4.6/busy/command/top_command.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3957 2023-04-10 09:34:40.000000 busy-3.4.6/busy/handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.550680 busy-3.4.6/busy/model/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/model/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1931 2023-04-10 09:34:40.000000 busy-3.4.6/busy/model/item.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2598 2023-03-30 16:53:52.000000 busy-3.4.6/busy/model/task.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.552796 busy-3.4.6/busy/queue/
--rw-r--r--   0 francispotter   (501) staff       (20)      102 2023-04-10 09:34:40.000000 busy-3.4.6/busy/queue/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5099 2023-04-10 09:34:40.000000 busy-3.4.6/busy/queue/queue.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2139 2023-04-10 09:34:40.000000 busy-3.4.6/busy/queue/todo_queue.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.553823 busy-3.4.6/busy/root/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/root/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2297 2023-04-10 09:34:40.000000 busy-3.4.6/busy/root/file_system_root.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2204 2023-03-30 16:53:52.000000 busy-3.4.6/busy/selector.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.556748 busy-3.4.6/busy/ui/
--rw-r--r--   0 francispotter   (501) staff       (20)      133 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     6839 2023-04-10 09:34:40.000000 busy-3.4.6/busy/ui/curses_ui.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1567 2023-04-10 09:34:40.000000 busy-3.4.6/busy/ui/shell_ui.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.558838 busy-3.4.6/busy/ui/tcl_ui/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/tcl_ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      824 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/tcl_ui/edit_task_widget.py
--rw-r--r--   0 francispotter   (501) staff       (20)      701 2023-03-30 16:53:52.000000 busy-3.4.6/busy/ui/tcl_ui/get_item_widget.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5178 2023-04-10 09:34:40.000000 busy-3.4.6/busy/ui/ui.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.562565 busy-3.4.6/busy/util/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     6682 2023-04-10 09:34:40.000000 busy-3.4.6/busy/util/class_family.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2882 2023-04-10 09:34:40.000000 busy-3.4.6/busy/util/date_util.py
--rw-r--r--   0 francispotter   (501) staff       (20)      217 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/python_version.py
--rw-r--r--   0 francispotter   (501) staff       (20)      973 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/super_wrapper.py
--rw-r--r--   0 francispotter   (501) staff       (20)      131 2023-03-30 16:53:52.000000 busy-3.4.6/busy/util/textbox_util.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.534568 busy-3.4.6/busy.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)    20450 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     2195 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       43 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       82 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:59:09.000000 busy-3.4.6/busy.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      596 2023-04-10 09:34:40.000000 busy-3.4.6/pyproject.toml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.571382 busy-3.4.6/sand/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-02-25 16:13:53.000000 busy-3.4.6/sand/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      336 2023-02-23 13:30:28.000000 busy-3.4.6/sand/_dataclass.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-04-05 00:41:16.000000 busy-3.4.6/sand/_readline_util.py
--rw-r--r--   0 francispotter   (501) staff       (20)      676 2023-02-25 17:04:15.000000 busy-3.4.6/sand/_textpad.py
--rw-r--r--   0 francispotter   (501) staff       (20)      233 2023-03-06 16:05:27.000000 busy-3.4.6/sand/chooser.py
--rw-r--r--   0 francispotter   (501) staff       (20)      282 2023-03-01 14:38:38.000000 busy-3.4.6/sand/rl-io.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1333 2023-03-01 15:07:59.000000 busy-3.4.6/sand/subprocess.py
--rw-r--r--   0 francispotter   (501) staff       (20)      806 2023-03-02 16:10:26.000000 busy-3.4.6/sand/wrapper.py
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-10 09:59:09.589730 busy-3.4.6/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.572221 busy-3.4.6/test/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/__init__.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.574121 busy-3.4.6/test/data_class_family/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      101 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/atriarch.py
--rw-r--r--   0 francispotter   (501) staff       (20)       76 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/child.py
--rw-r--r--   0 francispotter   (501) staff       (20)       74 2023-03-30 16:53:52.000000 busy-3.4.6/test/data_class_family/grandchild.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.574885 busy-3.4.6/test/handler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/handler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1205 2023-03-30 16:53:52.000000 busy-3.4.6/test/handler/test_handler.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.576635 busy-3.4.6/test/integration/
--rw-r--r--   0 francispotter   (501) staff       (20)      150 2023-04-10 09:34:40.000000 busy-3.4.6/test/integration/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      416 2023-04-10 09:34:40.000000 busy-3.4.6/test/integration/test_integration.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.581255 busy-3.4.6/test/model/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/model/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      433 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_item.py
--rw-r--r--   0 francispotter   (501) staff       (20)      845 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_item_io.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2857 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_queue.py
--rw-r--r--   0 francispotter   (501) staff       (20)      624 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_queue_replace.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1778 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_task.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4056 2023-04-10 09:34:40.000000 busy-3.4.6/test/model/test_todo_queue.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.583580 busy-3.4.6/test/root/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-10 09:34:40.000000 busy-3.4.6/test/root/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1406 2023-04-10 09:34:40.000000 busy-3.4.6/test/root/test_file.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2547 2023-04-10 09:34:40.000000 busy-3.4.6/test/root/test_file_system_root.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.585044 busy-3.4.6/test/ui/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/ui/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      357 2023-03-30 16:53:52.000000 busy-3.4.6/test/ui/test_shell_ui.py
--rw-r--r--   0 francispotter   (501) staff       (20)      790 2023-03-30 16:53:52.000000 busy-3.4.6/test/ui/test_ui_terminal_editor.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-10 09:59:09.588146 busy-3.4.6/test/util/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      797 2023-04-10 09:34:40.000000 busy-3.4.6/test/util/test_class_families.py
--rw-r--r--   0 francispotter   (501) staff       (20)      237 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/test_class_family.py
--rw-r--r--   0 francispotter   (501) staff       (20)      452 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/test_date.py
--rw-r--r--   0 francispotter   (501) staff       (20)      508 2023-03-30 16:53:52.000000 busy-3.4.6/test/util/test_python_version.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-10 09:58:56.000000 busy-3.4.6/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.196485 busy-5.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-31 06:33:57.000000 busy-5.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22558 2023-05-31 06:34:19.196485 busy-5.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22313 2023-05-31 06:33:57.000000 busy-5.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.187485 busy-5.0.0/busy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-31 06:33:57.000000 busy-5.0.0/busy/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.192485 busy-5.0.0/busy/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/activate_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/add_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/base_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     6843 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/curses_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/defer_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/delete_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/drop_and_pop_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/edit_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/finish_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/list_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/queues_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/resource_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/show_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/switch_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-31 06:33:57.000000 busy-5.0.0/busy/command/tags_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2023-05-31 06:33:57.000000 busy-5.0.0/busy/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.192485 busy-5.0.0/busy/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.193485 busy-5.0.0/busy/model/collection/
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/done_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/plan_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/skip_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/collection/todo_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-05-31 06:33:57.000000 busy-5.0.0/busy/model/item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.193485 busy-5.0.0/busy/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-31 06:33:57.000000 busy-5.0.0/busy/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-05-31 06:33:57.000000 busy-5.0.0/busy/storage/file_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.194485 busy-5.0.0/busy/ui/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6423 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/curses_ui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/shell_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.195485 busy-5.0.0/busy/ui/tcl_ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/tcl_ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/tcl_ui/edit_task_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/tcl_ui/get_item_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2023-05-31 06:33:57.000000 busy-5.0.0/busy/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.196485 busy-5.0.0/busy/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/python_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-05-31 06:33:57.000000 busy-5.0.0/busy/util/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:34:19.188485 busy-5.0.0/busy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22558 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-31 06:34:19.000000 busy-5.0.0/busy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-05-31 06:33:57.000000 busy-5.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 06:34:19.196485 busy-5.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-05-31 06:33:57.000000 busy-5.0.0/version
```

### Comparing `busy-3.4.6/LICENSE` & `busy-5.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Francis Potter
+Copyright (c) 2023 Francis Potter
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `busy-3.4.6/PKG-INFO` & `busy-5.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-Metadata-Version: 2.1
-Name: busy
-Version: 3.4.6
-Summary: Personal time management system
-Author-email: Francis Potter <busy@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Busy
 ====
 
+**Note: Busy 4 uses a different data model from previous versions. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
+
+_Using Busy? [Contact us!](mailto:busy@steampunkwizard.ca)_
+
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
 
 Principles
 ----------
@@ -30,79 +24,98 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-Beginners, see [INSTALLATION.md](INSTALLATION.md).
+tl;dr: `pipx install busy`
 
-Experienced folks, use [pipx](https://pypa.github.io/pipx/) to install Busy.
+You'll need a terminal emulator to access a command or shell prompt. Examples include:
 
-```bash
-pipx install busy
+- iTerm2 or Terminal on MacOS
+- Gnome Terminal or XTerm on Linux
+- CMD on Windows
+- Terminator on all platforms
+
+Busy requires `pipx`, which requires Python 3.6 or later. To check whether you already have the right version of Python on your system, start your terminal emulator and type:
+
+```
+python3 -V
 ```
 
-To upgrade:
+If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Ubuntu). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
+
+Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
+
+Once Python and PIP are installed, type:
 
-```bash
-pipx upgrade busy
+```
+pip3 install pipx
+pipx install busy
 ```
 
+```
+pipx upgrade busy
+```
 
 Overview
 --------
 
 Busy ships with two user interfaces, both of them terminal-based and keyboard-driven:
 
 - *Shell UI* - A command-line interface (CLI) using shell conventions and called directly from the shell, one command at a time.
 - *Curses UI* - A faster, more visual interface with one-key commands that remains visible the entire time it's being used.
 
 Some commands also use your favorite terminal-based text editor, such as Emacs, vi, or Nano. It's possible to use Busy without a text editor, but functionality is limited.
 
-Busy's core model is a collection of Items, the most interesting of which are Tasks. Items are organized into Queues, which are ordered sets. You work on the top Task in the Queue, and when it's done, that Task gets removed from the Queue to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
+Busy's core model is a collection of Items, which are typically tasks but can also be discussion topics, groceries to buy, or anything else you like. Items are organized into Queues, which are named sets of Items to do. You work on the top Item in a Queue, and when it's done, that Item gets marked as "done", to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
 
-In addition to the "tasks" Queue, Busy maintains the "plans" Queue for future tasks (don't worry about them yet!) and the "done" Queue as a record of what's been completed in the past.
+Busy actually moves Items between States within each Queue. Each Queue contains a Collection (ordered list) of Items for each State. The States are:
+
+- `todo`: Current Items for you to work on, discuss, or buy now.
+- `done`: Items that have been done, with the date completed.
+- `plan`: Items that have been deferred to a future date, with that date.
 
 Using the Shell UI
 ------------------
 
-To get started, add some Tasks to your default Queue.
+To get started, add some tasks to your default Queue.
 
 ```
-busy add --description "Take a shower"
-busy add --description "Do the laundry"
-busy add --description "Phone mom"
 busy add --description "Donate to the Busy project"
+busy add --description "Phone mom"
+busy add --description "Do the laundry"
+busy add --description "Take a shower"
 ```
 
 Then, when you're ready to start your day, ask Busy what to do first:
 
 ```
-busy top
+busy show
 ```
 
 Returns:
 
 ```
 Take a shower
 ```
 
-_Yes, Busy is great for tracking daily, personal, habitual tasks in addition to work tasks. It feels great to mark things as done!_
+That's the last Item you added, because Busy adds items to the top of the queue, turning it into a [LIFO stack](https://en.wikipedia.org/wiki/Stack_(abstract_data_type).
 
 When you've finished that task, mark it off to find the next task.
 
 ```
 busy finish
 ```
 
 It will ask you to confirm that you're done. Then request the next task:
 
 ```
-busy top
+busy show
 ```
 
 Which will tell you what to do next:
 
 ```
 Do the laundry
 ```
@@ -134,279 +147,300 @@
 2  Donate to the Busy project
 3  Do the laundry
 ```
 
 If you see a task on the list that seems urgent, and you intend to perform it immediately, pop it to the top of the list:
 
 ```
-busy pop 2
+busy pop --criteria 2
 ```
 
 _Our use of the term "pop" for a command doesn't quite fit with the computing term "pop". It might change in the future._
 
-Then `busy get` will return:
+Then `busy show` will return:
 
 ```
 Donate to the Busy project
 ```
 
 Let's say you realize that it's not an appropriate task for today, but you want to defer it to tomorrow:
 
 ```
 busy defer
 ```
 
-It will ask you to confirm "tomorrow" as the day for deferral. Agree with it for now.
+It will ask you to confirm "tomorrow" as the day for deferral. Agree with it for now. The Item will then be moved into the `plan` State with tomorrow's date as the plan date.
 
-At the start of a new day, tell Busy to add all the previously deferred Tasks to the current Queue:
+At the start of a new day, tell Busy to add all the previously deferred Items to the current Queue:
 
 ```
 busy activate
 ```
 
 Commands
 --------
 
 Here's a summary of the commands in Busy.
 
-- `add` adds a new item to the bottom of the queue. The item description may be included after the command or written to stdin (i.e. typed on the next line).
-- `top` gets the top item in the queue, referred to as the "current" item. There are no options.
+- `add` adds a new item to the top of the queue. The item description may be included after the command or typed on the next line.
+- `show` gets the top item in the queue, referred to as the "current" item.
+- `resource` shows the URL (if any) prefixed with an "@" symbol
+- `base` is like `show`, but removes resources, followons, and tags
 - `list` lists the items in the queue in order with their sequence numbers.
 - `pop` moves a task or set of items to the top of a queue.
 - `drop` moves a task or set of items to the bottom of a queue.
 - `delete` permanently removes a task or set of items from a queue.
 - `edit` opens a text editor to edit items - the default is to edit only the top item.
-- `manage` is the same as `edit`, but defaults to edit the whole queue.
-- `finish` removes a task or tasks from the `tasks` queue and adds it to the `done` queue, so it's complete. Good job!
-- `defer` removes a task or set of tasks from the `tasks` queue and schedules it or them to reappear at a future date in the `plans` queue.
-- `activate` moves current tasks from the `plans` queue to the `tasks` queue. Get to work!
+- `manage` is the same as `edit`, but defaults to edit the whole collection.
+- `finish` moves a task or tasks from the `todo` state to the `done` state, so it's complete. Good job!
+- `defer` moves a task or set of tasks from the `todo` state and schedules it or them to reappear at a future date in the `plan` state.
+- `activate` moves current tasks from the `plan` state to the `todo` state. Get to work!
 - `queues` to list all the queues.
 - `tags` to list all the tags.
+- `curses` launches the Curses UI, and is also the default if no command is provided.
+
+Here are some of the options which apply to some or all of the commands:
 
-Except for `add` and `top`, commands allow the designation of specific items to be acted upon. Item designation can be performed using sequence numbers or tags.
+- A queue name, which does not need an option designation
+- `--help` to find out which options apply
+- `--criteria` to designate items to be acted upon, using sequence numbers or tags
+- `--yes` to skip confirmation of any command that requires it
+- `--description` for the item description (`add` command only)
+- `--state` to work on Items of a different state
+- `--timing` applies to the `defer` command
 
 Sequence numbers
 ----------------
 
-Sequence numbers appear in the output from the `list` command. Note that the numbering starts with 1, and is not an ID -- the number of a item will change when the queue is modified. So always reference the most recent output from the `list` command.
+Sequence numbers appear in the output from the `list` command. Note that the numbering starts with 1, and is not an ID -- the number of a item will change when the collection is modified. So always reference the most recent output from the `list` command.
 
-To designate more than one item, separate the sequence numbers with a space.
+Sequence numbers are used with the `--criteria` option, which can be shortened to `-c`. To designate more than one item, separate the sequence numbers with a space.
 
-When used to designate items, a range of sequence numbers is separated by a hyphen, with no whitespace, and is inclusive. For example, `4-6` designates items 4, 5, and 6. A hyphen without a number after it includes all the items from that item to the end of the queue. A hyphen on its own indicates the last item in the queue.
+Another choice is ranges. A range of sequence numbers is separated by a hyphen, with no whitespace, and is inclusive. For example, `4-6` designates items 4, 5, and 6. A hyphen without a number after it includes all the items from that item to the end of the queue. A hyphen on its own indicates the last item in the queue.
 
 Below are some examples of task designations by sequence number.
 
-- `busy pop 5` pops item number 5
-- `busy drop 3-7` drops items 3 through 7 (4 items)
-- `busy list 3-` lists all the items from number 3 through the end of the list
-- `busy delete 3 5 7 9` deletes only the items designated
-- `busy defer -` defers the last task
-- `busy edit -4` is an error! Use `busy edit 1-4` instead
+- `busy pop -c 5` pops item number 5
+- `busy drop -c 3-7` drops items 3 through 7 (4 items)
+- `busy list -c 3-` lists all the items from number 3 through the end of the list
+- `busy delete -c 3 5 7 9` deletes only the items designated
+- `busy defer -c -` defers the last task
+- `busy edit -c -4` is an error! Use `busy edit -c 1-4` instead
 - `busy manage` allows you to edit the entire queue
 
 Items will always be handled in the order they appear in the queue, regardless of the order the criteria are provided. So for example, if a `pop` command designates some items, they will be moved to the top of the queue in the order, relative to each other, they currently appear in the queue.
 
-The sequence numbers in the `list` command output are from the queue itself. So the `list` command does not modify the sequence numbers, even when item designation is applied.
+The sequence numbers in the `list` command output are from the collection itself. So the `list` command does not modify the sequence numbers, even when item designation is applied.
 
 Tags
 ----
 
 Items can have tags, which are space-separated hashtags in the item description. An item can have no tags, one tag, or more than one tag. For example the following item description has the tag "errands":
 
 ```
 go to the supermarket #errands
 ```
 
-Tags cannot contain punctuation.
+The only punctuation that tags can contain is the hyphen ("-").
 
-Hash tags may be used for item designation, in which case the hash itself ("#") is omitted from the command line. For example, the following command will move all the items with the `#errands` tag to the top of the queue.
+Hash tags may be used as criteria in addition to sequence numbers. For example, the following command will move all the items with the `#errands` tag to the top of the queue.
 
 ```
-busy pop errands
+busy pop -c #errands
 ```
 
-Whitespace-separated item designation criteria are additive -- that is, a logical OR. For example, the following command will delete all the admin tasks, sales tasks, and tasks 3 and 4.
+Whitespace-separated criteria are additive -- that is, a logical OR. For example, the following command will delete all the admin tasks, sales tasks, and tasks 3 and 4.
 
 ```
-busy delete admin sales 3 4
+busy delete -c #admin #sales 3 4
 ```
 
+_Note to self: why does this work? Shouldn't the hash symbol indicate a comment?_
+
 Default item designations
 -------------------------
 
 For the most part, commands that accept item designations default to only act on the top item in the queue. The exceptions are:
 
-- `list` defaults to list the entire queue
-- `pop` defaults to pop the last item in the queue to the top
-- `activate` defaults to activate items for today (more on that below)
+- `list` and `manage` default to handle the entire collection
+- `pop` defaults to pop the last item in the collection to the top
+- `activate` defaults to activate `plan` items for today (more on that below)
 
 Alternate queues
 ----------------
 
-Busy will manage any number of queues, which are entirely separate ordered sets of items. For example, you might have a `shopping` queue for items to buy at the store, and a `movies` queue for films you'd like to watch. The default queue is called `tasks` and has special properties related to planning.
+Busy will manage any number of queues, which are entirely separate sets of items. For example, you might have a `shopping` queue for items to buy at the store, and a `movies` queue for films you'd like to watch. The default queue is called `tasks`.
 
-To designate an alternate queue, use the `--queue` option on a command. For example:
+To designate an alternate queue, enter it right after the command. For example:
 
 ```
-busy add "Skimmed Milk" --queue shopping
-busy top --queue movies
+busy add shopping -d "Skimmed Milk"
+busy list movies
 ```
 
 Managing plans
 --------------
 
-The default `tasks` queue supports several specific commands related to planning -- that is, scheduling tasks for the future. They are `finish`, `defer`, and `activate`. The task-specific commands do not accept a `--queue` modifier, because they only work on the default `tasks` queue. Planned tasks are kept in another special queue called `plans`, and completed tasks are kept in a queue called `done`.
+Busy supports several specific commands related to planning -- that is, scheduling tasks for the future. They are `finish`, `defer`, and `activate`. The task-specific commands handle items in the `plan` state and, in some cases, the `done` state.
 
-The task commands accept item designations. The `defer` and `finish` commands reference the `tasks` queue; the `activate` command references the `plans` queue. The default for `defer` and `finish` is the top item in the `tasks` queue; the default for `activate` is to activate only plans deferred to today or earlier.
+The task commands accept criteria. The `defer` and `finish` commands reference the `todo` collection; the `activate` command references the `plan` collection. The default for `defer` and `finish` is the top item in the collection; the default for `activate` is to activate only plans deferred to today or earlier.
 
 Planning by date
 ----------------
 
 Planning is by date, not time, and is relative to the current date according to the system clock.
 
-In the `defer` command, the date can be specified using the `--to` or `--for` option (they are interchangable). If the options are omitted, then the date can be provided as input.
+In the `defer` command, the date can be specified using the `--timing` option. If the option is omitted, then the date can be provided as input during confirmation.
 
 The date may take any of the following forms:
 
 - A specific date in `YYYY-MM-DD` format, such as `2018-10-28`. Slashes are also acceptable, but the order is always year, then month, then day.
 - A specific date without the year in `MM-DD` format, such as `7-4`, which will defer the item to that date in the future (even if it's in the next year).
 - A specific day of the month as a simple integer, such as `12`, which will defer the item to that day of the month, in either the current month or the next month.
 - An integer, a space, and the word `day` or `days`, such as `4 days`, which will defer the item to that number of days from today.
 - An integer without a space and the letter `d`, such as `4d`, which is a short form of `4 days`.
 - The word `tomorrow`, which is also the default if no date is provided.
 - The word `today`, which is a little odd but obvious.
 
-As an example, the following command will defer tasks 4, 5, and 6 from the `tasks` queue to the date 4 days from today, keeping them in the `plans` queue until that date.
+As an example, the following command will defer tasks 4, 5, and 6 from the `todo` collection to the date 4 days from today, keeping them in the `plan` collection until that date.
 
 ```
-busy defer 4-6 --for 4 days
+busy defer -c 4-6 -t "4 days"
 ```
 
-Note that the `plans` queue is keeping the task information (verbatim from the `tasks` queue) along with the date information (as an absolute date).
+Note that the `plan` collection is keeping the task information (verbatim from the `todo` collection) along with the date information (as an absolute date).
 
-To pull tasks off the `plans` queue and put them back on the `tasks` queue, use the `activate` command. There are two ways to use the `activate` command:
+To pull tasks from the `plan` collection and put them back into the `todo` collection, use the `activate` command. There are two ways to use the `activate` command:
 
-- With no item designation, in which case Busy activates all the tasks scheduled for today or earlier, bringing the `tasks` list up to date
-- With designated items from the `plans` queue; note that the `activate` command accepts item designation from the `plans` queue itself
+- With no criteria, in which case Busy activates all the tasks scheduled for today or earlier, bringing the `todo` list up to date
+- With designated items from the `plan` collection; note that the `activate` command accepts item designation from the `plan` queue itself so use `busy list -s plan` first to get the right list.
 
 Finishing and following up
 --------------------------
 
-Like `defer`, the `finish` command only works on the `tasks` queue. It removes the designated Task (or the top task if none is designated) from the queue and adds it to the `done` queue, with today's date to indicate when it was completed.
+The `finish` command removes the designated Task (or the top task if none is designated) from the `todo` state  and adds it to the `done` state, with today's date to indicate when it was completed.
 
-Optionally, a task can have a followon, which is another task to be added to the queue after the first task is finished. Followons are described in a task using an arrow notation. In the following example, the task "eat" has a followon task "drink":
+Optionally, a task can have a "followon", which is another task to be added as a `todo` after the first task is finished. Followons are described in a task using an arrow notation. In the following example, the task "eat" has a followon task "drink":
 
 ```
 eat --> drink
 ```
 
-Note that the hyphens and whitespace are optional; really the marker that matters for delimiting a followon is the right angle bracket (">"). Also note that right angle bracket is not a valid character in a task description.
+Note that the hyphens and whitespace are optional; really the marker that matters for delimiting a followon is the right angle bracket (">"). Also note that right angle bracket is not a valid character elsewhere in a task description.
 
-When the `finish` command is executed on the task above, the "eat" task will be recorded as "done" and the "drink" task will be added to the bottom of the `tasks` queue.
+When the `finish` command is executed on the task above, the "eat" task will be recorded as "done" and the "drink" task will be added to the top of the `todo` list.
 
-Note that followons can be chained. For example, when the `finish` command is run on the task illustrated below, a new task "drink > be merry" will be added to the queue. Only when that Task is finished will the "be merry" task itself appear on the queue.
+Note that followons can be chained. For example, when the `finish` command is run on the task illustrated below, a new task "drink > be merry" will be added to the `todo` collection`. Only when that Task is finished will the "be merry" task itself appear.
 
 ```
 eat > drink > be merry
 ```
 
 Repeating tasks
 ---------------
 
-A special type of followon is the repeat. In this case, instead of adding the next task to the bottom of the queue, the entire current task -- including the Followon itself -- is entered into the `plans` queue at some point in the future. Repeats allow for easy management of repeating tasks. Some examples follow.
+A special type of followon is the repeat. In this case, instead of adding the next task to the top of the `todo` list, the entire current task -- including the followon itself -- is entered into the `plan` collection at some point in the future. Repeats allow for easy management of repeating tasks. Some examples follow.
 
 - `check email --> repeat in 1 day`
 - `phone mom --> repeat on sunday`
 - `balance the checkbook --> repeat on 6`
 
 The exact syntax for a Repeat is the word "repeat" followed by either "on" or "in" and a relative date phrase -- the same phrases that work with the `defer` command.
 
-Note that the repetition itself only happens on the `finish` command. The completed task (i.e. "check email") is entered in the `done` queue and then the entire task (with the Repeat) is scheduled in the `plans` queue for the appropriate time in the future.
+Note that the repetition itself only happens when the `finish` command is executed. The completed task (i.e. "check email") is entered in the `done` list and then the entire task (with the Repeat) is scheduled in the `plan` list for the appropriate time in the future.
 
 Editing items
 -------------
 
-The `edit` and `manage` commands launch the user's default text editor to directly edit a task, the whole queue, or part of a queue. Note that `edit` and `manage` are identical commands except for their defaults.
+The `edit` and `manage` commands launch the user's default text editor to directly edit a task, the whole queue, or part of a queue. Note that `edit` and `manage` are identical commands except for their default criteria.
 
 The definition of the "default text editor" depends on the OS and configuration but here's the logic:
 
 1. Try the EDITOR environment variable
 1. If that doesn't exist, try the `sensible-editor` command (Ubuntu)
 1. If that doesn't exist, try the `open -W` command (OSX)
 
-You must quit the editor to accept the change back into Busy.
+You must save changes and quit the editor to accept the change back into Busy.
 
-The `edit` command with no criteria will edit the top item in the queue, and the `manage` command with no criteria will edit the entire queue. But it's also possible to designate items to be edited with both commands. The commands do their best to replace the edited items in place in the list order. So if you `edit` or `manage` a tag whose items are recently popped (at the top of the queue), then the edited items will still appear at the top. Even if you add items, they will be inserted after the last item in the edited set, not at the end of the queue. But all the items brought up in the editor will be edited. So if you remove an item in the editor, it will be deleted and the others will be moved up to take its place.
+The `edit` command with no criteria will edit the top item in the list, and the `manage` command with no criteria will edit the entire list. But it's also possible to designate items to be edited with both commands using criteria. The commands do their best to replace the edited items in place in the list order. So if you `edit` or `manage` a tag whose items are recently popped (at the top of the collection), then the edited items will still appear at the top. Even if you add items, they will be inserted after the last item in the edited set, not at the end of the queue. But all the items brought up in the editor will be edited. So if you remove an item in the editor, it will be deleted and the others will be moved up to take its place.
 
 For faster daily use - the Curses UI
 ------------------------------------
 
 Busy suports multiple user interfaces. The command line interface described above is the shell interface. The alternative is the curses UI, which draws an entirely new terminal in the same window.
 
-_We get it - "curses" is a terrible name. It's a reference to the underlying technology. It's likely to change._
+_We get it - "curses" is a terrible name. It's a reference to the underlying technology._
 
-As of now, the curses UI only supports the `tasks` queue. The commands can be triggered with single keystrokes, and only act on their default tasks (usually the top task). The UI always displays the current queue (which is always `tasks` for now) and the current (top) task at the top of the screen.
+In the Curses UI, commands can be triggered with single keystrokes, and only act on their default items (usually the top task). The UI always displays the current queue (which is always `tasks` for now) and the current (top) `todo` item` at the top of the screen.
 
 To invoke the curses UI, type:
 
 ```
 busy curses
 ```
 
-Commands within the UI are shown with a single letter underlined. The underlined letter is the keystroke that will invoke the command. Use `q` to quit. When inside a command, use ctrl-C to cancel the command and return to the main menu.
+Or it's the default so just type:
 
+```
+busy
+```
+
+Commands within the UI are shown with a single letter underlined. The underlined letter is the keystroke that will invoke the command. Use `q` to quit. When inside a command, use ctrl-C to cancel the command and return to the main menu.
 
 Data storage
 ------------
 
-Busy keeps the queues in plain text files, so if the tool doesn't do something you want, you may edit the files. The files are in a directory together, referred to as the "root". Each file is the name of the queue with a `.txt` extension. If a required file is missing, it will be created automatically. So typically, the root includes `tasks.txt`, `plans.txt`, `done.txt`, and any number of custom queue files.
+Busy keeps the collections in plain text files, so if the tool doesn't do something you want, you may edit the files. The files are in a directory together, referred to as the "root". Each file is the named according to the following convention:
 
-Technically, Busy data files are pipe-delimited data files, though `tasks.txt` and any custom queues only have one field ("description") while `plans.txt` and `done.txt` have only two fields (date and description).
+```
+<queue>.<state>.psv
+```
+
+If a required file is missing, it will be created automatically. So typically, the root includes `tasks.todo.psv`, `tasks.plan.psv`, `tasks.done.txt`, and any number of custom queue files.
+
+Technically, Busy data files are pipe-delimited data files, though the `todo` collections only have one field ("description") while the `plan` and `done` files have only two fields (date and description).
 
 Busy is not a database (yet). There is no support for managing separate fields in the Busy tool itself.
 
 The root is designated in one of the following ways, which are tried in order.
 
 - The `--root` option on any command
 - The `BUSY_ROOT` environment variable, if no `--root` option is provided
 - A directory at `~/.busy`, which will be generated as needed if no `--root` option or `BUSY_ROOT` environment variable are provided,
 
 Note that the `--root` option must come after `busy` but command-specific options (`--yes`, `--to`, `--for`, and `--queue`) must come after commands.
 
 The following example shows the `--root` option with command-specific options on the same command line.
 
 ```
-busy --root ~/.config/busy defer --to tuesday
+busy --root ~/.config/busy defer --t tuesday
 ```
 
-Note that Busy does not support concurrency in any form. If two commands are executing at the same time, they might overwrite each other. Overwriting is especially risky with the `edit` command, which keeps the user's editor open until they close it.
+Note that Busy does not support concurrency or locking in any form. If two commands are executing at the same time, they might overwrite each other. Overwriting is especially risky with the `edit` and `manage` commands, which keeps the user's editor open until they close it.
 
-The format is designed to be simple (i.e. non-default queues are really just lists of items) but not idiot-proof. Experimentation might result in unintended consequences.
+The format is designed to be simple but not idiot-proof. Experimentation might result in unintended consequences.
 
 Development
 ===========
 
 The code is intended to demonstrate some Python best practices:
 
 - *Object-oriented* with classes and subclasses.
 - *Dynamic configuration* using a unique approach we call "class families" - for example, the names of the commands are properties of the command classes, not in a big "if" statement.
-- *Extensive testing* with >90% test coverage, guaranteed by CI.
+- *Extensive testing* with high test coverage, guaranteed by CI.
 - *Leverage the standard library* by requiring 3rd party PIP modules for development, but not for usage.
 
 To set everything up:
 
-```
-sudo pip3 install vernum coverage pycodestyle twine
-```
+- Requires Python 3.6.5 or later
+- Clone the repo and CD into it
+- Set up a venv if that's your thing
+- `pip install -r requirements/freeze.txt`
+- To run it: `python -m busy` ...
 
-To get the full repo:
-
-```
-git clone git@gitlab.com:fpotter/tools/busy.git
-```
 We use Visual Studio Code to build Busy, so there is a VS Code configuration file in the repository.
 
 Then to run the test suite:
 
 ```
 make test
 ```
@@ -419,15 +453,15 @@
 
 And to check style:
 
 ```
 make style
 ```
 
-_Note to self: To publish a new build, use 'vernum' with 'major', 'minor', or 'patch' depending on how major the changes were since the last build. Then push. GitLab allows you to publish to PyPI in its UI, and only when Vernum has been run._
+_Note to self: To publish a new build, use 'vernum' with 'major', 'minor', or 'patch' depending on how major the changes were since the last build. Then push. GitLab allows you to publish to PyPI via CI/CD, and only when Vernum has been run._
 
 Command summary
 ===============
 
 Below is a reference list of all commands, handy to correlate the one-letter version with the full version. The one-letter version is used in the curses UI, and is an alternative option in the shell UI. Some of the listed commands are yet to be implemented; they are listed here merely to reserve their names.
 
 | Short | Full |
@@ -436,17 +470,16 @@
 | c | activate |
 | d | delete |
 | e | edit |
 | f | defer |
 | l | list |
 | m | manage |
 | n | finish |
-| p | pop |
-| q | quit (only in interactive UI) |
+| o | pop |
+| p | print |
+| q | quit |
 | r | drop |
-| s | shuffle |
+| s | skip |
 | t | tags |
 | u | queues (list) |
 | w | switch (queues) |
 |   | curses (only in shell UI) |
-|   | top |
-
```

### Comparing `busy-3.4.6/README.md` & `busy-5.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,24 @@
+Metadata-Version: 2.1
+Name: busy
+Version: 5.0.0
+Summary: Personal time management system
+Author-email: Francis Potter <busy@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.6.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Busy
 ====
 
+**Note: Busy 4 uses a different data model from previous versions. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
+
+_Using Busy? [Contact us!](mailto:busy@steampunkwizard.ca)_
+
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
 
 Principles
 ----------
@@ -20,79 +34,98 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-Beginners, see [INSTALLATION.md](INSTALLATION.md).
+tl;dr: `pipx install busy`
 
-Experienced folks, use [pipx](https://pypa.github.io/pipx/) to install Busy.
+You'll need a terminal emulator to access a command or shell prompt. Examples include:
 
-```bash
-pipx install busy
+- iTerm2 or Terminal on MacOS
+- Gnome Terminal or XTerm on Linux
+- CMD on Windows
+- Terminator on all platforms
+
+Busy requires `pipx`, which requires Python 3.6 or later. To check whether you already have the right version of Python on your system, start your terminal emulator and type:
+
+```
+python3 -V
 ```
 
-To upgrade:
+If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Ubuntu). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
+
+Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
+
+Once Python and PIP are installed, type:
 
-```bash
-pipx upgrade busy
+```
+pip3 install pipx
+pipx install busy
 ```
 
+```
+pipx upgrade busy
+```
 
 Overview
 --------
 
 Busy ships with two user interfaces, both of them terminal-based and keyboard-driven:
 
 - *Shell UI* - A command-line interface (CLI) using shell conventions and called directly from the shell, one command at a time.
 - *Curses UI* - A faster, more visual interface with one-key commands that remains visible the entire time it's being used.
 
 Some commands also use your favorite terminal-based text editor, such as Emacs, vi, or Nano. It's possible to use Busy without a text editor, but functionality is limited.
 
-Busy's core model is a collection of Items, the most interesting of which are Tasks. Items are organized into Queues, which are ordered sets. You work on the top Task in the Queue, and when it's done, that Task gets removed from the Queue to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
+Busy's core model is a collection of Items, which are typically tasks but can also be discussion topics, groceries to buy, or anything else you like. Items are organized into Queues, which are named sets of Items to do. You work on the top Item in a Queue, and when it's done, that Item gets marked as "done", to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
 
-In addition to the "tasks" Queue, Busy maintains the "plans" Queue for future tasks (don't worry about them yet!) and the "done" Queue as a record of what's been completed in the past.
+Busy actually moves Items between States within each Queue. Each Queue contains a Collection (ordered list) of Items for each State. The States are:
+
+- `todo`: Current Items for you to work on, discuss, or buy now.
+- `done`: Items that have been done, with the date completed.
+- `plan`: Items that have been deferred to a future date, with that date.
 
 Using the Shell UI
 ------------------
 
-To get started, add some Tasks to your default Queue.
+To get started, add some tasks to your default Queue.
 
 ```
-busy add --description "Take a shower"
-busy add --description "Do the laundry"
-busy add --description "Phone mom"
 busy add --description "Donate to the Busy project"
+busy add --description "Phone mom"
+busy add --description "Do the laundry"
+busy add --description "Take a shower"
 ```
 
 Then, when you're ready to start your day, ask Busy what to do first:
 
 ```
-busy top
+busy show
 ```
 
 Returns:
 
 ```
 Take a shower
 ```
 
-_Yes, Busy is great for tracking daily, personal, habitual tasks in addition to work tasks. It feels great to mark things as done!_
+That's the last Item you added, because Busy adds items to the top of the queue, turning it into a [LIFO stack](https://en.wikipedia.org/wiki/Stack_(abstract_data_type).
 
 When you've finished that task, mark it off to find the next task.
 
 ```
 busy finish
 ```
 
 It will ask you to confirm that you're done. Then request the next task:
 
 ```
-busy top
+busy show
 ```
 
 Which will tell you what to do next:
 
 ```
 Do the laundry
 ```
@@ -124,279 +157,300 @@
 2  Donate to the Busy project
 3  Do the laundry
 ```
 
 If you see a task on the list that seems urgent, and you intend to perform it immediately, pop it to the top of the list:
 
 ```
-busy pop 2
+busy pop --criteria 2
 ```
 
 _Our use of the term "pop" for a command doesn't quite fit with the computing term "pop". It might change in the future._
 
-Then `busy get` will return:
+Then `busy show` will return:
 
 ```
 Donate to the Busy project
 ```
 
 Let's say you realize that it's not an appropriate task for today, but you want to defer it to tomorrow:
 
 ```
 busy defer
 ```
 
-It will ask you to confirm "tomorrow" as the day for deferral. Agree with it for now.
+It will ask you to confirm "tomorrow" as the day for deferral. Agree with it for now. The Item will then be moved into the `plan` State with tomorrow's date as the plan date.
 
-At the start of a new day, tell Busy to add all the previously deferred Tasks to the current Queue:
+At the start of a new day, tell Busy to add all the previously deferred Items to the current Queue:
 
 ```
 busy activate
 ```
 
 Commands
 --------
 
 Here's a summary of the commands in Busy.
 
-- `add` adds a new item to the bottom of the queue. The item description may be included after the command or written to stdin (i.e. typed on the next line).
-- `top` gets the top item in the queue, referred to as the "current" item. There are no options.
+- `add` adds a new item to the top of the queue. The item description may be included after the command or typed on the next line.
+- `show` gets the top item in the queue, referred to as the "current" item.
+- `resource` shows the URL (if any) prefixed with an "@" symbol
+- `base` is like `show`, but removes resources, followons, and tags
 - `list` lists the items in the queue in order with their sequence numbers.
 - `pop` moves a task or set of items to the top of a queue.
 - `drop` moves a task or set of items to the bottom of a queue.
 - `delete` permanently removes a task or set of items from a queue.
 - `edit` opens a text editor to edit items - the default is to edit only the top item.
-- `manage` is the same as `edit`, but defaults to edit the whole queue.
-- `finish` removes a task or tasks from the `tasks` queue and adds it to the `done` queue, so it's complete. Good job!
-- `defer` removes a task or set of tasks from the `tasks` queue and schedules it or them to reappear at a future date in the `plans` queue.
-- `activate` moves current tasks from the `plans` queue to the `tasks` queue. Get to work!
+- `manage` is the same as `edit`, but defaults to edit the whole collection.
+- `finish` moves a task or tasks from the `todo` state to the `done` state, so it's complete. Good job!
+- `defer` moves a task or set of tasks from the `todo` state and schedules it or them to reappear at a future date in the `plan` state.
+- `activate` moves current tasks from the `plan` state to the `todo` state. Get to work!
 - `queues` to list all the queues.
 - `tags` to list all the tags.
+- `curses` launches the Curses UI, and is also the default if no command is provided.
+
+Here are some of the options which apply to some or all of the commands:
 
-Except for `add` and `top`, commands allow the designation of specific items to be acted upon. Item designation can be performed using sequence numbers or tags.
+- A queue name, which does not need an option designation
+- `--help` to find out which options apply
+- `--criteria` to designate items to be acted upon, using sequence numbers or tags
+- `--yes` to skip confirmation of any command that requires it
+- `--description` for the item description (`add` command only)
+- `--state` to work on Items of a different state
+- `--timing` applies to the `defer` command
 
 Sequence numbers
 ----------------
 
-Sequence numbers appear in the output from the `list` command. Note that the numbering starts with 1, and is not an ID -- the number of a item will change when the queue is modified. So always reference the most recent output from the `list` command.
+Sequence numbers appear in the output from the `list` command. Note that the numbering starts with 1, and is not an ID -- the number of a item will change when the collection is modified. So always reference the most recent output from the `list` command.
 
-To designate more than one item, separate the sequence numbers with a space.
+Sequence numbers are used with the `--criteria` option, which can be shortened to `-c`. To designate more than one item, separate the sequence numbers with a space.
 
-When used to designate items, a range of sequence numbers is separated by a hyphen, with no whitespace, and is inclusive. For example, `4-6` designates items 4, 5, and 6. A hyphen without a number after it includes all the items from that item to the end of the queue. A hyphen on its own indicates the last item in the queue.
+Another choice is ranges. A range of sequence numbers is separated by a hyphen, with no whitespace, and is inclusive. For example, `4-6` designates items 4, 5, and 6. A hyphen without a number after it includes all the items from that item to the end of the queue. A hyphen on its own indicates the last item in the queue.
 
 Below are some examples of task designations by sequence number.
 
-- `busy pop 5` pops item number 5
-- `busy drop 3-7` drops items 3 through 7 (4 items)
-- `busy list 3-` lists all the items from number 3 through the end of the list
-- `busy delete 3 5 7 9` deletes only the items designated
-- `busy defer -` defers the last task
-- `busy edit -4` is an error! Use `busy edit 1-4` instead
+- `busy pop -c 5` pops item number 5
+- `busy drop -c 3-7` drops items 3 through 7 (4 items)
+- `busy list -c 3-` lists all the items from number 3 through the end of the list
+- `busy delete -c 3 5 7 9` deletes only the items designated
+- `busy defer -c -` defers the last task
+- `busy edit -c -4` is an error! Use `busy edit -c 1-4` instead
 - `busy manage` allows you to edit the entire queue
 
 Items will always be handled in the order they appear in the queue, regardless of the order the criteria are provided. So for example, if a `pop` command designates some items, they will be moved to the top of the queue in the order, relative to each other, they currently appear in the queue.
 
-The sequence numbers in the `list` command output are from the queue itself. So the `list` command does not modify the sequence numbers, even when item designation is applied.
+The sequence numbers in the `list` command output are from the collection itself. So the `list` command does not modify the sequence numbers, even when item designation is applied.
 
 Tags
 ----
 
 Items can have tags, which are space-separated hashtags in the item description. An item can have no tags, one tag, or more than one tag. For example the following item description has the tag "errands":
 
 ```
 go to the supermarket #errands
 ```
 
-Tags cannot contain punctuation.
+The only punctuation that tags can contain is the hyphen ("-").
 
-Hash tags may be used for item designation, in which case the hash itself ("#") is omitted from the command line. For example, the following command will move all the items with the `#errands` tag to the top of the queue.
+Hash tags may be used as criteria in addition to sequence numbers. For example, the following command will move all the items with the `#errands` tag to the top of the queue.
 
 ```
-busy pop errands
+busy pop -c #errands
 ```
 
-Whitespace-separated item designation criteria are additive -- that is, a logical OR. For example, the following command will delete all the admin tasks, sales tasks, and tasks 3 and 4.
+Whitespace-separated criteria are additive -- that is, a logical OR. For example, the following command will delete all the admin tasks, sales tasks, and tasks 3 and 4.
 
 ```
-busy delete admin sales 3 4
+busy delete -c #admin #sales 3 4
 ```
 
+_Note to self: why does this work? Shouldn't the hash symbol indicate a comment?_
+
 Default item designations
 -------------------------
 
 For the most part, commands that accept item designations default to only act on the top item in the queue. The exceptions are:
 
-- `list` defaults to list the entire queue
-- `pop` defaults to pop the last item in the queue to the top
-- `activate` defaults to activate items for today (more on that below)
+- `list` and `manage` default to handle the entire collection
+- `pop` defaults to pop the last item in the collection to the top
+- `activate` defaults to activate `plan` items for today (more on that below)
 
 Alternate queues
 ----------------
 
-Busy will manage any number of queues, which are entirely separate ordered sets of items. For example, you might have a `shopping` queue for items to buy at the store, and a `movies` queue for films you'd like to watch. The default queue is called `tasks` and has special properties related to planning.
+Busy will manage any number of queues, which are entirely separate sets of items. For example, you might have a `shopping` queue for items to buy at the store, and a `movies` queue for films you'd like to watch. The default queue is called `tasks`.
 
-To designate an alternate queue, use the `--queue` option on a command. For example:
+To designate an alternate queue, enter it right after the command. For example:
 
 ```
-busy add "Skimmed Milk" --queue shopping
-busy top --queue movies
+busy add shopping -d "Skimmed Milk"
+busy list movies
 ```
 
 Managing plans
 --------------
 
-The default `tasks` queue supports several specific commands related to planning -- that is, scheduling tasks for the future. They are `finish`, `defer`, and `activate`. The task-specific commands do not accept a `--queue` modifier, because they only work on the default `tasks` queue. Planned tasks are kept in another special queue called `plans`, and completed tasks are kept in a queue called `done`.
+Busy supports several specific commands related to planning -- that is, scheduling tasks for the future. They are `finish`, `defer`, and `activate`. The task-specific commands handle items in the `plan` state and, in some cases, the `done` state.
 
-The task commands accept item designations. The `defer` and `finish` commands reference the `tasks` queue; the `activate` command references the `plans` queue. The default for `defer` and `finish` is the top item in the `tasks` queue; the default for `activate` is to activate only plans deferred to today or earlier.
+The task commands accept criteria. The `defer` and `finish` commands reference the `todo` collection; the `activate` command references the `plan` collection. The default for `defer` and `finish` is the top item in the collection; the default for `activate` is to activate only plans deferred to today or earlier.
 
 Planning by date
 ----------------
 
 Planning is by date, not time, and is relative to the current date according to the system clock.
 
-In the `defer` command, the date can be specified using the `--to` or `--for` option (they are interchangable). If the options are omitted, then the date can be provided as input.
+In the `defer` command, the date can be specified using the `--timing` option. If the option is omitted, then the date can be provided as input during confirmation.
 
 The date may take any of the following forms:
 
 - A specific date in `YYYY-MM-DD` format, such as `2018-10-28`. Slashes are also acceptable, but the order is always year, then month, then day.
 - A specific date without the year in `MM-DD` format, such as `7-4`, which will defer the item to that date in the future (even if it's in the next year).
 - A specific day of the month as a simple integer, such as `12`, which will defer the item to that day of the month, in either the current month or the next month.
 - An integer, a space, and the word `day` or `days`, such as `4 days`, which will defer the item to that number of days from today.
 - An integer without a space and the letter `d`, such as `4d`, which is a short form of `4 days`.
 - The word `tomorrow`, which is also the default if no date is provided.
 - The word `today`, which is a little odd but obvious.
 
-As an example, the following command will defer tasks 4, 5, and 6 from the `tasks` queue to the date 4 days from today, keeping them in the `plans` queue until that date.
+As an example, the following command will defer tasks 4, 5, and 6 from the `todo` collection to the date 4 days from today, keeping them in the `plan` collection until that date.
 
 ```
-busy defer 4-6 --for 4 days
+busy defer -c 4-6 -t "4 days"
 ```
 
-Note that the `plans` queue is keeping the task information (verbatim from the `tasks` queue) along with the date information (as an absolute date).
+Note that the `plan` collection is keeping the task information (verbatim from the `todo` collection) along with the date information (as an absolute date).
 
-To pull tasks off the `plans` queue and put them back on the `tasks` queue, use the `activate` command. There are two ways to use the `activate` command:
+To pull tasks from the `plan` collection and put them back into the `todo` collection, use the `activate` command. There are two ways to use the `activate` command:
 
-- With no item designation, in which case Busy activates all the tasks scheduled for today or earlier, bringing the `tasks` list up to date
-- With designated items from the `plans` queue; note that the `activate` command accepts item designation from the `plans` queue itself
+- With no criteria, in which case Busy activates all the tasks scheduled for today or earlier, bringing the `todo` list up to date
+- With designated items from the `plan` collection; note that the `activate` command accepts item designation from the `plan` queue itself so use `busy list -s plan` first to get the right list.
 
 Finishing and following up
 --------------------------
 
-Like `defer`, the `finish` command only works on the `tasks` queue. It removes the designated Task (or the top task if none is designated) from the queue and adds it to the `done` queue, with today's date to indicate when it was completed.
+The `finish` command removes the designated Task (or the top task if none is designated) from the `todo` state  and adds it to the `done` state, with today's date to indicate when it was completed.
 
-Optionally, a task can have a followon, which is another task to be added to the queue after the first task is finished. Followons are described in a task using an arrow notation. In the following example, the task "eat" has a followon task "drink":
+Optionally, a task can have a "followon", which is another task to be added as a `todo` after the first task is finished. Followons are described in a task using an arrow notation. In the following example, the task "eat" has a followon task "drink":
 
 ```
 eat --> drink
 ```
 
-Note that the hyphens and whitespace are optional; really the marker that matters for delimiting a followon is the right angle bracket (">"). Also note that right angle bracket is not a valid character in a task description.
+Note that the hyphens and whitespace are optional; really the marker that matters for delimiting a followon is the right angle bracket (">"). Also note that right angle bracket is not a valid character elsewhere in a task description.
 
-When the `finish` command is executed on the task above, the "eat" task will be recorded as "done" and the "drink" task will be added to the bottom of the `tasks` queue.
+When the `finish` command is executed on the task above, the "eat" task will be recorded as "done" and the "drink" task will be added to the top of the `todo` list.
 
-Note that followons can be chained. For example, when the `finish` command is run on the task illustrated below, a new task "drink > be merry" will be added to the queue. Only when that Task is finished will the "be merry" task itself appear on the queue.
+Note that followons can be chained. For example, when the `finish` command is run on the task illustrated below, a new task "drink > be merry" will be added to the `todo` collection`. Only when that Task is finished will the "be merry" task itself appear.
 
 ```
 eat > drink > be merry
 ```
 
 Repeating tasks
 ---------------
 
-A special type of followon is the repeat. In this case, instead of adding the next task to the bottom of the queue, the entire current task -- including the Followon itself -- is entered into the `plans` queue at some point in the future. Repeats allow for easy management of repeating tasks. Some examples follow.
+A special type of followon is the repeat. In this case, instead of adding the next task to the top of the `todo` list, the entire current task -- including the followon itself -- is entered into the `plan` collection at some point in the future. Repeats allow for easy management of repeating tasks. Some examples follow.
 
 - `check email --> repeat in 1 day`
 - `phone mom --> repeat on sunday`
 - `balance the checkbook --> repeat on 6`
 
 The exact syntax for a Repeat is the word "repeat" followed by either "on" or "in" and a relative date phrase -- the same phrases that work with the `defer` command.
 
-Note that the repetition itself only happens on the `finish` command. The completed task (i.e. "check email") is entered in the `done` queue and then the entire task (with the Repeat) is scheduled in the `plans` queue for the appropriate time in the future.
+Note that the repetition itself only happens when the `finish` command is executed. The completed task (i.e. "check email") is entered in the `done` list and then the entire task (with the Repeat) is scheduled in the `plan` list for the appropriate time in the future.
 
 Editing items
 -------------
 
-The `edit` and `manage` commands launch the user's default text editor to directly edit a task, the whole queue, or part of a queue. Note that `edit` and `manage` are identical commands except for their defaults.
+The `edit` and `manage` commands launch the user's default text editor to directly edit a task, the whole queue, or part of a queue. Note that `edit` and `manage` are identical commands except for their default criteria.
 
 The definition of the "default text editor" depends on the OS and configuration but here's the logic:
 
 1. Try the EDITOR environment variable
 1. If that doesn't exist, try the `sensible-editor` command (Ubuntu)
 1. If that doesn't exist, try the `open -W` command (OSX)
 
-You must quit the editor to accept the change back into Busy.
+You must save changes and quit the editor to accept the change back into Busy.
 
-The `edit` command with no criteria will edit the top item in the queue, and the `manage` command with no criteria will edit the entire queue. But it's also possible to designate items to be edited with both commands. The commands do their best to replace the edited items in place in the list order. So if you `edit` or `manage` a tag whose items are recently popped (at the top of the queue), then the edited items will still appear at the top. Even if you add items, they will be inserted after the last item in the edited set, not at the end of the queue. But all the items brought up in the editor will be edited. So if you remove an item in the editor, it will be deleted and the others will be moved up to take its place.
+The `edit` command with no criteria will edit the top item in the list, and the `manage` command with no criteria will edit the entire list. But it's also possible to designate items to be edited with both commands using criteria. The commands do their best to replace the edited items in place in the list order. So if you `edit` or `manage` a tag whose items are recently popped (at the top of the collection), then the edited items will still appear at the top. Even if you add items, they will be inserted after the last item in the edited set, not at the end of the queue. But all the items brought up in the editor will be edited. So if you remove an item in the editor, it will be deleted and the others will be moved up to take its place.
 
 For faster daily use - the Curses UI
 ------------------------------------
 
 Busy suports multiple user interfaces. The command line interface described above is the shell interface. The alternative is the curses UI, which draws an entirely new terminal in the same window.
 
-_We get it - "curses" is a terrible name. It's a reference to the underlying technology. It's likely to change._
+_We get it - "curses" is a terrible name. It's a reference to the underlying technology._
 
-As of now, the curses UI only supports the `tasks` queue. The commands can be triggered with single keystrokes, and only act on their default tasks (usually the top task). The UI always displays the current queue (which is always `tasks` for now) and the current (top) task at the top of the screen.
+In the Curses UI, commands can be triggered with single keystrokes, and only act on their default items (usually the top task). The UI always displays the current queue (which is always `tasks` for now) and the current (top) `todo` item` at the top of the screen.
 
 To invoke the curses UI, type:
 
 ```
 busy curses
 ```
 
-Commands within the UI are shown with a single letter underlined. The underlined letter is the keystroke that will invoke the command. Use `q` to quit. When inside a command, use ctrl-C to cancel the command and return to the main menu.
+Or it's the default so just type:
 
+```
+busy
+```
+
+Commands within the UI are shown with a single letter underlined. The underlined letter is the keystroke that will invoke the command. Use `q` to quit. When inside a command, use ctrl-C to cancel the command and return to the main menu.
 
 Data storage
 ------------
 
-Busy keeps the queues in plain text files, so if the tool doesn't do something you want, you may edit the files. The files are in a directory together, referred to as the "root". Each file is the name of the queue with a `.txt` extension. If a required file is missing, it will be created automatically. So typically, the root includes `tasks.txt`, `plans.txt`, `done.txt`, and any number of custom queue files.
+Busy keeps the collections in plain text files, so if the tool doesn't do something you want, you may edit the files. The files are in a directory together, referred to as the "root". Each file is the named according to the following convention:
 
-Technically, Busy data files are pipe-delimited data files, though `tasks.txt` and any custom queues only have one field ("description") while `plans.txt` and `done.txt` have only two fields (date and description).
+```
+<queue>.<state>.psv
+```
+
+If a required file is missing, it will be created automatically. So typically, the root includes `tasks.todo.psv`, `tasks.plan.psv`, `tasks.done.txt`, and any number of custom queue files.
+
+Technically, Busy data files are pipe-delimited data files, though the `todo` collections only have one field ("description") while the `plan` and `done` files have only two fields (date and description).
 
 Busy is not a database (yet). There is no support for managing separate fields in the Busy tool itself.
 
 The root is designated in one of the following ways, which are tried in order.
 
 - The `--root` option on any command
 - The `BUSY_ROOT` environment variable, if no `--root` option is provided
 - A directory at `~/.busy`, which will be generated as needed if no `--root` option or `BUSY_ROOT` environment variable are provided,
 
 Note that the `--root` option must come after `busy` but command-specific options (`--yes`, `--to`, `--for`, and `--queue`) must come after commands.
 
 The following example shows the `--root` option with command-specific options on the same command line.
 
 ```
-busy --root ~/.config/busy defer --to tuesday
+busy --root ~/.config/busy defer --t tuesday
 ```
 
-Note that Busy does not support concurrency in any form. If two commands are executing at the same time, they might overwrite each other. Overwriting is especially risky with the `edit` command, which keeps the user's editor open until they close it.
+Note that Busy does not support concurrency or locking in any form. If two commands are executing at the same time, they might overwrite each other. Overwriting is especially risky with the `edit` and `manage` commands, which keeps the user's editor open until they close it.
 
-The format is designed to be simple (i.e. non-default queues are really just lists of items) but not idiot-proof. Experimentation might result in unintended consequences.
+The format is designed to be simple but not idiot-proof. Experimentation might result in unintended consequences.
 
 Development
 ===========
 
 The code is intended to demonstrate some Python best practices:
 
 - *Object-oriented* with classes and subclasses.
 - *Dynamic configuration* using a unique approach we call "class families" - for example, the names of the commands are properties of the command classes, not in a big "if" statement.
-- *Extensive testing* with >90% test coverage, guaranteed by CI.
+- *Extensive testing* with high test coverage, guaranteed by CI.
 - *Leverage the standard library* by requiring 3rd party PIP modules for development, but not for usage.
 
 To set everything up:
 
-```
-sudo pip3 install vernum coverage pycodestyle twine
-```
+- Requires Python 3.6.5 or later
+- Clone the repo and CD into it
+- Set up a venv if that's your thing
+- `pip install -r requirements/freeze.txt`
+- To run it: `python -m busy` ...
 
-To get the full repo:
-
-```
-git clone git@gitlab.com:fpotter/tools/busy.git
-```
 We use Visual Studio Code to build Busy, so there is a VS Code configuration file in the repository.
 
 Then to run the test suite:
 
 ```
 make test
 ```
@@ -409,15 +463,15 @@
 
 And to check style:
 
 ```
 make style
 ```
 
-_Note to self: To publish a new build, use 'vernum' with 'major', 'minor', or 'patch' depending on how major the changes were since the last build. Then push. GitLab allows you to publish to PyPI in its UI, and only when Vernum has been run._
+_Note to self: To publish a new build, use 'vernum' with 'major', 'minor', or 'patch' depending on how major the changes were since the last build. Then push. GitLab allows you to publish to PyPI via CI/CD, and only when Vernum has been run._
 
 Command summary
 ===============
 
 Below is a reference list of all commands, handy to correlate the one-letter version with the full version. The one-letter version is used in the curses UI, and is an alternative option in the shell UI. Some of the listed commands are yet to be implemented; they are listed here merely to reserve their names.
 
 | Short | Full |
@@ -426,17 +480,16 @@
 | c | activate |
 | d | delete |
 | e | edit |
 | f | defer |
 | l | list |
 | m | manage |
 | n | finish |
-| p | pop |
-| q | quit (only in interactive UI) |
+| o | pop |
+| p | print |
+| q | quit |
 | r | drop |
-| s | shuffle |
+| s | skip |
 | t | tags |
 | u | queues (list) |
 | w | switch (queues) |
 |   | curses (only in shell UI) |
-|   | top |
-
```

### Comparing `busy-3.4.6/busy/command/activate_command.py` & `busy-5.0.0/busy/command/activate_command.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,52 @@
-from ..command.command import TodoCommand
-from busy.util import date_util
-
+from dataclasses import dataclass
 
-# The Activate command is unusal because any criteria apply to the plans queue,
-# not the main tasks queue.
+from busy.command.command import QueueCommand
+from busy.util import date_util
 
 
 def is_today_or_earlier(plan):
-    return plan.date <= date_util.today()
+    return plan.plan_date <= date_util.today()
 
-class ActivateCommand(TodoCommand):
 
+@dataclass
+class ActivateCommand(QueueCommand):
+
+    timing: str = ""
+    yes: bool = None
+    collection_state: str = 'plan'
     name = 'activate'
     key = 'c'
-
-
-    # Change in this version: "today" is the default if no criteria are given,
-    # not a specific option.
+    default_criteria = [is_today_or_earlier]
 
     @classmethod
     def set_parser(self, parser):
         super().set_parser(parser)
-        self._add_criteria_arg(parser)
+        # parser.add_argument('--timing', '-t', default='today')
         self._add_confirmation_arg(parser)
 
-
     def clean_args(self):
+        # def update_timing():
+        #     self.timing = self.ui.get_string("Timing", "today")
         super().clean_args()
-        self._ui.output('\n'.join(self._strings))
-        self.confirm(f"Activate {self.count()}")
-
-
-    # Indices behave differently, because they apply to the plans queue. We're
-    # also going to do the defaulting here.
-    #
-    # TODO: Create a simpler way to handle the confirmation on another queue.
-
-    @property
-    def _indices(self):
-        if not hasattr(self, '_indices_'):
-            if self.is_omitted('criteria'):
-                indices = self.queue.plans.indices(is_today_or_earlier)
-                self._indices_ = indices
-            else:
-                self._indices_ = self.queue.plans.select(*self._criteria)
-        return self._indices_
-
-    @property
-    def _strings(self):
-        if not hasattr(self, '_strings_'):
-            self._strings_ = self.queue.plans.strings(*self._indices)
-        return self._strings_
-
+        # For now, handling criteria as normal
+        if self.selection:
+            if not self.provided('yes'):
+                items = self.collection.items(self.selection)
+                self.ui.output('\n'.join([str(i) for i in items]))
+                intro = f"Activate {self.count()}"
+                # self.confirm(intro, update_timing)
+                self.confirm(intro)
 
-    @TodoCommand.wrap
+    @QueueCommand.wrap
     def execute(self):
-        if not self._indices:
+        if not self.selection:
             self.status = "Activated nothing"
-        elif not self._namespace.yes:
+        elif self.yes is False:
             self.status = "Activate command canceled"
         else:
-            activated = self.queue.activate(*self._indices)
-            self.status = f"Activated {self.count(activated)}"
+            todos = self.storage.get_collection(self.queue)
+            activated = self.collection.delete(self.selection)
+            for item in activated:
+                item.state = 'todo'
+            todos[0:0] = activated
+            self.status = f"Activated {self.count()}"
```

### Comparing `busy-3.4.6/busy/command/delete_command.py` & `busy-5.0.0/busy/command/delete_command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from ..command.command import QueueCommand
+from dataclasses import dataclass
 
+from busy.command.command import CollectionCommand
 
-class DeleteCommand(QueueCommand):
 
+@dataclass
+class DeleteCommand(CollectionCommand):
+
+    yes: bool = None
     name = 'delete'
     key = 'd'
-    prompt = 'd)elete'
+    default_criteria = [1]
 
     @classmethod
     def set_parser(self, parser):
         super().set_parser(parser)
-        parser.add_argument('--yes', action='store_true')
-        self._add_criteria_arg(parser)
-
-
-    # TODO: Make a convenience method to set the default
+        parser.add_argument('--yes', action='store_true', default=None)
 
     def clean_args(self):
         super().clean_args()
-        if self.is_omitted('criteria'):
-            self._namespace.criteria = [1]
-        if self._indices:
-            self._ui.output('\n'.join(self._strings))
+        if self.selection:
+            items = self.collection.items(self.selection)
+            self.ui.output('\n'.join([str(i) for i in items]))
             self.confirm(f"Delete {self.count()}")
 
     # Assume the indices have been already set, before confirmation.
 
-    @QueueCommand.wrap
+    @CollectionCommand.wrap
     def execute(self):
-        if self._namespace.yes:
-            deleted = self.queue.delete(*self._indices)
+        if self.yes:
+            deleted = self.collection.delete(self.selection)
             self.status = f"Deleted {self.count(deleted)}"
         else:
             self.status = "Delete command canceled"
```

### Comparing `busy-3.4.6/busy/command/list_command.py` & `busy-5.0.0/busy/command/add_command.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from ..command.command import QueueCommand
+from dataclasses import dataclass
 
+from busy.command.command import QueueCommand
+from busy.model.item import Item
 
-class ListCommand(QueueCommand):
 
-    name = 'list'
-    # key = "l"
+@dataclass
+class AddCommand(QueueCommand):
+
+    description: str = ""
+    name = 'add'
+    key = 'a'
 
     @classmethod
     def set_parser(self, parser):
         super().set_parser(parser)
-        self._add_criteria_arg(parser)
+        parser.add_argument('--description', '-d', nargs='?')
+
+    def clean_args(self):
+        super().clean_args()
+        if not self.provided('description'):
+            self.description = self.ui.get_string("Description")
 
     @QueueCommand.wrap
     def execute(self):
-        listed = self.queue.list(*self._criteria)
-        if len(listed) == 1:
-            self.status = f"Listed 1 Item"
-        elif listed:
-            self.status = f"Listed {str(len(listed))} Items"
+        if self.description:
+            item = Item(self.description)
+            self.collection.insert(0, item)
+            self.status = "Added: " + self.description
         else:
-            self.status = "Listed nothing"
-        fmtstring = "{0:>6}  " + self.queue.itemclass.listfmt
-        return "\n".join([fmtstring.format(i, t) for i, t in listed])
-
-
+            self.status = "Nothing added"
```

### Comparing `busy-3.4.6/busy/handler.py` & `busy-5.0.0/busy/handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,103 +6,92 @@
 # there. Keeping the imports in one place allows the class families to be more
 # modular.
 #
 # A Handler instance provides the following properties. For the most part, these
 # properties are how commands access other class families. Remember that the
 # Namespace from the Handler is the original Namespace, so use the one passed in
 # to the execute() method of the Command for actual usage in an interactive UI.
-# Also, the Handler doesn't hold a queue property, because it is only used by
-# certain commands. Instead, get your queue from your root yourself!
-#
-# namespace - The argparse Namespace from the original parsing of the command
-# line
-#
-# root - The Root object for retrieval and storage of items. This is the main
-# way that a command gets its root.
-#
-# ui - The UI instance being implemented. This is the main way a command gets
-# its UI.
-#
-# command - The original Command instance being implemented. Interactive UIs
-# might instantiate other Commands.
 
 
-from argparse import ArgumentParser
 import sys
+from argparse import ArgumentParser
 from pathlib import Path
 from sys import argv
 
 from busy.command.command import Command
-from busy.ui.ui import UserCancelError
-from busy.ui.ui import UI
-from busy.root.file_system_root import FileSystemRoot
+from busy.storage.file_storage import FileStorage
+from busy.ui.ui import UI, UserCancelError
 from busy.util.python_version import confirm_python_version
 
 PYTHON_VERSION = (3, 6, 5)
 
+
 def main(*args):
-    if not args:
-        args = argv[1:]
-    confirm_python_version(PYTHON_VERSION) 
-    parser = get_parser()      
+    """Start everything from the command line
+
+    args - optional entry point for testing
+    """
+    args = args if args else argv[1:]
+    confirm_python_version(PYTHON_VERSION)
+    parser = get_parser()
     namespace = parser.parse_args(args)
     try:
         handler = Handler(namespace)
         handler.execute()
     except (RuntimeError, ValueError) as error:
         print(f"Error: {str(error)}")
 
+
 def get_parser():
+    """Return the CLI parser"""
     parser = ArgumentParser(prog='busy')
-    parser.add_argument('--root', action='store', \
-        help='file system path to busy data', \
-        default=None)
+    parser.add_argument('--root', action='store',
+                        help='file system path to busy data',
+                        default=None)
     subparsers = parser.add_subparsers(dest='command')
     for command in Command.family_members('name'):
         key = command.get_member_attr('key')
         aliases = [key] if key else []
         subparser = subparsers.add_parser(command.name, aliases=aliases)
         command.set_parser(subparser)
     return parser
 
 
 class Handler():
 
     def __init__(self, namespace):
-        self.namespace = namespace
-        self.root = FileSystemRoot(namespace.root)
-        command_class = Command.family_member('name', namespace.command or 'curses')
+        """
+        namespace - ArgParse Namespace from initial CLI entry
+        """
+        nsvars = vars(namespace)
+        self.storage = FileStorage(nsvars.pop('root'))
+        command = nsvars.pop('command')
+        command = command if command else 'curses'
+        command_class = Command.family_member('name', command)
         if not command_class:
-            raise RuntimeError(f"Unknown command {namespace.command}")
-        self.ui = UI.family_member('name', command_class.ui)(self)
-        self.command = command_class(root=self.root, ui=self.ui, \
-                                     namespace=self.namespace)
-
-    # Handle the command and output its final status
+            raise RuntimeError(f"Unknown command {command}")
+        self.ui = UI.family_member('name', command_class.uitype)(self)
+        self.command = command_class(
+            storage=self.storage, ui=self.ui, **nsvars)
 
     def execute(self):
+        """Handle the command and output its final status"""
         result = self.command.execute()
         if result:
             print(result)
         if self.command.status:
             print(self.command.status)
 
-
     # Some useful methods so other components don't need to import from
     # different class families
-    
+
     def get_commands(self, *attributes):
         return Command.family_members(*attributes)
 
-    def get_command_values(self, *attributes):
-        return Command.family_attrs(*attributes)
-
-
-    # A method for commands within interactive UIs. Use our own root but the UI
+    # A method for commands within interactive UIs. Use our own storage but the UI
     # is passed in. Returns None if attribute value doesn't resolve.
-    
+
     def get_command(self, attribute, value, **kwargs):
         member = Command.family_member(attribute, value)
         if member:
-            args = {'root':self.root} | kwargs
+            args = {'storage': self.storage} | kwargs
             return member(**kwargs)
-
```

### Comparing `busy-3.4.6/busy/selector.py` & `busy-5.0.0/busy/util/selector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 
 
 class Selector:
 
     CRITERIUM_TYPES = []
 
     @classmethod
@@ -9,14 +10,15 @@
         self.CRITERIUM_TYPES.append(criterium_type)
 
     @classmethod
     def get_criterium(self, word):
         for criterium_type in self.CRITERIUM_TYPES:
             if criterium_type.match(word):
                 return criterium_type(word)
+        raise RuntimeError(f"Invalid selection criterium {word}")
 
     def __init__(self, args):
         self.criteria = [c for c in [self.get_criterium(w) for w in args] if c]
 
     def hit(self, index, value, count):
         if self.criteria:
             return any([c.hit(index, value, count) for c in self.criteria])
@@ -43,15 +45,15 @@
 
 Selector.add_criterium_type(NumberCriterium)
 
 
 class RangeCriterium:
 
     def match(word):
-        return '-' in str(word)
+        return isinstance(word, str) and bool(re.match(r'^\d*\-\d*$', word))
 
     def __init__(self, word):
         split = word.split('-')
         self.start = int(split[0]) - 1 if split[0] else None
         self.end = int(split[1]) - 1 if split[1] else None
 
     def hit(self, index, value, count):
@@ -65,27 +67,30 @@
 
 Selector.add_criterium_type(RangeCriterium)
 
 
 class TagCriterium:
 
     def match(word):
-        return str(word).isidentifier()
+        return isinstance(
+            word, str) and bool(
+            re.match(r'^\#[a-zA-Z0-9\-]+$', word))
 
     def __init__(self, word):
         self.tag = str(word).lower()
 
     def hit(self, index, value, count):
-        return self.tag in value.tags
+        return self.tag in str(value).lower().split()
 
 
 Selector.add_criterium_type(TagCriterium)
 
 
 class FunctionCriterium:
+    """Evaluates a function against the value (not the index)"""
 
     def match(arg):
         return callable(arg)
 
     def __init__(self, arg):
         self.func = arg
```

### Comparing `busy-3.4.6/busy/ui/curses_ui.py` & `busy-5.0.0/busy/ui/curses_ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,45 +9,35 @@
 # Status region (_statuswin) - 6 lines at the top. Current queue name, current
 # task, some blank space, status of the most recent operation, and input prompt
 # for the main command.
 #
 # List region (_listwin) - Takes up the space between the other two regions.
 # Shows mostly lists of tasks for confirmation and/or management.
 #
-# Edit region (_editwin) - 2 lines at the bottom. Used for editing of individual
-# task descriptions, such as when adding a new task to the queue.
+# Edit region (_editwin) - 2 lines at the bottom. Used for editing of
+# individual task descriptions, such as when adding a new task to the queue.
 
 
 import curses
 from argparse import Namespace
 from string import capwords
 from time import sleep
 
-from busy.ui.ui import TerminalUI
-from busy.ui.ui import UserCancelError
-from busy.ui.ui import Prompt
-from busy.ui.ui import Chooser
+from busy.ui.ui import Chooser, Prompt, TerminalUI, UserCancelError
 
 
 class CursesUI(TerminalUI):  # pragma: nocover
 
     name = "curses"
 
     def start(self):
         self._mode = "WORK"
-        # Set up the main prompt once for simplicity
-        # keynames = self.handler.get_command_values('key', 'name')
-        # keynames.add(('q', 'quit'))
-        # skeynames = sorted(keynames, key=lambda kn: kn[1])
-        # self._main_prompt = Prompt(choices=skeynames)
-
-        # Set up the main command chooser
         chooser = Chooser()
         commands = self.handler.get_commands('key')
-        scommands = sorted(commands, key=lambda c:c.name)
+        scommands = sorted(commands, key=lambda c: c.name)
         for command in scommands:
             chooser.add_choice(
                 keys=[command.key],
                 words=[command.name],
                 action=command
             )
         chooser.add_choice(keys=['q'], words=['quit'])
@@ -66,22 +56,21 @@
         """
         window = self._statuswin
         if prompt.intro:
             window.addstr(prompt.intro + " ", curses.color_pair(3))
         if prompt.default:
             window.addstr(f"[{prompt.default}] ", curses.color_pair(3))
         for choice in prompt.choices:  # TODO: Deal with raw prompt case
-            if choice.word==prompt.default:
+            if choice.word == prompt.default:
                 continue
             pre, it, post = choice.word.partition(choice.key)
             window.addstr(pre, curses.color_pair(3))
             window.addstr(it, curses.A_UNDERLINE + curses.color_pair(3))
             window.addstr(post + " ", curses.color_pair(3))
-        window.addstr("--> ", curses.color_pair(3))
-
+        window.addstr(": ", curses.color_pair(3))
 
     # TODO: Use a better editing component
     #
     # NOTE: get_string assumes that everything has been cleared and we are in
     # the right place.
 
     def get_string(self, intro, default=""):
@@ -97,17 +86,17 @@
         return value
 
     def get_option(self, chooser):
         """Get a 1-keystroke choice from the user"""
         self._update_status(chooser)
         key = self._get_key()
         return chooser.choice_by_key(key)
-    
+
     def term_loop(self, fullwin):
-        self._queue_name = "tasks"
+        self.queue = "tasks"
         curses.init_color(curses.COLOR_BLACK, 200, 200, 200)
         curses.init_pair(1, curses.COLOR_CYAN, curses.COLOR_BLACK)
         curses.init_pair(2, curses.COLOR_YELLOW, curses.COLOR_BLACK)
         curses.init_pair(3, curses.COLOR_GREEN, curses.COLOR_BLACK)
         h, w = fullwin.getmaxyx()
         self._statuswin = curses.newwin(5, w-2, 1, 1)
         self._descwin = curses.newwin(h-8, w-2, 7, 1)
@@ -120,59 +109,59 @@
             self._update_status(self._command_prompt)
             try:
                 key = self._get_key()
             except UserCancelError:
                 break
             if key == "q":
                 break
-            command = self.handler.get_command('key', key, ui=self, \
-                    root=self.handler.root, queue_name=self._queue_name)
+            command = self.handler.get_command(
+                'key', key, ui=self, storage=self.handler.storage,
+                queue=self.queue)
             if not command:
                 self._status = f"Invalid command {key}"
                 continue
             command_name = capwords(command.name)
             self._status = f"{command_name} in progress"
             self._update_status()
             try:
                 result = command.execute()
                 self._status = command.status or ""
-                if hasattr(command, 'queue_name'):
-                    self._queue_name = command.queue_name
+                if hasattr(command, 'queue'):
+                    self.queue = command.queue
             except UserCancelError:
                 self._status = f"{command_name} command canceled"
 
     def _update_status(self, prompt=None):
-        queue = self.handler.root.get_queue(self._queue_name)
+        collection = self.handler.storage.get_collection(self.queue)
         self._statuswin.clear()
         self._statuswin.move(0, 0)
         self._statuswin.addstr("Queue: ", curses.color_pair(1))
-        self._statuswin.addstr(capwords(self._queue_name), curses.A_BOLD)
+        self._statuswin.addstr(capwords(self.queue), curses.A_BOLD)
         self._statuswin.move(1, 0)
-        self._statuswin.addstr("Top:   ", curses.color_pair(1))
-        self._statuswin.addstr(str(queue.top()) or '', curses.A_BOLD)
+        self._statuswin.addstr("Todo:   ", curses.color_pair(1))
+        self._statuswin.addstr(
+            str(collection[0] if collection else ''), curses.A_BOLD)
         self._statuswin.move(3, 0)
         self._statuswin.addstr(self._status, curses.color_pair(2))
         self._statuswin.move(4, 0)
         if prompt:
             self.write_prompt(prompt)
         cursor = self._statuswin.getyx()
         self._statuswin.refresh()
         self._statuswin.move(*cursor)
 
     # Convenience method to get one keystroke from the user.
-    #     
+    #
     def _get_key(self):
         try:
             key = self._statuswin.getkey()
         except (KeyboardInterrupt, curses.error):
             raise UserCancelError
-        # self._statuswin.addstr(key)
         return key
 
-
     # def listmode(self):
     #     length = len(list.splitlines())
     #     if length:
     #         listpad = curses.newpad(length, curses.COLS)
     #         listpad.addstr(list)
     #         self.listmode = True
     #         listpad.move(cursor, 0)
```

### Comparing `busy-3.4.6/busy/ui/shell_ui.py` & `busy-5.0.0/busy/ui/shell_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# The UI to execute one command passed in through the shell. There will be
-# limited interactivity, if the user omits an argument on the command line, but
-# otherwise this is a run and done situation.
-#
-# The code for argparse lives at https://github.com/python/cpython/blob/main/Lib/argparse.py
-
-
 from argparse import ArgumentParser
 from io import StringIO
 
 from wizlib.rlinput import rlinput
 
 from busy.ui.ui import TerminalUI
 from busy.ui.ui import UserCancelError
 from busy.ui.ui import Prompt
 
 
 class ShellUI(TerminalUI):
 
+    """The UI to execute one command passed in through the shell. There will be
+    limited interactivity, if the user omits an argument on the command line,
+    but otherwise this is a run and done situation.
+    """
+
     name = "shell"
 
     def output(self, intro=""):
         """Print some regular output"""
         if intro:
             print(intro)
 
@@ -28,25 +26,24 @@
         prompt = Prompt(intro=intro)
         return rlinput(prompt=self._prompt_string(prompt), default=default)
 
     def get_option(self, chooser):
         """Get a choice from the user"""
         key = rlinput(prompt=self._prompt_string(chooser))
         return chooser.choice_by_key(key)
-    
+
     def _prompt_string(self, prompt):
-        result = ""
+        result = []
         if prompt.intro:
-            result += prompt.intro + " "
+            result.append(prompt.intro)
         if prompt.default:
-            result += f"[{prompt.default}] "
+            result.append(f"[{prompt.default}]")
         for choice in prompt.choices:
-            if choice.word==prompt.default:
+            if choice.word == prompt.default:
                 continue
             pre, it, post = choice.word.partition(choice.key)
-            result += f"{pre}({it}){post} "
-        return result + "--> "
+            result.append(f"{pre}({it}){post}")
+        return " ".join(result) + ": "
 
     def write_prompt(self, prompt):
         """Output the prompt"""
-        print(self._prompt_string(prompt) , end="")
-
+        print(self._prompt_string(prompt), end="")
```

### Comparing `busy-3.4.6/busy/ui/tcl_ui/edit_task_widget.py` & `busy-5.0.0/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.6/busy/ui/tcl_ui/get_item_widget.py` & `busy-5.0.0/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.6/busy/ui/ui.py` & `busy-5.0.0/busy/ui/ui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Abstract classes for UIs. The idea here is to allow many different user
 # interfaces (shell, curses, Slack, etc) to drive the same data model without
 # the data model needing specific UI knowledge.
 #
-# The UI keeps a reference to the Handler. The Handler will bring a Command with
-# it, and this is the main root command. In the case of a Shell-type UI, that is
-# the command to be executed. In the case of an interactive UI, it's really just
-# a placeholder; the UI will instantiate other commands as it proceeds. But the
-# Handler won't know about those.
+# The UI keeps a reference to the Handler. The Handler will bring a Command
+# with it, and this is the main root command. In the case of a Shell-type UI,
+# that is the command to be executed. In the case of an interactive UI, it's
+# really just a placeholder; the UI will instantiate other commands as it
+# proceeds. But the Handler won't know about those.
 #
 # Commands might call back to the UI for confirmations or arguments that are
 # previously omitted, using the get_ methods.
 
 #
 # UI end classes must implement the following interface:
 #
@@ -21,72 +21,70 @@
 # short running (in the case of a shell UI) or long-running (in the case of an
 # interactive UI).
 #
 # output(intro=""): Output some multi-line text explaining an action, usually a
 # list of items being acted upon.
 #
 # get_string(prompt, default=""): For arguments that are omitted, get a string
-# from the user. The prompt is just a word (like "Description") telling the user
-# what to input.
+# from the user. The prompt is just a word (like "Description") telling the
+# user what to input.
 #
-# get_confirmation(verb): For delete-oriented commands to
-# confirm with the user before proceeding. Verb is what we're asking the user to
-# confirm. Description can be multiple lines, as with get_string. Returns a
-# boolean saying whether the action is confirmed.
+# get_confirmation(verb): For delete-oriented commands to confirm with the user
+# before proceeding. Verb is what we're asking the user to confirm. Description
+# can be multiple lines, as with get_string. Returns a boolean saying whether
+# the action is confirmed.
 
-import subprocess
-from tempfile import NamedTemporaryFile
-from pathlib import Path
-import shutil
 import os
 import re
-from io import StringIO
+import shutil
+import subprocess
 from dataclasses import dataclass, field
 from enum import Enum
+from io import StringIO
+from pathlib import Path
+from tempfile import NamedTemporaryFile
 
-from busy.model.item import write_items
-from busy.model.item import read_items
+from busy.model.collection import Collection
 from busy.util.class_family import ClassFamily
 
 
-
 @dataclass
 class Choice:
     """One option of several"""
 
-    keys:list[str] = field(default_factory=list)
-    words:list[str] = field(default_factory=list)
-    action:object = None
+    keys: list[str] = field(default_factory=list)
+    words: list[str] = field(default_factory=list)
+    action: object = None
 
     @property
     def key(self):
         return self.keys[0]
-    
+
     @property
     def word(self):
         return self.words[0]
 
     def hit_key(self, key):
         return key in self.keys
 
     def hit_word(self, word):
         return word in self.words
-    
+
     def call(self, *args, **kwargs):
         if callable(self.action):
             return self.action(*args, **kwargs)
 
 
 @dataclass
 class Prompt:
     """Tell the user what kind of input to provide"""
 
-    intro:str = ""
-    default:str = ""
-    choices:list = field(default_factory=list)
+    intro: str = ""
+    default: str = ""
+    choices: list = field(default_factory=list)
 
 
 @dataclass
 class Chooser(Prompt):
     """Hold a set of choices and get the result"""
 
     def add_choice(self, *args, **kwargs):
@@ -105,64 +103,80 @@
         choice = next(iter(chosenlist), None)
         if callable(choice):
             return choice()
         else:
             return choice
 
 
+@dataclass
 class UI(ClassFamily):
 
-    def __init__(self, handler=None):
-        self.handler = handler
+    handler: object
 
     def get_chooser(self, *args, **kwargs):
         """Return a chooser that can be set up with options"""
         return Chooser(*args, **kwargs)
-    
+
     # TODO: Make start an abstract method
     def start(self):
         pass
 
     # TODO: Make get_option an abstract method
-    def get_option(self, chooser:Chooser):
+    def get_option(self, chooser: Chooser):
         """Get an option from a list from the user"""
         pass
 
     # TODO: Make get_string an abstract method
     def get_string(self, intro, default=""):
         """Get a string value from the user"""
         pass
 
+    def edit_items(self, collection: Collection, indices):
+        pass
 
 # Terminal UIs include Shell and Curses, since both will rely on a
 # terminal-based editor for the e.g. Manage command.
 
+
 class TerminalUI(UI):
 
     # A convenience method to get a full textual prompt for a string input
 
     def full_prompt(self, prompt, default=None):
         if default:
             return f'{prompt} [{default}]: '
         else:
             return f'{prompt}: '
 
-
-    def edit_items(self, itemclass, *items):
+    @staticmethod
+    def edit_text(text):
         commands = [['sensible-editor'], ['open', '-W']]
         with NamedTemporaryFile(mode="w+") as tempfile:
-            write_items(tempfile, *items)
+            tempfile.write(text)
             tempfile.seek(0)
             command = [os.environ.get('EDITOR')]
             if not command[0] or not shutil.which(command[0]):
                 iterator = (c for c in commands if shutil.which(c[0]))
                 command = next(filter(None, iterator), None)
                 if not command:
-                    raise RuntimeError("A text editor at the $EDITOR environment variable is required")
+                    raise RuntimeError(
+                            "A text editor at the $EDITOR " +
+                            "environment variable is required")
             subprocess.run(command + [tempfile.name])
             tempfile.seek(0)
-            new_items = read_items(tempfile, itemclass)
-            return new_items
+            return tempfile.read()
+
+    def edit_items(self, collection: Collection, indices):
+        with StringIO() as oldio:
+            collection.write_items(oldio, indices)
+            oldio.seek(0)
+            oldtext = oldio.read()
+        newtext = self.edit_text(oldtext)
+        with StringIO() as newio:
+            newio.write(newtext)
+            newio.seek(0)
+            newitems = collection.read_items(newio, indices)
+        return newitems
 
 
 class UserCancelError(Exception):
     pass
```

### Comparing `busy-3.4.6/busy/util/class_family.py` & `busy-5.0.0/busy/util/class_family.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# A class family is a set of class definitions that use single inheritance (each
-# subclass inherits from only one parent) and often multiple inheritance
-# (subclasses can inherit from subclasses). So it's a hierarchy of classes, with
-# one super-parent at the top.
+# A class family is a set of class definitions that use single inheritance
+# (each subclass inherits from only one parent) and often multiple inheritance
+# (subclasses can inherit from subclasses). So it's a hierarchy of classes,
+# with one super-parent at the top.
 #
 # We offer a way for members of the family to declare themselves simply by
 # living in the right package location. Then those classes can be instantiated
-# using keys or names, without having to be specifically called. The members act
-# independently of each other.
+# using keys or names, without having to be specifically called. The members
+# act independently of each other.
 #
 # What we get, after importing everything and loading it all, is essentially a
 # little database of classes, where class-level properties become keys for
 # looking up member classes. So, for example, we can have a family of commands,
 # and use a command string to look up the right command.
 #
 # Ultimately, the super-parent of the family -- the class at the top of the
@@ -23,31 +23,29 @@
 #
 # In the process of loading and querying the class family, we need to *avoid*
 # inheritance of attributes. There might be abstract intermediary classes that
 # don't want to play. So we use __dict__ to ensure we're only seeing the
 # atttributes that are defined on that specific class.
 
 
-from pathlib import Path
 from importlib import import_module
-from re import match
 from inspect import getmodule
+from pathlib import Path
+from re import match
 
 
 class ClassFamily:
 
-
     # Return an attribute of this specific class, not inherited.
 
     @classmethod
     def get_member_attr(self, attribute):
         if attribute in self.__dict__:
             return self.__dict__[attribute]
 
-
     # True or False: This class has all the attributes provided. Return True if
     # no attributes provided. Use __subclasses__ so we only look at direct
     # descendents, and __dict__ so we only look at attributes defined here (not
     # inherited).
 
     @classmethod
     def has_member_attrs(self, *attributes):
@@ -56,99 +54,75 @@
         matches = [a in self.__dict__ for a in attributes]
 
         # Python's all() function returns True if the list is empty. So we kill
         # two birds with one stone here - get a hit if there are no attributes,
         # and avoid the empty-matches problem.
         return all(matches + list(attributes))
 
-
     # Return a set of myself and all my descendents that have certain
     # attributes. If no attribute names are provided, return the entire family.
 
     @classmethod
     def family_members(self, *attributes):
 
         # Put myself into a set if I qualify
         hits = {self} if self.has_member_attrs(*attributes) else set()
 
         # Go through my subclasses
         for kid in self.family_children():
 
             # Call the same function on each subclass
             hits |= kid.family_members(*attributes)
-        
+
         # Send it back
         return hits
 
-
-    # Return a set of tuples of all the values of a specific attribute that
-    # exist in the family. The set avoids repetition of values in the result. We
-    # recognize that the method name has cultural implications, and we find that
-    # fact ironic and funny.
-
     @classmethod
-    def family_attrs(self, *attributes):
-
+    def family_attrs(self, attribute):
+        """
+        Return a set of all the values of a specific attribute that exist in
+        the family. The set avoids repetition of values in the result.
+        """
         # Put myself into a set if I qualify
-        if self.has_member_attrs(*attributes):
-            values = {tuple(self.get_member_attr(a) for a in attributes)}
+        if self.has_member_attrs(attribute):
+            values = {self.get_member_attr(attribute)}
         else:
             values = set()
 
         # Go through my subclasses
         for kid in self.family_children():
 
             # Call the same function on each subclass
-            values |= kid.family_attrs(*attributes)
-        
+            values |= kid.family_attrs(attribute)
+
         # Send it back
         return values
 
-
-        # Start with an empty set
-        result = set()
-
-        # If I have the provided attribute, get its value. Use __dict__ rather
-        # than hasattr() and getattr() to refer only to myself, rather than
-        # inherited attributes.
-        for attribute in attributes:
-            if attribute in self.__dict__:
-                result |= {self.__dict__[attribute]}
-
-        # Go through my subclasses, collecting their values
-        for kid in self.family_children():
-            result |=  kid.family_values(attribute)
-        
-        # Return it
-        return result
-
-
     # Return a specific family member that has a specified value of an
     # attribute. Assume that there is only one, so return it as soon as it's
     # found.
 
     @classmethod
     def family_member(self, attribute, value):
 
         # See if I qualify, and if so, return myself. Use __dict__ rather than
-        # hasattr() and getattr() to refer only to myself, rather than inherited
-        # attributes.
+        # hasattr() and getattr() to refer only to myself, rather than
+        # inherited attributes.
         if attribute in self.__dict__:
             if self.__dict__[attribute] == value:
                 return self
-            
+
         # Go through the subclasses, doing the same. The return statement will
-        # exit the loop, so we get out as soon as we find one, without having to
-        # evaluate others.
+        # exit the loop, so we get out as soon as we find one, without having
+        # to evaluate others.
         for kid in self.family_children():
             found = kid.family_member(attribute, value)
             if found:
                 return found
 
-
     # Import the whole family, so they show up as subclasses. Then return this
     # classes subclasses. This obviates the need to import everything at
     # initialization. It happens when needed, and only once.  Family members
     # must be in modules (files) in the same directory as the parent (me).
     # Furthermore, all the files in that directory will be imported. The only
     # exception is a file with the same name as myself, to avoid circular
     # imports. This is a private method, intended to be called when needed.
@@ -170,8 +144,7 @@
                     import_module(f'{module_name}.{import_file.stem}')
 
             # Prevent it from needing to run again
             self._family_imported = True
 
         # Return the subclasses (children)
         return self.__subclasses__()
-
```

### Comparing `busy-3.4.6/busy/util/date_util.py` & `busy-5.0.0/busy/util/date_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 # Various utilities related to date handling
 
+import functools
+import re
 from datetime import date as Date
 from datetime import datetime as DateTime
 from datetime import timedelta as TimeDelta
-import re
-import functools
-
 
 # Isolate the today function so it can easily be patched for testing.
 
 today = Date.today
 
 
 # The string format we always use to express a date is YYYY-MM-DD
 
 FORMAT = re.compile(r'^(\d{4})(?:\-|\/)(\d{1,2})(?:\-|\/)(\d{1,2})$')
 
 
-# Take almost anything - a date, a tuple, a string - and return an actual date
-# object.
-
 def absolute_date(info):
+    """Cast other types to datetime.date or None"""
+    if not info:
+        return None
     if isinstance(info, Date):
         return info
     elif isinstance(info, tuple):
         return Date(*info)
     elif isinstance(info, str) and FORMAT.match(info):
         return Date(*(int(x) for x in FORMAT.match(info).groups()))
     raise RuntimeError("Invalid date %s" % info)
 
 
-# Given a string like "tomorrow" or "in 4 days", return a date. If the input
-# provided is not a string, then just pass it along.
+# Refactored to only accept a string
 
-def relative_date(value):
-    if isinstance(value, str):
-        value = value.lower()
-        result = next(filter(None, (h(value) for h in HANDLERS)), None)
-        if result:
-            return result
-    return absolute_date(value)
+def relative_date(value: str):
+    """Given a string like "tomorrow" or "in 4 days", return a date"""
+    value = value.lower()
+    result = next(filter(None, (h(value) for h in HANDLERS)), None)
+    if result:
+        return result
+    else:
+        return absolute_date(value)
 
 
 # Used during import to bring in different handlers for relative dates. Called
 # during import.
 
 HANDLERS = []
 
+
 def _register(expression=r'(.*)'):
     compiled = re.compile(expression)
+
     def chain(func):
         @functools.wraps(func)
         def wrapper(string):
             match = compiled.match(string)
             if match:
                 return func(today(), *match.groups())
         HANDLERS.append(wrapper)
@@ -62,40 +63,46 @@
 
 # The actual different types of expressions for relative dates.
 
 @_register(r'today')
 def _match_today(today):
     return today
 
+
 @_register(r'tomorrow')
 def _match_tomorrow(today):
     return today + TimeDelta(1)
 
+
 @_register(r'^(\d+)\s+days?$')
 def _match_days(today, days):
     return today + TimeDelta(int(days))
 
+
 @_register(r'^(\d+)d$')
 def _match_d(today, days):
     return today + TimeDelta(int(days))
 
+
 @_register(r'^(\d{1,2})$')
 def _match_day_num(today, day):
     if today.day < int(day):
         return Date(today.year, today.month, int(day))
     else:
         year = today.year + (today.month // 12)
         month = (today.month % 12) + 1
         return Date(year, month, int(day))
 
+
 @_register(r'(\d{1,2})(?:\-|\/)(\d{1,2})$')
 def _match_month_day_num(today, month, day):
     if today < Date(today.year, int(month), int(day)):
         return Date(today.year, int(month), int(day))
     else:
         return Date(today.year + 1, int(month), int(day))
 
+
 @_register(r'^(mon?|tue?s?|wed?n?e?s?|thu?r?s?|fri?|sat?u?r?|sun?)(?:day)?$')
 def _match_weekday(today, weekday):
-    index = ['mo','tu','we','th','fr','sa','su'].index(weekday[0:2])
+    index = ['mo', 'tu', 'we', 'th', 'fr', 'sa', 'su'].index(weekday[0:2])
     days = (6 - today.weekday() + index) % 7 + 1
     return today + TimeDelta(days)
```

### Comparing `busy-3.4.6/busy/util/super_wrapper.py` & `busy-5.0.0/busy/util/super_wrapper.py`

 * *Files identical despite different names*

### Comparing `busy-3.4.6/busy.egg-info/PKG-INFO` & `busy-5.0.0/busy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 3.4.6
+Version: 5.0.0
 Summary: Personal time management system
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Busy
 ====
 
+**Note: Busy 4 uses a different data model from previous versions. There's a conversion script, which must be run using regular Python. Also, many of the commands' behaviour and options have changed.**
+
+_Using Busy? [Contact us!](mailto:busy@steampunkwizard.ca)_
+
 Busy is a personal time management tool, designed to help us all through our crazy busy days with as little stress as possible. It's simple, fast, and fun to use.
 
 Usage
 =====
 
 Principles
 ----------
@@ -30,79 +34,98 @@
 - *Editable data*: The data is stored in text files, which can easily be edited outside of Busy itself. (In fact, Busy started as a todo.txt type of approach and grew from there.)
 
 _The idea of Importance over Urgency comes from the book "The 7 Habits of Highly Effective People". Although we firmly disagree with Steven Covey's statements on gay rights, the book contains excellent ideas._
 
 Installation
 ------------
 
-Beginners, see [INSTALLATION.md](INSTALLATION.md).
+tl;dr: `pipx install busy`
 
-Experienced folks, use [pipx](https://pypa.github.io/pipx/) to install Busy.
+You'll need a terminal emulator to access a command or shell prompt. Examples include:
+
+- iTerm2 or Terminal on MacOS
+- Gnome Terminal or XTerm on Linux
+- CMD on Windows
+- Terminator on all platforms
+
+Busy requires `pipx`, which requires Python 3.6 or later. To check whether you already have the right version of Python on your system, start your terminal emulator and type:
 
-```bash
-pipx install busy
+```
+python3 -V
 ```
 
-To upgrade:
+If you don't have Python, or your version is out of date, install or upgrade it. In most cases, you'll want to do so using your system's package manager (such as Homebrew on MacOS or APT on Ubuntu). If you're not familiar with package managers, then download Python from [the Python.org site](https://www.python.org/downloads/) directly and follow the instructions provided there. When done, use the version check above to confirm it's installed and the version is 3.6.5 or greater.
+
+Python comes with PIP, which enables installation of Python packages from a central server called PyPI.
+
+Once Python and PIP are installed, type:
 
-```bash
-pipx upgrade busy
+```
+pip3 install pipx
+pipx install busy
 ```
 
+```
+pipx upgrade busy
+```
 
 Overview
 --------
 
 Busy ships with two user interfaces, both of them terminal-based and keyboard-driven:
 
 - *Shell UI* - A command-line interface (CLI) using shell conventions and called directly from the shell, one command at a time.
 - *Curses UI* - A faster, more visual interface with one-key commands that remains visible the entire time it's being used.
 
 Some commands also use your favorite terminal-based text editor, such as Emacs, vi, or Nano. It's possible to use Busy without a text editor, but functionality is limited.
 
-Busy's core model is a collection of Items, the most interesting of which are Tasks. Items are organized into Queues, which are ordered sets. You work on the top Task in the Queue, and when it's done, that Task gets removed from the Queue to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
+Busy's core model is a collection of Items, which are typically tasks but can also be discussion topics, groceries to buy, or anything else you like. Items are organized into Queues, which are named sets of Items to do. You work on the top Item in a Queue, and when it's done, that Item gets marked as "done", to reveal the next one. There is a default Queue (called "tasks") but you can also create other Queues, for example a shopping list or discussion list.
+
+Busy actually moves Items between States within each Queue. Each Queue contains a Collection (ordered list) of Items for each State. The States are:
 
-In addition to the "tasks" Queue, Busy maintains the "plans" Queue for future tasks (don't worry about them yet!) and the "done" Queue as a record of what's been completed in the past.
+- `todo`: Current Items for you to work on, discuss, or buy now.
+- `done`: Items that have been done, with the date completed.
+- `plan`: Items that have been deferred to a future date, with that date.
 
 Using the Shell UI
 ------------------
 
-To get started, add some Tasks to your default Queue.
+To get started, add some tasks to your default Queue.
 
 ```
-busy add --description "Take a shower"
-busy add --description "Do the laundry"
-busy add --description "Phone mom"
 busy add --description "Donate to the Busy project"
+busy add --description "Phone mom"
+busy add --description "Do the laundry"
+busy add --description "Take a shower"
 ```
 
 Then, when you're ready to start your day, ask Busy what to do first:
 
 ```
-busy top
+busy show
 ```
 
 Returns:
 
 ```
 Take a shower
 ```
 
-_Yes, Busy is great for tracking daily, personal, habitual tasks in addition to work tasks. It feels great to mark things as done!_
+That's the last Item you added, because Busy adds items to the top of the queue, turning it into a [LIFO stack](https://en.wikipedia.org/wiki/Stack_(abstract_data_type).
 
 When you've finished that task, mark it off to find the next task.
 
 ```
 busy finish
 ```
 
 It will ask you to confirm that you're done. Then request the next task:
 
 ```
-busy top
+busy show
 ```
 
 Which will tell you what to do next:
 
 ```
 Do the laundry
 ```
@@ -134,279 +157,300 @@
 2  Donate to the Busy project
 3  Do the laundry
 ```
 
 If you see a task on the list that seems urgent, and you intend to perform it immediately, pop it to the top of the list:
 
 ```
-busy pop 2
+busy pop --criteria 2
 ```
 
 _Our use of the term "pop" for a command doesn't quite fit with the computing term "pop". It might change in the future._
 
-Then `busy get` will return:
+Then `busy show` will return:
 
 ```
 Donate to the Busy project
 ```
 
 Let's say you realize that it's not an appropriate task for today, but you want to defer it to tomorrow:
 
 ```
 busy defer
 ```
 
-It will ask you to confirm "tomorrow" as the day for deferral. Agree with it for now.
+It will ask you to confirm "tomorrow" as the day for deferral. Agree with it for now. The Item will then be moved into the `plan` State with tomorrow's date as the plan date.
 
-At the start of a new day, tell Busy to add all the previously deferred Tasks to the current Queue:
+At the start of a new day, tell Busy to add all the previously deferred Items to the current Queue:
 
 ```
 busy activate
 ```
 
 Commands
 --------
 
 Here's a summary of the commands in Busy.
 
-- `add` adds a new item to the bottom of the queue. The item description may be included after the command or written to stdin (i.e. typed on the next line).
-- `top` gets the top item in the queue, referred to as the "current" item. There are no options.
+- `add` adds a new item to the top of the queue. The item description may be included after the command or typed on the next line.
+- `show` gets the top item in the queue, referred to as the "current" item.
+- `resource` shows the URL (if any) prefixed with an "@" symbol
+- `base` is like `show`, but removes resources, followons, and tags
 - `list` lists the items in the queue in order with their sequence numbers.
 - `pop` moves a task or set of items to the top of a queue.
 - `drop` moves a task or set of items to the bottom of a queue.
 - `delete` permanently removes a task or set of items from a queue.
 - `edit` opens a text editor to edit items - the default is to edit only the top item.
-- `manage` is the same as `edit`, but defaults to edit the whole queue.
-- `finish` removes a task or tasks from the `tasks` queue and adds it to the `done` queue, so it's complete. Good job!
-- `defer` removes a task or set of tasks from the `tasks` queue and schedules it or them to reappear at a future date in the `plans` queue.
-- `activate` moves current tasks from the `plans` queue to the `tasks` queue. Get to work!
+- `manage` is the same as `edit`, but defaults to edit the whole collection.
+- `finish` moves a task or tasks from the `todo` state to the `done` state, so it's complete. Good job!
+- `defer` moves a task or set of tasks from the `todo` state and schedules it or them to reappear at a future date in the `plan` state.
+- `activate` moves current tasks from the `plan` state to the `todo` state. Get to work!
 - `queues` to list all the queues.
 - `tags` to list all the tags.
+- `curses` launches the Curses UI, and is also the default if no command is provided.
+
+Here are some of the options which apply to some or all of the commands:
 
-Except for `add` and `top`, commands allow the designation of specific items to be acted upon. Item designation can be performed using sequence numbers or tags.
+- A queue name, which does not need an option designation
+- `--help` to find out which options apply
+- `--criteria` to designate items to be acted upon, using sequence numbers or tags
+- `--yes` to skip confirmation of any command that requires it
+- `--description` for the item description (`add` command only)
+- `--state` to work on Items of a different state
+- `--timing` applies to the `defer` command
 
 Sequence numbers
 ----------------
 
-Sequence numbers appear in the output from the `list` command. Note that the numbering starts with 1, and is not an ID -- the number of a item will change when the queue is modified. So always reference the most recent output from the `list` command.
+Sequence numbers appear in the output from the `list` command. Note that the numbering starts with 1, and is not an ID -- the number of a item will change when the collection is modified. So always reference the most recent output from the `list` command.
 
-To designate more than one item, separate the sequence numbers with a space.
+Sequence numbers are used with the `--criteria` option, which can be shortened to `-c`. To designate more than one item, separate the sequence numbers with a space.
 
-When used to designate items, a range of sequence numbers is separated by a hyphen, with no whitespace, and is inclusive. For example, `4-6` designates items 4, 5, and 6. A hyphen without a number after it includes all the items from that item to the end of the queue. A hyphen on its own indicates the last item in the queue.
+Another choice is ranges. A range of sequence numbers is separated by a hyphen, with no whitespace, and is inclusive. For example, `4-6` designates items 4, 5, and 6. A hyphen without a number after it includes all the items from that item to the end of the queue. A hyphen on its own indicates the last item in the queue.
 
 Below are some examples of task designations by sequence number.
 
-- `busy pop 5` pops item number 5
-- `busy drop 3-7` drops items 3 through 7 (4 items)
-- `busy list 3-` lists all the items from number 3 through the end of the list
-- `busy delete 3 5 7 9` deletes only the items designated
-- `busy defer -` defers the last task
-- `busy edit -4` is an error! Use `busy edit 1-4` instead
+- `busy pop -c 5` pops item number 5
+- `busy drop -c 3-7` drops items 3 through 7 (4 items)
+- `busy list -c 3-` lists all the items from number 3 through the end of the list
+- `busy delete -c 3 5 7 9` deletes only the items designated
+- `busy defer -c -` defers the last task
+- `busy edit -c -4` is an error! Use `busy edit -c 1-4` instead
 - `busy manage` allows you to edit the entire queue
 
 Items will always be handled in the order they appear in the queue, regardless of the order the criteria are provided. So for example, if a `pop` command designates some items, they will be moved to the top of the queue in the order, relative to each other, they currently appear in the queue.
 
-The sequence numbers in the `list` command output are from the queue itself. So the `list` command does not modify the sequence numbers, even when item designation is applied.
+The sequence numbers in the `list` command output are from the collection itself. So the `list` command does not modify the sequence numbers, even when item designation is applied.
 
 Tags
 ----
 
 Items can have tags, which are space-separated hashtags in the item description. An item can have no tags, one tag, or more than one tag. For example the following item description has the tag "errands":
 
 ```
 go to the supermarket #errands
 ```
 
-Tags cannot contain punctuation.
+The only punctuation that tags can contain is the hyphen ("-").
 
-Hash tags may be used for item designation, in which case the hash itself ("#") is omitted from the command line. For example, the following command will move all the items with the `#errands` tag to the top of the queue.
+Hash tags may be used as criteria in addition to sequence numbers. For example, the following command will move all the items with the `#errands` tag to the top of the queue.
 
 ```
-busy pop errands
+busy pop -c #errands
 ```
 
-Whitespace-separated item designation criteria are additive -- that is, a logical OR. For example, the following command will delete all the admin tasks, sales tasks, and tasks 3 and 4.
+Whitespace-separated criteria are additive -- that is, a logical OR. For example, the following command will delete all the admin tasks, sales tasks, and tasks 3 and 4.
 
 ```
-busy delete admin sales 3 4
+busy delete -c #admin #sales 3 4
 ```
 
+_Note to self: why does this work? Shouldn't the hash symbol indicate a comment?_
+
 Default item designations
 -------------------------
 
 For the most part, commands that accept item designations default to only act on the top item in the queue. The exceptions are:
 
-- `list` defaults to list the entire queue
-- `pop` defaults to pop the last item in the queue to the top
-- `activate` defaults to activate items for today (more on that below)
+- `list` and `manage` default to handle the entire collection
+- `pop` defaults to pop the last item in the collection to the top
+- `activate` defaults to activate `plan` items for today (more on that below)
 
 Alternate queues
 ----------------
 
-Busy will manage any number of queues, which are entirely separate ordered sets of items. For example, you might have a `shopping` queue for items to buy at the store, and a `movies` queue for films you'd like to watch. The default queue is called `tasks` and has special properties related to planning.
+Busy will manage any number of queues, which are entirely separate sets of items. For example, you might have a `shopping` queue for items to buy at the store, and a `movies` queue for films you'd like to watch. The default queue is called `tasks`.
 
-To designate an alternate queue, use the `--queue` option on a command. For example:
+To designate an alternate queue, enter it right after the command. For example:
 
 ```
-busy add "Skimmed Milk" --queue shopping
-busy top --queue movies
+busy add shopping -d "Skimmed Milk"
+busy list movies
 ```
 
 Managing plans
 --------------
 
-The default `tasks` queue supports several specific commands related to planning -- that is, scheduling tasks for the future. They are `finish`, `defer`, and `activate`. The task-specific commands do not accept a `--queue` modifier, because they only work on the default `tasks` queue. Planned tasks are kept in another special queue called `plans`, and completed tasks are kept in a queue called `done`.
+Busy supports several specific commands related to planning -- that is, scheduling tasks for the future. They are `finish`, `defer`, and `activate`. The task-specific commands handle items in the `plan` state and, in some cases, the `done` state.
 
-The task commands accept item designations. The `defer` and `finish` commands reference the `tasks` queue; the `activate` command references the `plans` queue. The default for `defer` and `finish` is the top item in the `tasks` queue; the default for `activate` is to activate only plans deferred to today or earlier.
+The task commands accept criteria. The `defer` and `finish` commands reference the `todo` collection; the `activate` command references the `plan` collection. The default for `defer` and `finish` is the top item in the collection; the default for `activate` is to activate only plans deferred to today or earlier.
 
 Planning by date
 ----------------
 
 Planning is by date, not time, and is relative to the current date according to the system clock.
 
-In the `defer` command, the date can be specified using the `--to` or `--for` option (they are interchangable). If the options are omitted, then the date can be provided as input.
+In the `defer` command, the date can be specified using the `--timing` option. If the option is omitted, then the date can be provided as input during confirmation.
 
 The date may take any of the following forms:
 
 - A specific date in `YYYY-MM-DD` format, such as `2018-10-28`. Slashes are also acceptable, but the order is always year, then month, then day.
 - A specific date without the year in `MM-DD` format, such as `7-4`, which will defer the item to that date in the future (even if it's in the next year).
 - A specific day of the month as a simple integer, such as `12`, which will defer the item to that day of the month, in either the current month or the next month.
 - An integer, a space, and the word `day` or `days`, such as `4 days`, which will defer the item to that number of days from today.
 - An integer without a space and the letter `d`, such as `4d`, which is a short form of `4 days`.
 - The word `tomorrow`, which is also the default if no date is provided.
 - The word `today`, which is a little odd but obvious.
 
-As an example, the following command will defer tasks 4, 5, and 6 from the `tasks` queue to the date 4 days from today, keeping them in the `plans` queue until that date.
+As an example, the following command will defer tasks 4, 5, and 6 from the `todo` collection to the date 4 days from today, keeping them in the `plan` collection until that date.
 
 ```
-busy defer 4-6 --for 4 days
+busy defer -c 4-6 -t "4 days"
 ```
 
-Note that the `plans` queue is keeping the task information (verbatim from the `tasks` queue) along with the date information (as an absolute date).
+Note that the `plan` collection is keeping the task information (verbatim from the `todo` collection) along with the date information (as an absolute date).
 
-To pull tasks off the `plans` queue and put them back on the `tasks` queue, use the `activate` command. There are two ways to use the `activate` command:
+To pull tasks from the `plan` collection and put them back into the `todo` collection, use the `activate` command. There are two ways to use the `activate` command:
 
-- With no item designation, in which case Busy activates all the tasks scheduled for today or earlier, bringing the `tasks` list up to date
-- With designated items from the `plans` queue; note that the `activate` command accepts item designation from the `plans` queue itself
+- With no criteria, in which case Busy activates all the tasks scheduled for today or earlier, bringing the `todo` list up to date
+- With designated items from the `plan` collection; note that the `activate` command accepts item designation from the `plan` queue itself so use `busy list -s plan` first to get the right list.
 
 Finishing and following up
 --------------------------
 
-Like `defer`, the `finish` command only works on the `tasks` queue. It removes the designated Task (or the top task if none is designated) from the queue and adds it to the `done` queue, with today's date to indicate when it was completed.
+The `finish` command removes the designated Task (or the top task if none is designated) from the `todo` state  and adds it to the `done` state, with today's date to indicate when it was completed.
 
-Optionally, a task can have a followon, which is another task to be added to the queue after the first task is finished. Followons are described in a task using an arrow notation. In the following example, the task "eat" has a followon task "drink":
+Optionally, a task can have a "followon", which is another task to be added as a `todo` after the first task is finished. Followons are described in a task using an arrow notation. In the following example, the task "eat" has a followon task "drink":
 
 ```
 eat --> drink
 ```
 
-Note that the hyphens and whitespace are optional; really the marker that matters for delimiting a followon is the right angle bracket (">"). Also note that right angle bracket is not a valid character in a task description.
+Note that the hyphens and whitespace are optional; really the marker that matters for delimiting a followon is the right angle bracket (">"). Also note that right angle bracket is not a valid character elsewhere in a task description.
 
-When the `finish` command is executed on the task above, the "eat" task will be recorded as "done" and the "drink" task will be added to the bottom of the `tasks` queue.
+When the `finish` command is executed on the task above, the "eat" task will be recorded as "done" and the "drink" task will be added to the top of the `todo` list.
 
-Note that followons can be chained. For example, when the `finish` command is run on the task illustrated below, a new task "drink > be merry" will be added to the queue. Only when that Task is finished will the "be merry" task itself appear on the queue.
+Note that followons can be chained. For example, when the `finish` command is run on the task illustrated below, a new task "drink > be merry" will be added to the `todo` collection`. Only when that Task is finished will the "be merry" task itself appear.
 
 ```
 eat > drink > be merry
 ```
 
 Repeating tasks
 ---------------
 
-A special type of followon is the repeat. In this case, instead of adding the next task to the bottom of the queue, the entire current task -- including the Followon itself -- is entered into the `plans` queue at some point in the future. Repeats allow for easy management of repeating tasks. Some examples follow.
+A special type of followon is the repeat. In this case, instead of adding the next task to the top of the `todo` list, the entire current task -- including the followon itself -- is entered into the `plan` collection at some point in the future. Repeats allow for easy management of repeating tasks. Some examples follow.
 
 - `check email --> repeat in 1 day`
 - `phone mom --> repeat on sunday`
 - `balance the checkbook --> repeat on 6`
 
 The exact syntax for a Repeat is the word "repeat" followed by either "on" or "in" and a relative date phrase -- the same phrases that work with the `defer` command.
 
-Note that the repetition itself only happens on the `finish` command. The completed task (i.e. "check email") is entered in the `done` queue and then the entire task (with the Repeat) is scheduled in the `plans` queue for the appropriate time in the future.
+Note that the repetition itself only happens when the `finish` command is executed. The completed task (i.e. "check email") is entered in the `done` list and then the entire task (with the Repeat) is scheduled in the `plan` list for the appropriate time in the future.
 
 Editing items
 -------------
 
-The `edit` and `manage` commands launch the user's default text editor to directly edit a task, the whole queue, or part of a queue. Note that `edit` and `manage` are identical commands except for their defaults.
+The `edit` and `manage` commands launch the user's default text editor to directly edit a task, the whole queue, or part of a queue. Note that `edit` and `manage` are identical commands except for their default criteria.
 
 The definition of the "default text editor" depends on the OS and configuration but here's the logic:
 
 1. Try the EDITOR environment variable
 1. If that doesn't exist, try the `sensible-editor` command (Ubuntu)
 1. If that doesn't exist, try the `open -W` command (OSX)
 
-You must quit the editor to accept the change back into Busy.
+You must save changes and quit the editor to accept the change back into Busy.
 
-The `edit` command with no criteria will edit the top item in the queue, and the `manage` command with no criteria will edit the entire queue. But it's also possible to designate items to be edited with both commands. The commands do their best to replace the edited items in place in the list order. So if you `edit` or `manage` a tag whose items are recently popped (at the top of the queue), then the edited items will still appear at the top. Even if you add items, they will be inserted after the last item in the edited set, not at the end of the queue. But all the items brought up in the editor will be edited. So if you remove an item in the editor, it will be deleted and the others will be moved up to take its place.
+The `edit` command with no criteria will edit the top item in the list, and the `manage` command with no criteria will edit the entire list. But it's also possible to designate items to be edited with both commands using criteria. The commands do their best to replace the edited items in place in the list order. So if you `edit` or `manage` a tag whose items are recently popped (at the top of the collection), then the edited items will still appear at the top. Even if you add items, they will be inserted after the last item in the edited set, not at the end of the queue. But all the items brought up in the editor will be edited. So if you remove an item in the editor, it will be deleted and the others will be moved up to take its place.
 
 For faster daily use - the Curses UI
 ------------------------------------
 
 Busy suports multiple user interfaces. The command line interface described above is the shell interface. The alternative is the curses UI, which draws an entirely new terminal in the same window.
 
-_We get it - "curses" is a terrible name. It's a reference to the underlying technology. It's likely to change._
+_We get it - "curses" is a terrible name. It's a reference to the underlying technology._
 
-As of now, the curses UI only supports the `tasks` queue. The commands can be triggered with single keystrokes, and only act on their default tasks (usually the top task). The UI always displays the current queue (which is always `tasks` for now) and the current (top) task at the top of the screen.
+In the Curses UI, commands can be triggered with single keystrokes, and only act on their default items (usually the top task). The UI always displays the current queue (which is always `tasks` for now) and the current (top) `todo` item` at the top of the screen.
 
 To invoke the curses UI, type:
 
 ```
 busy curses
 ```
 
-Commands within the UI are shown with a single letter underlined. The underlined letter is the keystroke that will invoke the command. Use `q` to quit. When inside a command, use ctrl-C to cancel the command and return to the main menu.
+Or it's the default so just type:
 
+```
+busy
+```
+
+Commands within the UI are shown with a single letter underlined. The underlined letter is the keystroke that will invoke the command. Use `q` to quit. When inside a command, use ctrl-C to cancel the command and return to the main menu.
 
 Data storage
 ------------
 
-Busy keeps the queues in plain text files, so if the tool doesn't do something you want, you may edit the files. The files are in a directory together, referred to as the "root". Each file is the name of the queue with a `.txt` extension. If a required file is missing, it will be created automatically. So typically, the root includes `tasks.txt`, `plans.txt`, `done.txt`, and any number of custom queue files.
+Busy keeps the collections in plain text files, so if the tool doesn't do something you want, you may edit the files. The files are in a directory together, referred to as the "root". Each file is the named according to the following convention:
 
-Technically, Busy data files are pipe-delimited data files, though `tasks.txt` and any custom queues only have one field ("description") while `plans.txt` and `done.txt` have only two fields (date and description).
+```
+<queue>.<state>.psv
+```
+
+If a required file is missing, it will be created automatically. So typically, the root includes `tasks.todo.psv`, `tasks.plan.psv`, `tasks.done.txt`, and any number of custom queue files.
+
+Technically, Busy data files are pipe-delimited data files, though the `todo` collections only have one field ("description") while the `plan` and `done` files have only two fields (date and description).
 
 Busy is not a database (yet). There is no support for managing separate fields in the Busy tool itself.
 
 The root is designated in one of the following ways, which are tried in order.
 
 - The `--root` option on any command
 - The `BUSY_ROOT` environment variable, if no `--root` option is provided
 - A directory at `~/.busy`, which will be generated as needed if no `--root` option or `BUSY_ROOT` environment variable are provided,
 
 Note that the `--root` option must come after `busy` but command-specific options (`--yes`, `--to`, `--for`, and `--queue`) must come after commands.
 
 The following example shows the `--root` option with command-specific options on the same command line.
 
 ```
-busy --root ~/.config/busy defer --to tuesday
+busy --root ~/.config/busy defer --t tuesday
 ```
 
-Note that Busy does not support concurrency in any form. If two commands are executing at the same time, they might overwrite each other. Overwriting is especially risky with the `edit` command, which keeps the user's editor open until they close it.
+Note that Busy does not support concurrency or locking in any form. If two commands are executing at the same time, they might overwrite each other. Overwriting is especially risky with the `edit` and `manage` commands, which keeps the user's editor open until they close it.
 
-The format is designed to be simple (i.e. non-default queues are really just lists of items) but not idiot-proof. Experimentation might result in unintended consequences.
+The format is designed to be simple but not idiot-proof. Experimentation might result in unintended consequences.
 
 Development
 ===========
 
 The code is intended to demonstrate some Python best practices:
 
 - *Object-oriented* with classes and subclasses.
 - *Dynamic configuration* using a unique approach we call "class families" - for example, the names of the commands are properties of the command classes, not in a big "if" statement.
-- *Extensive testing* with >90% test coverage, guaranteed by CI.
+- *Extensive testing* with high test coverage, guaranteed by CI.
 - *Leverage the standard library* by requiring 3rd party PIP modules for development, but not for usage.
 
 To set everything up:
 
-```
-sudo pip3 install vernum coverage pycodestyle twine
-```
+- Requires Python 3.6.5 or later
+- Clone the repo and CD into it
+- Set up a venv if that's your thing
+- `pip install -r requirements/freeze.txt`
+- To run it: `python -m busy` ...
 
-To get the full repo:
-
-```
-git clone git@gitlab.com:fpotter/tools/busy.git
-```
 We use Visual Studio Code to build Busy, so there is a VS Code configuration file in the repository.
 
 Then to run the test suite:
 
 ```
 make test
 ```
@@ -419,15 +463,15 @@
 
 And to check style:
 
 ```
 make style
 ```
 
-_Note to self: To publish a new build, use 'vernum' with 'major', 'minor', or 'patch' depending on how major the changes were since the last build. Then push. GitLab allows you to publish to PyPI in its UI, and only when Vernum has been run._
+_Note to self: To publish a new build, use 'vernum' with 'major', 'minor', or 'patch' depending on how major the changes were since the last build. Then push. GitLab allows you to publish to PyPI via CI/CD, and only when Vernum has been run._
 
 Command summary
 ===============
 
 Below is a reference list of all commands, handy to correlate the one-letter version with the full version. The one-letter version is used in the curses UI, and is an alternative option in the shell UI. Some of the listed commands are yet to be implemented; they are listed here merely to reserve their names.
 
 | Short | Full |
@@ -436,17 +480,16 @@
 | c | activate |
 | d | delete |
 | e | edit |
 | f | defer |
 | l | list |
 | m | manage |
 | n | finish |
-| p | pop |
-| q | quit (only in interactive UI) |
+| o | pop |
+| p | print |
+| q | quit |
 | r | drop |
-| s | shuffle |
+| s | skip |
 | t | tags |
 | u | queues (list) |
 | w | switch (queues) |
 |   | curses (only in shell UI) |
-|   | top |
-
```

### Comparing `busy-3.4.6/pyproject.toml` & `busy-5.0.0/pyproject.toml`

 * *Files identical despite different names*

