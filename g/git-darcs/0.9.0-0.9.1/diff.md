# Comparing `tmp/git_darcs-0.9.0.tar.gz` & `tmp/git_darcs-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_darcs-0.9.0.tar", max compression
+gzip compressed data, was "git_darcs-0.9.1.tar", max compression
```

## Comparing `git_darcs-0.9.0.tar` & `git_darcs-0.9.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    34523 2023-05-31 15:50:59.768095 git_darcs-0.9.0/LICENSE
--rw-r--r--   0        0        0    13062 2023-05-31 15:51:01.838159 git_darcs-0.9.0/README.md
--rw-r--r--   0        0        0    27097 2023-05-31 15:51:48.552919 git_darcs-0.9.0/git_darcs.py
--rw-r--r--   0        0        0     1260 2023-05-31 15:55:09.032377 git_darcs-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    14175 1970-01-01 00:00:00.000000 git_darcs-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 16:32:15.570570 git_darcs-0.9.1/LICENSE
+-rw-r--r--   0        0        0    13062 2023-05-31 16:32:17.860640 git_darcs-0.9.1/README.md
+-rw-r--r--   0        0        0    27153 2023-05-31 16:32:18.273986 git_darcs-0.9.1/git_darcs.py
+-rw-r--r--   0        0        0     1282 2023-05-31 16:37:06.876179 git_darcs-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    14120 1970-01-01 00:00:00.000000 git_darcs-0.9.1/PKG-INFO
```

### Comparing `git_darcs-0.9.0/LICENSE` & `git_darcs-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_darcs-0.9.0/README.md` & `git_darcs-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `git_darcs-0.9.0/git_darcs.py` & `git_darcs-0.9.1/git_darcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,30 +302,28 @@
     )
     msg = res.stdout.decode("UTF-8").strip()
     if _verbose:
         print(msg)
     return msg
 
 
-def onelines(rev, *, last=None):
+def onelines(rev, *, last=None, merges=False):
     """Get the short-message of a commit from git."""
     if last:
-        res = run(
-            [
-                "git",
-                "log",
-                "--oneline",
-                "--no-decorate",
-                "--date-order",
-                "--no-merges",
-                f"{last}..{rev}",
-            ],
-            stdout=PIPE,
-            check=True,
-        )
+        cmd = [
+            "git",
+            "log",
+            "--oneline",
+            "--no-decorate",
+            "--date-order",
+        ]
+        if merges:
+            cmd += ["--no-merges"]
+        cmd += (f"{last}..{rev}",)
+        res = run(cmd, stdout=PIPE, check=True)
     else:
         res = run(
             ["git", "log", "--oneline", "--no-decorate", "--max-count=1", rev],
             stdout=PIPE,
             check=True,
         )
     msg = res.stdout.decode("UTF-8").strip()
@@ -346,15 +344,17 @@
         print(head)
     return head
 
 
 def record_all(rev, *, last=None, postfix=None, comments=None):
     """Record all change onto the darcs-repo."""
     assert rev != last
-    msgs = onelines(rev, last=last)
+    msgs = onelines(rev, last=last, merges=False)
+    if not msgs:
+        msgs = onelines(rev, last=last, merges=True)
     msg = msgs[0]
     comments = "\n".join(msgs[1:])
     by = author(rev)
     if postfix:
         msg = f"{msg} {postfix}"
     elif comments:
         msg = f"{msg}\n\n{comments}"
@@ -389,40 +389,40 @@
         if _verbose:
             print(res.stdout.decode("UTF-8").strip())
     except CalledProcessError as e:
         if "No changes!" not in e.stdout.decode("UTF-8"):
             raise
 
 
+def get_rev_list_cmd(head, base, merges=False):
+    """Create the cmd to linearized path from git."""
+    cmd = [
+        "git",
+        "rev-list",
+        "--reverse",
+        "--topo-order",
+        "--ancestry-path",
+    ]
+    if not merges:
+        cmd += ["--no-merges"]
+    cmd += [f"{base}..{head}"]
+    return cmd
+
+
 def get_rev_list(head, base):
     """Get a linearized path from base to head from git."""
     with Popen(
-        [
-            "git",
-            "rev-list",
-            "--reverse",
-            "--topo-order",
-            "--ancestry-path",
-            "--no-merges",
-            f"{base}..{head}",
-        ],
+        get_rev_list_cmd(head, base, merges=False),
         stdout=PIPE,
     ) as res:
         while line := res.stdout.readline():
             yield line.decode("UTF-8").strip()
         else:
             with Popen(
-                [
-                    "git",
-                    "rev-list",
-                    "--reverse",
-                    "--topo-order",
-                    "--ancestry-path",
-                    f"{base}..{head}",
-                ],
+                get_rev_list_cmd(head, base, merges=True),
                 stdout=PIPE,
             ) as res:
                 while line := res.stdout.readline():
                     yield line.decode("UTF-8").strip()
 
 
 def get_base():
```

### Comparing `git_darcs-0.9.0/pyproject.toml` & `git_darcs-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-darcs"
-version = "0.9.0"
+version = "0.9.1"
 description = " Incremental import of git into darcs and back again"
 authors = ["Jean-Louis Fuchs <jean-louis.fuchs@adfinis.com>"]
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/ganwell/git-darcs"
 repository = "https://github.com/ganwell/git-darcs"
 keywords = ["git", "darcs", "import", "incremental"]
 readme = "README.md"
@@ -21,15 +21,14 @@
 [tool.poetry.scripts]
 git-darcs = 'git_darcs:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 tqdm = "^4.64.0"
 click = "^8.1.3"
-Flake8-pyproject = "^1.1.0.post0"
 readchar = "^4.0.3"
 colorama = "^0.4.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 mypy = "^1.3.0"
 pdbpp = "^0.10.3"
@@ -39,14 +38,16 @@
 flake8 = "^6.0.0"
 flake8-bugbear = "^23.5.9"
 flake8-debugger = "^4.1.2"
 flake8-isort = "^6.0.0"
 flake8-docstrings = "^1.6.0"
 flake8-string-format = "^0.3.0"
 flake8-tuple = "^0.4.1"
+python-lsp-black = "^1.3.0"
+flake8-pyproject = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.flake8]
 max-line-length = 160
```

### Comparing `git_darcs-0.9.0/PKG-INFO` & `git_darcs-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-darcs
-Version: 0.9.0
+Version: 0.9.1
 Summary:  Incremental import of git into darcs and back again
 Home-page: https://github.com/ganwell/git-darcs
 License: AGPL-3.0-or-later
 Keywords: git,darcs,import,incremental
 Author: Jean-Louis Fuchs
 Author-email: jean-louis.fuchs@adfinis.com
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,14 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Version Control
-Requires-Dist: Flake8-pyproject (>=1.1.0.post0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.5,<0.5.0)
 Requires-Dist: readchar (>=4.0.3,<5.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Project-URL: Repository, https://github.com/ganwell/git-darcs
 Description-Content-Type: text/markdown
```

