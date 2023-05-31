# Comparing `tmp/pyromark-0.1.2.tar.gz` & `tmp/pyromark-0.1.3.tar.gz`

## Comparing `pyromark-0.1.2.tar` & `pyromark-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 pyromark-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123     1065 2023-05-21 17:32:18.000000 pyromark-0.1.2/LICENSE
--rw-r--r--   0     1001      123     3505 2023-05-21 17:32:18.000000 pyromark-0.1.2/README.md
--rw-r--r--   0     1001      123     2888 2023-05-21 17:32:18.000000 pyromark-0.1.2/pyproject.toml
--rw-r--r--   0     1001      123      488 2023-05-21 17:32:18.000000 pyromark-0.1.2/pyromark.pyi
--rw-r--r--   0     1001      123     2132 2023-05-21 17:32:18.000000 pyromark-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123     8539 2023-05-21 17:32:18.000000 pyromark-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 pyromark-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 pyromark-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     1065 2023-05-31 15:31:37.000000 pyromark-0.1.3/LICENSE
+-rw-r--r--   0     1001      123     3505 2023-05-31 15:31:37.000000 pyromark-0.1.3/README.md
+-rw-r--r--   0     1001      123     2894 2023-05-31 15:31:37.000000 pyromark-0.1.3/pyproject.toml
+-rw-r--r--   0     1001      123      488 2023-05-31 15:31:37.000000 pyromark-0.1.3/pyromark.pyi
+-rw-r--r--   0     1001      123     2132 2023-05-31 15:31:37.000000 pyromark-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123     8539 2023-05-31 15:31:37.000000 pyromark-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 pyromark-0.1.3/PKG-INFO
```

### Comparing `pyromark-0.1.2/LICENSE` & `pyromark-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyromark-0.1.2/README.md` & `pyromark-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyromark-0.1.2/pyproject.toml` & `pyromark-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.15.1,<0.16"]
+requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [project]
 name = "pyromark"
 description = "Blazingly fast Markdown parser"
 readme = "README.md"
 keywords = ["converter", "html"]
@@ -90,14 +90,15 @@
     "D400",
     "D401",
     "D407",
     "D415",
     "D417",
     "DJ008",
     "ERA001",
+    "FBT002",
     "PD901",
     "PLR0911",
     "PLR0912",
     "PLR0913",
     "PLR0915",
     "PT012",
     "RUF001",
```

### Comparing `pyromark-0.1.2/src/lib.rs` & `pyromark-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyromark-0.1.2/Cargo.lock` & `pyromark-0.1.3/Cargo.lock`

 * *Files 13% similar despite different names*

```diff
@@ -46,26 +46,26 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -84,17 +84,17 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulldown-cmark"
 version = "0.9.3"
@@ -104,85 +104,85 @@
  "bitflags",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyromark"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "pulldown-cmark",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -228,17 +228,17 @@
 checksum = "50f37be617794602aabbeee0be4f259dc1778fabe05e2d67ee8f79326d5cb4f6"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

### Comparing `pyromark-0.1.2/PKG-INFO` & `pyromark-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyromark
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

