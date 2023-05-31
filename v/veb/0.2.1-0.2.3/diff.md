# Comparing `tmp/veb-0.2.1.tar.gz` & `tmp/veb-0.2.3.tar.gz`

## Comparing `veb-0.2.1.tar` & `veb-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 veb-0.2.1/.coveragerc
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 veb-0.2.1/.flake8
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 veb-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 veb-0.2.1/noxfile.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 veb-0.2.1/perftest.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 veb-0.2.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 veb-0.2.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 veb-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 veb-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 veb-0.2.1/veb/__init__.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 veb-0.2.1/veb/_core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 veb-0.2.1/veb/tests/__init__.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 veb-0.2.1/veb/tests/test_core.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 veb-0.2.1/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 veb-0.2.1/COPYING
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 veb-0.2.1/README.rst
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 veb-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 veb-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 veb-0.2.3/.coveragerc
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 veb-0.2.3/.flake8
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 veb-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 veb-0.2.3/noxfile.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 veb-0.2.3/perftest.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 veb-0.2.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 veb-0.2.3/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 veb-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 veb-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 veb-0.2.3/veb/__init__.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 veb-0.2.3/veb/_core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 veb-0.2.3/veb/tests/__init__.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 veb-0.2.3/veb/tests/test_core.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 veb-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 veb-0.2.3/COPYING
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 veb-0.2.3/README.rst
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 veb-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 veb-0.2.3/PKG-INFO
```

### Comparing `veb-0.2.1/.pre-commit-config.yaml` & `veb-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `veb-0.2.1/noxfile.py` & `veb-0.2.3/noxfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
+import os
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
-DOCS = ROOT / "docs"
 PACKAGE = ROOT / "veb"
 
 
 nox.options.sessions = []
 
 
 def session(default=True, **kwargs):
@@ -18,44 +18,66 @@
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
 @session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
 def tests(session):
-    dependencies = ["virtue", ROOT]
-    if session.posargs == ["coverage"]:
-        dependencies.append("coverage[toml]")
-        session.install(*dependencies)
-        session.run("coverage", "run", "-m", "virtue", PACKAGE)
-        session.run("coverage", "report")
+    session.install("virtue", ROOT)
+
+    if session.posargs and session.posargs[0] == "coverage":
+        if len(session.posargs) > 1 and session.posargs[1] == "github":
+            posargs = session.posargs[2:]
+            github = os.environ["GITHUB_STEP_SUMMARY"]
+        else:
+            posargs, github = session.posargs[1:], None
+
+        session.install("coverage[toml]")
+        session.run("coverage", "run", *posargs, "-m", "virtue", "veb")
+
+        if github is None:
+            session.run("coverage", "report")
+        else:
+            with open(github, "a") as summary:
+                summary.write("### Coverage\n\n")
+                summary.flush()  # without a flush, output seems out of order.
+                session.run(
+                    "coverage",
+                    "report",
+                    "--format=markdown",
+                    stdout=summary,
+                )
     else:
-        session.install(*dependencies)
-        session.run("virtue", *session.posargs, PACKAGE)
+        session.run("virtue", *session.posargs, "veb")
 
 
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
+    session.run("python", "-m", "twine", "check", "--strict", tmpdir + "/veb*")
+
+
+@session()
+def secrets(session):
+    session.install("detect-secrets")
+    session.run("detect-secrets", "scan", ROOT)
 
 
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
+
+
+@session(default=False)
+def bandit(session):
+    session.install("bandit")
+    session.run("bandit", "--recursive", PACKAGE)
```

### Comparing `veb-0.2.1/.github/SECURITY.md` & `veb-0.2.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `veb-0.2.1/.github/workflows/ci.yml` & `veb-0.2.3/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   list:
     runs-on: ubuntu-latest
     outputs:
       noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - id: noxenvs-matrix
         run: |
           echo >>$GITHUB_OUTPUT noxenvs=$(
             nox --list-sessions |
             grep '^* ' |
             cut -d ' ' -f 2- |
             jq --raw-input --slurp 'split("\n") | map(select(. != ""))'
@@ -44,50 +44,56 @@
     needs: list
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest]
         noxenv: ${{ fromJson(needs.list.outputs.noxenvs) }}
+        posargs: [""]
+        include:
+          - os: ubuntu-latest
+            noxenv: tests-3.11
+            posargs: coverage github
 
     steps:
       - uses: actions/checkout@v3
       - name: Install dependencies
         run: sudo apt-get update && sudo apt-get install -y libenchant-2-dev
         if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
       - name: Install dependencies
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up nox
-        uses: wntrblm/nox@2022.11.21
+        uses: wntrblm/nox@2023.04.22
       - name: Run nox
-        run: nox -s "${{ matrix.noxenv }}"
+        run: nox -s "${{ matrix.noxenv }}" -- ${{ matrix.posargs }}
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
+    environment:
+      name: PyPI
+      url: https://pypi.org/p/veb
+    permissions:
+      contents: write
+      id-token: write
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: python -m pip install build
       - name: Create packages
         run: python -m build .
       - name: Publish to PyPI
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          password: ${{ secrets.pypi_password }}
+        uses: pypa/gh-action-pypi-publish@release/v1
       - name: Create a Release
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
-        uses: actions/github-script@v6
+        uses: softprops/action-gh-release@v1
         with:
-          github-token: ${{ secrets.GITHUB_TOKEN }}
-          script: |
-            await github.request(`POST /repos/${{ github.repository }}/releases`, {
-              tag_name: "${{ github.ref }}",
-              generate_release_notes: true
-            });
+          files: |
+            dist/*
+          generate_release_notes: true
```

### Comparing `veb-0.2.1/veb/_core.py` & `veb-0.2.3/veb/_core.py`

 * *Files identical despite different names*

### Comparing `veb-0.2.1/veb/tests/test_core.py` & `veb-0.2.3/veb/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `veb-0.2.1/COPYING` & `veb-0.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `veb-0.2.1/README.rst` & `veb-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `veb-0.2.1/PKG-INFO` & `veb-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veb
-Version: 0.2.1
+Version: 0.2.3
 Summary: Dynamically-allocated reduced-space van Emde Boas trees.
 Project-URL: Homepage, https://github.com/Julian/veb
 Project-URL: Issues, https://github.com/Julian/veb/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/veb
 Author: Julian Berman
 Author-email: Julian+veb@GrayVines.com
@@ -12,21 +12,21 @@
 License-File: COPYING
 Keywords: data structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 =======
 ``veb``
 =======
 
 |PyPI| |Pythons| |CI|
```

