# Comparing `tmp/git_darcs-0.8.7.tar.gz` & `tmp/git_darcs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_darcs-0.8.7.tar", max compression
+gzip compressed data, was "git_darcs-0.9.0.tar", max compression
```

## Comparing `git_darcs-0.8.7.tar` & `git_darcs-0.9.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    34523 2022-12-15 04:56:03.339252 git_darcs-0.8.7/LICENSE
--rw-r--r--   0        0        0    13062 2022-12-20 15:11:00.476877 git_darcs-0.8.7/README.md
--rw-r--r--   0        0        0    26970 2023-05-19 18:26:24.758132 git_darcs-0.8.7/git_darcs.py
--rw-r--r--   0        0        0     1255 2023-05-19 18:28:44.065711 git_darcs-0.8.7/pyproject.toml
--rw-r--r--   0        0        0    14225 1970-01-01 00:00:00.000000 git_darcs-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-31 15:50:59.768095 git_darcs-0.9.0/LICENSE
+-rw-r--r--   0        0        0    13062 2023-05-31 15:51:01.838159 git_darcs-0.9.0/README.md
+-rw-r--r--   0        0        0    27097 2023-05-31 15:51:48.552919 git_darcs-0.9.0/git_darcs.py
+-rw-r--r--   0        0        0     1260 2023-05-31 15:55:09.032377 git_darcs-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14175 1970-01-01 00:00:00.000000 git_darcs-0.9.0/PKG-INFO
```

### Comparing `git_darcs-0.8.7/LICENSE` & `git_darcs-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_darcs-0.8.7/README.md` & `git_darcs-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `git_darcs-0.8.7/git_darcs.py` & `git_darcs-0.9.0/git_darcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,14 +266,17 @@
         ["git", "checkout", rev],
         check=True,
     )
 
 
 def is_ancestor(rev, last):
     """Check if revisiion can fast-forward."""
+    # I don't know why git thinks revs are their own ancestor
+    if rev == last:
+        return False
     try:
         run(["git", "merge-base", "--is-ancestor", last, rev], check=True)
         return True
     except CalledProcessError:
         return False
 
 
@@ -342,14 +345,15 @@
     if _verbose:
         print(head)
     return head
 
 
 def record_all(rev, *, last=None, postfix=None, comments=None):
     """Record all change onto the darcs-repo."""
+    assert rev != last
     msgs = onelines(rev, last=last)
     msg = msgs[0]
     comments = "\n".join(msgs[1:])
     by = author(rev)
     if postfix:
         msg = f"{msg} {postfix}"
     elif comments:
@@ -416,14 +420,15 @@
                     f"{base}..{head}",
                 ],
                 stdout=PIPE,
             ) as res:
                 while line := res.stdout.readline():
                     yield line.decode("UTF-8").strip()
 
+
 def get_base():
     """Get the root/base commit from git."""
     base = (
         run(
             ["git", "rev-list", "--max-parents=0", "HEAD"],
             check=True,
             stdout=PIPE,
```

### Comparing `git_darcs-0.8.7/pyproject.toml` & `git_darcs-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-darcs"
-version = "0.8.7"
+version = "0.9.0"
 description = " Incremental import of git into darcs and back again"
 authors = ["Jean-Louis Fuchs <jean-louis.fuchs@adfinis.com>"]
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/ganwell/git-darcs"
 repository = "https://github.com/ganwell/git-darcs"
 keywords = ["git", "darcs", "import", "incremental"]
 readme = "README.md"
@@ -18,32 +18,32 @@
     "LICENSE",
 ]
 
 [tool.poetry.scripts]
 git-darcs = 'git_darcs:main'
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 tqdm = "^4.64.0"
 click = "^8.1.3"
 Flake8-pyproject = "^1.1.0.post0"
 readchar = "^4.0.3"
 colorama = "^0.4.5"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
-mypy = "^0.971"
+mypy = "^1.3.0"
 pdbpp = "^0.10.3"
-black = "^22.6.0"
+black = "^23.3.0"
 isort = "^5.10.1"
 python-lsp-server = "^1.5.0"
-flake8 = "^5.0.4"
-flake8-bugbear = "^22.8.23"
+flake8 = "^6.0.0"
+flake8-bugbear = "^23.5.9"
 flake8-debugger = "^4.1.2"
-flake8-isort = "^4.2.0"
+flake8-isort = "^6.0.0"
 flake8-docstrings = "^1.6.0"
 flake8-string-format = "^0.3.0"
 flake8-tuple = "^0.4.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `git_darcs-0.8.7/PKG-INFO` & `git_darcs-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: git-darcs
-Version: 0.8.7
+Version: 0.9.0
 Summary:  Incremental import of git into darcs and back again
 Home-page: https://github.com/ganwell/git-darcs
 License: AGPL-3.0-or-later
 Keywords: git,darcs,import,incremental
 Author: Jean-Louis Fuchs
 Author-email: jean-louis.fuchs@adfinis.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Version Control
 Requires-Dist: Flake8-pyproject (>=1.1.0.post0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
```

