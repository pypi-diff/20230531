# Comparing `tmp/usort-1.1.0b1.tar.gz` & `tmp/usort-1.1.0b2.tar.gz`

## Comparing `usort-1.1.0b1.tar` & `usort-1.1.0b2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 usort-1.1.0b1/.flake8
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 usort-1.1.0b1/.mailmap
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 usort-1.1.0b1/.readthedocs.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 usort-1.1.0b1/.vars.ini
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 usort-1.1.0b1/CHANGELOG.md
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 usort-1.1.0b1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 usort-1.1.0b1/CONTRIBUTING.md
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 usort-1.1.0b1/MAINTAINERS.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 usort-1.1.0b1/MANIFEST.in
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 usort-1.1.0b1/Makefile
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 usort-1.1.0b1/check_backcompat.py
--rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 usort-1.1.0b1/check_copyright.sh
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 usort-1.1.0b1/.github/dependabot.yml
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 usort-1.1.0b1/.github/workflows/build.yml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/api.rst
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/changelog.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/code-of-conduct.rst
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/conf.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/contributing.rst
--rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/guide.rst
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/index.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/maintainers.rst
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/versioning.rst
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/why.rst
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/_static/custom.css
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/_static/fbopensource.png
--rw-r--r--   0        0        0    21530 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/_static/opensource.png
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/_templates/badges.html
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 usort-1.1.0b1/docs/_templates/meta.html
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/__main__.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/api.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/cli.py
--rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/config.py
--rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/sorting.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/stdlibs.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/translate.py
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/types.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/util.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/version.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/__main__.py
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/cli.py
--rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/config.py
--rw-r--r--   0        0        0    31701 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/functional.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/sorting.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/stdlibs.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/translate.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/types.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 usort-1.1.0b1/usort/tests/util.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 usort-1.1.0b1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 usort-1.1.0b1/LICENSE
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 usort-1.1.0b1/README.md
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 usort-1.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 usort-1.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 usort-1.1.0b2/.flake8
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 usort-1.1.0b2/.mailmap
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 usort-1.1.0b2/.readthedocs.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 usort-1.1.0b2/.vars.ini
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 usort-1.1.0b2/CHANGELOG.md
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 usort-1.1.0b2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 usort-1.1.0b2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 usort-1.1.0b2/MAINTAINERS.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 usort-1.1.0b2/MANIFEST.in
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 usort-1.1.0b2/Makefile
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 usort-1.1.0b2/check_backcompat.py
+-rwxr-xr-x   0        0        0      449 2020-02-02 00:00:00.000000 usort-1.1.0b2/check_copyright.sh
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 usort-1.1.0b2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 usort-1.1.0b2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/api.rst
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/changelog.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/code-of-conduct.rst
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/conf.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/contributing.rst
+-rw-r--r--   0        0        0    20678 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/guide.rst
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/index.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/maintainers.rst
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/versioning.rst
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/why.rst
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/_static/custom.css
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/_static/fbopensource.png
+-rw-r--r--   0        0        0    21530 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/_static/opensource.png
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/_templates/badges.html
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 usort-1.1.0b2/docs/_templates/meta.html
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/__main__.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/api.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/cli.py
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/config.py
+-rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/sorting.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/stdlibs.py
+-rw-r--r--   0        0        0    14727 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/translate.py
+-rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/types.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/util.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/version.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/__main__.py
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/cli.py
+-rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/config.py
+-rw-r--r--   0        0        0    33010 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/functional.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/sorting.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/stdlibs.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/translate.py
+-rw-r--r--   0        0        0    10127 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/types.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 usort-1.1.0b2/usort/tests/util.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 usort-1.1.0b2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 usort-1.1.0b2/LICENSE
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 usort-1.1.0b2/README.md
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 usort-1.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 usort-1.1.0b2/PKG-INFO
```

### Comparing `usort-1.1.0b1/CHANGELOG.md` & `usort-1.1.0b2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 1.1.0b2
+
+Beta release
+
+- New `magic_commas` option to force multi-line import style like black (#252, #247)
+- Fix dropped inline comments on last import item without trailing comma (#251, #249)
+
+```shell-session
+$ git shortlog -sn v1.1.0b1...
+     5  Amethyst Reese
+```
+
 ## 1.1.0b1
 
 Beta release
 
 - Splits basic import statements with multiple names (#140)
 - Uniformly collapse blank lines within a category (#201)
 - Support 3.10+ syntax by enabling the LibCST native parser by default (#244)
@@ -13,14 +25,25 @@
     37  dependabot[bot]
      5  Zsolt Dollenstein
      4  Loren Arthur
      1  Arseny Boykov
      1  Tim Hatch
 ```
 
+## 1.0.6
+
+Bugfix release
+
+* Fix dropped inline comments on last import item without trailing comma (#251, #249)
+
+```shell-session
+$ git shortlog -sn v1.0.5...
+     4  Amethyst Reese
+```
+
 ## 1.0.5
 
 Bugfix release
 
 * Fix AssertionError when sorting multiple statements on one line (#203, #204)
 * Deprecated: Python 3.6 support will be dropped in v1.1.0 (#154)
```

### Comparing `usort-1.1.0b1/CODE_OF_CONDUCT.md` & `usort-1.1.0b2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/CONTRIBUTING.md` & `usort-1.1.0b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/MAINTAINERS.md` & `usort-1.1.0b2/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/Makefile` & `usort-1.1.0b2/Makefile`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/check_backcompat.py` & `usort-1.1.0b2/check_backcompat.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,31 +23,45 @@
 from tempfile import TemporaryDirectory
 from typing import List, Optional
 from urllib.request import urlopen
 
 from packaging.version import Version
 
 REPO_ROOT = Path(__file__).parent.resolve()
-TARGET_VERSION = Version("1.0.0")
+MINIMUM_VERSION = Version("1.0.0")
 PYPI_JSON_URL = "https://pypi.org/pypi/usort/json"
 
 
-def get_public_versions() -> List[Version]:
+def get_current_version() -> Version:
+    with TemporaryDirectory() as td:
+        root = Path(td).resolve()
+        usort = setup_virtualenv(root)
+        proc = subprocess.run(
+            (usort, "--version"), encoding="utf-8", capture_output=True, check=True
+        )
+        return Version(proc.stdout.rpartition(" ")[-1])
+
+
+def get_public_versions(
+    current_version: Version, minimum_version: Version
+) -> List[Version]:
     """
-    Find all non-yanked versions of usort >= TARGET_VERSION
+    Find all non-yanked versions of usort.
+
+    Limits results such that TARGET_VERSION <= CANDIDATE_VERSION <= CURRENT_VERSION
     """
     with urlopen(PYPI_JSON_URL) as request:
         data = json.loads(request.read())
 
     versions: List[Version] = []
     for version_str in data["releases"]:
         version = Version(version_str)
         if all(dist["yanked"] for dist in data["releases"][version_str]):
             continue
-        if version >= TARGET_VERSION:
+        if minimum_version <= version <= current_version:
             versions.append(version)
 
     return sorted(versions, reverse=True)
 
 
 def setup_virtualenv(root: Path, version: Optional[Version] = None) -> Path:
     """
@@ -96,21 +110,25 @@
             try:
                 print(f"checking version {version} ...")
                 usort = setup_virtualenv(root, version)
                 subprocess.run((usort, "--version"), check=True)
                 subprocess.run((usort, "check", "usort"), check=True)
                 print("clean\n")
             except Exception as e:
-                failures.append(version)
+                failures.append((version, e))
 
         return failures
 
 
 def main() -> None:
-    versions = get_public_versions()
+    current_version = get_current_version()
+    minimum_version = MINIMUM_VERSION
+    print(f"{current_version = !s}\n{minimum_version = !s}\n")
+
+    versions = get_public_versions(current_version, minimum_version)
     versions_str = ", ".join(str(v) for v in versions)
     print(f"discovered versions {versions_str}\n")
 
     failures = check_versions(versions)
     if failures:
         print("Sorting failed in versions:")
         for version, exc in failures:
```

### Comparing `usort-1.1.0b1/.github/workflows/build.yml` & `usort-1.1.0b2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/docs/conf.py` & `usort-1.1.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/docs/guide.rst` & `usort-1.1.0b2/docs/guide.rst`

 * *Files 3% similar despite different names*

```diff
@@ -497,14 +497,43 @@
     :value: true
 
     Whether to run a heuristic to detect the top-level name of the file being sorted,
     and consider that name as first-party.  This heuristic happens after other options
     are loaded, so such names cannot be overridden to another category if this is
     enabled.
 
+.. attribute:: magic_commas
+    :type: bool
+    :value: false
+
+    Whether to follow black's "magic trailing comma" behavior when sorting
+    multi-line imports.
+
+    When set to ``false`` (the default), µsort will automatically collapse
+    multi-line imports into a single line if they fit within the configured
+    line length, regardless of trailing commas, with the intent that imports
+    are managed by tools rather than humans. This enables µsort to keep imports
+    as compact as possible, even if users or tools add or remove import items.
+
+    When set to ``true``, µsort will expand and maintain multi-line imports
+    if they have a trailing comma on the last import item, enabling humans
+    to more easily read and manage longer lists of imports. Removing trailing
+    commas will enable µsort to collapse the import to a single line, while
+    adding parentheses and a trailing comma to a single line import will force
+    µsort to expand it to a multi-line import, matching black's behavior for
+    normal collection literals.
+
+    .. note::
+
+        This feature is a "backward incompatible" sorting change, as versions
+        of µsort before 1.1.0 will not obey this feature flag, and will
+        potentially collapse these multi-line imports. Be sure that all
+        developers and CI systems have upgraded to µsort 1.1.0 or newer before
+        enabling this feature in a production codebase.
+
 .. attribute:: merge_imports
     :type: bool
     :value: true
 
     Whether to merge sequential imports from the same base module.
     See `Merging`_ for details on how this works.
```

### Comparing `usort-1.1.0b1/docs/versioning.rst` & `usort-1.1.0b2/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/docs/why.rst` & `usort-1.1.0b2/docs/why.rst`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/docs/_static/fbopensource.png` & `usort-1.1.0b2/docs/_static/fbopensource.png`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/docs/_static/opensource.png` & `usort-1.1.0b2/docs/_static/opensource.png`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/docs/_templates/meta.html` & `usort-1.1.0b2/docs/_templates/meta.html`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/__init__.py` & `usort-1.1.0b2/usort/__init__.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/api.py` & `usort-1.1.0b2/usort/api.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/cli.py` & `usort-1.1.0b2/usort/cli.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/config.py` & `usort-1.1.0b2/usort/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,17 @@
     # as block separators, similar to non-import statements.
     side_effect_modules: List[str] = field(default_factory=list)
     side_effect_re: Pattern[str] = field(default=re.compile(""))
 
     # Whether to perform the first-party heuristic during find()
     first_party_detection: bool = True
 
+    # Whether to follow black-style for magic trailing commas
+    magic_commas: bool = False
+
     # Whether to merge imports when sorting
     merge_imports: bool = True
 
     # gitignore-style filename patterns to exclude when sorting entire directories
     excludes: List[str] = field(default_factory=list)
 
     # Needed for formatting final imports
@@ -152,16 +155,18 @@
             self.categories = [Category(x) for x in tbl["categories"]]
         if "default_category" in tbl:
             self.default_category = Category(tbl["default_category"])
         if "side_effect_modules" in tbl:
             self.side_effect_modules.extend(tbl["side_effect_modules"])
         if "first_party_detection" in tbl:
             self.first_party_detection = tbl["first_party_detection"]
+        if "magic_commas" in tbl:
+            self.magic_commas = bool(tbl["magic_commas"])
         if "merge_imports" in tbl:
-            self.merge_imports = tbl["merge_imports"]
+            self.merge_imports = bool(tbl["merge_imports"])
         if "excludes" in tbl:
             self.excludes = tbl["excludes"]
 
         for cat, names in tbl.get("known", {}).items():
             typed_cat = Category(cat)
             if cat not in self.categories:
                 raise ValueError(f"Known set for {cat} without it having an order")
```

### Comparing `usort-1.1.0b1/usort/sorting.py` & `usort-1.1.0b2/usort/sorting.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/translate.py` & `usort-1.1.0b2/usort/translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,20 +70,28 @@
                 # )
                 comments.initial.extend(
                     line.comment.value for line in ws.empty_lines if line.comment
                 )
 
             assert imp.rpar is not None
             if isinstance(imp.rpar.whitespace_before, cst.ParenthesizedWhitespace):
+                # from foo import (
+                #     bar
+                #     # THIS PART
+                # )
                 comments.final.extend(
                     line.comment.value
                     for line in imp.rpar.whitespace_before.empty_lines
                     if line.comment
                 )
 
+                # from foo import (
+                #     bar,
+                #     baz  # THIS PART (NO COMMA!)
+                # )
                 if imp.rpar.whitespace_before.first_line.comment:
                     comments.inline.extend(
                         split_inline_comment(
                             imp.rpar.whitespace_before.first_line.comment.value
                         )
                     )
 
@@ -117,16 +125,18 @@
 def item_from_node(
     node: cst.ImportAlias, stem: Optional[str] = None, before: Sequence[str] = ()
 ) -> SortableImportItem:
     name = with_dots(node.name)
     asname = with_dots(node.asname.name) if node.asname else ""
     comments = ImportItemComments()
     comments.before.extend(before)
+    comma = False
 
     if isinstance(node.comma, cst.Comma):
+        comma = True
         if (
             isinstance(node.comma.whitespace_before, cst.ParenthesizedWhitespace)
             and node.comma.whitespace_before.first_line.comment
         ):
             # from foo import (
             #     bar  # THIS PART
             #     ,
@@ -154,15 +164,17 @@
             #   # THIS PART
             #   c,  # (but only if it's not the last item)
             # )
             comments.following.extend(
                 line.comment.value for line in ws.empty_lines if line.comment
             )
 
-    return SortableImportItem(name=name, asname=asname, comments=comments, stem=stem)
+    return SortableImportItem(
+        name=name, asname=asname, comments=comments, stem=stem, comma=comma
+    )
 
 
 def import_from_node(node: cst.SimpleStatementLine, config: Config) -> SortableImport:
     # TODO: This duplicates (differently) what's in the LibCST import metadata visitor.
 
     stem: Optional[str] = None
     items: List[SortableImportItem] = []
@@ -199,14 +211,18 @@
     # assume that "following" comments are actually meant for an item after that
     prev: Optional[SortableImportItem] = None
     for item in items:
         if prev is not None and prev.comments.following:
             item.comments.before.extend(prev.comments.following)
             prev.comments.following.clear()
         prev = item
+    # inline comments after the last import (without a comma)
+    if prev is not None and comments.inline:
+        prev.comments.inline.extend(comments.inline)
+        comments.inline.clear()
     # following comments on the last item should maybe be on the import itself
     if prev is not None and prev.comments.following:
         comments.final.extend(prev.comments.following)
         prev.comments.following.clear()
 
     imp = SortableImport(
         stem=stem,
@@ -218,14 +234,16 @@
     )
     return imp
 
 
 def import_to_node(
     imp: SortableImport, module: cst.Module, indent: str, config: Config
 ) -> cst.BaseStatement:
+    if config.magic_commas and imp.stem and imp.trailing_comma:
+        return import_to_node_multi(imp, module)
     node = import_to_node_single(imp, module)
     content = indent + render_node(node, module).rstrip()
     # basic imports can't be reflowed, so only deal with from-imports
     if imp.stem and len(content) > config.line_length:
         node = import_to_node_multi(imp, module)
     return node
 
@@ -247,14 +265,15 @@
         asname = cst.AsName(name=cst.Name(item.asname)) if item.asname else None
         node = cst.ImportAlias(name=name, asname=asname)
         names.append(node)
         trailing_comments += item.comments.before
         trailing_comments += item.comments.inline
         trailing_comments += item.comments.following
 
+    trailing_comments += imp.comments.inline
     trailing_comments += imp.comments.final
     trailing_comments += imp.comments.last_inline
     if trailing_comments:
         text = COMMENT_INDENT.join(trailing_comments)
         trailing_whitespace = cst.TrailingWhitespace(
             whitespace=cst.SimpleWhitespace(COMMENT_INDENT), comment=cst.Comment(text)
         )
@@ -320,15 +339,17 @@
         if inline:
             first_line = cst.TrailingWhitespace(
                 whitespace=cst.SimpleWhitespace(COMMENT_INDENT),
                 comment=cst.Comment(inline),
             )
 
         if idx == item_count - 1:
-            following = item.comments.following + imp.comments.final
+            following = (
+                item.comments.following + imp.comments.inline + imp.comments.final
+            )
         else:
             following = item.comments.following
 
         after = cst.ParenthesizedWhitespace(
             indent=True,
             first_line=first_line,
             empty_lines=[
```

### Comparing `usort-1.1.0b1/usort/types.py` & `usort-1.1.0b2/usort/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,19 @@
     ndots: int
 
 
 @dataclass(order=True)
 class SortableImportItem:
     name: str = field(order=str.casefold)
     asname: Optional[str] = field(eq=True, order=case_insensitive_ordering)
-    comments: ImportItemComments = field(eq=False, order=False)
+    comments: ImportItemComments = field(
+        eq=False, order=False, factory=ImportItemComments
+    )
     stem: Optional[str] = field(order=False, default=None, repr=False)
+    comma: bool = field(eq=False, order=False, default=False, repr=False)
 
     @property
     def fullname(self) -> str:
         return stem_join(self.stem, self.name)
 
     def __add__(self, other: "SortableImportItem") -> "SortableImportItem":
         if not isinstance(other, SortableImportItem):
@@ -129,16 +132,16 @@
 
 
 @dataclass(order=True, repr=False)
 class SortableImport:
     sort_key: SortKey = field(init=False)
     stem: Optional[str] = field(order=case_insensitive_ordering)  # "from" imports
     items: List[SortableImportItem] = field()
-    comments: ImportComments = field(order=False)
-    indent: str = field(order=False)
+    comments: ImportComments = field(order=False, factory=ImportComments)
+    indent: str = field(order=False, default="")
     config: Config = field(eq=False, order=False, factory=Config)
 
     # for cli/debugging only
     node: cst.CSTNode = field(eq=False, order=False, factory=cst.EmptyLine)
 
     def __repr__(self) -> str:
         items = indent(("\n".join(f"{item!r}," for item in self.items)), "        ")
@@ -200,14 +203,20 @@
             comments=self.comments + other.comments,
             indent=self.indent,
             config=self.config,
             node=self.node,
         )
 
     @property
+    def trailing_comma(self) -> bool:
+        if self.items:
+            return self.items[-1].comma
+        return False
+
+    @property
     def imported_names(self) -> Dict[str, str]:
         results: Dict[str, str] = {}
 
         for item in self.items:
             key = item.asname or item.name
             if self.stem is None and not item.asname:
                 key = top_level_name(item.name)
```

### Comparing `usort-1.1.0b1/usort/util.py` & `usort-1.1.0b2/usort/util.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/tests/__init__.py` & `usort-1.1.0b2/usort/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/tests/cli.py` & `usort-1.1.0b2/usort/tests/cli.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/tests/config.py` & `usort-1.1.0b2/usort/tests/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -167,14 +167,56 @@
             # from foo.bar import foo
             self.assertFalse(config.is_side_effect_import("foo.bar", ["foo"]))
             # from foo.bar import baz
             self.assertTrue(config.is_side_effect_import("foo.bar", ["baz"]))
             # from foo.bar import bazzy
             self.assertFalse(config.is_side_effect_import("foo.bar", ["bazzy"]))
 
+    def test_config_magic_commas(self) -> None:
+        with tempfile.TemporaryDirectory() as d:
+            d_path = Path(d)
+            (d_path / "foo").mkdir(parents=True)
+            (d_path / "foo" / "bar.py").write_text("import os")
+
+            with self.subTest("default"):
+                (d_path / "foo" / "pyproject.toml").write_text("")
+                conf = Config.find(d_path / "foo" / "bar.py")
+                self.assertFalse(conf.magic_commas)
+
+            with self.subTest("enabled"):
+                (d_path / "foo" / "pyproject.toml").write_text(
+                    """\
+[tool.usort]
+magic_commas = true
+"""
+                )
+                conf = Config.find(d_path / "foo" / "bar.py")
+                self.assertTrue(conf.magic_commas)
+
+    def test_config_merge_imports(self) -> None:
+        with tempfile.TemporaryDirectory() as d:
+            d_path = Path(d)
+            (d_path / "foo").mkdir(parents=True)
+            (d_path / "foo" / "bar.py").write_text("import os")
+
+            with self.subTest("default"):
+                (d_path / "foo" / "pyproject.toml").write_text("")
+                conf = Config.find(d_path / "foo" / "bar.py")
+                self.assertTrue(conf.merge_imports)
+
+            with self.subTest("disabled"):
+                (d_path / "foo" / "pyproject.toml").write_text(
+                    """\
+[tool.usort]
+merge_imports = false
+"""
+                )
+                conf = Config.find(d_path / "foo" / "bar.py")
+                self.assertFalse(conf.merge_imports)
+
     def test_config_excludes(self) -> None:
         with tempfile.TemporaryDirectory() as d:
             d_path = Path(d)
             (d_path / "foo").mkdir(parents=True)
             (d_path / "foo" / "bar.py").write_text("import os")
 
             with self.subTest("default config"):
```

### Comparing `usort-1.1.0b1/usort/tests/functional.py` & `usort-1.1.0b2/usort/tests/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,90 +404,96 @@
                 # eleven
             """,
         )
 
     def test_multi_line_maintain(self) -> None:
         self.assertUsortResult(
             """
-                from fuzz import buzz
+                from phi import rho
                 # one
-                from foo import (  # two
+                from alpha import (  # two
                     # three
-                    bar,  # four
+                    beta,  # four
                     # five
-                    baz # six
+                    delta # six
                     , # seven
-                    # eight
-                )  # nine
-                # ten
+                    gamma # eight
+                    # nine
+                )  # ten
+                # eleven
             """,
             """
                 # one
-                from foo import (  # two
+                from alpha import (  # two
                     # three
-                    bar,  # four
+                    beta,  # four
                     # five
-                    baz,  # six  # seven
-                    # eight
-                )  # nine
-                from fuzz import buzz
-                # ten
+                    delta,  # six  # seven
+                    gamma,  # eight
+                    # nine
+                )  # ten
+                from phi import rho
+                # eleven
             """,
         )
 
     def test_multi_line_maintain_inner(self) -> None:
         self.assertUsortResult(
             """
                 def foo():
-                    from fuzz import buzz
+                    from phi import rho
                     # one
-                    from foo import (  # two
+                    from alpha import (  # two
                         # three
-                        bar,  # four
+                        beta,  # four
                         # five
-                        baz # six
+                        delta # six
                         , # seven
-                        # eight
-                    )  # nine
-                    # ten
+                        gamma # eight
+                        # nine
+                    )  # ten
+                    # eleven
             """,
             """
                 def foo():
                     # one
-                    from foo import (  # two
+                    from alpha import (  # two
                         # three
-                        bar,  # four
+                        beta,  # four
                         # five
-                        baz,  # six  # seven
-                        # eight
-                    )  # nine
-                    from fuzz import buzz
-                    # ten
+                        delta,  # six  # seven
+                        gamma,  # eight
+                        # nine
+                    )  # ten
+                    from phi import rho
+                    # eleven
             """,
         )
 
     def test_multi_line_collapse(self) -> None:
         self.assertUsortResult(
             """
                 from fuzz import buzz
                 # 1
-                from foo import (  # 2
+                from a import (  # 2
                     # 3
-                    bar,  # 4
+                    b,  # 4
                     # 5
-                    baz # 6
+                    c # 6
                     , # 7
-                )  # 8
-                # 9
+                    d # 8
+                    # 9
+                )  # 10
+                # 11
             """,
             """
                 # 1
-                from foo import bar, baz  # 2  # 3  # 4  # 5  # 6  # 7  # 8
+                from a import b, c, d  # 2  # 3  # 4  # 5  # 6  # 7  # 8  # 9  # 10
                 from fuzz import buzz
-                # 9
+                # 11
             """,
         )
 
     def test_multi_line_collapse_inner(self) -> None:
         self.assertUsortResult(
             """
                 def foo():
@@ -726,14 +732,54 @@
                 import math  # noqa  # fun
 
                 import black  # fun
                 import usort  # noqa
             """,
         )
 
+    def test_magic_commas_disabled(self) -> None:
+        self.assertUsortResult(
+            """
+                from a import (
+                    b,
+                    c,
+                )
+                from foo import ( # important comment
+                    bar,
+                    baz  # @manual
+                )
+            """,
+            """
+                from a import b, c
+                from foo import bar, baz  # important comment  # @manual
+            """,
+        )
+
+    def test_magic_commas_enabled(self) -> None:
+        self.assertUsortResult(
+            """
+                from a import (
+                    b,
+                    c,
+                )
+                from foo import (  # important comment
+                    bar,
+                    baz  # @manual
+                )
+            """,
+            """
+                from a import (
+                    b,
+                    c,
+                )
+                from foo import bar, baz  # important comment  # @manual
+            """,
+            Config(magic_commas=True),
+        )
+
     def test_merging_import_items(self) -> None:
         self.assertUsortResult(
             """
                 import os
                 import os.path
                 from typing import List, Dict, Tuple, Set, Optional
                 import os
```

### Comparing `usort-1.1.0b1/usort/tests/sorting.py` & `usort-1.1.0b2/usort/tests/sorting.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/tests/stdlibs.py` & `usort-1.1.0b2/usort/tests/stdlibs.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/usort/tests/translate.py` & `usort-1.1.0b2/usort/tests/translate.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 
 import libcst as cst
 
 from ..config import Config
 from ..sorting import ImportSorter
 from ..translate import import_from_node
+from ..types import SortableImport, SortableImportItem
 from ..util import parse_import
 
 
 class SortableImportTest(unittest.TestCase):
     def test_import_from_node_Import(self) -> None:
         imp = import_from_node(parse_import("import a"), Config())
         self.assertIsNone(imp.stem)
@@ -77,14 +78,35 @@
 
         imp = import_from_node(parse_import("from . import a as b"), Config())
         self.assertEqual(".", imp.stem)
         self.assertEqual("a", imp.items[0].name)
         self.assertEqual("b", imp.items[0].asname)
         self.assertEqual({"b": ".a"}, imp.imported_names)
 
+    def test_import_from_node_multiline(self) -> None:
+        imp = import_from_node(parse_import("from a import (\n  b,\n  c\n)"), Config())
+        expected = SortableImport(
+            stem="a",
+            items=[
+                SortableImportItem(name="b", asname="", stem="a", comma=True),
+                SortableImportItem(name="c", asname="", stem="a", comma=False),
+            ],
+        )
+        self.assertListEqual(expected.items, imp.items)
+
+        imp = import_from_node(parse_import("from a import (\n  b,\n  c,\n)"), Config())
+        expected = SortableImport(
+            stem="a",
+            items=[
+                SortableImportItem(name="b", asname="", stem="a", comma=True),
+                SortableImportItem(name="c", asname="", stem="a", comma=True),
+            ],
+        )
+        self.assertListEqual(expected.items, imp.items)
+
 
 class IsSortableTest(unittest.TestCase):
     def test_is_sortable(self) -> None:
         sorter = ImportSorter(module=cst.Module([]), path=Path(), config=Config())
         self.assertTrue(sorter.is_sortable_import(parse_import("import a")))
         self.assertTrue(sorter.is_sortable_import(parse_import("from a import b")))
         self.assertFalse(
```

### Comparing `usort-1.1.0b1/usort/tests/types.py` & `usort-1.1.0b2/usort/tests/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -210,14 +210,35 @@
 
         with self.subTest("bad types"):
             with self.assertRaisesRegex(
                 TypeError, "unsupported.+'SortableImport'.+'int'"
             ):
                 a += 10  # type: ignore
 
+    def test_sortable_import_trailing_comma(self) -> None:
+        imp = types.SortableImport(
+            stem="a",
+            items=[
+                types.SortableImportItem(name="b", asname="", stem="a", comma=True),
+                types.SortableImportItem(name="c", asname="", stem="a", comma=True),
+                types.SortableImportItem(name="d", asname="", stem="a", comma=False),
+            ],
+        )
+        self.assertFalse(imp.trailing_comma)
+
+        imp = types.SortableImport(
+            stem="a",
+            items=[
+                types.SortableImportItem(name="b", asname="", stem="a", comma=True),
+                types.SortableImportItem(name="c", asname="", stem="a", comma=True),
+                types.SortableImportItem(name="d", asname="", stem="a", comma=True),
+            ],
+        )
+        self.assertTrue(imp.trailing_comma)
+
     def test_sortable_block_repr(self) -> None:
         imp = types.SortableBlock(
             start_idx=0,
             end_idx=2,
             imports=[
                 types.SortableImport(
                     stem="foo",
```

### Comparing `usort-1.1.0b1/usort/tests/util.py` & `usort-1.1.0b2/usort/tests/util.py`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/.gitignore` & `usort-1.1.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/LICENSE` & `usort-1.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/README.md` & `usort-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/pyproject.toml` & `usort-1.1.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `usort-1.1.0b1/PKG-INFO` & `usort-1.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usort
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Safe, minimal import sorting
 Project-URL: Changelog, https://usort.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://usort.readthedocs.io
 Project-URL: Github, https://github.com/facebook/usort
 Author: Meta
 Author-email: Tim Hatch <thatch@fb.com>, Amethyst Reese <amethyst@fb.com>
 License: MIT License
```

