# Comparing `tmp/skulk-2.0.0-py2.py3-none-any.whl.zip` & `tmp/skulk-2.0.0rc1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8891 bytes, number of entries: 10
--rw-r--r--  2.0 unx        5 b- defN 23-May-31 02:38 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-May-31 02:37 skulk/__init__.py
--rw-r--r--  2.0 unx     9348 b- defN 23-May-31 02:37 skulk/bumper.py
--rw-r--r--  2.0 unx     9146 b- defN 23-May-31 02:37 skulk/skulk.py
--rw-r--r--  2.0 unx     2625 b- defN 23-May-31 02:37 skulk/util.py
--rw-r--r--  2.0 unx      646 b- defN 23-May-31 02:38 skulk-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-31 02:38 skulk-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-May-31 02:38 skulk-2.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-31 02:38 skulk-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      733 b- defN 23-May-31 02:38 skulk-2.0.0.dist-info/RECORD
-10 files, 22663 bytes uncompressed, 7649 bytes compressed:  66.2%
+Zip file size: 8921 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       10 b- defN 23-May-30 06:09 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 06:09 skulk/__init__.py
+-rw-r--r--  2.0 unx     9348 b- defN 23-May-30 06:09 skulk/bumper.py
+-rw-r--r--  2.0 unx     9105 b- defN 23-May-30 06:09 skulk/skulk.py
+-rw-r--r--  2.0 unx     2625 b- defN 23-May-30 06:09 skulk/util.py
+-rw-r--r--  2.0 unx      649 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      749 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/RECORD
+10 files, 22646 bytes uncompressed, 7649 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.0.0.dist-info/METADATA
+Filename: skulk-2.0.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.0.0.dist-info/WHEEL
+Filename: skulk-2.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.0.0.dist-info/entry_points.txt
+Filename: skulk-2.0.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.0.0.dist-info/top_level.txt
+Filename: skulk-2.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.0.0.dist-info/RECORD
+Filename: skulk-2.0.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.0.0
+2.0.0-rc.1
```

## skulk/skulk.py

```diff
@@ -50,15 +50,15 @@
         self.working_dir = self.repo.working_dir
         self.hook_filename = os.path.join(self.working_dir, ".git", "hooks", "pre-push")
         self.changelog_filename = os.path.join(self.working_dir, "CHANGELOG.md")
         self.version_filename = os.path.join(self.working_dir, "VERSION")
         self.pip_name = util.get_pip_name(self.repo)
         self.bumper = None
         self.edit_changelog = False
-        self.changelog_addition = ""
+        self.changelog_addition = None
 
     def run(self):
         """
         Guide the user to ensure version and changelog are valid.
         """
 
         # wizard.check_pre_push_hook()
@@ -195,20 +195,19 @@
 
         if self.edit_changelog:
             commits = self.get_commits()
             commit_messages = ["\n# Raw commit messages for reference.\n"]
             commit_messages.extend([f"* {c.summary} [{c.hexsha[:7]}]" for c in commits])
             commit_block = "\n".join(commit_messages) or ""
 
-            print("Here are some recent commits for reference:")
             print(commit_block)
 
-            # self.changelog_addition = commit_block
+            self.changelog_addition = commit_block
             if write_block:
-                self.changelog_addition = block
+                self.changelog_addition = commit_block + "\n\n" + block
 
     def resolve_changelog(self):
         """Help the user to get the changelog file up-to-date."""
         with open(self.changelog_filename, "r", encoding="utf-8") as clog:
             content = clog.read() or "--"
 
         content = self.changelog_addition + "\n\n" + content
```

## Comparing `skulk-2.0.0.dist-info/METADATA` & `skulk-2.0.0rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

