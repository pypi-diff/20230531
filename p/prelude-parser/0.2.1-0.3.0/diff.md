# Comparing `tmp/prelude_parser-0.2.1.tar.gz` & `tmp/prelude_parser-0.3.0.tar.gz`

## Comparing `prelude_parser-0.2.1.tar` & `prelude_parser-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 prelude_parser-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123      439 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/dependabot.yml
--rw-r--r--   0     1001      123      539 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/release-draft-template.yml
--rw-r--r--   0     1001      123     2599 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/workflows/pypi_publish.yml
--rw-r--r--   0     1001      123      309 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/workflows/release-drafter.yml
--rw-r--r--   0     1001      123     1889 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.github/workflows/testing.yml
--rw-r--r--   0     1001      123      686 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.gitignore
--rw-r--r--   0     1001      123      640 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     7889 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1080 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/LICENSE
--rw-r--r--   0     1001      123     2801 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/README.md
--rw-r--r--   0     1001      123      595 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/justfile
--rw-r--r--   0     1001      123      115 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/__init__.py
--rw-r--r--   0     1001      123      399 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/_prelude_parser.pyi
--rw-r--r--   0     1001      123      911 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/pandas.py
--rw-r--r--   0     1001      123     1753 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/parser.py
--rw-r--r--   0     1001      123      901 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/polars.py
--rw-r--r--   0     1001      123        0 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/prelude_parser/py.typed
--rw-r--r--   0     1001      123     1876 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123      132 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/requirements-dev.txt
--rw-r--r--   0     1001      123    10754 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/__init__.py
--rw-r--r--   0     1001      123     1304 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/assets/test1.xml
--rw-r--r--   0     1001      123     1839 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/assets/test2.xml
--rw-r--r--   0     1001      123     2122 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/assets/test3.xml
--rw-r--r--   0     1001      123      312 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/conftest.py
--rw-r--r--   0     1001      123      942 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/test_pandas.py
--rw-r--r--   0     1001      123     8018 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/test_parser.py
--rw-r--r--   0     1001      123     1004 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/tests/test_polars.py
--rw-r--r--   0     1001      123    15614 2023-05-29 12:10:53.000000 prelude_parser-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 prelude_parser-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 prelude_parser-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123      439 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/.github/dependabot.yml
+-rw-r--r--   0     1001      123      539 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/.github/release-draft-template.yml
+-rw-r--r--   0     1001      123     2599 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0     1001      123      309 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0     1001      123     1889 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/.github/workflows/testing.yml
+-rw-r--r--   0     1001      123      686 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/.gitignore
+-rw-r--r--   0     1001      123      640 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     7889 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1080 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     2801 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/README.md
+-rw-r--r--   0     1001      123      595 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/justfile
+-rw-r--r--   0     1001      123      115 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/prelude_parser/__init__.py
+-rw-r--r--   0     1001      123      399 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/prelude_parser/_prelude_parser.pyi
+-rw-r--r--   0     1001      123      911 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/prelude_parser/pandas.py
+-rw-r--r--   0     1001      123     1753 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/prelude_parser/parser.py
+-rw-r--r--   0     1001      123      901 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/prelude_parser/polars.py
+-rw-r--r--   0     1001      123        0 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/prelude_parser/py.typed
+-rw-r--r--   0     1001      123     1876 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123      132 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     8521 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/__init__.py
+-rw-r--r--   0     1001      123     1304 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/assets/test1.xml
+-rw-r--r--   0     1001      123     1839 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/assets/test2.xml
+-rw-r--r--   0     1001      123     2122 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/assets/test3.xml
+-rw-r--r--   0     1001      123      312 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/conftest.py
+-rw-r--r--   0     1001      123      944 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/test_pandas.py
+-rw-r--r--   0     1001      123     8018 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/test_parser.py
+-rw-r--r--   0     1001      123     1006 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/tests/test_polars.py
+-rw-r--r--   0     1001      123    15573 2023-05-31 01:48:46.000000 prelude_parser-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 prelude_parser-0.3.0/PKG-INFO
```

### Comparing `prelude_parser-0.2.1/Cargo.toml` & `prelude_parser-0.3.0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "prelude-parser"
-version = "0.2.1"
+version = "0.3.0"
 description = "Parses XML files exported from Prelude EDC into formats usable by Python."
 edition = "2021"
 license = "MIT"
 homepage = "https://github.com/pbs-data-solutions/prelude-parser"
 repository = "https://github.com/pbs-data-solutions/prelude-parser"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "_prelude_parser"
 crate-type = ["cdylib"]
 
 [dependencies]
-chrono = "0.4.24"
+chrono = "0.4.25"
 pyo3 = { version = "0.18.3", features = ["extension-module", "abi3-py38"] }
 roxmltree = "0.18.0"
```

### Comparing `prelude_parser-0.2.1/.github/release-draft-template.yml` & `prelude_parser-0.3.0/.github/release-draft-template.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/.github/workflows/pypi_publish.yml` & `prelude_parser-0.3.0/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/.github/workflows/testing.yml` & `prelude_parser-0.3.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/.gitignore` & `prelude_parser-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/.pre-commit-config.yaml` & `prelude_parser-0.3.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -15,11 +15,11 @@
       language_version: python3
       args: [--line-length=100]
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
     - id: mypy
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.269
+    rev: v0.0.270
     hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `prelude_parser-0.2.1/CONTRIBUTING.md` & `prelude_parser-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/LICENSE` & `prelude_parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/README.md` & `prelude_parser-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/justfile` & `prelude_parser-0.3.0/justfile`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/prelude_parser/pandas.py` & `prelude_parser-0.3.0/prelude_parser/pandas.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/prelude_parser/parser.py` & `prelude_parser-0.3.0/prelude_parser/parser.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/prelude_parser/polars.py` & `prelude_parser-0.3.0/prelude_parser/polars.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/pyproject.toml` & `prelude_parser-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/tests/assets/test1.xml` & `prelude_parser-0.3.0/tests/assets/test1.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/tests/assets/test2.xml` & `prelude_parser-0.3.0/tests/assets/test2.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/tests/assets/test3.xml` & `prelude_parser-0.3.0/tests/assets/test3.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/tests/test_pandas.py` & `prelude_parser-0.3.0/tests/test_polars.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import pandas as pd
+import polars as pl
+from polars.testing import assert_frame_equal
 
-from prelude_parser.pandas import to_dataframe
+from prelude_parser.polars import to_dataframe
 
 
 def test_pandas_to_dataframe(test_file_1):
     result = to_dataframe(test_file_1)
     data = {
-        "BaseForm": [
+        "base_form": [
             "communications.form.name.communications",
             "communications.form.name.communications",
         ],
-        "FormGroup": ["Communications", "Communications"],
-        "FormNumber": [None, None],
-        "FormState": ["In-Work", "In-Work"],
-        "FormTitle": ["Communications", "Communications"],
-        "PatientId": ["1681574905819", "1681574994823"],
-        "PatientName": ["ABC-001", "ABC-002"],
-        "SiteId": ["1681574834910", "1681574834910"],
-        "SiteName": ["Some Site", "Some Site"],
-        "StudyName": ["PBS", "PBS"],
         "communications_made": ["Yes", "Yes"],
+        "form_group": ["Communications", "Communications"],
+        "form_number": [None, None],
+        "form_state": ["In-Work", "In-Work"],
+        "form_title": ["Communications", "Communications"],
+        "patient_id": [1681574905819, 1681574994823],
+        "patient_name": ["ABC-001", "ABC-002"],
+        "site_id": [1681574834910, 1681574834910],
+        "site_name": ["Some Site", "Some Site"],
+        "study_name": ["PBS", "PBS"],
     }
-    expected = pd.DataFrame.from_dict(data)
-    result = result.reindex(sorted(result.columns), axis=1)
-    assert expected.equals(result)
+    expected = pl.from_dict(data)  # type: ignore
+    result = result.pipe(lambda x: x.select(sorted(x.columns)))
+    assert_frame_equal(expected, result)
```

### Comparing `prelude_parser-0.2.1/tests/test_parser.py` & `prelude_parser-0.3.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.2.1/Cargo.lock` & `prelude_parser-0.3.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -39,21 +45,21 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "fdbc37d37da9e5bce8173f3a41b71d9bf3c674deebbaceacd0ebdabde76efb03"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
@@ -128,24 +134,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -177,15 +173,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "prelude-parser"
-version = "0.2.1"
+version = "0.3.0"
 dependencies = [
  "chrono",
  "pyo3",
  "roxmltree",
 ]
 
 [[package]]
```

### Comparing `prelude_parser-0.2.1/PKG-INFO` & `prelude_parser-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-parser
-Version: 0.2.1
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

