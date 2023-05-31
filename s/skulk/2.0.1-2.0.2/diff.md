# Comparing `tmp/skulk-2.0.1-py2.py3-none-any.whl.zip` & `tmp/skulk-2.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8872 bytes, number of entries: 10
--rw-r--r--  2.0 unx        5 b- defN 23-May-31 06:10 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-May-31 06:10 skulk/__init__.py
--rw-r--r--  2.0 unx     9548 b- defN 23-May-31 06:10 skulk/bumper.py
--rw-r--r--  2.0 unx     9146 b- defN 23-May-31 06:10 skulk/skulk.py
--rw-r--r--  2.0 unx     2625 b- defN 23-May-31 06:10 skulk/util.py
--rw-r--r--  2.0 unx      646 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      733 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/RECORD
-10 files, 22863 bytes uncompressed, 7630 bytes compressed:  66.6%
+Zip file size: 8945 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        5 b- defN 23-May-31 20:30 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 20:30 skulk/__init__.py
+-rw-r--r--  2.0 unx     9548 b- defN 23-May-31 20:30 skulk/bumper.py
+-rw-r--r--  2.0 unx     8984 b- defN 23-May-31 20:30 skulk/skulk.py
+-rw-r--r--  2.0 unx     3128 b- defN 23-May-31 20:30 skulk/util.py
+-rw-r--r--  2.0 unx      646 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      733 b- defN 23-May-31 20:30 skulk-2.0.2.dist-info/RECORD
+10 files, 23204 bytes uncompressed, 7703 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.0.1.dist-info/METADATA
+Filename: skulk-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.0.1.dist-info/WHEEL
+Filename: skulk-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.0.1.dist-info/entry_points.txt
+Filename: skulk-2.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.0.1.dist-info/top_level.txt
+Filename: skulk-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.0.1.dist-info/RECORD
+Filename: skulk-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.0.1
+2.0.2
```

## skulk/skulk.py

```diff
@@ -168,60 +168,73 @@
             sys.exit(0)
 
     def ask_do_tag_release(self):
         """Ask the user if he wants to make a pre-release from this branch."""
         return util.yes_no(
             "Do you want to tag and deploy from this branch?",
             "No, push only",
-            "Yes, push and deploy a taged release.",
+            "Yes, push and deploy a tagged release.",
         )
 
     def ask_changelog_additions(self):
         """Generate the reference additions to the changelog.
 
         Do not write anything to the changelog file yet."""
-        block = ""
-        write_block = self.bumper.next_version or self.changelog_needs_unreleased_stub()
+        stub = ""
         if self.bumper.next_version:
             self.edit_changelog = True
             date_string = datetime.date.today().strftime("%d %b %Y")
-            block = f"## Version:{self.bumper.next_version} -- {date_string}\n\n"
+            stub = f"## Version:{self.bumper.next_version} -- {date_string}\n\n"
         else:
             self.edit_changelog = util.yes_no(
                 "No version bump. Do you want to add entries in the changelog anyway?"
             )
-            block = "## Unreleased\n\n"
-        sections = ["Added", "Changed", "Deprecated", "Removed", "Fixed", "Security"]
-        block += "\n".join([f"### {s}\n" for s in sections])
+            stub = "## Unreleased\n\n"
 
         if self.edit_changelog:
-            commits = self.get_commits()
-            commit_messages = ["\n# Raw commit messages for reference.\n"]
-            commit_messages.extend([f"* {c.summary} [{c.hexsha[:7]}]" for c in commits])
-            commit_block = "\n".join(commit_messages) or ""
-
-            print("Here are some recent commits for reference:")
-            print(commit_block)
-
-            # self.changelog_addition = commit_block
-            if write_block:
-                self.changelog_addition = block
+            terminal_advice = util.yellow(
+                "Here are some recent commit message for reference:\n"
+            )
+            terminal_advice += "-" * 30 + "\n"
+
+            commits = util.get_recent_commits(self.repo)
+ 
+            commit_messages = ([f"* {c.summary} [{c.hexsha[:7]}]" for c in commits])
+            terminal_advice += "\n".join(commit_messages) or ""
+            terminal_advice += "\n" + ("-" * 30) + "\n"
+
+            sections = [
+                "Added",
+                "Changed",
+                "Deprecated",
+                "Removed",
+                "Fixed",
+                "Security",
+            ]
+            terminal_advice += util.yellow(
+                "You may want to use these headngs to categorize your changelog entries:\n"
+            )
+            terminal_advice += "".join([f"### {s}\n" for s in sections])
+            terminal_advice += "-" * 30 + "\n\n"
+            print(terminal_advice)
+
+            if self.bumper.next_version or self.changelog_needs_unreleased_stub():
+                self.changelog_addition = stub
 
     def resolve_changelog(self):
         """Help the user to get the changelog file up-to-date."""
         with open(self.changelog_filename, "r", encoding="utf-8") as clog:
             content = clog.read() or "--"
 
         content = self.changelog_addition + "\n\n" + content
 
         with open(self.changelog_filename, "w", encoding="utf-8") as clog:
             clog.write(content)
 
         print("Resolve CHANGELOG:")
-        print("Edit and save the changelog now.")
 
         input(
             util.green(
                 "Please EDIT and SAVE your CHANGELOG (There's no need to commit), then press enter to continue."
             )
         )
 
@@ -233,28 +246,14 @@
         for line in datafile:
             if line.startswith("## Unreleased"):
                 return False
             elif line.startswith("## Version"):
                 return True
         return True
 
-    # PRIVATE
-
-    def get_commits(self):
-        """Get commits that are on the active branch but not on the master branch."""
-        result = []
-        master_shas = set(
-            [c.hexsha for c in self.repo.iter_commits(rev=self.repo.branches.master)]
-        )
-        for commit in self.repo.iter_commits(rev=self.branch):
-            if commit.hexsha in master_shas:
-                continue
-            result.append(commit)
-        return result
-
 
 def main():
     """Run the wizard."""
     wizard = Skulk()
     wizard.run()
```

## skulk/util.py

```diff
@@ -1,15 +1,11 @@
 import os
 import sys
-import re
 from git import InvalidGitRepositoryError, Repo
-import subprocess
-import semver
-import functools
-# from semver.version import Version
+
 
 MOCKED = True
 PROD_PYPI_INDEX = "https://pypi.org/simple/"
 
 
 def yellow(rhs):
     """Return the rhs in red."""
@@ -95,7 +91,27 @@
         first_line = first_nonblank_line(manifest_file)
         if first_line[0] == "#":
             return first_line.split(" ")[1]
     except IndexError: 
         pass
     return base_name
     
+
+def get_recent_commits(repo):
+    """Get commits frm here back to the last tag on the master branch."""
+    branch = repo.active_branch
+    master_shas = set(
+        [c.hexsha for c in repo.iter_commits(rev=repo.branches.master)]
+    )
+    tag_shas = [t.commit.hexsha for t in reversed(repo.tags)]
+    
+    master_tag_sha = None
+    for sha in tag_shas:
+        if sha in master_shas:
+            master_tag_sha = sha
+            break
+    result = []
+    for c in repo.iter_commits(rev=branch):
+        result.append(c)
+        if c.hexsha == master_tag_sha:
+            break
+    return result
```

## Comparing `skulk-2.0.1.dist-info/METADATA` & `skulk-2.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.0.1
+Version: 2.0.2
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

## Comparing `skulk-2.0.1.dist-info/RECORD` & `skulk-2.0.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-skulk/VERSION,sha256=A0Z0ibj7YgWYiwpSn5RFtnqM9RBJvuo7KuHdxyWz0lQ,5
+skulk/VERSION,sha256=MRhnIb5Q0QM1Rd_u6dbuEYtU-xuXTqkJqy6WDgt8BJs,5
 skulk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 skulk/bumper.py,sha256=Ug0uQLthCbuR7NQTpTtTTTxosX1cnKntsOr410POrSU,9548
-skulk/skulk.py,sha256=K-nHSOBNrqhTAdz9XFBGF8kiXMElm9det5iJbd-O-yE,9146
-skulk/util.py,sha256=64hqDrkuXZTPVmCydXUdsp_79Gl_UU8QcqxeDzH6PQk,2625
-skulk-2.0.1.dist-info/METADATA,sha256=WnciNUg0ouhrPGqMOrv9mGsJ8W7tMVeQPwwwzBWKoOQ,646
-skulk-2.0.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-skulk-2.0.1.dist-info/entry_points.txt,sha256=Gis7pLiCEkPWw7tn3_U-G9XPwOtBvTL4m11EqDi613o,44
-skulk-2.0.1.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
-skulk-2.0.1.dist-info/RECORD,,
+skulk/skulk.py,sha256=Io5jj1wPNgRx6nHz-UVdX6-hl7cmz8aQZddBG1VBgJ8,8984
+skulk/util.py,sha256=ycjIuZn0HUBKgQzXMnjhx4cL_0zh63ZA7PEAHlfRow4,3128
+skulk-2.0.2.dist-info/METADATA,sha256=gq9QYM-BiJphHSGg0N-8wJZ9nQMhq0vZk_U_wdSoSwQ,646
+skulk-2.0.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+skulk-2.0.2.dist-info/entry_points.txt,sha256=Gis7pLiCEkPWw7tn3_U-G9XPwOtBvTL4m11EqDi613o,44
+skulk-2.0.2.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
+skulk-2.0.2.dist-info/RECORD,,
```

