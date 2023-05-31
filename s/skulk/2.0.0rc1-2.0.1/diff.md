# Comparing `tmp/skulk-2.0.0rc1-py2.py3-none-any.whl.zip` & `tmp/skulk-2.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8921 bytes, number of entries: 10
--rw-r--r--  2.0 unx       10 b- defN 23-May-30 06:09 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-May-30 06:09 skulk/__init__.py
--rw-r--r--  2.0 unx     9348 b- defN 23-May-30 06:09 skulk/bumper.py
--rw-r--r--  2.0 unx     9105 b- defN 23-May-30 06:09 skulk/skulk.py
--rw-r--r--  2.0 unx     2625 b- defN 23-May-30 06:09 skulk/util.py
--rw-r--r--  2.0 unx      649 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      749 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/RECORD
-10 files, 22646 bytes uncompressed, 7649 bytes compressed:  66.2%
+Zip file size: 8872 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        5 b- defN 23-May-31 06:10 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 06:10 skulk/__init__.py
+-rw-r--r--  2.0 unx     9548 b- defN 23-May-31 06:10 skulk/bumper.py
+-rw-r--r--  2.0 unx     9146 b- defN 23-May-31 06:10 skulk/skulk.py
+-rw-r--r--  2.0 unx     2625 b- defN 23-May-31 06:10 skulk/util.py
+-rw-r--r--  2.0 unx      646 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      733 b- defN 23-May-31 06:10 skulk-2.0.1.dist-info/RECORD
+10 files, 22863 bytes uncompressed, 7630 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.0.0rc1.dist-info/METADATA
+Filename: skulk-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.0.0rc1.dist-info/WHEEL
+Filename: skulk-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.0.0rc1.dist-info/entry_points.txt
+Filename: skulk-2.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.0.0rc1.dist-info/top_level.txt
+Filename: skulk-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.0.0rc1.dist-info/RECORD
+Filename: skulk-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.0.0-rc.1
+2.0.1
```

## skulk/bumper.py

```diff
@@ -61,51 +61,33 @@
         else:
             do_bump = True
             print(
                 f"The local VERSION file contains an invalid version: {self.current_version}. It has been used already."
             )
             print("You'll need to bump the version.")
 
-        latest = semver.Version.parse(self.latest_version)
-
-        version_options = [
-            (str(latest.next_version(part="prerelease")), "The next pre-release"),
-            (str(latest.next_version(part="patch")), "The next patch release"),
-            (
-                str(latest.next_version(part="minor").bump_prerelease()),
-                "Pre-release for a new feature",
-            ),
-            (str(latest.next_version(part="minor")), "Release a new feature"),
-            (
-                str(latest.next_version(part="major").bump_prerelease()),
-                "Pre-release for a breaking change",
-            ),
-            (str(latest.next_version(part="major")), "Release a breaking change"),
-        ]
+        version_options = get_version_options(self.latest_version)
 
         version_options += [
-            ("Explicit", "Specify a version manually. This is not recommended."),
-            (
-                "Cancel",
-                "I changed my mind. I don't want to tag or release. I just want to push.",
-            ),
-            ("Exit!", ""),
+            "Explicit: Specify a version manually. This is not recommended.",
+            "Cancel: I changed my mind. I don't want to tag or release. I just want to push.",
+            "Exit!"
         ]
 
-        options = [f"{v[0]: <16} {v[1]}" for v in version_options]
-        num_options = len(options)
+        # options = [f"{v[0]: <16} {v[1]}" for v in version_options]
+        num_options = len(version_options)
         exit_option = num_options
         no_tags_option = num_options - 1
         custom_option = num_options - 2
 
         bump_type = 0
         msg = "Choose a new version"
-        while bump_type not in range(1, len(options) + 1):
+        while bump_type not in range(1, len(version_options) + 1):
             print(msg)
-            for i, opt in enumerate(options):
+            for i, opt in enumerate(version_options):
                 n = i + 1
                 print(f"{n}: {opt}")
             bump_type = input(util.green("Enter a number: "))
             if not bump_type.isdigit():
                 bump_type = 0
             bump_type = int(bump_type)
             msg = f"Please choose a number between 1 and {num_options}."
@@ -135,15 +117,15 @@
                 else:
                     custom_valid = True
                     msg = f"Version {custom_version} is valid."
                     self.next_version = custom_version
         elif bump_type == no_tags_option:  # no tags
             self.next_version = None
         else:  # bump_type is one of the regular options
-            self.next_version = str(version_options[bump_type - 1][0])
+            self.next_version = str(version_options[bump_type - 1])
         print(self.next_version)
         if self.next_version:
             print(f"You bumped the version to: {self.next_version}")
         else:
             print("You chose to push with no tag or release.")
 
     def _set_versions(self):
@@ -159,57 +141,16 @@
         self.latest_version = _sorted_versions(
             [self.latest_pypi_version, self.latest_tag_version]
         )[-1]
 
     def get_pypi_versions(self):
         """
         Return a list of all PyPi versions for the named package.
-
-        The package may not exist on PyPi, in which case we return an empty list. We
-        don't error out, because it's perfectly valid for no package to exist. We
-        can still deploy there.
         """
-
-        # notice this command says: Install version== (i.e. it requests an invalid
-        # version). It fails as intended, and the result is a message to say can't
-        # find version in versions. It lists the existing versions which we split
-        # and return. Check for py3 and py 27 compatible by using both pips.
-        args = [
-            "pip3",
-            "install",
-            "--index-url",
-            util.PROD_PYPI_INDEX,
-            f"{self.pip_name}==",
-        ]
-        output = subprocess.Popen(
-            args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
-        ).communicate()
-        if len(output) < 2 or "none" in output[1].decode("utf-8"):
-            args = [
-                "pip2.7",
-                "install",
-                "--index-url",
-                util.PROD_PYPI_INDEX,
-                f"{self.pip_name}==",
-            ]
-            output = subprocess.Popen(
-                args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
-            ).communicate()
-            if len(output) < 2 or "none" in output[1].decode("utf-8"):
-                return []
-
-        output = output[1]
-        regex = re.compile(
-            r"^.*Could not find a version.*from versions:(.*)\).*", re.DOTALL
-        )
-        match = regex.match(output.decode("utf-8"))
-        if match:
-            result = [v.strip() for v in match.group(1).split(r", ")]
-            return _sorted_versions([v for v in result if semver.Version.is_valid(v)])
-        return []
+        return _get_pypi_versions(self.pip_name)
 
     def get_tags(self):
         """Return a list of all tags in the repo."""
         return _sorted_versions([str(tag) for tag in self.repo.tags])
 
     def is_released_version(self, version):
         """Return True if the version has been released to PyPi or tagged in the repo."""
@@ -218,23 +159,17 @@
         release_version = str(
             semver.Version.parse(version).replace(prerelease=None, build=None)
         )
         if release_version in self.versions["pypi"] + self.versions["tags"]:
             return release_version
         return None
 
-
-# def version_compare(version1, version2):
-#     """Compare two versions.
-
-#     Versions may be semvers or tuples with semver at element[0].
-#     """
-#     if isinstance(version1, tuple) and isinstance(version2, tuple):
-#        return semver.compare(str(version1[0]), str(version2[0]))
-#     return semver.compare(str(version1), str(version2))
+def _pypi_to_semver(p):
+    """Convert a PyPi version to a semver."""
+    return p.replace("rc", "-rc.")
 
 
 def _sorted_versions(versions):
     """Sort a list of versions."""
     return sorted(versions, key=functools.cmp_to_key(semver.compare))
 
 
@@ -243,7 +178,86 @@
     version = util.first_nonblank_line(filename)
     if not version:
         sys.stderr.write(
             f"Can't get version string from the version file: {filename}. using 0.0.1\n"
         )
         return "0.0.1"
     return version if semver.Version.is_valid(version) else "0.0.1"
+
+
+def _get_pypi_versions(pip_name):
+    """
+    Return a list of all PyPi versions for the named package.
+
+    The package may not exist on PyPi, in which case we return an empty list. We
+    don't error out, because it's perfectly valid for no package to exist. We
+    can still deploy there.
+    """
+
+    # notice this command says: Install version== (i.e. it requests an invalid
+    # version). It fails as intended, and the result is a message to say can't
+    # find version in versions. It lists the existing versions which we split
+    # and return. Check for py3 and py 27 compatible by using both pips.
+    args = [
+        "pip3",
+        "install",
+        "--index-url",
+        util.PROD_PYPI_INDEX,
+        f"{pip_name}==",
+    ]
+    output = subprocess.Popen(
+        args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    ).communicate()
+    if len(output) < 2 or "none" in output[1].decode("utf-8"):
+        args = [
+            "pip2.7",
+            "install",
+            "--index-url",
+            util.PROD_PYPI_INDEX,
+            f"{pip_name}==",
+        ]
+        output = subprocess.Popen(
+            args, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+        ).communicate()
+        if len(output) < 2 or "none" in output[1].decode("utf-8"):
+            return []
+
+    output = output[1]
+    regex = re.compile(
+        r"^.*Could not find a version.*from versions:(.*)\).*", re.DOTALL
+    )
+    match = regex.match(output.decode("utf-8"))
+    if match:
+        result = [_pypi_to_semver(v.strip()) for v in match.group(1).split(r", ")]
+
+        return _sorted_versions([v for v in result if semver.Version.is_valid(v)])
+    return []
+
+
+def get_version_options(latest_version):
+    """Return a list of the most likely versions to bump to
+    
+    See the tests for examples.
+    """
+    latest = semver.Version.parse(latest_version)
+    if latest.prerelease:
+        version_options = [
+            str(latest.next_version(part="prerelease")),
+            str(latest.next_version(part="patch")),
+        ]
+        latest = latest.replace(prerelease=None)
+        version_options += [
+            str(latest.next_version(part="minor").bump_prerelease()),
+            str(latest.next_version(part="minor")),
+            str(latest.next_version(part="major").bump_prerelease()),
+            str(latest.next_version(part="major")),
+        ]
+    else:
+        version_options = [
+            str(latest.next_version(part="prerelease")),
+            str(latest.next_version(part="patch")),
+            str(latest.next_version(part="minor").bump_prerelease()),
+            str(latest.next_version(part="minor")),
+            str(latest.next_version(part="major").bump_prerelease()),
+            str(latest.next_version(part="major")),
+        ]
+    return version_options
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
-        self.changelog_addition = None
+        self.changelog_addition = ""
 
     def run(self):
         """
         Guide the user to ensure version and changelog are valid.
         """
 
         # wizard.check_pre_push_hook()
@@ -195,19 +195,20 @@
 
         if self.edit_changelog:
             commits = self.get_commits()
             commit_messages = ["\n# Raw commit messages for reference.\n"]
             commit_messages.extend([f"* {c.summary} [{c.hexsha[:7]}]" for c in commits])
             commit_block = "\n".join(commit_messages) or ""
 
+            print("Here are some recent commits for reference:")
             print(commit_block)
 
-            self.changelog_addition = commit_block
+            # self.changelog_addition = commit_block
             if write_block:
-                self.changelog_addition = commit_block + "\n\n" + block
+                self.changelog_addition = block
 
     def resolve_changelog(self):
         """Help the user to get the changelog file up-to-date."""
         with open(self.changelog_filename, "r", encoding="utf-8") as clog:
             content = clog.read() or "--"
 
         content = self.changelog_addition + "\n\n" + content
```

## Comparing `skulk-2.0.0rc1.dist-info/METADATA` & `skulk-2.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.0.0rc1
+Version: 2.0.1
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

## Comparing `skulk-2.0.0rc1.dist-info/RECORD` & `skulk-2.0.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-skulk/VERSION,sha256=9hNpYAYjM6P8IFcmPTbqsyNgrep7Oy37HWq0RCmR91U,10
+skulk/VERSION,sha256=A0Z0ibj7YgWYiwpSn5RFtnqM9RBJvuo7KuHdxyWz0lQ,5
 skulk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-skulk/bumper.py,sha256=UMqPRQD3Pt1HrG0lcBb7-f2oqHCx_jZEpgVto5yDbcU,9348
-skulk/skulk.py,sha256=sGpBUM8pXlOY7sUNJaKk-WtCC43npxC_YcmQFP4A4Kk,9105
+skulk/bumper.py,sha256=Ug0uQLthCbuR7NQTpTtTTTxosX1cnKntsOr410POrSU,9548
+skulk/skulk.py,sha256=K-nHSOBNrqhTAdz9XFBGF8kiXMElm9det5iJbd-O-yE,9146
 skulk/util.py,sha256=64hqDrkuXZTPVmCydXUdsp_79Gl_UU8QcqxeDzH6PQk,2625
-skulk-2.0.0rc1.dist-info/METADATA,sha256=A9mn7KXnlsWYQbQF9zUDlw2wxlL7V0hw2kStK8aCqyY,649
-skulk-2.0.0rc1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-skulk-2.0.0rc1.dist-info/entry_points.txt,sha256=Gis7pLiCEkPWw7tn3_U-G9XPwOtBvTL4m11EqDi613o,44
-skulk-2.0.0rc1.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
-skulk-2.0.0rc1.dist-info/RECORD,,
+skulk-2.0.1.dist-info/METADATA,sha256=WnciNUg0ouhrPGqMOrv9mGsJ8W7tMVeQPwwwzBWKoOQ,646
+skulk-2.0.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+skulk-2.0.1.dist-info/entry_points.txt,sha256=Gis7pLiCEkPWw7tn3_U-G9XPwOtBvTL4m11EqDi613o,44
+skulk-2.0.1.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
+skulk-2.0.1.dist-info/RECORD,,
```

