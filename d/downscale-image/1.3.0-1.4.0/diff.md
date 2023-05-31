# Comparing `tmp/downscale_image-1.3.0.tar.gz` & `tmp/downscale_image-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downscale_image-1.3.0.tar", max compression
+gzip compressed data, was "downscale_image-1.4.0.tar", max compression
```

## Comparing `downscale_image-1.3.0.tar` & `downscale_image-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2004 2023-05-31 01:57:55.142932 downscale_image-1.3.0/downscale_image/__init__.py
--rw-r--r--   0        0        0     3312 2023-05-31 01:57:55.259932 downscale_image-1.3.0/downscale_image/__main__.py
--rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.3.0/downscale_image/_registry_utils.py
--rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.3.0/LICENSE
--rw-r--r--   0        0        0     1030 2023-05-31 01:59:54.004497 downscale_image-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.3.0/README.md
--rw-r--r--   0        0        0     1453 2023-05-31 02:00:19.550647 downscale_image-1.3.0/setup.py
--rw-r--r--   0        0        0     1287 2023-05-31 02:00:19.551648 downscale_image-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2334 2023-05-31 02:34:02.914113 downscale_image-1.4.0/downscale_image/__init__.py
+-rw-r--r--   0        0        0     3646 2023-05-31 02:35:59.492199 downscale_image-1.4.0/downscale_image/__main__.py
+-rw-r--r--   0        0        0     1275 2023-05-31 01:43:25.169575 downscale_image-1.4.0/downscale_image/_registry_utils.py
+-rw-r--r--   0        0        0     1084 2022-10-01 17:29:23.915284 downscale_image-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1030 2023-05-31 02:37:09.032544 downscale_image-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-05-31 01:43:25.163574 downscale_image-1.4.0/README.md
+-rw-r--r--   0        0        0     1453 2023-05-31 02:37:20.241079 downscale_image-1.4.0/setup.py
+-rw-r--r--   0        0        0     1287 2023-05-31 02:37:20.242079 downscale_image-1.4.0/PKG-INFO
```

### Comparing `downscale_image-1.3.0/downscale_image/__main__.py` & `downscale_image-1.4.0/downscale_image/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,38 +11,42 @@
 
 _ON_WINDOWS = platform.system().lower() == "windows"
 
 if _ON_WINDOWS:
     from downscale_image import _registry_utils
 
 _DEFAULT_MATCHES = (
-    ["!.venv/", "!.git/", "!objects/", "!.ts/"]
+    ["!.venv/", "!.git/", "!objects/", "!.ts/*"]
     + [f"*{ext}" for ext in downscale_image.SUPPORTED_FILE_EXTENSIONS]
     + [f"*{ext}".upper() for ext in downscale_image.SUPPORTED_FILE_EXTENSIONS]
 )
 _CWD = pathlib.Path.cwd()
 
 
 @click.command()
+@click.version_option()
 @click.option(
     "--max-size",
     default=2,
     help="Max output size (in MB)",
     type=click.FloatRange(min=0, min_open=True),
     show_default=True,
 )
 @click.option(
-    "--suffix", default="_smaller", help="Additional name to add when generating new file name."
-)
-@click.option(
     "--prefix",
     default="",
     help="Additional part of name to add start of new file name. (include a '/' to denote a folder)",
 )
 @click.option(
+    "--suffix", default="_smaller", help="Additional name to add when generating new file name.", show_default=True
+)
+@click.option(
+    "--override-output-format", help="Change output file extensions (useful for wanting to switch from png to jpg or vice verse)"
+)
+@click.option(
     "--add-to-right-click-menu",
     help="(Windows only) Register this program in right click menu for supported file types.",
     is_flag=True,
     default=False,
 )
 @click.argument(
     "in_file",
@@ -52,29 +56,30 @@
 )
 def main(
     max_size,
     in_file: typing.Tuple[pathlib.Path],
     add_to_right_click_menu: bool,
     suffix: str,
     prefix: str,
+    override_output_format: typing.Optional[str],
 ):
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
-                pathspec.patterns.GitWildMatchPattern, _DEFAULT_MATCHES + [f"*{suffix}.*"]
+                pathspec.patterns.GitWildMatchPattern, _DEFAULT_MATCHES + [f"!*{suffix}.*"]
             )
             files_to_prcoess.extend([path / p for p in spec.match_tree(path)])
         else:
             files_to_prcoess.append(path)
 
     fail_count = 0
     last_error = None
@@ -83,18 +88,18 @@
     for file in files_to_prcoess:
         try:
             file = file.resolve().relative_to(_CWD)
         except ValueError:
             file = file.resolve()
         print(f"Downscaling {file}...")
         try:
-            downscale_image.downscale(
-                file, max_mega_bytes=max_size, output_prefix=prefix, outtput_suffix=suffix
+            output = downscale_image.downscale(
+                file, max_mega_bytes=max_size, output_prefix=prefix, outtput_suffix=suffix, override_output_format=override_output_format
             )
-            print(f"Finished")
+            print(f"Finished. Output stored in {output}\n\n")
         except Exception as e:
             fail_count += 1
             if fail_count > 5:
                 print("Several errors have occured, stopping")
                 break
             print("An error occured", file=sys.stderr)
             print(e, file=sys.stderr)
```

### Comparing `downscale_image-1.3.0/downscale_image/_registry_utils.py` & `downscale_image-1.4.0/downscale_image/_registry_utils.py`

 * *Files identical despite different names*

### Comparing `downscale_image-1.3.0/LICENSE` & `downscale_image-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `downscale_image-1.3.0/pyproject.toml` & `downscale_image-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "downscale_image"
-version = "1.3.0"
+version = "1.4.0"
 description = "downscale image to desired file size"
 authors = ["mshafer1"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mshafer1/downscale_image"
 include = [
     "LICENSE",
```

### Comparing `downscale_image-1.3.0/README.md` & `downscale_image-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `downscale_image-1.3.0/setup.py` & `downscale_image-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.0', 'pathspec>=0.10.1,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['downscale-image = downscale_image.__main__:main']}
 
 setup_kwargs = {
     'name': 'downscale-image',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'downscale image to desired file size',
     'long_description': '# downscale_image\nA utility to downscale an image to the desired file size.\n\nRelies on an install of ffmpeg to incrementally downscale the image file into a new file.\n\nThis modules provides the script `downscale-image`\n\n```\n> downscale-image --help\nUsage: downscale-image [OPTIONS] FILE_OR_DIRECTORY\n\n  Downscale file_or_directory to desired max-size.\n\nOptions:\n  --max-size INTEGER RANGE   Max output size (in MB)  [default: 2; x>0]\n  --add-to-right-click-menu  (Windows only) Register this program in right\n                             click menu for supported file types.\n  --help                     Show this message and exit.\n\n```\n',
     'author': 'mshafer1',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mshafer1/downscale_image',
```

### Comparing `downscale_image-1.3.0/PKG-INFO` & `downscale_image-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: downscale-image
-Version: 1.3.0
+Version: 1.4.0
 Summary: downscale image to desired file size
 Home-page: https://github.com/mshafer1/downscale_image
 License: MIT
 Author: mshafer1
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

