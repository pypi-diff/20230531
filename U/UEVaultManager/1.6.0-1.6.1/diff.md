# Comparing `tmp/UEVaultManager-1.6.0.tar.gz` & `tmp/UEVaultManager-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.6.0.tar", last modified: Fri May 26 09:33:08 2023, max compression
+gzip compressed data, was "UEVaultManager-1.6.1.tar", last modified: Wed May 31 15:36:42 2023, max compression
```

## Comparing `UEVaultManager-1.6.0.tar` & `UEVaultManager-1.6.1.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:08.110046 UEVaultManager-1.6.0/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     6125 2023-05-26 09:33:08.109046 UEVaultManager-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:07.945317 UEVaultManager-1.6.0/UEVaultManager/
--rw-rw-rw-   0        0        0      776 2023-05-26 09:30:41.000000 UEVaultManager-1.6.0/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:07.989783 UEVaultManager-1.6.0/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-25 16:36:39.000000 UEVaultManager-1.6.0/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.0/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:07.992785 UEVaultManager-1.6.0/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.0/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.0/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0    72462 2023-05-26 08:33:52.000000 UEVaultManager-1.6.0/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    47576 2023-05-25 16:37:11.000000 UEVaultManager-1.6.0/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:07.993785 UEVaultManager-1.6.0/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:08.007946 UEVaultManager-1.6.0/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.6.0/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.0/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:08.025946 UEVaultManager-1.6.0/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.0/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.0/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23585 2023-05-26 09:04:11.000000 UEVaultManager-1.6.0/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.0/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.6.0/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:08.049945 UEVaultManager-1.6.0/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-25 16:35:27.000000 UEVaultManager-1.6.0/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.6.0/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.0/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.0/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.0/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.0/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.0/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30505 2023-05-25 16:36:21.000000 UEVaultManager-1.6.0/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:08.056944 UEVaultManager-1.6.0/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1694 2023-05-26 08:33:52.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:08.088045 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6799 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4683 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6674 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    33896 2023-05-26 08:33:28.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14553 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0    13326 2023-05-26 09:11:59.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14067 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6145 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    42998 2023-05-26 08:32:35.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-25 16:37:42.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0     9681 2023-05-25 16:59:35.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     5390 2023-05-26 07:28:45.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/functions_no_deps.py
--rw-rw-rw-   0        0        0     2631 2023-05-25 16:37:41.000000 UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:08.108046 UEVaultManager-1.6.0/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3478 2023-05-25 16:35:05.000000 UEVaultManager-1.6.0/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.6.0/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.0/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.6.0/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.0/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.0/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.0/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:33:07.977035 UEVaultManager-1.6.0/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6125 2023-05-26 09:33:07.000000 UEVaultManager-1.6.0/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2269 2023-05-26 09:33:07.000000 UEVaultManager-1.6.0/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 09:33:07.000000 UEVaultManager-1.6.0/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-26 09:33:07.000000 UEVaultManager-1.6.0/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      286 2023-05-26 09:33:07.000000 UEVaultManager-1.6.0/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 09:33:07.000000 UEVaultManager-1.6.0/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 09:33:08.110046 UEVaultManager-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.455720 UEVaultManager-1.6.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     6127 2023-05-31 15:36:42.455720 UEVaultManager-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.416697 UEVaultManager-1.6.1/UEVaultManager/
+-rw-rw-rw-   0        0        0      778 2023-05-31 15:32:58.000000 UEVaultManager-1.6.1/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.423696 UEVaultManager-1.6.1/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25469 2023-05-25 16:36:39.000000 UEVaultManager-1.6.1/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.1/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.425696 UEVaultManager-1.6.1/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.1/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.6.1/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.1/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.6.1/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    72462 2023-05-26 08:33:52.000000 UEVaultManager-1.6.1/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47576 2023-05-25 16:37:11.000000 UEVaultManager-1.6.1/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.426697 UEVaultManager-1.6.1/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.428696 UEVaultManager-1.6.1/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.6.1/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.1/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.432721 UEVaultManager-1.6.1/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.1/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.1/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23585 2023-05-26 09:04:11.000000 UEVaultManager-1.6.1/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.1/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.6.1/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.438720 UEVaultManager-1.6.1/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-25 16:35:27.000000 UEVaultManager-1.6.1/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.6.1/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.1/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.1/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.1/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.1/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.1/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30505 2023-05-25 16:36:21.000000 UEVaultManager-1.6.1/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.439721 UEVaultManager-1.6.1/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1694 2023-05-26 08:33:52.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.449721 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    33931 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0    13332 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    43221 2023-05-31 15:30:23.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0     9681 2023-05-25 16:59:35.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     5756 2023-05-31 13:10:59.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/functions_no_deps.py
+-rw-rw-rw-   0        0        0     2631 2023-05-31 15:29:53.000000 UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.454721 UEVaultManager-1.6.1/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3478 2023-05-25 16:35:05.000000 UEVaultManager-1.6.1/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-05-18 09:32:02.000000 UEVaultManager-1.6.1/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.1/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.6.1/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.1/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.1/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.1/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:36:42.420697 UEVaultManager-1.6.1/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6127 2023-05-31 15:36:42.000000 UEVaultManager-1.6.1/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-05-31 15:36:42.000000 UEVaultManager-1.6.1/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:36:42.000000 UEVaultManager-1.6.1/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-31 15:36:42.000000 UEVaultManager-1.6.1/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      300 2023-05-31 15:36:42.000000 UEVaultManager-1.6.1/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 15:36:42.000000 UEVaultManager-1.6.1/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 15:36:42.455720 UEVaultManager-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.1/setup.py
```

### Comparing `UEVaultManager-1.6.0/LICENSE` & `UEVaultManager-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/PKG-INFO` & `UEVaultManager-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.0
+Version: 1.6.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.6.0 ## codename: Virgo
+ UEVaultManager ## version:1.6.1 ## codename: Virgo+1
```

### Comparing `UEVaultManager-1.6.0/README.md` & `UEVaultManager-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/__init__.py` & `UEVaultManager-1.6.1/UEVaultManager/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.6.0'
+__version__ = '1.6.1'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
 # 5 Virgo Shaka
-__codename__ = 'Virgo'
+__codename__ = 'Virgo+1'
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/api/egs.py` & `UEVaultManager-1.6.1/UEVaultManager/api/egs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/api/uevm.py` & `UEVaultManager-1.6.1/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.6.1/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/assets/main.ico` & `UEVaultManager-1.6.1/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/cli.py` & `UEVaultManager-1.6.1/UEVaultManager/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/core.py` & `UEVaultManager-1.6.1/UEVaultManager/core.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.6.1/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.6.1/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.6.1/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.6.1/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.6.1/UEVaultManager/lfs/uevmlfs.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.6.1/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.6.1/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/app.py` & `UEVaultManager-1.6.1/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/chunk.py` & `UEVaultManager-1.6.1/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/config.py` & `UEVaultManager-1.6.1/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/csv.py` & `UEVaultManager-1.6.1/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/downloading.py` & `UEVaultManager-1.6.1/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/egl.py` & `UEVaultManager-1.6.1/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.6.1/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/models/manifest.py` & `UEVaultManager-1.6.1/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/main.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 
         def __init__(self, container):
             super().__init__(container)
             pack_def_options = {'ipadx': 3, 'ipady': 3}
 
             text_content = ExtendedText(self)
             scrollbar = ttk.Scrollbar(self)
-            scrollbar.pack(side="right", fill="y")
             scrollbar.config(command=text_content.yview)
             text_content.config(yscrollcommand=scrollbar.set)
             scrollbar.pack(side=tk.RIGHT, fill=tk.Y, **pack_def_options)
             text_content.pack(side=tk.LEFT, fill=tk.BOTH, expand=True, **pack_def_options)
 
             self.text_content = text_content
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     def set_colors(self) -> None:
         """
         Initializes the colors of some cells depending on their values.
         """
         if not gui_g.s.use_colors_for_data:
             self.redraw()
             return
-        log_debug(f'set_colors')
+        log_debug('set_colors')
         self.gradient_color_cells(col_names=['Review'], cmap='Set3', alpha=1)
         self.color_cells_if(col_names=['Purchased', 'On sale'], color='lightgreen', value_to_check='True')
         self.color_cells_if(col_names=['Grab result'], color='lightblue', value_to_check='NO_ERROR')
         self.color_cells_if_not(col_names=['Status'], color='#555555', value_to_check='ACTIVE')
         self.color_rows_if(col_names=['Status'], color='#555555', value_to_check='SUNSET')
         self.color_rows_if(col_names=['Obsolete'], color='#777777', value_to_check='True')
         self.redraw()
@@ -256,15 +256,15 @@
             start = min(start, len(self.data))
             end = min(end, len(self.data))
             try:
                 # Update table with data for current page
                 self.model.df = self.data.iloc[start:end]
             except AttributeError:
                 # self.redraw()
-                log_debug(f'AttributeError in show_page')
+                log_debug('AttributeError in show_page')
                 self.set_colors()
                 return
         else:
             # Update table with all data
             self.model.df = self.data_filtered
             self.current_page = 0
         # self.redraw()
@@ -556,15 +556,15 @@
                 button = ttk.Button(inner_frame_url, text="Open URL", command=self.open_asset_url)
                 button.pack(side=tk.RIGHT)
             elif lower_key in ('description', 'comment'):
                 entry = ExtendedText(edit_row_window.content_frame, height=3)
                 entry.set_content(value)
                 entry.grid(row=i, column=1, sticky=tk.EW)
             elif lower_key in ('must buy', 'obsolete', 'purchased', 'on sale'):
-                entry = ExtendedCheckButton(edit_row_window.content_frame, label='')
+                entry = ExtendedCheckButton(edit_row_window.content_frame, label='', images_folder=gui_g.s.assets_folder)
                 entry.set_content(value)
                 entry.grid(row=i, column=1, sticky=tk.EW)
             else:
                 # other field is just a usual entry
                 entry = ttk.Entry(edit_row_window.content_frame)
                 entry.insert(0, value)
                 entry.grid(row=i, column=1, sticky=tk.EW)
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         if master is None:
             print('A container is needed to display this widget')
             return
         ext_args = self._extract_extended_args(kwargs, function_signature=ExtendedWidget.__init__)
         ExtendedWidget.__init__(self, **ext_args)
         # by default , images are searched in a folder named 'statics' in the directory of this file
         if images_folder is None:
-            images_folder = path_from_relative_to_absolute('./statics/')
+            images_folder = path_from_relative_to_absolute('./assets/')
         self._img_checked = tk.PhotoImage(file=os.path.join(images_folder, 'checked_16.png'))  # Path to the checked image
         self._img_uncheckked = tk.PhotoImage(file=os.path.join(images_folder, 'unchecked_16.png'))  # Path to the unchecked image
         self.widget_type = WidgetType.CHECKBUTTON
         self.default_content = False
         self._var = tk.BooleanVar(value=self.default_content)
         frm_inner = ttk.Frame(master)
         lbl_text = ttk.Label(frm_inner, text='')  # no text bydefault
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         # the following folders are relative to the current file location
         # they must be used trought path_from_relative_to_absolute
         # following vars are not set as properties to avoid storing absolute paths in the config file
         self.cache_folder = gui_fn.path_from_relative_to_absolute(self.config_vars['cache_folder'])
         self.results_folder = gui_fn.path_from_relative_to_absolute(self.config_vars['results_folder'])
 
-        # Folder for assets (aka. images, icon... not "UE assets") used for the GUI. THIS IS NOT A SETTING
+        # Folder for assets (aka. images, icon... not "UE assets") used for the GUI. THIS IS NOT A SETTING THAT CAN BE CHANGED BY THE USER
         self.assets_folder = gui_fn.path_from_relative_to_absolute('../../assets')
 
         self.app_icon_filename = os.path.join(self.assets_folder, 'main.ico')
         self.default_image_filename = os.path.join(self.assets_folder, 'UEVM_200x200.png')
 
         if self.config_vars['reopen_last_file'] and os.path.isfile((self.config_vars['last_opened_file'])):
             self.csv_filename = self.config_vars['last_opened_file']
@@ -196,15 +196,15 @@
         else:
             self.config_path = os.path.join(self.path, 'config_gui.ini')
 
         # try loading config
         try:
             self.config.read(self.config_path)
         except Exception as error:
-            log(f'Unable to read configuration file, please ensure that file is valid! '
+            log('Unable to read configuration file, please ensure that file is valid! '
                 f'(Error: {repr(error)})')
             log('Continuing with blank config in safe-mode...')
             self.config.read_only = True
 
         # make sure "UEVaultManager" section exists
         has_changed = False
         if 'UEVaultManager' not in self.config:
@@ -267,14 +267,13 @@
             return
 
         # if config file has been modified externally, back-up the user-modified version before writing
         if os.path.exists(self.config_path):
             if (mod_time := int(os.stat(self.config_path).st_mtime)) != self.config.mod_time:
                 new_filename = f'config.{mod_time}.ini'
                 log(
-                    f'Configuration file has been modified while UEVaultManager was running, '
-                    f'user-modified config will be renamed to "{new_filename}"...'
+                    f'Configuration file has been modified while UEVaultManager was running\nUser-modified config will be renamed to "{new_filename}"...'
                 )
                 os.rename(self.config_path, os.path.join(os.path.dirname(self.config_path), new_filename))
 
         with open(self.config_path, 'w') as cf:
             self.config.write(cf)
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 """
 Implementation for:
 - TaggedLabelFrame: a custom LabelFrame widget that allows child widgets to be identified by tags
 """
 import tkinter as tk
 from tkinter import ttk
 
-import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 from UEVaultManager.tkgui.modules.ExtendedWidgetClasses import WidgetType, ExtendedWidget, ExtendedEntry, ExtendedText, ExtendedLabel, \
     ExtendedCheckButton
 from UEVaultManager.tkgui.modules.functions import log_error, log_warning, log_debug
-from UEVaultManager.tkgui.modules.functions_no_deps import path_from_relative_to_absolute
 
 
 class TaggedLabelFrame(ttk.LabelFrame):
     """
     A custom LabelFrame widget that allows child widgets to be identified by tags.
     :param args: Args to pass to the widget
     :param kwargs: Kwargs to pass to the widget
@@ -33,29 +31,31 @@
         tag: str,
         widget_type: WidgetType.ENTRY,
         default_content=None,
         width=None,
         height=None,
         label=None,
         layout_option='',
+        images_folder=None,
         add_label_before=True,
         focus_out_callback=None,
         click_on_callback=None
     ) -> None:
         """
         Adds a child widget to the LabelFrame and associates it with the given tag.
         Note: we can not use command parameter to manage callback here because it should be transmited
         to the parent widget and in that case tag won't be available as an indentificator
         :param tag: Tag to search for (case-insensitive)
         :param widget_type: Type of widget to add. A string value of 'text', 'checkbutton', or 'entry'
         :param width: Width of the child widget. Only used for text widgets
         :param height: Height of the child widget. Only used for text widgets
         :param label: Text to display in the child widget.
         :param default_content: Default content of the child widget
-        :param layout_option: Layout options to use. Default, full width.
+        :param layout_option: Layout options to use. Default, full width
+        :param images_folder: folder for image used by some widgets
         :param add_label_before: If True, adds a label before the child widget
         :param focus_out_callback: Callback to call when the child widget loses focus
         :param click_on_callback: Callback to call when the child widget is clicked or checked
         """
         tag = tag.lower()
         frame = ttk.Frame(self)
         frame.pack(**self.lblf_fw_options)
@@ -65,17 +65,18 @@
         if widget_type == WidgetType.ENTRY:
             child = ExtendedEntry(master=frame, tag=tag, default_content=default_content, height=height, width=width)
         elif widget_type == WidgetType.TEXT:
             child = ExtendedText(master=frame, tag=tag, default_content=default_content, wrap=tk.WORD, height=height, width=width)
         elif widget_type == WidgetType.LABEL:
             child = ExtendedLabel(master=frame, tag=tag, default_content=default_content)
         elif widget_type == WidgetType.CHECKBUTTON:
-            child = ExtendedCheckButton(master=frame, tag=tag, default_content=default_content, label=label)
+            child = ExtendedCheckButton(master=frame, tag=tag, default_content=default_content, label=label, images_folder=images_folder)
         else:
-            log_error(f'Invalid widget type: {widget_type}')
+            error = f'Invalid widget type: {widget_type}'
+            log_error(error)
             return
 
         self._tagged_child[tag] = child
 
         layout_option = self.pack_fw_options if layout_option == '' else layout_option
         child.pack(side=tk.LEFT, **layout_option)
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,24 +75,24 @@
         self.editable_table.bind('<Motion>', self.on_mouse_over_cell)
         self.editable_table.bind('<Leave>', self.on_mouse_leave_cell)
         self.editable_table.bind('<<CellSelectionChanged>>', self.on_selection_change)
         self.protocol('WM_DELETE_WINDOW', self.on_close)
 
         if show_open_file_dialog:
             if self.load_file() == '':
-                gui_f.log_error(f'This application could not run without a file to read data from')
+                gui_f.log_error('This application could not run without a file to read data from')
                 self.quit()
 
         # Quick edit the first row
         self.editable_table.update_quick_edit(quick_edit_frame=self.control_frame.lbtf_quick_edit, row=0)
 
         if rebuild_data or self.editable_table.must_rebuild:
             if gui_f.box_okcancel('Data are invalid or empty. They will be rebuilt from sources files. Do you want to continue ?'):
                 if not self.editable_table.rebuild_data():
-                    gui_f.log_error(f'Rebuild data error. This application could not run without a file to read from or some data to build from it')
+                    gui_f.log_error('Rebuild data error. This application could not run without a file to read from or some data to build from it')
                     self.destroy()  # self.quit() won't work here
                     return
             else:
                 self.destroy()  # self.quit() won't work here
 
     class ToolbarFrame(ttk.Frame):
         """
@@ -303,15 +303,20 @@
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Url', focus_out_callback=container.on_quick_edit_focus_out)
             lbtf_quick_edit.add_child(
                 widget_type=WidgetType.TEXT, tag='Comment', focus_out_callback=container.on_quick_edit_focus_out, width=10, height=4
             )
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Stars', focus_out_callback=container.on_quick_edit_focus_out)
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Test result', focus_out_callback=container.on_quick_edit_focus_out)
             lbtf_quick_edit.add_child(
-                widget_type=WidgetType.CHECKBUTTON, tag='Must buy', label='', click_on_callback=container.on_switch_edit_flag, default_content=False
+                widget_type=WidgetType.CHECKBUTTON,
+                tag='Must buy',
+                label='',
+                images_folder=gui_g.s.assets_folder,
+                click_on_callback=container.on_switch_edit_flag,
+                default_content=False
             )
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Installed folder', default_content='Installed in')
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Origin', focus_out_callback=container.on_quick_edit_focus_out)
             lbtf_quick_edit.add_child(widget_type=WidgetType.ENTRY, tag='Alternative', focus_out_callback=container.on_quick_edit_focus_out)
 
             lbt_image_preview = ttk.LabelFrame(self, text='Image Preview')
             lbt_image_preview.pack(**lblf_fw_options, anchor=tk.SW)
@@ -822,14 +827,17 @@
     def run_cli_command(self, command_name='') -> None:
         """
         Execute the 'status' command and display the result in DisplayContentWindow
         :param command_name: the name of the command to execute
         """
         if command_name == '':
             return
+        if gui_g.UEVM_cli_ref is None:
+            gui_f.from_cli_only_message()
+            return
         row = self.editable_table.getSelectedRow()
         col = self.editable_table.model.df.columns.get_loc('App name')
         app_name = self.editable_table.model.getValueAt(row, col)
 
         # gui_g.UEVM_cli_args['offline'] = True  # speed up some commands
         # set default options for the cli command to execute
         gui_g.UEVM_cli_args['gui'] = True
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/functions.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/functions_no_deps.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/functions_no_deps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 # coding=utf-8
 """
 Utilities functions and tools
 These functions DO NOT depend on the globals.py module and be freely imported
 """
 import ctypes as ct
 import os
+import sys
 
 import ttkbootstrap as ttk
 from screeninfo import get_monitors
 
 
 def path_from_relative_to_absolute(path: str) -> str:
     """
     Build the path of the file to reference relative to the currently running script
     :param path: the relative path to the file. If the path is already absolute, it is returned as is
     :return: the absolute path of the file
     """
+
     if os.path.isabs(path):
         return path
-    current_script_path = os.path.abspath(__file__)
-    current_script_directory = os.path.dirname(current_script_path)
+
+    try:
+        # PyInstaller creates a temp folder and stores path in _MEIPASS
+        # noinspection PyProtectedMember,PyUnresolvedReferences
+        # base_path = sys._MEIPASS
+        current_script_directory = sys._MEIPASS
+    except AttributeError:
+        # base_path = os.path.abspath(".")
+        current_script_path = os.path.abspath(__file__)
+        current_script_directory = os.path.dirname(current_script_path)
+
     absolute_path = os.path.join(current_script_directory, path)
-    return os.path.abspath(absolute_path)
+    absolute_path = os.path.abspath(absolute_path)
+    return absolute_path
 
 
 def center_window_on_screen(screen_index: int, height: int, width: int) -> str:
     """
     Calculate the geometry of the window to display in the center of the given screen
     :param screen_index: the index of the screen to use
     :param height: the height of the window
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.6.1/UEVaultManager/tkgui/modules/globals.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.6.1/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/utils/cli.py` & `UEVaultManager-1.6.1/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.6.1/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.6.1/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.6.1/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.6.1/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.0/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.6.1/UEVaultManager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.0
+Version: 1.6.1
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.6.0 ## codename: Virgo
+ UEVaultManager ## version:1.6.1 ## codename: Virgo+1
```

### Comparing `UEVaultManager-1.6.0/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.6.1/UEVaultManager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 UEVaultManager.egg-info/entry_points.txt
 UEVaultManager.egg-info/requires.txt
 UEVaultManager.egg-info/top_level.txt
 UEVaultManager/api/__init__.py
 UEVaultManager/api/egs.py
 UEVaultManager/api/uevm.py
 UEVaultManager/assets/UEVM_200x200.png
+UEVaultManager/assets/checked_16.png
 UEVaultManager/assets/main.ico
+UEVaultManager/assets/unchecked_16.png
 UEVaultManager/downloader/__init__.py
 UEVaultManager/downloader/mp/__init__.py
 UEVaultManager/downloader/mp/manager.py
 UEVaultManager/downloader/mp/workers.py
 UEVaultManager/lfs/__init__.py
 UEVaultManager/lfs/egl.py
 UEVaultManager/lfs/eos.py
```

### Comparing `UEVaultManager-1.6.0/setup.py` & `UEVaultManager-1.6.1/setup.py`

 * *Files identical despite different names*

