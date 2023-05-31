# Comparing `tmp/color_palette_extract-0.3.0.tar.gz` & `tmp/color_palette_extract-0.4.0.tar.gz`

## Comparing `color_palette_extract-0.3.0.tar` & `color_palette_extract-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 color_palette_extract-0.3.0/Cargo.toml
--rwxr-xr-x   0     1001      123      242 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/.github/workflows/build-wheels.sh
--rw-r--r--   0     1001      123     2835 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/.github/workflows/build.yml
--rw-r--r--   0     1001      123      685 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/.gitignore
--rw-r--r--   0     1001      123       24 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/README.md
--rw-r--r--   0     1001      123      329 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123      292 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/run.py
--rw-r--r--   0     1001      123     1373 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123     6155 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/test/airbnb.png
--rw-r--r--   0     1001      123  1152390 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/test/instagram.png
--rw-r--r--   0     1001      123     8948 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/test/instagram.svg
--rw-r--r--   0     1001      123    10752 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/test/mastercard.webp
--rw-r--r--   0     1001      123    49709 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/test/test.jpg
--rw-r--r--   0     1001      123     5286 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/test/test2.png
--rw-r--r--   0     1001      123     2557 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/test/test3.jpeg
--rw-r--r--   0     1001      123    32261 2023-05-16 11:15:44.000000 color_palette_extract-0.3.0/Cargo.lock
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 color_palette_extract-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 color_palette_extract-0.4.0/Cargo.toml
+-rwxr-xr-x   0     1001      123      242 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/.github/workflows/build-wheels.sh
+-rw-r--r--   0     1001      123     2835 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0     1001      123      685 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/.gitignore
+-rw-r--r--   0     1001      123       24 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/README.md
+-rw-r--r--   0     1001      123      329 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123      292 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/run.py
+-rw-r--r--   0     1001      123     1493 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123     6155 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/airbnb.png
+-rw-r--r--   0     1001      123  1152390 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/instagram.png
+-rw-r--r--   0     1001      123     8948 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/instagram.svg
+-rw-r--r--   0     1001      123    10752 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/mastercard.webp
+-rw-r--r--   0     1001      123    49709 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/test.jpg
+-rw-r--r--   0     1001      123     5286 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/test2.png
+-rw-r--r--   0     1001      123     2557 2023-05-31 07:32:18.000000 color_palette_extract-0.4.0/test/test3.jpeg
+-rw-r--r--   0     1001      123    32261 2023-05-31 07:33:51.000000 color_palette_extract-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 color_palette_extract-0.4.0/PKG-INFO
```

### Comparing `color_palette_extract-0.3.0/.github/workflows/build.yml` & `color_palette_extract-0.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/.gitignore` & `color_palette_extract-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/src/lib.rs` & `color_palette_extract-0.4.0/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 
 use colors_transform::{Color, Rgb};
 use pyo3::wrap_pyfunction;
 
 #[pyfunction]
-fn extract_from_bytes(data: &PyBytes) -> PyResult<Vec<Vec<f32>>> {
+fn extract_from_bytes(
+    data: &PyBytes, 
+    has_alpha: bool, 
+    down_size_to: f64,
+    small_bucket: f64,
+) -> PyResult<Vec<Vec<f32>>> {
     let mut result: Vec<Vec<f32>> = Vec::new();
 
     let img = image::load_from_memory(data.as_bytes()).unwrap();
 
-    let colors = dominant_color::get_colors(img.to_rgb8().into_raw().as_slice(), false);
+    let colors = dominant_color::get_colors_with_config(img.to_rgb8().into_raw().as_slice(), has_alpha, down_size_to, small_bucket);
 
     let mut group: Vec<f32> = Vec::new();
     for color in colors {
         group.push(color as f32);
         if group.len() == 3 {
             result.push(vec![group[0], group[1], group[2]]);
             group.clear();
```

### Comparing `color_palette_extract-0.3.0/test/airbnb.png` & `color_palette_extract-0.4.0/test/airbnb.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/test/instagram.png` & `color_palette_extract-0.4.0/test/instagram.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/test/instagram.svg` & `color_palette_extract-0.4.0/test/instagram.svg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/test/mastercard.webp` & `color_palette_extract-0.4.0/test/mastercard.webp`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/test/test.jpg` & `color_palette_extract-0.4.0/test/test.jpg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/test/test2.png` & `color_palette_extract-0.4.0/test/test2.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/test/test3.jpeg` & `color_palette_extract-0.4.0/test/test3.jpeg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.3.0/Cargo.lock` & `color_palette_extract-0.4.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "color_palette_extract"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
  "colors-transform",
  "dominant_color",
  "image",
  "pyo3",
  "pyo3-file",
 ]
```

