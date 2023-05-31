# Comparing `tmp/lana-0.1.5.tar.gz` & `tmp/lana-0.1.6.tar.gz`

## Comparing `lana-0.1.5.tar` & `lana-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 lana-0.1.5/Cargo.toml
--rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.5/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.5/LICENSE
--rw-r--r--   0      501       20      640 2023-05-30 15:23:21.000000 lana-0.1.5/README.md
--rw-r--r--   0      501       20      475 2023-05-30 15:56:16.000000 lana-0.1.5/examples/competition.py
--rw-r--r--   0      501       20      354 2023-05-31 10:09:28.000000 lana-0.1.5/examples/example.py
--rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.5/lana/__init__.py
--rw-r--r--   0      501       20      651 2023-05-30 15:32:41.000000 lana-0.1.5/pyproject.toml
--rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.5/src/lib.rs
--rw-r--r--   0      501       20     3376 2023-05-31 10:09:39.000000 lana-0.1.5/src/matrix.rs
--rw-r--r--   0      501       20      885 2023-05-30 13:33:31.000000 lana-0.1.5/test/test_matrix.py
--rw-r--r--   0      501       20     9870 2023-05-31 09:47:02.000000 lana-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lana-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 lana-0.1.6/Cargo.toml
+-rw-r--r--   0      501       20      726 2023-05-31 13:58:49.000000 lana-0.1.6/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.6/LICENSE
+-rw-r--r--   0      501       20      640 2023-05-30 15:23:21.000000 lana-0.1.6/README.md
+-rw-r--r--   0      501       20      475 2023-05-30 15:56:16.000000 lana-0.1.6/examples/competition.py
+-rw-r--r--   0      501       20     5243 2023-05-31 15:01:48.000000 lana-0.1.6/examples/example.ipynb
+-rw-r--r--   0      501       20      509 2023-05-31 16:27:08.000000 lana-0.1.6/lana/__init__.py
+-rw-r--r--   0      501       20      651 2023-05-30 15:32:41.000000 lana-0.1.6/pyproject.toml
+-rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.6/src/lib.rs
+-rw-r--r--   0      501       20     5173 2023-05-31 16:19:08.000000 lana-0.1.6/src/matrix.rs
+-rw-r--r--   0      501       20      885 2023-05-30 13:33:31.000000 lana-0.1.6/test/test_matrix.py
+-rw-r--r--   0      501       20     9870 2023-05-31 13:57:32.000000 lana-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lana-0.1.6/PKG-INFO
```

### Comparing `lana-0.1.5/.gitignore` & `lana-0.1.6/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -71,8 +71,9 @@
 # Pyenv
 .python-version
 
 .env/
 target/
 .github/
 
-build.py
+build.py
+lab.py
```

### Comparing `lana-0.1.5/LICENSE` & `lana-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.1.5/README.md` & `lana-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lana-0.1.5/pyproject.toml` & `lana-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.1.5/test/test_matrix.py` & `lana-0.1.6/test/test_matrix.py`

 * *Files identical despite different names*

### Comparing `lana-0.1.5/Cargo.lock` & `lana-0.1.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "pyo3",
  "rayon",
 ]
 
 [[package]]
 name = "libc"
```

### Comparing `lana-0.1.5/PKG-INFO` & `lana-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Experimental Linear Algebra library written in Rust
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
```

