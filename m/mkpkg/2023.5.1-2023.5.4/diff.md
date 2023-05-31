# Comparing `tmp/mkpkg-2023.5.1.tar.gz` & `tmp/mkpkg-2023.5.4.tar.gz`

## Comparing `mkpkg-2023.5.1.tar` & `mkpkg-2023.5.4.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.coveragerc
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.flake8
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.readthedocs.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.testr.conf
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/codecov.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/test-requirements.txt
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/tox.ini
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/SECURITY.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/release.yml
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/Makefile
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/conf.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/index.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/requirements.in
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/__main__.py
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/_cli.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.coveragerc.j2
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.flake8
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.pre-commit-config.yaml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.testr.conf
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/COPYING.j2
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/README.rst.j2
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/codecov.yml
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/pyproject.toml.j2
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/tests.py.j2
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/tox.ini.j2
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/FUNDING.yml
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/SECURITY.md.j2
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/release.yml
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/.github/workflows/ci.yml.j2
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/docs/index.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/docs/requirements.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/__init__.py.j2
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/__main__.py.j2
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/_build.py.j2
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/template/package/_cli.py.j2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/tests/__init__.py
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/mkpkg/tests/test_integration.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/COPYING
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/README.rst
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 mkpkg-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.coveragerc
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.readthedocs.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/codecov.yml
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/noxfile.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/test-requirements.in
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/test-requirements.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/SECURITY.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/release.yml
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/Makefile
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/conf.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/index.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/requirements.in
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/__main__.py
+-rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/_cli.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.coveragerc.j2
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/COPYING.j2
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/README.rst.j2
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/codecov.yml
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/noxfile.py.j2
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/pyproject.toml.j2
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/tests.py.j2 -> package/tests/test_integration.py.j2
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/FUNDING.yml
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/SECURITY.md.j2
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/release.yml
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/.github/workflows/ci.yml.j2
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/docs/conf.py.j2
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/docs/index.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/docs/requirements.in.j2
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/__init__.py.j2
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/__main__.py.j2
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/_build.py.j2
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/_cli.py.j2
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/template/package/tests/test_integration.py.j2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/tests/__init__.py
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/mkpkg/tests/test_integration.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/COPYING
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/README.rst
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 mkpkg-2023.5.4/PKG-INFO
```

### Comparing `mkpkg-2023.5.1/.pre-commit-config.yaml` & `mkpkg-2023.5.4/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-ast
-      - id: check-docstring-first
       - id: check-toml
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.269"
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
-    rev: v3.3.1
-    hooks:
-      - id: pyupgrade
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
```

### Comparing `mkpkg-2023.5.1/.github/SECURITY.md` & `mkpkg-2023.5.4/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.1/docs/Makefile` & `mkpkg-2023.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.1/docs/requirements.txt` & `mkpkg-2023.5.4/docs/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,103 @@
 #
-# This file is autogenerated by pip-compile with python 3.11
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
-#    pip-compile docs/requirements.in
+#    pip-compile --resolver=backtracking docs/requirements.in
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
-babel==2.11.0
+babel==2.12.1
     # via sphinx
-beautifulsoup4==4.11.1
+beautifulsoup4==4.12.2
     # via furo
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via mkpkg
-docutils==0.19
-    # via sphinx
-furo==2022.12.7
+contourpy==1.0.7
+    # via matplotlib
+cycler==0.11.0
+    # via matplotlib
+docutils==0.20.1
+    # via sphinx
+fonttools==4.39.4
+    # via matplotlib
+furo==2023.5.20
     # via -r docs/requirements.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via
     #   mkpkg
     #   sphinx
-markupsafe==2.1.1
+kiwisolver==1.4.4
+    # via matplotlib
+markupsafe==2.1.2
     # via jinja2
+matplotlib==3.7.1
+    # via sphinxext-opengraph
 file:.#egg=mkpkg
     # via -r docs/requirements.in
-packaging==22.0
-    # via sphinx
+numpy==1.24.3
+    # via
+    #   contourpy
+    #   matplotlib
+packaging==23.1
+    # via
+    #   matplotlib
+    #   sphinx
+pillow==9.5.0
+    # via matplotlib
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   furo
     #   pygments-github-lexers
     #   sphinx
 pygments-github-lexers==0.0.5
     # via -r docs/requirements.in
-pytz==2022.7
-    # via babel
-requests==2.28.1
+pyparsing==3.0.9
+    # via matplotlib
+python-dateutil==2.8.2
+    # via matplotlib
+requests==2.31.0
     # via sphinx
+six==1.16.0
+    # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
-soupsieve==2.3.2.post1
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.0.1
     # via
     #   -r docs/requirements.in
     #   furo
     #   mkpkg
     #   sphinx-basic-ng
     #   sphinxcontrib-spelling
+    #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b1
     # via furo
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sphinxcontrib-spelling==7.7.0
+sphinxcontrib-spelling==8.0.0
+    # via -r docs/requirements.in
+sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
-urllib3==1.26.13
+urllib3==2.0.2
     # via requests
```

### Comparing `mkpkg-2023.5.1/mkpkg/_cli.py` & `mkpkg-2023.5.4/mkpkg/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,21 @@
     "py38": "Programming Language :: Python :: 3.8",
     "py39": "Programming Language :: Python :: 3.9",
     "py310": "Programming Language :: Python :: 3.10",
     "py311": "Programming Language :: Python :: 3.11",
     "py312": "Programming Language :: Python :: 3.12",
     "jython": "Programming Language :: Python :: 2.7",
 }
-TEST_DEPS = {
-    "pytest": ["pytest"],
-    "twisted.trial": ["twisted"],
-    "virtue": ["virtue"],
+TEST_DEP = {
+    "pytest": "pytest",
+    "twisted.trial": "twisted",
+    "virtue": "virtue",
 }
 TEMPLATE = Path(__file__).with_name("template")
 
-PYPI_TOKEN_URL = "https://pypi.org/manage/account/token/"
 READTHEDOCS_IMPORT_URL = "https://readthedocs.org/dashboard/import/manual/"
 
 
 def dedented(*args, **kwargs):
     return textwrap.dedent(*args, **kwargs).lstrip("\n")
 
 
@@ -72,28 +71,28 @@
     default="",
     help="a (rst) README for the package",
 )
 @click.option(
     "-t",
     "--test-runner",
     default="virtue",
-    type=click.Choice(TEST_DEPS.keys()),
+    type=click.Choice(sorted(TEST_DEP)),
     help="the test runner to use",
 )
 @click.option(
     "-s",
     "--supports",
     multiple=True,
     type=click.Choice(sorted(VERSION_CLASSIFIERS)),
     default=["py38", "py39", "py310", "py311", "pypy3"],
     help="a version of Python supported by the package",
 )
 @click.option(
     "--status",
-    type=click.Choice(STATUS_CLASSIFIERS),
+    type=click.Choice(list(STATUS_CLASSIFIERS)),
     default="alpha",
     help="the initial package development status",
 )
 @click.option(
     "--docs/--no-docs",
     default=False,
     help="generate a Sphinx documentation template for the new package",
@@ -117,15 +116,15 @@
     default=False,
     help="include a build script for CFFI modules",
 )
 @click.option(
     "--style/--no-style",
     "style",
     default=True,
-    help="(don't) run pyflakes by default in tox runs.",
+    help="(don't) run pyflakes by default in nox runs.",
 )
 @click.option(
     "--init-vcs/--no-init-vcs",
     default=True,
     help="don't initialize a VCS.",
 )
 @click.option(
@@ -150,15 +149,14 @@
     style,
     init_vcs,
     closed,
 ):
     """
     Oh how exciting! Create a new Python package.
     """
-
     if name.startswith("python-"):
         package_name = name[len("python-") :]
     elif name.endswith(".py"):
         package_name = name[: -len(".py")]
     else:
         package_name = name
     package_name = package_name.lower().replace("-", "_")
@@ -182,45 +180,43 @@
         supports=supports,
         test_runner=test_runner,
     )
 
     package = Path(package_name)
 
     if single_module:
-        tests = "{toxinidir}/tests.py"
+        tests = "tests.py"
 
         if len(cli) > 1:
             sys.exit("Cannot create a single module with multiple CLIs.")
         elif cli:
             scripts = [f'{cli[0]} = "{package_name}:main"']
             script = env.get_template("package/_cli.py.j2").render(
                 program_name=cli[0],
             )
         else:
             scripts = []
-            script = ""
+            script = '"""\nFill me in!\n"""\n'
 
         script_name = package_name + ".py"
         core_source_paths = {
             script_name: script,
             "tests.py": env.get_template("tests.py.j2").render(),
         }
-        style_paths = ["{toxinidir}/" + script_name, tests]
 
     else:
         tests = package_name
 
+        init, tests = package / "__init__.py", package / "tests"
+        integration = env.get_template("package/tests/test_integration.py.j2")
         core_source_paths = {
-            package / "tests" / "__init__.py": "",
-            package
-            / "__init__.py": env.get_template(
-                "package/__init__.py.j2",
-            ).render(),
+            init: env.get_template("package/__init__.py.j2").render(),
+            tests / "__init__.py": "",
+            tests / "test_integration.py": integration.render(),
         }
-        style_paths = ["{toxinidir}/" + package_name]
 
         if cffi:
             core_source_paths[package / "_build.py"] = env.get_template(
                 "package/_build.py.j2",
             ).render(cname=_cname(name))
 
         if len(cli) == 1:
@@ -280,22 +276,19 @@
                 version not in {"jython", "pypy2", "pypy3"}
                 for version in supports
             ),
             pypy="pypy2" in supports or "pypy3" in supports,
             jython="jython" in supports,
         ),
         ".coveragerc": env.get_template(".coveragerc.j2").render(),
-        "tox.ini": env.get_template("tox.ini.j2").render(
-            test_deps=TEST_DEPS[test_runner],
+        ".pre-commit-config.yaml": template(".pre-commit-config.yaml"),
+        "noxfile.py": env.get_template("noxfile.py.j2").render(
+            test_dep=TEST_DEP[test_runner],
             tests=tests,
-            style_paths=style_paths,
         ),
-        ".flake8": template(".flake8"),
-        ".pre-commit-config.yaml": template(".pre-commit-config.yaml"),
-        ".testr.conf": template(".testr.conf"),
     }
 
     if not closed:
         files[".github/workflows/ci.yml"] = env.get_template(
             ".github/workflows/ci.yml.j2",
         ).render(
             schedule_hour=randint(3, 7),
@@ -316,55 +309,14 @@
         root.mkdir()
 
     for path, content in targets.items():
         path = root / path
         path.parent.mkdir(parents=True, exist_ok=True)
         path.write_text(dedented(content))
 
-    if docs:
-        (root / "docs").mkdir()
-        (root / "docs" / "requirements.in").write_text(
-            template("docs", "requirements.in"),
-        )
-
-        subprocess.check_call(
-            [
-                sys.executable,
-                "-m",
-                "sphinx.cmd.quickstart",
-                "--quiet",
-                "--project",
-                name,
-                "--author",
-                author,
-                "--release",
-                "",
-                "--ext-autodoc",
-                "--ext-coverage",
-                "--ext-doctest",
-                "--ext-intersphinx",
-                "--ext-viewcode",
-                "--extensions",
-                "sphinx.ext.napoleon",
-                "--extensions",
-                "sphinxcontrib.spelling",
-                "--makefile",
-                "--no-batchfile",
-                str(root / "docs"),
-            ],
-        )
-
-        # Fix sphinx-quickstart not writing a trailing newline.
-        with root.joinpath("docs", "conf.py").open("a") as file:
-            file.write("\n")
-
-        (root / "docs" / "index.rst").write_text(template("docs", "index.rst"))
-
-        click.echo(f"Set up documentation at: {READTHEDOCS_IMPORT_URL}")
-
     if init_vcs and not bare:
         subprocess.check_call(["git", "init", "--quiet", name])
 
         git_dir = root / ".git"
         subprocess.check_call(
             [
                 "git",
@@ -384,26 +336,52 @@
                 "commit",
                 "--quiet",
                 "-m",
                 "Initial commit",
             ],
         )
 
+    if docs:
+        docs = root / "docs"
+        docs.mkdir()
+
+        requirements = env.get_template("docs/requirements.in.j2").render()
+        (docs / "requirements.in").write_text(requirements)
+        subprocess.check_call(
+            [
+                sys.executable,
+                "-m",
+                "piptools",
+                "compile",
+                "--quiet",
+                "--resolver",
+                "backtracking",
+                "-U",
+                str(docs.joinpath("requirements.in").absolute()),
+            ],
+            cwd=root.absolute(),
+        )
+        conf = env.get_template("docs/conf.py.j2").render()
+        (docs / "conf.py").write_text(conf)
+        (docs / "index.rst").write_text(template("docs/index.rst"))
+
+        click.echo(f"Set up documentation at: {READTHEDOCS_IMPORT_URL}")
+
         if not closed:
             click.echo(
                 dedent(
-                    f"""
-                    Set up:
-
-                      * a PyPI token from {PYPI_TOKEN_URL} named
-                        'GitHub Actions - {name}'
+                    """
+                    Be sure to:
 
-                    and include them in the GitHub secrets at
-                    https://github.com/Julian/{name}/settings/secrets
-                    """,
+                      * Fill in the description in the pyproject.toml and in
+                        the docstring for __init__.py
+                      * Set up a pending PyPI publisher from the appropriate
+                        PyPI page https://pypi.org/manage/account/publishing/
+                        (named 'PyPI')
+                    """
                 ),
             )
 
 
 def template(*segments):
     return TEMPLATE.joinpath(*segments).read_text()
```

### Comparing `mkpkg-2023.5.1/mkpkg/template/.pre-commit-config.yaml` & `mkpkg-2023.5.4/mkpkg/template/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-ast
-      - id: check-json
       - id: check-toml
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.269"
+    hooks:
+      - id: ruff
   - repo: https://github.com/PyCQA/isort
-    rev: v5.11.3
+    rev: 5.12.0
     hooks:
       - id: isort
-  - repo: https://github.com/PyCQA/flake8
-    rev: "5.0.4"
-    hooks:
-      - id: flake8
-  - repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
-    hooks:
-      - id: yesqa
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.2
-    hooks:
-      - id: pyupgrade
   - repo: https://github.com/psf/black
-    rev: 22.8.0
+    rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.4"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
```

### Comparing `mkpkg-2023.5.1/mkpkg/template/COPYING.j2` & `mkpkg-2023.5.4/mkpkg/template/COPYING.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.1/mkpkg/template/README.rst.j2` & `mkpkg-2023.5.4/mkpkg/template/README.rst.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.1/mkpkg/template/.github/SECURITY.md.j2` & `mkpkg-2023.5.4/mkpkg/template/.github/SECURITY.md.j2`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.1/mkpkg/tests/test_integration.py` & `mkpkg-2023.5.4/mkpkg/tests/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-try:
-    from tempfile import TemporaryDirectory
-except Exception:
-    from backports.tempfile import TemporaryDirectory
-
+from tempfile import TemporaryDirectory
 from unittest import TestCase
+import json
+import os
 import subprocess
 import sys
 
 from mkpkg._cli import Path
 
 
 class TestMkpkg(TestCase):
     def test_it_creates_packages_that_pass_their_tests(self):
         root = self.mkpkg("foo")
         _fix_readme(root / "foo")
-        self.assertToxSucceeds(root / "foo", "--skip-missing-interpreters")
+        self.assertNoxSucceeds(root / "foo")
 
     def test_it_creates_packages_with_docs_that_pass_their_tests(self):
-        root = self.mkpkg("mkpkg", "--docs")
-        _fix_readme(root / "mkpkg")
-        self.assertToxSucceeds(root / "mkpkg", "--skip-missing-interpreters")
+        root = self.mkpkg("foo", "--docs")
+        _fix_readme(root / "foo")
+        self.assertNoxSucceeds(root / "foo")
 
     def test_it_creates_single_modules_that_pass_their_tests(self):
         root = self.mkpkg("foo", "--single")
         _fix_readme(root / "foo")
-        self.assertToxSucceeds(root / "foo", "--skip-missing-interpreters")
+        self.assertNoxSucceeds(root / "foo")
 
     def test_it_creates_cffi_packages_that_pass_their_tests(self):
         root = self.mkpkg("foo", "--cffi")
         _fix_readme(root / "foo")
-        self.assertToxSucceeds(root / "foo", "--skip-missing-interpreters")
+        self.assertNoxSucceeds(root / "foo")
 
     def test_it_creates_clis(self):
         foo = self.mkpkg("foo", "--cli", "bar") / "foo"
         cli = foo / "foo" / "_cli.py"
         cli.write_text(
             cli.read_text().replace(
                 "def main():\n    pass",
@@ -82,83 +80,73 @@
         root = self.mkpkg("foo", "--no-init-vcs")
         self.assertFalse((root / "foo" / ".git").is_dir())
 
     def test_it_skips_vcs_when_bare(self):
         root = self.mkpkg("foo", "--bare")
         self.assertFalse((root / "foo" / ".git").is_dir())
 
-    def test_default_tox_envs(self):
-        envlist = self.tox(self.mkpkg("foo") / "foo", "-l").stdout
+    def test_default_envs(self):
+        envlist = self.envs(self.mkpkg("foo") / "foo")
         self.assertEqual(
-            set(envlist.splitlines()),
+            envlist,
             {
-                b"py38-build",
-                b"py38-audit",
-                b"py38-tests",
-                b"py39-build",
-                b"py39-audit",
-                b"py39-tests",
-                b"py310-build",
-                b"py310-audit",
-                b"py310-tests",
-                b"py311-build",
-                b"py311-audit",
-                b"py311-tests",
-                b"pypy3-build",
-                b"pypy3-audit",
-                b"pypy3-tests",
-                b"readme",
-                b"secrets",
-                b"style",
+                "tests-3.8",
+                "tests-3.9",
+                "tests-3.10",
+                "tests-3.11",
+                "tests-pypy3",
+                "audit",
+                "build",
+                "readme",
+                "secrets",
+                "style",
+                "typing",
             },
         )
 
-    def test_docs_tox_envs(self):
-        envlist = self.tox(self.mkpkg("foo", "--docs") / "foo", "-l").stdout
+    def test_docs_envs(self):
+        envlist = self.envs(self.mkpkg("foo", "--docs") / "foo")
         self.assertEqual(
-            set(envlist.splitlines()),
+            envlist,
             {
-                b"py38-build",
-                b"py38-audit",
-                b"py38-tests",
-                b"py39-build",
-                b"py39-audit",
-                b"py39-tests",
-                b"pypy3-build",
-                b"pypy3-audit",
-                b"pypy3-tests",
-                b"readme",
-                b"secrets",
-                b"style",
-                b"docs-dirhtml",
-                b"docs-doctest",
-                b"docs-linkcheck",
-                b"docs-spelling",
-                b"docs-style",
+                "tests-3.8",
+                "tests-3.9",
+                "tests-3.10",
+                "tests-3.11",
+                "tests-pypy3",
+                "audit",
+                "build",
+                "readme",
+                "secrets",
+                "style",
+                "typing",
+                "docs(dirhtml)",
+                "docs(doctest)",
+                "docs(linkcheck)",
+                "docs(man)",
+                "docs(spelling)",
+                "docs(style)",
             },
         )
 
     def test_it_runs_style_checks_by_default(self):
-        root = self.mkpkg("foo")
-        envlist = self.tox(root / "foo", "-l").stdout
-        self.assertIn(b"style", envlist)
+        envlist = self.envs(self.mkpkg("foo") / "foo")
+        self.assertIn("style", envlist)
 
     def test_it_runs_style_checks_when_explicitly_asked(self):
-        root = self.mkpkg("foo", "--style")
-        envlist = self.tox(root / "foo", "-l").stdout
-        self.assertIn(b"style", envlist)
+        envlist = self.envs(self.mkpkg("foo", "--style") / "foo")
+        self.assertIn("style", envlist)
 
     def test_it_skips_style_checks_when_asked(self):
-        root = self.mkpkg("foo", "--no-style")
-        envlist = self.tox(root / "foo", "-l").stdout
-        self.assertNotIn(b"style", envlist)
+        envlist = self.envs(self.mkpkg("foo", "--no-style") / "foo")
+        self.assertNotIn("style", envlist)
 
-    def assertToxSucceeds(self, *args, **kwargs):
+    def assertNoxSucceeds(self, *args, **kwargs):
         try:
-            self.tox(*args, **kwargs)
+            self.nox(*args, **kwargs)
         except subprocess.CalledProcessError as error:
             if error.stdout:
                 sys.stdout.buffer.write(b"\nStdout:\n\n")
                 sys.stdout.buffer.write(error.stdout)
             if error.stderr:
                 sys.stderr.buffer.write(b"\nStderr:\n\n")
                 sys.stderr.buffer.write(error.stderr)
@@ -171,44 +159,44 @@
             [sys.executable, "-m", "mkpkg"] + list(argv),
             cwd=directory.name,
             env=dict(
                 GIT_AUTHOR_NAME="mkpkg unittests",
                 GIT_AUTHOR_EMAIL="mkpkg-unittests@local",
                 GIT_COMMITTER_NAME="mkpkg unittests",
                 GIT_COMMITTER_EMAIL="mkpkg-unittests@local",
+                PATH=os.environ.get("PATH", ""),  # needed to find e.g. git
             ),
             stdout=subprocess.DEVNULL,
             check=True,
         )
         return Path(directory.name)
 
-    def tox(self, path, *argv):
+    def nox(self, path, *argv):
         return subprocess.run(
             [
                 sys.executable,
                 "-m",
-                "tox",
-                "-c",
-                str(path / "tox.ini"),
-                "-p",
-                "auto",
-                "--workdir",
-                str(path / "tox-work-dir"),
+                "nox",
+                "--noxfile",
+                str(path / "noxfile.py"),
+                "--envdir",
+                str(path / "nox-env-dir"),
             ]
             + list(argv),
             check=True,
             capture_output=True,
         )
 
+    def envs(self, path):
+        output = self.nox(path, "--list-sessions", "--json").stdout
+        return {each["session"] for each in json.loads(output)}
+
     def venv(self, package):
         venv = package / "venv"
-        subprocess.run(
-            [sys.executable, "-m", "virtualenv", "--quiet", str(venv)],
-            check=True,
-        )
+        subprocess.run([sys.executable, "-m", "venv", str(venv)], check=True)
         subprocess.run(
             [
                 str(venv / "bin" / "python"),
                 "-m",
                 "pip",
                 "install",
                 "--quiet",
```

### Comparing `mkpkg-2023.5.1/COPYING` & `mkpkg-2023.5.4/COPYING`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.1/README.rst` & `mkpkg-2023.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `mkpkg-2023.5.1/PKG-INFO` & `mkpkg-2023.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkpkg
-Version: 2023.5.1
+Version: 2023.5.4
 Summary: A package @Julian uses to create Python packages.
 Project-URL: Homepage, https://github.com/Julian/mkpkg
 Project-URL: Documentation, https://mkpkg.readthedocs.io/
 Project-URL: Issues, https://github.com/Julian/mkpkg/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/mkpkg
 Author: Julian Berman
@@ -14,23 +14,23 @@
 Keywords: packaging,templating
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: click
 Requires-Dist: jinja2
+Requires-Dist: pip-tools
 Requires-Dist: sphinx
 Description-Content-Type: text/x-rst
 
 =========
 ``mkpkg``
 =========
```

