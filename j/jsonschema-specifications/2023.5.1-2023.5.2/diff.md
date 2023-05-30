# Comparing `tmp/jsonschema_specifications-2023.5.1.tar.gz` & `tmp/jsonschema_specifications-2023.5.2.tar.gz`

## Comparing `jsonschema_specifications-2023.5.1.tar` & `jsonschema_specifications-2023.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.coveragerc
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.flake8
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.readthedocs.yml
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/release.yml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/Makefile
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/api.rst
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/conf.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/index.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/requirements.in
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/requirements.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/__init__.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/_core.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/metaschema.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/applicator
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/content
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/core
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/validation
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/metaschema.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/applicator
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/content
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/core
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/format
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/format-annotation
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/format-assertion
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/unevaluated
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/validation
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft3/metaschema.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft4/metaschema.json
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft6/metaschema.json
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft7/metaschema.json
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/jsonschema_specifications/tests/test_jsonschema_specifications.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/COPYING
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/README.rst
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.coveragerc
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.flake8
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/release.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/Makefile
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/api.rst
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/conf.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/index.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/requirements.in
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/_core.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/metaschema.json
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/applicator
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/content
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/core
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/validation
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/metaschema.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/applicator
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/content
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/core
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/format
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/format-annotation
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/format-assertion
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/unevaluated
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/validation
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft3/metaschema.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft4/metaschema.json
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft6/metaschema.json
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft7/metaschema.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/jsonschema_specifications/tests/test_jsonschema_specifications.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/COPYING
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/README.rst
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 jsonschema_specifications-2023.5.2/PKG-INFO
```

### Comparing `jsonschema_specifications-2023.5.1/.pre-commit-config.yaml` & `jsonschema_specifications-2023.5.2/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -10,30 +10,22 @@
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.270"
+    hooks:
+      - id: ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
-  - repo: https://github.com/PyCQA/flake8
-    rev: "6.0.0"
-    hooks:
-      - id: flake8
-  - repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
-    hooks:
-      - id: yesqa
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
-    hooks:
-      - id: pyupgrade
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
```

### Comparing `jsonschema_specifications-2023.5.1/noxfile.py` & `jsonschema_specifications-2023.5.2/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,40 +22,39 @@
 
 @session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
 def tests(session):
     session.install("pytest", ROOT)
     session.run("pytest", "--verbosity=3")
 
 
+@session()
+def audit(session):
+    session.install("pip-audit", ROOT)
+    session.run("python", "-m", "pip_audit")
+
+
 @session(tags=["build"])
 def build(session):
     session.install("build")
     tmpdir = session.create_tmp()
     session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
 
 
 @session(tags=["style"])
 def readme(session):
     session.install("build", "twine")
     tmpdir = session.create_tmp()
     session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("python", "-m", "twine", "check", tmpdir + "/*")
+    session.run("python", "-m", "twine", "check", "--strict", tmpdir + "/*")
 
 
 @session(tags=["style"])
 def style(session):
-    session.install(
-        "flake8",
-        "flake8-broken-line",
-        "flake8-bugbear",
-        "flake8-commas",
-        "flake8-quotes",
-        "flake8-tidy-imports",
-    )
-    session.run("python", "-m", "flake8", PACKAGE, __file__)
+    session.install("ruff")
+    session.run("ruff", "check", ROOT)
 
 
 @session()
 def typing(session):
     session.install("mypy", ROOT)
     session.run("python", "-m", "mypy", PACKAGE)
```

### Comparing `jsonschema_specifications-2023.5.1/.github/SECURITY.md` & `jsonschema_specifications-2023.5.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/.github/workflows/ci.yml` & `jsonschema_specifications-2023.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/docs/Makefile` & `jsonschema_specifications-2023.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/docs/conf.py` & `jsonschema_specifications-2023.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/docs/index.rst` & `jsonschema_specifications-2023.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/docs/requirements.txt` & `jsonschema_specifications-2023.5.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/_core.py` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from referencing import Resource
 
 
 def _schemas():
     """
     All schemas we ship.
     """
-
     # importlib.resources.abc.Traversal doesn't have nice ways to do this that
     # I'm aware of...
     #
     # It can't recurse arbitrarily, e.g. no ``.glob()``.
     #
     # So this takes some liberties given the real layout of what we ship
     # (only 2 levels of nesting, no directories within the second level).
```

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/metaschema.json` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/applicator` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/applicator`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/content` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/content`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/core` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/core`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/meta-data`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft201909/vocabularies/validation` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft201909/vocabularies/validation`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/metaschema.json` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/applicator` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/applicator`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/content` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/content`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/core` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/core`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/meta-data`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft202012/vocabularies/validation` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft202012/vocabularies/validation`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft3/metaschema.json` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft3/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft4/metaschema.json` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft4/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft6/metaschema.json` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft6/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/jsonschema_specifications/schemas/draft7/metaschema.json` & `jsonschema_specifications-2023.5.2/jsonschema_specifications/schemas/draft7/metaschema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/COPYING` & `jsonschema_specifications-2023.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/README.rst` & `jsonschema_specifications-2023.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `jsonschema_specifications-2023.5.1/PKG-INFO` & `jsonschema_specifications-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-specifications
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: The JSON Schema meta-schemas and vocabularies, exposed as a Registry
 Project-URL: Documentation, https://jsonschema-specifications.readthedocs.io/
 Project-URL: Homepage, https://github.com/python-jsonschema/jsonschema-specifications
 Project-URL: Issues, https://github.com/python-jsonschema/jsonschema-specifications/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/python-jsonschema/jsonschema-specifications
 Author: Julian Berman
```

