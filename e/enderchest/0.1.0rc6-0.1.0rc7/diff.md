# Comparing `tmp/enderchest-0.1.0rc6.tar.gz` & `tmp/enderchest-0.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.0rc6.tar", last modified: Mon May 29 14:00:36 2023, max compression
+gzip compressed data, was "enderchest-0.1.0rc7.tar", last modified: Tue May 30 04:45:18 2023, max compression
```

## Comparing `enderchest-0.1.0rc6.tar` & `enderchest-0.1.0rc7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    31191 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.433473 enderchest-0.1.0rc6/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/sync/rsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    22451 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:00:36.433473 enderchest-0.1.0rc6/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 14:00:36.000000 enderchest-0.1.0rc6/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-29 14:00:36.437473 enderchest-0.1.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-29 14:00:28.000000 enderchest-0.1.0rc6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31191 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27865 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/sync/rsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21416 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22911 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-30 04:45:18.000000 enderchest-0.1.0rc7/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-30 04:45:18.000000 enderchest-0.1.0rc7/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:45:18.000000 enderchest-0.1.0rc7/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 04:45:18.000000 enderchest-0.1.0rc7/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 04:45:18.000000 enderchest-0.1.0rc7/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 04:45:18.000000 enderchest-0.1.0rc7/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 04:45:18.170498 enderchest-0.1.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-05-30 04:45:10.000000 enderchest-0.1.0rc7/versioneer.py
```

### Comparing `enderchest-0.1.0rc6/LICENSE` & `enderchest-0.1.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/PKG-INFO` & `enderchest-0.1.0rc7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -33,14 +33,31 @@
 EnderChest is a command-line utility for selectively sharing Minecraft assets
 (configurations, mods, worlds, etc.)...
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
+### A Note On Linking
+
+Starting with Minecraft 1.20, Mojang by default
+[no longer allows worlds to load if they are or if they contain symbolic links](https://help.minecraft.net/hc/en-us/articles/16165590199181).
+While it is true that an improper symlink could cause Minecraft to write data
+to a place it shouldn't, nothing in EnderChest will ever generate a symlink whose
+target is outside of your EnderChest folder _unless you place_ a symbolic link in
+your EnderChest pointing to somewhere else (which you may want to do so that your
+screenshots, for example, point to your "My Pictures" folder).
+
+If you still have concerns about symlinks or questions about how they work,
+read through
+[this guide](https://www.makeuseof.com/tag/what-is-a-symbolic-link-what-are-its-uses-makeuseof-explains/)
+or [watch this explainer](https://www.youtube.com/watch?v=mA08E59-zo8), and if
+you still have questions, feel free to
+[open an issue](https://github.com/OpenBagTwo/EnderChest/issues/new?assignees=OpenBagTwo&labels=question&title=symlink%20question).
+
 ## Installation
 
 EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
 The latest release can be installed from PyPI via `pip`:
```

### Comparing `enderchest-0.1.0rc6/README.md` & `enderchest-0.1.0rc7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,31 @@
 EnderChest is a command-line utility for selectively sharing Minecraft assets
 (configurations, mods, worlds, etc.)...
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
+### A Note On Linking
+
+Starting with Minecraft 1.20, Mojang by default
+[no longer allows worlds to load if they are or if they contain symbolic links](https://help.minecraft.net/hc/en-us/articles/16165590199181).
+While it is true that an improper symlink could cause Minecraft to write data
+to a place it shouldn't, nothing in EnderChest will ever generate a symlink whose
+target is outside of your EnderChest folder _unless you place_ a symbolic link in
+your EnderChest pointing to somewhere else (which you may want to do so that your
+screenshots, for example, point to your "My Pictures" folder).
+
+If you still have concerns about symlinks or questions about how they work,
+read through
+[this guide](https://www.makeuseof.com/tag/what-is-a-symbolic-link-what-are-its-uses-makeuseof-explains/)
+or [watch this explainer](https://www.youtube.com/watch?v=mA08E59-zo8), and if
+you still have questions, feel free to
+[open an issue](https://github.com/OpenBagTwo/EnderChest/issues/new?assignees=OpenBagTwo&labels=question&title=symlink%20question).
+
 ## Installation
 
 EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
 The latest release can be installed from PyPI via `pip`:
```

### Comparing `enderchest-0.1.0rc6/enderchest/cli.py` & `enderchest-0.1.0rc7/enderchest/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,32 @@
 
 def _place(
     minecraft_root: Path,
     errors: str = "prompt",
     cleanup: bool = False,
     stop_at_first_failure: bool = False,
     ignore_errors: bool = False,
+    absolute: bool = False,
+    relative: bool = False,
 ) -> None:
-    """Wrapper to coalesce error-handling flags"""
+    """Wrapper to coalesce error-handling flags and also abs/rel"""
 
     if stop_at_first_failure:
         errors = "abort"
     if ignore_errors:  # elif?
         errors = "ignore"
     # else: errors = errors
-    place.place_ender_chest(minecraft_root, cleanup=cleanup, error_handling=errors)
+
+    if absolute is True:
+        # technically we get this for free already
+        relative = False
+
+    place.place_ender_chest(
+        minecraft_root, cleanup=cleanup, error_handling=errors, relative=relative
+    )
 
 
 def _craft_shulker_box(minecraft_root: Path, name: str | None = None, **kwargs):
     """Wrapper to handle the fact that name is a required argument"""
     assert name  # it's required by the parser, so this should be fine
     craft.craft_shulker_box(minecraft_root, name, **kwargs)
 
@@ -368,14 +377,27 @@
             "skip-instance",
             "skip-shulker-box",
             "abort",
         ),
         default="prompt",
         help="specify how to handle linking errors (default behavior is to prompt after every error)",
     )
+    link_type = place_parser.add_mutually_exclusive_group()
+    link_type.add_argument(
+        "--absolute",
+        "-a",
+        action="store_true",
+        help="use absolute paths for all link targets",
+    )
+    link_type.add_argument(
+        "--relative",
+        "-r",
+        action="store_true",
+        help="use relative paths for all link targets",
+    )
 
     # gather instance options
     gather_instance_parser = action_parsers[f"gather {_instance_aliases[0]}"]
     gather_instance_parser.add_argument(
         "search_paths",
         nargs="+",
         action="extend",
```

### Comparing `enderchest-0.1.0rc6/enderchest/craft.py` & `enderchest-0.1.0rc7/enderchest/craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/enderchest.py` & `enderchest-0.1.0rc7/enderchest/enderchest.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from urllib.parse import ParseResult, urlparse
 
 from . import filesystem as fs
 from . import instance as i
 from . import sync
 from ._version import get_versions
 from .loggers import CRAFT_LOGGER, GATHER_LOGGER
+from .sync import path_from_uri
 
 
 @dataclass(init=False, repr=False)
 class EnderChest:
     """Configuration of an EnderChest
 
     Parameters
@@ -51,14 +52,21 @@
     root : Path
         The path to this EnderChest folder
     instances : list-like of InstanceSpec
         The instances registered with this EnderChest
     remotes : list-like of (ParseResult, str) pairs
         The other EnderChest installations this EnderChest is aware of, paired
         with their aliases
+    offer_to_update_symlink_allowlist: bool
+        By default, EnderChest will offer to create or update `allowed_symlinks.txt`
+        on any 1.20+ instances that do not already blanket allow links into
+        EnderChest. **EnderChest will never modify that or any other Minecraft
+        file without your express consent.** If you would prefer to edit these
+        files yourself (or simply not symlink your world saves), change this
+        parameter to False.
     sync_confirm_wait: bool or int
         The default behavior when syncing EnderChests is to first perform a dry
         run of every sync operation and then wait 5 seconds before proceeding with the
         real sync. The idea is to give the user time to interrupt the sync if
         the dry run looks wrong. This can be changed by either raising or lowering
         the value of confirm, by disabling the dry-run-first behavior entirely
         (`confirm=False`) or by requiring that the user explicitly confirms
@@ -66,14 +74,15 @@
         when actually calling the sync commands.
     """
 
     name: str
     _uri: ParseResult
     _instances: list[i.InstanceSpec]
     _remotes: dict[str, ParseResult]
+    offer_to_update_symlink_allowlist: bool = True
     sync_confirm_wait: bool | int = 5
 
     def __init__(
         self,
         uri: str | ParseResult | Path,
         name: str | None = None,
         remotes: Iterable[str | ParseResult | tuple[str, str] | tuple[ParseResult, str]]
@@ -114,15 +123,15 @@
         return self._uri.geturl()
 
     def __repr__(self) -> str:
         return f"EnderChest({self.uri, self.name})"
 
     @property
     def root(self) -> Path:
-        return fs.ender_chest_folder(Path(self._uri.path))
+        return fs.ender_chest_folder(path_from_uri(self._uri), check_exists=False)
 
     @property
     def instances(self) -> tuple[i.InstanceSpec, ...]:
         return tuple(self._instances)
 
     def register_instance(self, instance: i.InstanceSpec) -> i.InstanceSpec:
         """Register a new Minecraft installation
@@ -237,21 +246,25 @@
         instances: list[i.InstanceSpec] = []
         remotes: list[str | tuple[str, str]] = []
 
         scheme: str | None = None
         netloc: str | None = None
         name: str | None = None
         sync_confirm_wait: str | None = None
+        offer_to_update_symlink_allowlist: bool = True
 
         for section in parser.sections():
             if section == "properties":
                 scheme = parser[section].get("sync-protocol")
                 netloc = parser[section].get("address")
                 name = parser[section].get("name")
                 sync_confirm_wait = parser[section].get("sync-confirmation-time")
+                offer_to_update_symlink_allowlist = parser[section].getboolean(
+                    "offer-to-update-symlink-allowlist", True
+                )
             elif section == "remotes":
                 for remote in parser[section].items():
                     if remote[1] is None:
                         raise ValueError("All remotes must have an alias specified")
                     else:
                         remotes.append((remote[1], remote[0]))
             else:
@@ -274,14 +287,17 @@
                     try:
                         ender_chest.sync_confirm_wait = int(sync_confirm_wait)
                     except ValueError:
                         raise ValueError(
                             "Invalid value for sync-confirmation-time:"
                             f" {sync_confirm_wait}"
                         )
+        ender_chest.offer_to_update_symlink_allowlist = (
+            offer_to_update_symlink_allowlist
+        )
         return ender_chest
 
     def write_to_cfg(self, config_file: Path | None = None) -> str:
         """Write this EnderChest's configuration to INI
 
         Parameters
         ----------
@@ -307,14 +323,19 @@
         config.set(
             "properties",
             "sync-confirmation-time",
             str(self.sync_confirm_wait)
             if self.sync_confirm_wait is not True
             else "prompt",
         )
+        config.set(
+            "properties",
+            "offer-to-update-symlink-allowlist",
+            str(self.offer_to_update_symlink_allowlist),
+        )
         config.set("properties", "last_modified", dt.datetime.now().isoformat(sep=" "))
         config.set(
             "properties", "generated_by_enderchest_version", get_versions()["version"]
         )
 
         config.add_section("remotes")
         for uri, name in self.remotes:
```

### Comparing `enderchest-0.1.0rc6/enderchest/filesystem.py` & `enderchest-0.1.0rc7/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/gather.py` & `enderchest-0.1.0rc7/enderchest/gather.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Functionality for finding, resolving and parsing local installations and instances"""
 import json
 import logging
+import os
+import re
 from configparser import ConfigParser, ParsingError
 from pathlib import Path
 from typing import Iterable, Sequence
 from urllib.parse import ParseResult
 
 from enderchest.sync import render_remote
 
 from . import filesystem as fs
 from .enderchest import EnderChest, create_ender_chest
 from .instance import InstanceSpec, _parse_version
 from .loggers import GATHER_LOGGER
-from .shulker_box import ShulkerBox
+from .prompt import prompt
+from .shulker_box import ShulkerBox, _matches_version
 
 
 def load_ender_chest(minecraft_root: Path) -> EnderChest:
     """Load the configuration from the enderchest.cfg file in the EnderChest
     folder.
 
     Parameters
@@ -394,37 +397,44 @@
     -----
     - If a minecraft installation is found but cannot be parsed
       (or parsed as specified) this method will report that failure but then
       continue on.
     - As a corollary, if _no_ valid Minecraft installations can be found, this
       method will return an empty list.
     """
+    try:
+        ender_chest = load_ender_chest(minecraft_root)
+    except FileNotFoundError:
+        # because this method can be called during crafting
+        ender_chest = EnderChest(minecraft_root)
     GATHER_LOGGER.debug(f"Searching for Minecraft folders inside {search_path}")
     instances: list[InstanceSpec] = []
     for folder in fs.minecraft_folders(search_path):
         folder_path = folder.absolute()
         GATHER_LOGGER.debug(f"Found minecraft installation at {folder}")
         if official is not False:
             try:
                 instances.append(gather_metadata_for_official_instance(folder_path))
                 GATHER_LOGGER.info(
                     f"Gathered official Minecraft installation from {folder}"
                 )
+                _check_for_allowed_symlinks(ender_chest, instances[-1])
                 continue
             except ValueError as not_official:
                 GATHER_LOGGER.log(
                     logging.DEBUG if official is None else logging.WARNING,
                     (f"{folder} is not an official instance:" f"\n{not_official}",),
                 )
         if official is not True:
             try:
                 instances.append(gather_metadata_for_mmc_instance(folder_path))
                 GATHER_LOGGER.info(
                     f"Gathered MMC-like Minecraft installation from {folder}"
                 )
+                _check_for_allowed_symlinks(ender_chest, instances[-1])
                 continue
             except ValueError as not_mmc:
                 GATHER_LOGGER.log(
                     logging.DEBUG if official is None else logging.WARNING,
                     f"{folder} is not an MMC-like instance:\n{not_mmc}",
                 )
         GATHER_LOGGER.warning(
@@ -690,7 +700,106 @@
                 ender_chest.register_remote(remote)
             else:
                 ender_chest.register_remote(*remote)
         except ValueError as bad_remote:
             GATHER_LOGGER.warning(bad_remote)
 
     create_ender_chest(minecraft_root, ender_chest)
+
+
+def _check_for_allowed_symlinks(
+    ender_chest: EnderChest, instance: InstanceSpec
+) -> None:
+    """Check if the instance:
+        - is 1.20+
+        - has not already blanket-allowed symlinks into the EnderChest
+
+    and if it hasn't, offer to update the allow-list now *but only if* the user
+    hasn't already told EnderChest "shut up I know what I'm doing."
+
+    Parameters
+    ----------
+    ender_chest : EnderChest
+        This EnderChest
+    instance : InstanceSpec
+        The instance spec to check
+    """
+    if ender_chest.offer_to_update_symlink_allowlist is False:
+        return
+
+    if not any(
+        _needs_symlink_allowlist(version) for version in instance.minecraft_versions
+    ):
+        return
+    ender_chest_abspath = os.path.abspath(ender_chest.root)
+
+    symlink_allowlist = instance.root / "allowed_symlinks.txt"
+
+    try:
+        allowlist_contents = symlink_allowlist.read_text()
+        already_allowed = ender_chest_abspath in allowlist_contents.splitlines()
+        allowlist_needs_newline = not allowlist_contents.endswith("\n")
+    except FileNotFoundError:
+        already_allowed = False
+        allowlist_needs_newline = False
+
+    if already_allowed:
+        return
+
+    GATHER_LOGGER.warning(
+        """
+Starting with Minecraft 1.20, Mojang by default no longer allows worlds
+to load if they are or if they contain symbolic links.
+Read more: https://help.minecraft.net/hc/en-us/articles/16165590199181"""
+    )
+
+    response = prompt(
+        f"Would you like EnderChest to add {ender_chest_abspath} to {symlink_allowlist}?",
+        "Y/n",
+    )
+
+    if response.lower() not in ("y", "yes"):
+        return
+
+    with symlink_allowlist.open("a") as f:
+        if allowlist_needs_newline:
+            f.write("\n")
+        f.write(ender_chest_abspath + "\n")
+
+    GATHER_LOGGER.info(f"{symlink_allowlist} updated.")
+
+
+def _needs_symlink_allowlist(version: str) -> bool:
+    """Determine if a version needs `allowed_symlinks.txt` in order to link
+    to EnderChest. Note that this is going a little broader than is strictly
+    necessary.
+
+    Parameters
+    ----------
+    version: str
+        The version string to check against
+
+    Returns
+    -------
+    bool
+        Returns False if the Minecraft version predates the symlink ban. Returns
+        True if it doesn't (or is marginal).
+
+    Notes
+    -----
+    Have I mentioned that parsing Minecraft version strings is a pain in the
+    toucans?
+    """
+    # first see if it follows basic semver
+    if _matches_version(">1.19", _parse_version(version.split("-")[0])):
+        return True
+    if _matches_version("1.20.0*", _parse_version(version.split("-")[0])):
+        return True
+    # is it a snapshot?
+    if match := re.match("^([1-2][0-9])w([0-9]{1,2})", version.lower()):
+        year, week = match.groups()
+        if int(year) > 23:
+            return True
+        if int(year) == 23 and int(week) > 18:
+            return True
+
+    return False
```

### Comparing `enderchest-0.1.0rc6/enderchest/instance.py` & `enderchest-0.1.0rc7/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/loggers.py` & `enderchest-0.1.0rc7/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/place.py` & `enderchest-0.1.0rc7/enderchest/place.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .shulker_box import ShulkerBox
 
 
 def place_ender_chest(
     minecraft_root: Path,
     cleanup: bool = True,
     error_handling: str = "abort",
+    relative: bool = True,
     rollback=False,
 ) -> None:
     """Link all instance files and folders to all shulker boxes
 
     Parameters
     ----------
     minecraft_root : Path
@@ -37,14 +38,18 @@
           - pass in `error_handling="skip"` to abort linking the current instance
             to the current shulker box but otherwise continue on
           - pass in `error_handling="skip-instance"` to abort linking the current
             instance altogether but to otherwise continue on with other instances
           - pass in `error_handling="skip-shulker-box"` to abort linking to the current
             shulker box altogether but to otherwise continue on with other boxes
           - pass in `error_handling="prompt"` to ask what to do on each failure
+    relative : bool, optional
+        By default, links will use relative paths when possible. To use absolute
+        paths instead (see: https://bugs.mojang.com/projects/MC/issues/MC-263046),
+        pass in `relative=False`.
     rollback: bool, optional
         In the future in the event of linking errors passing in `rollback=True`
         can be used to roll back any changes that have already been applied
         based on the error-handling method specified.
     """
     if rollback is not False:
         raise NotImplementedError("Rollbacks are not currently supported")
@@ -169,15 +174,15 @@
             resources.remove(fs.shulker_box_config(minecraft_root, shulker_box.name))
 
             match_exit = "pass"
             for link_folder in shulker_box.link_folders:
                 resources -= {box_root / link_folder}
                 resources -= set((box_root / link_folder).rglob("*"))
                 try:
-                    link_resource(link_folder, box_root, instance_root)
+                    link_resource(link_folder, box_root, instance_root, relative)
                 except (OSError, NotADirectoryError) as oh_no:
                     PLACE_LOGGER.error(
                         f"Error linking shulker box {shulker_box.name}"
                         f" to instance {instance.name}:"
                         f"\n  {(instance.root / link_folder)} is a"
                         " non-empty directory"
                     )
@@ -197,14 +202,15 @@
                 for resource in resources:
                     resource_path = resource.relative_to(box_root)
                     try:
                         link_resource(
                             resource_path,
                             box_root,
                             instance_root,
+                            relative,
                         )
                     except (OSError, NotADirectoryError) as oh_no:
                         PLACE_LOGGER.error(
                             f"Error linking shulker box {shulker_box.name}"
                             f" to instance {instance.name}:"
                             f"\n  {(instance.root / resource_path)}"
                             " already exists"
@@ -229,27 +235,34 @@
                         file.unlink()
 
             if match_exit == "break":
                 break
 
 
 def link_resource(
-    resource_path: str | Path, shulker_root: Path, instance_root: Path
+    resource_path: str | Path,
+    shulker_root: Path,
+    instance_root: Path,
+    relative: bool,
 ) -> None:
     """Create a symlink for the specified resource from an instance's space
     pointing to the tagged file / folder living inside a shulker box.
 
     Parameters
     ----------
     resource_path : str or Path
         Location of the resource relative to the instance's ".minecraft" folder
     shulker_root : Path
         The path to the shulker box
     instance_root : Path
         The path to the instance's ".minecraft" folder
+    relative : bool
+        If True, the link will be use a relative path if possible. Otherwise,
+        an absolute path will be used, regardless of whether a a relative or
+        absolute path was provided.
 
     Raises
     ------
     NotADirectoryError
         If a file already exists where you're attempting to place the symlink
     OSError
         If a non-empty directory already exists where you're attempting to
@@ -260,32 +273,32 @@
     - This method will create any folders that do not exist within an instance
     - This method will overwrite existing symlinks and empty folders
       but will not overwrite or delete any actual files.
     """
     instance_path = (instance_root / resource_path).expanduser().absolute()
     instance_path.parent.mkdir(parents=True, exist_ok=True)
 
-    relative_path = os.path.relpath(
-        (shulker_root / resource_path).expanduser().absolute(), instance_path.parent
-    )
+    target: str | Path = (shulker_root / resource_path).expanduser().absolute()
+    if relative:
+        target = os.path.relpath(target, instance_path.parent)
 
     if instance_path.is_symlink():
         # remove previous symlink in this spot
         PLACE_LOGGER.debug(f"Removing old link at {instance_path}")
         instance_path.unlink()
     else:
         try:
             os.rmdir(instance_path)
-            PLACE_LOGGER.debug(f"Removed empty diretory at {instance_path}")
+            PLACE_LOGGER.debug(f"Removed empty directory at {instance_path}")
         except FileNotFoundError:
             pass  # A-OK
 
-    PLACE_LOGGER.debug(f"Linking {instance_path} to {relative_path}")
+    PLACE_LOGGER.debug(f"Linking {instance_path} to {target}")
     os.symlink(
-        relative_path,
+        target,
         instance_path,
         target_is_directory=(shulker_root / resource_path).is_dir(),
     )
 
 
 def _rglob(root: Path, max_depth: int) -> Iterable[Path]:
     """Find all files (and directories* and symlinks) in the path up to the
```

### Comparing `enderchest-0.1.0rc6/enderchest/prompt.py` & `enderchest-0.1.0rc7/enderchest/prompt.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/remote.py` & `enderchest-0.1.0rc7/enderchest/remote.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/shulker_box.py` & `enderchest-0.1.0rc7/enderchest/shulker_box.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/sync/__init__.py` & `enderchest-0.1.0rc7/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/sync/file.py` & `enderchest-0.1.0rc7/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/sync/rsync.py` & `enderchest-0.1.0rc7/enderchest/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/conftest.py` & `enderchest-0.1.0rc7/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_cli.py` & `enderchest-0.1.0rc7/enderchest/test/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,32 +241,51 @@
         ids=("--ignore-errors", "--errors=ignore"),
     )
     def test_ignore_errors(self, place_log, flags):
         action, *_, options = cli.parse_args(["enderchest", "place", *flags])
         action(Path(), **options)
         assert place_log[0][1]["error_handling"] == "ignore"
 
+    def test_absolute_path_links_is_the_default(self, place_log):
+        action, *_, options = cli.parse_args(["enderchest", "place"])
+        action(Path(), **options)
+        assert place_log[0][1]["relative"] is False
+
+    @pytest.mark.parametrize(
+        "flag, expected",
+        (("-a", False), ("--absolute", False), ("-r", True), ("--relative", True)),
+    )
+    def test_explicitly_specify_abs_or_rel(self, place_log, flag, expected):
+        action, *_, options = cli.parse_args(["enderchest", "place"])
+        action(Path(), **options)
+        assert place_log[0][1]["relative"] is False
+
 
 class TestGather(ActionTestSuite):
     action = "gather minecraft"
     required_args = ("~",)
 
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
-    def test_gather_requires_at_least_one_search_path(self, with_root):
+    def test_gather_requires_at_least_one_search_path(self, with_root, capsys):
         more_args = ("--root", "/minecraft") if with_root else ()
         with pytest.raises(SystemExit):
             cli.parse_args(["enderchest", *self.action.split(), *more_args])
 
+        _ = capsys.readouterr()  # suppress outputs
+
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
-    def test_single_arg_interpreted_as_search_path(self, with_root):
+    def test_single_arg_interpreted_as_search_path(self, with_root, capsys):
         more_args = ("--root", ".") if with_root else ()
 
         _, root, _, options = cli.parse_args(
             ["enderchest", *self.action.split(), *more_args, "~"]
         )
+
+        _ = capsys.readouterr()  # suppress outputs
+
         assert (root.resolve(), options["search_paths"]) == (
             Path(".").resolve(),
             [Path("~")],
         )
 
     def test_first_arg_interpreted_as_root(self):  # I actually really don't like this
         _, root, _, options = cli.parse_args(
@@ -287,19 +306,21 @@
 
 
 class TestGatherRemote(ActionTestSuite):
     action = "gather enderchests"
     required_args = ("sftp://openbagtwo@steamdeck/home/deck",)
 
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
-    def test_gather_requires_at_least_one_remote(self, with_root):
+    def test_gather_requires_at_least_one_remote(self, with_root, capsys):
         more_args = ("--root", "/minecraft") if with_root else ()
         with pytest.raises(SystemExit):
             cli.parse_args(["enderchest", *self.action.split(), *more_args])
 
+        _ = capsys.readouterr()  # suppress outputs
+
     @pytest.mark.parametrize("with_root", (False, True), ids=("no_root", "with-root"))
     def test_single_arg_interpreted_as_remote(self, with_root):
         more_args = ("--root", ".") if with_root else ()
 
         _, root, _, options = cli.parse_args(
             [
                 "enderchest",
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_craft.py` & `enderchest-0.1.0rc7/enderchest/test/test_craft.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
             remotes=[
                 "irc://you@irl/home/upstairs",
                 ("file:///lockbox", "undisclosed location"),
             ],
             instances=utils.TESTING_INSTANCES,
         )
 
+        original_ender_chest.sync_confirm_wait = 27
+        original_ender_chest.offer_to_update_symlink_allowlist = False
+
         original_ender_chest.write_to_cfg(
             Path(tmpdir) / "EnderChest" / "enderchest.cfg"
         )
 
         parsed_ender_chest = EnderChest.from_cfg(
             Path(tmpdir) / "EnderChest" / "enderchest.cfg"
         )
@@ -187,45 +190,52 @@
         error_log = "\n".join(
             record.msg for record in caplog.records if record.levelname == "ERROR"
         )
         assert "There is already an EnderChest installed" in error_log
 
         assert fs.ender_chest_config(minecraft_root).read_text() == original_config
 
-    def test_craft_chest_from_config(self, minecraft_root, home, caplog):
+    def test_craft_chest_from_config(
+        self, minecraft_root, home, caplog, monkeypatch, capsys
+    ):
         # we'll be testing overwriting
         create_ender_chest(
             minecraft_root,
             EnderChest(
                 "sftp://openbagtwo@battlestation" + minecraft_root.absolute().as_posix()
             ),
         )
 
+        never = utils.scripted_prompt(["no"])
+        monkeypatch.setattr("builtins.input", never)
+
         craft.craft_ender_chest(
             minecraft_root,
             instance_search_paths=(minecraft_root / "instances", home),
             remotes=("rsync://deck@steamdeck/home/deck/minecraft",),
             overwrite=True,
         )
 
+        _ = capsys.readouterr()  # suppress outputs
+
         assert not [record for record in caplog.records if record.levelname == "ERROR"]
 
         chest = load_ender_chest(minecraft_root)
         assert len(chest.instances) == 4
         assert len(chest.remotes) == 1
 
     def test_giving_default_responses_results_in_the_expected_chest(
         self,
         monkeypatch,
         minecraft_root,
         home,
         capsys,
         caplog,
     ):
-        script_reader = utils.scripted_prompt([""] * 7)
+        script_reader = utils.scripted_prompt([""] * 8)
         monkeypatch.setattr("builtins.input", script_reader)
 
         chest = craft.specify_ender_chest_from_prompt(minecraft_root)
 
         _ = capsys.readouterr()  # suppress outputs
 
         assert not [record for record in caplog.records if record.levelname == "ERROR"]
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_instance.py` & `enderchest-0.1.0rc7/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_place.py` & `enderchest-0.1.0rc7/enderchest/test/test_place.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,22 @@
 
         yield
 
         # check on teardown that all those "do_not_touch" files are untouched
         for path, contents in do_not_touch.items():
             assert path.read_text() == contents
 
+    @pytest.mark.parametrize("relative", (True, False), ids=("relative", "absolute"))
+    @utils.parametrize_over_instances("official", "axolotl")
+    def test_respects_the_relative_parameter(self, minecraft_root, instance, relative):
+        place.place_ender_chest(minecraft_root, relative=relative)
+        instance_folder = utils.resolve(instance.root, minecraft_root)
+
+        assert (instance_folder / "logs").readlink().is_absolute() is (not relative)
+
     @utils.parametrize_over_instances("official", "axolotl")
     def test_place_replaces_empty_folders(self, minecraft_root, instance):
         place.place_ender_chest(minecraft_root)
         instance_folder = utils.resolve(instance.root, minecraft_root)
 
         assert (instance_folder / "logs").resolve() == (
             minecraft_root / "EnderChest" / "global" / "logs"
```

### Comparing `enderchest-0.1.0rc6/enderchest/test/test_sync.py` & `enderchest-0.1.0rc7/enderchest/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.0rc7/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.0rc7/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/enderchest/test/utils.py` & `enderchest-0.1.0rc7/enderchest/test/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,16 +242,16 @@
     Returns
     -------
     list of ShulkerBox
         A list of parsed shulker boxes corresponding to the ones rendered
         on the system
     """
     enderchest_folder.mkdir(parents=True, exist_ok=True)
-    with as_file(testing_files.ENDERCHEST_CONFIG) as enderchest_cfg:
-        shutil.copy(enderchest_cfg, enderchest_folder)
+    with as_file(testing_files.ENDERCHEST_CONFIG) as config_file:
+        shutil.copy(config_file, enderchest_folder)
     shulker_boxes: list[ShulkerBox] = []
     for shulker_name, shulker_config in shulkers:
         (enderchest_folder / shulker_name).mkdir(parents=True, exist_ok=True)
         config_path = enderchest_folder / shulker_name / fs.SHULKER_BOX_CONFIG_NAME
         with config_path.open("w") as config_file:
             config_file.write(shulker_config)
         shulker_boxes.append(ShulkerBox.from_cfg(config_path))
@@ -356,17 +356,17 @@
     """Parse the above table of shulker-to-instance matches"""
     matches: list[tuple[str, str, bool]] = []
     rows = MATCH_CSV.splitlines()
     header = rows.pop(0)
     shulker_boxes = [cell.strip() for cell in header.split(",")[1:]]
     for row in rows:
         cells = [cell.strip() for cell in row.split(",")]
-        instance = cells.pop(0)
+        mc = cells.pop(0)
         for i, cell in enumerate(cells):
-            matches.append((shulker_boxes[i], instance, cell == "True"))
+            matches.append((shulker_boxes[i], mc, cell == "True"))
     return matches
 
 
 TESTING_SHULKER_INSTANCE_MATCHES = tuple(_parse_match_csv())
 
 
 def resolve(path: Path, minecraft_root: Path) -> Path:
@@ -402,15 +402,15 @@
         instances will be included
 
     Notes
     -----
       - The parametrized tests will be ordered as provided
       - The name of the parametrized argument provided to the test will be "instance"
     """
-    instance_lookup = {instance.name: instance for instance in TESTING_INSTANCES}
+    instance_lookup = {mc.name: mc for mc in TESTING_INSTANCES}
     if len(instance_names) == 0:
         instance_names = tuple(instance_lookup.keys())
 
     instances = [instance_lookup[name] for name in instance_names]
 
     return pytest.mark.parametrize("instance", instances, ids=instance_names)
 
@@ -448,18 +448,16 @@
 ) -> InstanceSpec:
     """Shortcut constructor"""
     return InstanceSpec(
         name, root, tuple(minecraft_versions or ()), modloader, tuple(tags or ())
     )
 
 
-def normalize_instance(instance: InstanceSpec) -> InstanceSpec:
+def normalize_instance(mc: InstanceSpec) -> InstanceSpec:
     """Normalize the values inside an instance tuple"""
-    return instance._replace(
+    return mc._replace(
         # this should be fully checked by instance.equals()
-        root=instance.root.expanduser().relative_to(
-            instance.root.expanduser().parent.parent
-        ),
-        modloader=_normalize_modloader(instance.modloader)[0],
-        minecraft_versions=tuple(sorted(instance.minecraft_versions)),
-        tags=tuple(sorted(tag.lower() for tag in instance.tags)),
+        root=mc.root.expanduser().relative_to(mc.root.expanduser().parent.parent),
+        modloader=_normalize_modloader(mc.modloader)[0],
+        minecraft_versions=tuple(sorted(mc.minecraft_versions)),
+        tags=tuple(sorted(tag.lower() for tag in mc.tags)),
     )
```

### Comparing `enderchest-0.1.0rc6/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.0rc7/enderchest.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -33,14 +33,31 @@
 EnderChest is a command-line utility for selectively sharing Minecraft assets
 (configurations, mods, worlds, etc.)...
 
 1. ...across different computers
 1. ...across different instances on the same computer
 1. ...across server and client installations
 
+### A Note On Linking
+
+Starting with Minecraft 1.20, Mojang by default
+[no longer allows worlds to load if they are or if they contain symbolic links](https://help.minecraft.net/hc/en-us/articles/16165590199181).
+While it is true that an improper symlink could cause Minecraft to write data
+to a place it shouldn't, nothing in EnderChest will ever generate a symlink whose
+target is outside of your EnderChest folder _unless you place_ a symbolic link in
+your EnderChest pointing to somewhere else (which you may want to do so that your
+screenshots, for example, point to your "My Pictures" folder).
+
+If you still have concerns about symlinks or questions about how they work,
+read through
+[this guide](https://www.makeuseof.com/tag/what-is-a-symbolic-link-what-are-its-uses-makeuseof-explains/)
+or [watch this explainer](https://www.youtube.com/watch?v=mA08E59-zo8), and if
+you still have questions, feel free to
+[open an issue](https://github.com/OpenBagTwo/EnderChest/issues/new?assignees=OpenBagTwo&labels=question&title=symlink%20question).
+
 ## Installation
 
 EnderChest is written for **Python 3.10 or greater,** but should otherwise
 run on any architecture or operating system.
 
 The latest release can be installed from PyPI via `pip`:
```

### Comparing `enderchest-0.1.0rc6/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.0rc7/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/setup.py` & `enderchest-0.1.0rc7/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.0rc6/versioneer.py` & `enderchest-0.1.0rc7/versioneer.py`

 * *Files identical despite different names*

