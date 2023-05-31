# Comparing `tmp/downscale_image-1.4.0.tar.gz` & `tmp/downscale_image-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downscale_image-1.4.0.tar", max compression
+gzip compressed data, was "downscale_image-1.4.1.tar", max compression
```

## Comparing `downscale_image-1.4.0.tar` & `downscale_image-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2334 2023-05-31 02:34:02.914113 downscale_image-1.4.0/downscale_image/__init__.py
--rw-r--r--   0        0        0     3646 2023-05-31 02:35:59.492199 downscale_image-1.4.0/downscale_image/__main__.py
--rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.0/downscale_image/_registry_utils.py
--rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.0/LICENSE
--rw-r--r--   0        0        0     1030 2023-05-31 02:37:09.032544 downscale_image-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.0/README.md
--rw-r--r--   0        0        0     1453 2023-05-31 02:37:20.241079 downscale_image-1.4.0/setup.py
--rw-r--r--   0        0        0     1287 2023-05-31 02:37:20.242079 downscale_image-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2365 2023-05-31 02:53:51.764840 downscale_image-1.4.1/downscale_image/__init__.py
+-rw-r--r--   0        0        0     3646 2023-05-31 02:35:59.492199 downscale_image-1.4.1/downscale_image/__main__.py
+-rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.1/downscale_image/_registry_utils.py
+-rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-31 02:56:32.494086 downscale_image-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.1/README.md
+-rw-r--r--   0        0        0     1453 2023-05-31 02:57:14.575802 downscale_image-1.4.1/setup.py
+-rw-r--r--   0        0        0     1287 2023-05-31 02:57:14.576991 downscale_image-1.4.1/PKG-INFO
```

### Comparing `downscale_image-1.4.0/downscale_image/__init__.py` & `downscale_image-1.4.1/downscale_image/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     """Incrementally downscale img until it is <= max_mega_bytes in size."""
     current_size = _get_file_size_in_mega(img)
     working_img = img
     current_scale = 1.0
     current_multiplier = 10
 
     if current_size <= max_mega_bytes:
+        print("Not changing")
         return img
 
     out_suffix = f".{override_output_format}" if override_output_format else ".".join(img.suffixes)
     working_img = img.parent / (output_prefix + img.stem + outtput_suffix + out_suffix)
     working_img.parent.mkdir(exist_ok=True, parents=True)
     shutil.copyfile(img, working_img)
```

### Comparing `downscale_image-1.4.0/downscale_image/__main__.py` & `downscale_image-1.4.1/downscale_image/__main__.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.0/downscale_image/_registry_utils.py` & `downscale_image-1.4.1/downscale_image/_registry_utils.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.0/LICENSE` & `downscale_image-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.0/pyproject.toml` & `downscale_image-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "downscale_image"
-version = "1.4.0"
+version = "1.4.1"
 description = "downscale image to desired file size"
 authors = ["mshafer1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mshafer1/downscale_image"
 include = [
     "LICENSE",
```

### Comparing `downscale_image-1.4.0/README.md` & `downscale_image-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `downscale_image-1.4.0/setup.py` & `downscale_image-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.0', 'pathspec>=0.10.1,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['downscale-image = downscale_image.__main__:main']}
 
 setup_kwargs = {
     'name': 'downscale-image',
-    'version': '1.4.0',
+    'version': '1.4.1',
     'description': 'downscale image to desired file size',
     'long_description': '# downscale_image\nA utility to downscale an image to the desired file size.\n\nRelies on an install of ffmpeg to incrementally downscale the image file into a new file.\n\nThis modules provides the script `downscale-image`\n\n```\n> downscale-image --help\nUsage: downscale-image [OPTIONS] FILE_OR_DIRECTORY\n\n  Downscale file_or_directory to desired max-size.\n\nOptions:\n  --max-size INTEGER RANGE   Max output size (in MB)  [default: 2; x>0]\n  --add-to-right-click-menu  (Windows only) Register this program in right\n                             click menu for supported file types.\n  --help                     Show this message and exit.\n\n```\n',
     'author': 'mshafer1',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mshafer1/downscale_image',
```

### Comparing `downscale_image-1.4.0/PKG-INFO` & `downscale_image-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: downscale-image
-Version: 1.4.0
+Version: 1.4.1
 Summary: downscale image to desired file size
 Home-page: https://github.com/mshafer1/downscale_image
 License: MIT
 Author: mshafer1
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

