# Comparing `tmp/downscale_image-1.2.0.tar.gz` & `tmp/downscale_image-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downscale_image-1.2.0.tar", max compression
+gzip compressed data, was "downscale_image-1.3.0.tar", max compression
```

## Comparing `downscale_image-1.2.0.tar` & `downscale_image-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1925 2022-11-05 13:12:13.904710 downscale_image-1.2.0/downscale_image/__init__.py
--rw-r--r--   0        0        0     2877 2022-11-05 15:01:55.472676 downscale_image-1.2.0/downscale_image/__main__.py
--rw-r--r--   0        0        0     1275 2022-11-05 15:01:55.472676 downscale_image-1.2.0/downscale_image/_registry_utils.py
--rw-r--r--   0        0        0     1084 2022-11-05 13:12:13.902711 downscale_image-1.2.0/LICENSE
--rw-r--r--   0        0        0     1030 2022-11-05 15:01:55.473675 downscale_image-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      657 2022-11-05 15:01:55.471673 downscale_image-1.2.0/README.md
--rw-r--r--   0        0        0     1453 2022-11-05 15:02:06.665674 downscale_image-1.2.0/setup.py
--rw-r--r--   0        0        0     1338 2022-11-05 15:02:06.665674 downscale_image-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2004 2023-05-31 01:57:55.142932 downscale_image-1.3.0/downscale_image/__init__.py
+-rw-r--r--   0        0        0     3312 2023-05-31 01:57:55.259932 downscale_image-1.3.0/downscale_image/__main__.py
+-rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.3.0/downscale_image/_registry_utils.py
+-rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-31 01:59:54.004497 downscale_image-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.3.0/README.md
+-rw-r--r--   0        0        0     1453 2023-05-31 02:00:19.550647 downscale_image-1.3.0/setup.py
+-rw-r--r--   0        0        0     1287 2023-05-31 02:00:19.551648 downscale_image-1.3.0/PKG-INFO
```

### Comparing `downscale_image-1.2.0/downscale_image/__init__.py` & `downscale_image-1.3.0/downscale_image/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,24 +35,26 @@
             "Error, Could not find ffmpeg to execute. Make sure it is on the PATH variable.",
             file=sys.stderr,
         )
         raise
     return result
 
 
-def downscale(img: pathlib.Path, max_mega_bytes: int) -> pathlib.Path:
+def downscale(
+    img: pathlib.Path, max_mega_bytes: float, *_, output_prefix="", outtput_suffix="_smaller"
+) -> pathlib.Path:
     """Incrementally downscale img until it is <= max_mega_bytes in size."""
     current_size = _get_file_size_in_mega(img)
     working_img = img
     current_scale = 1.0
 
     if current_size <= max_mega_bytes:
         return img
 
-    working_img = img.parent / (img.stem + "_smaller" + ".".join(img.suffixes))
+    working_img = img.parent / (output_prefix + img.stem + outtput_suffix + ".".join(img.suffixes))
     shutil.copyfile(img, working_img)
 
     while current_size > max_mega_bytes:
         if working_img.is_file():
             working_img.unlink()
 
         working_img = _scale(img, scale=current_scale)
```

### Comparing `downscale_image-1.2.0/downscale_image/__main__.py` & `downscale_image-1.3.0/downscale_image/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,56 +11,70 @@
 
 _ON_WINDOWS = platform.system().lower() == "windows"
 
 if _ON_WINDOWS:
     from downscale_image import _registry_utils
 
 _DEFAULT_MATCHES = (
-    ["!.venv/", "!.git/", "!objects/"]
+    ["!.venv/", "!.git/", "!objects/", "!.ts/"]
     + [f"*{ext}" for ext in downscale_image.SUPPORTED_FILE_EXTENSIONS]
     + [f"*{ext}".upper() for ext in downscale_image.SUPPORTED_FILE_EXTENSIONS]
 )
 _CWD = pathlib.Path.cwd()
 
 
 @click.command()
 @click.option(
     "--max-size",
     default=2,
     help="Max output size (in MB)",
-    type=click.IntRange(min=0, min_open=True),
+    type=click.FloatRange(min=0, min_open=True),
     show_default=True,
 )
 @click.option(
+    "--suffix", default="_smaller", help="Additional name to add when generating new file name."
+)
+@click.option(
+    "--prefix",
+    default="",
+    help="Additional part of name to add start of new file name. (include a '/' to denote a folder)",
+)
+@click.option(
     "--add-to-right-click-menu",
     help="(Windows only) Register this program in right click menu for supported file types.",
     is_flag=True,
     default=False,
 )
 @click.argument(
     "in_file",
     nargs=-1,
     metavar="FILE_OR_DIRECTORY",
     type=click.Path(exists=True, dir_okay=True, path_type=pathlib.Path),
 )
-def main(max_size, in_file: typing.Tuple[pathlib.Path], add_to_right_click_menu: bool):
+def main(
+    max_size,
+    in_file: typing.Tuple[pathlib.Path],
+    add_to_right_click_menu: bool,
+    suffix: str,
+    prefix: str,
+):
     """Downscale file_or_directory to desired max-size."""
     if add_to_right_click_menu:
         if not _ON_WINDOWS:
             raise Exception("Error, registry right click menus are only support on Windows.")
         exe = pathlib.Path(sys.argv[0])
         args = []
         _registry_utils.register_downscale_commands(str(exe), args)
 
     files_to_prcoess: typing.List[pathlib.Path] = []
 
     for path in in_file:
         if path.is_dir():
             spec = pathspec.PathSpec.from_lines(
-                pathspec.patterns.GitWildMatchPattern, _DEFAULT_MATCHES
+                pathspec.patterns.GitWildMatchPattern, _DEFAULT_MATCHES + [f"*{suffix}.*"]
             )
             files_to_prcoess.extend([path / p for p in spec.match_tree(path)])
         else:
             files_to_prcoess.append(path)
 
     fail_count = 0
     last_error = None
@@ -69,15 +83,17 @@
     for file in files_to_prcoess:
         try:
             file = file.resolve().relative_to(_CWD)
         except ValueError:
             file = file.resolve()
         print(f"Downscaling {file}...")
         try:
-            downscale_image.downscale(file, max_mega_bytes=max_size)
+            downscale_image.downscale(
+                file, max_mega_bytes=max_size, output_prefix=prefix, outtput_suffix=suffix
+            )
             print(f"Finished")
         except Exception as e:
             fail_count += 1
             if fail_count > 5:
                 print("Several errors have occured, stopping")
                 break
             print("An error occured", file=sys.stderr)
```

### Comparing `downscale_image-1.2.0/downscale_image/_registry_utils.py` & `downscale_image-1.3.0/downscale_image/_registry_utils.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.2.0/LICENSE` & `downscale_image-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `downscale_image-1.2.0/pyproject.toml` & `downscale_image-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "downscale_image"
-version = "1.2.0"
+version = "1.3.0"
 description = "downscale image to desired file size"
 authors = ["mshafer1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mshafer1/downscale_image"
 include = [
     "LICENSE",
```

### Comparing `downscale_image-1.2.0/README.md` & `downscale_image-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `downscale_image-1.2.0/setup.py` & `downscale_image-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.0', 'pathspec>=0.10.1,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['downscale-image = downscale_image.__main__:main']}
 
 setup_kwargs = {
     'name': 'downscale-image',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'downscale image to desired file size',
     'long_description': '# downscale_image\nA utility to downscale an image to the desired file size.\n\nRelies on an install of ffmpeg to incrementally downscale the image file into a new file.\n\nThis modules provides the script `downscale-image`\n\n```\n> downscale-image --help\nUsage: downscale-image [OPTIONS] FILE_OR_DIRECTORY\n\n  Downscale file_or_directory to desired max-size.\n\nOptions:\n  --max-size INTEGER RANGE   Max output size (in MB)  [default: 2; x>0]\n  --add-to-right-click-menu  (Windows only) Register this program in right\n                             click menu for supported file types.\n  --help                     Show this message and exit.\n\n```\n',
     'author': 'mshafer1',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mshafer1/downscale_image',
```

### Comparing `downscale_image-1.2.0/PKG-INFO` & `downscale_image-1.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: downscale-image
-Version: 1.2.0
+Version: 1.3.0
 Summary: downscale image to desired file size
 Home-page: https://github.com/mshafer1/downscale_image
 License: MIT
 Author: mshafer1
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.0)
 Requires-Dist: pathspec (>=0.10.1,<0.11.0)
 Project-URL: Repository, https://github.com/mshafer1/downscale_image
 Description-Content-Type: text/markdown
```

