# Comparing `tmp/cro3n-0.0.2.tar.gz` & `tmp/cro3n-0.0.3.tar.gz`

## Comparing `cro3n-0.0.2.tar` & `cro3n-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      316 1970-01-01 00:00:00.000000 cro3n-0.0.2/Cargo.toml
--rw-r--r--   0     1001      121     1658 2022-09-02 09:30:05.000000 cro3n-0.0.2/.github/workflows/release.yml
--rw-r--r--   0     1001      121      329 2022-09-02 09:30:05.000000 cro3n-0.0.2/.gitignore
--rw-r--r--   0     1001      121        7 2022-09-02 09:30:05.000000 cro3n-0.0.2/.python-version
--rw-r--r--   0     1001      121     1061 2022-09-02 09:30:05.000000 cro3n-0.0.2/LICENSE
--rw-r--r--   0     1001      121     1639 2022-09-02 09:30:05.000000 cro3n-0.0.2/README.md
--rw-r--r--   0        0        0       10 2022-09-02 09:31:28.000000 cro3n-0.0.2/dist/cro3n-0.0.2.tar.gz
--rw-r--r--   0     1001      121     1226 2022-09-02 09:30:05.000000 cro3n-0.0.2/example/python/example.py
--rw-r--r--   0     1001      121     1302 2022-09-02 09:30:05.000000 cro3n-0.0.2/pyproject.toml
--rwxr-xr-x   0     1001      121      769 2022-09-02 09:30:29.000000 cro3n-0.0.2/run-maturin-action.sh
--rw-r--r--   0     1001      121     1803 2022-09-02 09:30:05.000000 cro3n-0.0.2/src/lib.rs
--rw-r--r--   0        0        0    12255 2022-09-02 09:31:24.000000 cro3n-0.0.2/Cargo.lock
--rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 cro3n-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      316 1970-01-01 00:00:00.000000 cro3n-0.0.3/Cargo.toml
+-rw-r--r--   0     1001      123     1658 2023-05-31 15:58:42.000000 cro3n-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      329 2023-05-31 15:58:42.000000 cro3n-0.0.3/.gitignore
+-rw-r--r--   0     1001      123        7 2023-05-31 15:58:42.000000 cro3n-0.0.3/.python-version
+-rw-r--r--   0     1001      123     1061 2023-05-31 15:58:42.000000 cro3n-0.0.3/LICENSE
+-rw-r--r--   0     1001      123     1733 2023-05-31 15:58:42.000000 cro3n-0.0.3/README.md
+-rw-r--r--   0        0        0       10 2023-05-31 16:01:42.000000 cro3n-0.0.3/dist/cro3n-0.0.3.tar.gz
+-rw-r--r--   0     1001      123     1226 2023-05-31 15:58:42.000000 cro3n-0.0.3/example/python/example.py
+-rw-r--r--   0     1001      123     1302 2023-05-31 15:58:42.000000 cro3n-0.0.3/pyproject.toml
+-rwxr-xr-x   0     1001      123      834 2023-05-31 15:59:18.000000 cro3n-0.0.3/run-maturin-action.sh
+-rw-r--r--   0     1001      123     1925 2023-05-31 15:58:42.000000 cro3n-0.0.3/src/lib.rs
+-rw-r--r--   0        0        0    16005 2023-05-31 16:01:38.000000 cro3n-0.0.3/Cargo.lock
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 cro3n-0.0.3/PKG-INFO
```

### Comparing `cro3n-0.0.2/.github/workflows/release.yml` & `cro3n-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cro3n-0.0.2/LICENSE` & `cro3n-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cro3n-0.0.2/README.md` & `cro3n-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,50 +36,50 @@
 00000230: 959a e295 90e2 959d 2020 e295 9ae2 9590  ........  ......
 00000240: e295 90e2 9590 e295 9d0a 6060 600a 0a5b  ..........```..[
 00000250: 215b 5265 6c65 6173 655d 2868 7474 7073  ![Release](https
 00000260: 3a2f 2f67 6974 6875 622e 636f 6d2f 5374  ://github.com/St
 00000270: 7261 7944 7261 676f 6e2f 6372 6f33 6e2f  rayDragon/cro3n/
 00000280: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
 00000290: 732f 7265 6c65 6173 652e 796d 6c2f 6261  s/release.yml/ba
-000002a0: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-000002b0: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
-000002c0: 7468 7562 2e63 6f6d 2f53 7472 6179 4472  thub.com/StrayDr
-000002d0: 6167 6f6e 2f63 726f 336e 2f61 6374 696f  agon/cro3n/actio
-000002e0: 6e73 2f77 6f72 6b66 6c6f 7773 2f72 656c  ns/workflows/rel
-000002f0: 6561 7365 2e79 6d6c 290a 5b21 5b47 6974  ease.yml).[![Git
-00000300: 4875 6220 6c61 7374 2063 6f6d 6d69 745d  Hub last commit]
-00000310: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000320: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
-00000330: 6173 742d 636f 6d6d 6974 2f73 7472 6179  ast-commit/stray
-00000340: 6472 6167 6f6e 2f63 726f 336e 295d 2868  dragon/cro3n)](h
-00000350: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000360: 6d2f 5374 7261 7944 7261 676f 6e2f 6372  m/StrayDragon/cr
-00000370: 6f33 6e2f 636f 6d6d 6974 7329 0a5b 215b  o3n/commits).[![
-00000380: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
-00000390: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000003a0: 692f 762f 6372 6f33 6e29 5d28 6874 7470  i/v/cro3n)](http
-000003b0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000003c0: 6a65 6374 2f63 726f 336e 290a 5b21 5b50  ject/cro3n).[![P
-000003d0: 7950 4920 2d20 5079 7468 6f6e 2056 6572  yPI - Python Ver
-000003e0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-000003f0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000400: 692f 7079 7665 7273 696f 6e73 2f63 726f  i/pyversions/cro
-00000410: 336e 295d 2868 7474 7073 3a2f 2f70 7970  3n)](https://pyp
-00000420: 692e 6f72 672f 7072 6f6a 6563 742f 6372  i.org/project/cr
-00000430: 6f33 6e29 0a5b 215b 5079 5049 202d 2049  o3n).[![PyPI - I
-00000440: 6d70 6c65 6d65 6e74 6174 696f 6e5d 2868  mplementation](h
-00000450: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000460: 6473 2e69 6f2f 7079 7069 2f69 6d70 6c65  ds.io/pypi/imple
-00000470: 6d65 6e74 6174 696f 6e2f 6372 6f33 6e29  mentation/cro3n)
-00000480: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-00000490: 7267 2f70 726f 6a65 6374 2f63 726f 336e  rg/project/cro3n
-000004a0: 290a 5b21 5b50 7950 4920 2d20 4c69 6365  ).[![PyPI - Lice
-000004b0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
-000004c0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000004d0: 2f6c 2f63 726f 336e 295d 2868 7474 7073  /l/cro3n)](https
+000002a0: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+000002b0: 2f2f 6769 7468 7562 2e63 6f6d 2f53 7472  //github.com/Str
+000002c0: 6179 4472 6167 6f6e 2f63 726f 336e 2f61  ayDragon/cro3n/a
+000002d0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+000002e0: 2f72 656c 6561 7365 2e79 6d6c 290a 5b21  /release.yml).[!
+000002f0: 5b47 6974 4875 6220 6c61 7374 2063 6f6d  [GitHub last com
+00000300: 6d69 745d 2868 7474 7073 3a2f 2f69 6d67  mit](https://img
+00000310: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000320: 7562 2f6c 6173 742d 636f 6d6d 6974 2f73  ub/last-commit/s
+00000330: 7472 6179 6472 6167 6f6e 2f63 726f 336e  traydragon/cro3n
+00000340: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000350: 622e 636f 6d2f 5374 7261 7944 7261 676f  b.com/StrayDrago
+00000360: 6e2f 6372 6f33 6e2f 636f 6d6d 6974 7329  n/cro3n/commits)
+00000370: 0a5b 215b 5079 5049 5d28 6874 7470 733a  .[![PyPI](https:
+00000380: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000390: 2f70 7970 692f 762f 6372 6f33 6e29 5d28  /pypi/v/cro3n)](
+000003a0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000003b0: 2f70 726f 6a65 6374 2f63 726f 336e 290a  /project/cro3n).
+000003c0: 5b21 5b50 7950 4920 2d20 5079 7468 6f6e  [![PyPI - Python
+000003d0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+000003e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000003f0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+00000400: 2f63 726f 336e 295d 2868 7474 7073 3a2f  /cro3n)](https:/
+00000410: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000420: 742f 6372 6f33 6e29 0a5b 215b 5079 5049  t/cro3n).[![PyPI
+00000430: 202d 2049 6d70 6c65 6d65 6e74 6174 696f   - Implementatio
+00000440: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+00000450: 6869 656c 6473 2e69 6f2f 7079 7069 2f69  hields.io/pypi/i
+00000460: 6d70 6c65 6d65 6e74 6174 696f 6e2f 6372  mplementation/cr
+00000470: 6f33 6e29 5d28 6874 7470 733a 2f2f 7079  o3n)](https://py
+00000480: 7069 2e6f 7267 2f70 726f 6a65 6374 2f63  pi.org/project/c
+00000490: 726f 336e 290a 5b21 5b47 6974 4875 625d  ro3n).[![GitHub]
+000004a0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000004b0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+000004c0: 6963 656e 7365 2f73 7472 6179 6472 6167  icense/straydrag
+000004d0: 6f6e 2f63 726f 336e 295d 2868 7474 7073  on/cro3n)](https
 000004e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5374  ://github.com/St
 000004f0: 7261 7944 7261 676f 6e2f 6372 6f33 6e2f  rayDragon/cro3n/
 00000500: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
 00000510: 4529 0a0a 2d2d 2d0a 0a41 6e6f 7468 6572  E)..---..Another
 00000520: 206f 6e65 202a 2a63 726f 6e20 6578 7072   one **cron expr
 00000530: 6573 7369 6f6e 2a2a 2075 7469 6c73 2070  ession** utils p
 00000540: 6163 6b61 6765 2066 6f72 2070 7974 686f  ackage for pytho
@@ -94,10 +94,16 @@
 000005d0: 2320 4578 616d 706c 650a 7365 6520 5b65  # Example.see [e
 000005e0: 7861 6d70 6c65 2f70 7974 686f 6e5d 282e  xample/python](.
 000005f0: 2f65 7861 6d70 6c65 2f70 7974 686f 6e29  /example/python)
 00000600: 0a0a 2323 2052 656c 6174 6564 2050 726f  ..## Related Pro
 00000610: 6a65 6374 730a 0a2d 205b 7a73 6c61 7974  jects..- [zslayt
 00000620: 6f6e 2f63 726f 6e5d 2868 7474 7073 3a2f  on/cron](https:/
 00000630: 2f67 6974 6875 622e 636f 6d2f 7a73 6c61  /github.com/zsla
-00000640: 7974 6f6e 2f63 726f 6e29 0a0a 2323 204c  yton/cron)..## L
-00000650: 4943 454e 5345 0a5b 4d49 545d 282e 2f4c  ICENSE.[MIT](./L
-00000660: 4943 454e 5345 29                        ICENSE)
+00000640: 7974 6f6e 2f63 726f 6e29 0a2d 205b 5079  yton/cron).- [Py
+00000650: 4f33 2f6d 6174 7572 696e 5d28 6874 7470  O3/maturin](http
+00000660: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
+00000670: 794f 332f 6d61 7475 7269 6e29 0a2d 205b  yO3/maturin).- [
+00000680: 5079 4f33 2f70 796f 335d 2868 7474 7073  PyO3/pyo3](https
+00000690: 3a2f 2f67 6974 6875 622e 636f 6d2f 5079  ://github.com/Py
+000006a0: 4f33 2f70 796f 3329 0a0a 2323 204c 4943  O3/pyo3)..## LIC
+000006b0: 454e 5345 0a5b 4d49 545d 282e 2f4c 4943  ENSE.[MIT](./LIC
+000006c0: 454e 5345 29                             ENSE)
```

### Comparing `cro3n-0.0.2/example/python/example.py` & `cro3n-0.0.3/example/python/example.py`

 * *Files identical despite different names*

### Comparing `cro3n-0.0.2/pyproject.toml` & `cro3n-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/#configuring-metadata
 name = "cro3n"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `cro3n-0.0.2/run-maturin-action.sh` & `cro3n-0.0.3/run-maturin-action.sh`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 set -e
 echo "::group::Install Rust"
 which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain stable
 export PATH="$HOME/.cargo/bin:$PATH"
 rustup override set stable
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
-export PATH="$PATH:/opt/python/cp36-cp36m/bin:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin"
+export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/download/v0.13.2/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v0.13.7/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
+python3 -m pip install cffi || true
 echo "::endgroup::"
 maturin build --release --sdist -o ./dist --find-interpreter
```

### Comparing `cro3n-0.0.2/src/lib.rs` & `cro3n-0.0.3/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use chrono::Utc;
 use cron::Schedule;
 use pyo3::{exceptions::PyValueError, prelude::*};
 use std::str::FromStr;
 
 /// validate cron expression
 #[pyfunction]
+#[pyo3(signature = (expression))]
 fn check_cron_expression(expression: String) -> PyResult<String> {
     let result = match Schedule::from_str(expression.as_str()) {
         Ok(_) => String::new(),
         Err(error) => format!("Check `{}` failed, due to {:?}", &expression, error),
     };
     Ok(result)
 }
@@ -22,14 +23,15 @@
 }
 
 #[pymethods]
 impl CronExpr {
     /// crate::cron::Schedule wrapper class
     /// NOTE: will raise ValueError when wrong input
     #[new]
+    #[pyo3(text_signature = "(expression)")]
     fn py_new(expression: String) -> PyResult<Self> {
         let err_msg = match Schedule::from_str(expression.as_str()) {
             Ok(_) => String::new(),
             Err(error) => format!("Check `{}` failed, due to {:?}", &expression, error),
         };
         if !err_msg.is_empty() {
             Err(PyValueError::new_err(err_msg))
@@ -38,14 +40,15 @@
                 source: expression.clone(),
                 schedule: Schedule::from_str(expression.as_str()).unwrap(),
             })
         }
     }
     /// Get next n upcomming time
     /// Example: ['2022-09-02 21:01:00 UTC', '2022-09-03 21:01:00 UTC', '2022-09-04 21:01:00 UTC', '2022-09-05 21:01:00 UTC', '2022-09-06 21:01:00 UTC']
+    #[pyo3(text_signature = "($self, n)")]
     fn next_n_upcoming_time_literals(&self, n: usize) -> PyResult<Vec<String>> {
         Ok(self
             .schedule
             .upcoming(Utc)
             .take(n)
             .map(|dt| format!("{}", dt))
             .collect())
```

### Comparing `cro3n-0.0.2/Cargo.lock` & `cro3n-0.0.3/Cargo.lock`

 * *Files 14% similar despite different names*

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
@@ -21,48 +27,54 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.11.0"
+version = "3.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
+name = "cc"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1ad822118d20d2c234f427000d5acc36eabe1e29a348c89b63dd60b13f28e5d"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.22"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfd4d1b31faaa3a89d7934dbded3111da0d2ef28e3ebccdb4f0179f5929d1ef1"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
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
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cro3n"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "chrono",
  "cron",
  "pyo3",
 ]
 
 [[package]]
@@ -74,209 +86,215 @@
  "chrono",
  "nom",
  "once_cell",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.47"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c495f162af0bf17656d0014a0eded5f3cd2f365fdd204548c2869db89359dc7"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
+ "iana-time-zone-haiku",
  "js-sys",
- "once_cell",
  "wasm-bindgen",
- "winapi",
+ "windows",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "js-sys"
-version = "0.3.59"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "258451ab10b34f8af53416d1fdab72c22e805f0c92a1136d59470ec0b11138b2"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.132"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8371e4e5341c3a96db127eb2465ac681ced4c433e01dd0e938adbef26ba93ba5"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
-version = "0.4.8"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f80bf5aacaf25cbfc8210d1cfb718f2bf3b11c4c54e5afe36c236853a8ec390"
+checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "nom"
-version = "7.1.1"
+version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8903e5a29a317527874d0402f867152a3d21c908bb0b933e416c65e301d4c36"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
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
 
 [[package]]
 name = "once_cell"
-version = "1.13.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "074864da206b4973b84eb91683020dbefd6a8c3f0f38e054d93954e891935e4e"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.3"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a279cbf25cb0757810394fbc1e359949b59e348145c643a939a525692e6929"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.43"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a2ca2c61bc9f3d74d2886294ab7b9853abd9c1ad903a3ac7815c58989bb7bab"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.16.6"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0220c44442c9b239dd4357aa856ac468a4f5e1f0df19ddb89b2522952eb4c6ca"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.16.6"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c819d397859445928609d0ec5afc2da5204e0d0f73d6bf9e153b04e83c9cdc2"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.16.6"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca882703ab55f54702d7bfe1189b41b0af10272389f04cae38fe4cd56c65f75f"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.16.6"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "568749402955ad7be7bad9a09b8593851cd36e549ac90bfd44079cea500f3f21"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.16.6"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "611f64e82d98f447787e82b8e7b0ebc681e1eb78fc1252668b2c605ffb4e1eb8"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -290,117 +308,128 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.9.0"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+
+[[package]]
+name = "syn"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
 name = "syn"
-version = "1.0.99"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58dbef6ec655055e20b86b15a8cc6d439cca19b667537ac6a1369572d151ab13"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.4"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "time"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db9e6914ab8b1ae1c260a4ae7a49b6c5611b40328a735b21862567685e73255"
+checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
 dependencies = [
  "libc",
  "wasi",
  "winapi",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.3"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4f5b37a154999a8f3f98cc23a628d850e154479cd94decf3414696e12e31aaf"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.82"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc7652e3f6c4706c8d9cd54832c4a4ccb9b5336e2c3bd154d5cccfbf1c1f5f7d"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.82"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "662cd44805586bd52971b9586b1df85cdbbd9112e4ef4d8f41559c334dc6ac3f"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.82"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b260f13d3012071dfb1512849c033b1925038373aea48ced3012c09df952c602"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.82"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5be8e654bdd9b79216c2929ab90721aa82faf65c48cdf08bdc4e7f51357b80da"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.82"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6598dd0bd3c7d51095ff6531a5b23e02acdc81804e30d8f07afb77b7215a140a"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -417,48 +446,137 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
 name = "windows-sys"
-version = "0.36.1"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `cro3n-0.0.2/PKG-INFO` & `cro3n-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cro3n
-Version: 0.0.2
+Version: 0.0.3
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,32 +13,32 @@
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 Summary: Another one **cron expression** utils package for python
 Author-email: straydragon <straydragonv@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Bug Tracker, https://github.com/straydragon/cro3n/issues
 Project-URL: Homepage, https://github.com/straydragon/cro3n
+Project-URL: Bug Tracker, https://github.com/straydragon/cro3n/issues
 
 ```
  ██████╗ ██████╗   ██████╗3 ███╗   ██╗
 ██╔════╝ ██╔══██╗ ██╔═══██╗ ████╗  ██║
 ██║      ██████╔╝ ██║   ██║ ██╔██╗ ██║
 ██║      ██╔══██╗ ██║   ██║ ██║╚██╗██║
 ╚██████╗ ██║  ██║ ╚██████╔╝ ██║ ╚████║
  ╚═════╝ ╚═╝  ╚═╝  ╚═════╝  ╚═╝  ╚═══╝
 ```
 
-[![Release](https://github.com/StrayDragon/cro3n/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/StrayDragon/cro3n/actions/workflows/release.yml)
+[![Release](https://github.com/StrayDragon/cro3n/actions/workflows/release.yml/badge.svg)](https://github.com/StrayDragon/cro3n/actions/workflows/release.yml)
 [![GitHub last commit](https://img.shields.io/github/last-commit/straydragon/cro3n)](https://github.com/StrayDragon/cro3n/commits)
 [![PyPI](https://img.shields.io/pypi/v/cro3n)](https://pypi.org/project/cro3n)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cro3n)](https://pypi.org/project/cro3n)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/cro3n)](https://pypi.org/project/cro3n)
-[![PyPI - License](https://img.shields.io/pypi/l/cro3n)](https://github.com/StrayDragon/cro3n/blob/main/LICENSE)
+[![GitHub](https://img.shields.io/github/license/straydragon/cro3n)](https://github.com/StrayDragon/cro3n/blob/main/LICENSE)
 
 ---
 
 Another one **cron expression** utils package for python, wrapped on rust crate [zslayton/cron](https://github.com/zslayton/cron).
 
 ## Installation
 ```bash
@@ -47,10 +47,12 @@
 
 ## Example
 see [example/python](./example/python)
 
 ## Related Projects
 
 - [zslayton/cron](https://github.com/zslayton/cron)
+- [PyO3/maturin](https://github.com/PyO3/maturin)
+- [PyO3/pyo3](https://github.com/PyO3/pyo3)
 
 ## LICENSE
 [MIT](./LICENSE)
```

