# Comparing `tmp/slamcore_utils-0.1.5a0.tar.gz` & `tmp/slamcore_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slamcore_utils-0.1.5a0.tar", max compression
+gzip compressed data, was "slamcore_utils-0.1.6.tar", max compression
```

## Comparing `slamcore_utils-0.1.5a0.tar` & `slamcore_utils-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0     1526 2023-01-31 13:35:48.396216 slamcore_utils-0.1.5a0/LICENSE.md
--rw-r--r--   0        0        0     3897 2023-01-31 13:35:48.396216 slamcore_utils-0.1.5a0/README.md
--rw-r--r--   0        0        0     1745 2023-01-31 13:35:48.396216 slamcore_utils-0.1.5a0/pyproject.toml
--rw-r--r--   0        0        0      360 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/__init__.py
--rw-r--r--   0        0        0     3053 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/arg_parser.py
--rw-r--r--   0        0        0     1300 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/data_converter.py
--rw-r--r--   0        0        0      679 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/dataset_dir_converter.py
--rw-r--r--   0        0        0     2881 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/fs.py
--rw-r--r--   0        0        0     3522 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/logging.py
--rw-r--r--   0        0        0     7047 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/openloris_converter.py
--rw-r--r--   0        0        0     3211 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/progress_bar.py
--rwxr-xr-x   0        0        0     2185 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/scripts/convert_openloris.py
--rwxr-xr-x   0        0        0     8824 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/scripts/setup_dataset.py
--rw-r--r--   0        0        0    15121 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/euroc_capture_info.json
--rw-r--r--   0        0        0    24299 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/openlorismain_capture_info.json
--rw-r--r--   0        0        0    24320 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/openlorismarket_capture_info.json
--rw-r--r--   0        0        0    15153 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/tum1024_capture_info.json
--rw-r--r--   0        0        0    15149 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/tum512_capture_info.json
--rw-r--r--   0        0        0      936 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/share/setup_dataset.json
--rw-r--r--   0        0        0      253 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/string.py
--rw-r--r--   0        0        0    13587 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/test_utils.py
--rw-r--r--   0        0        0     2330 2023-01-31 13:35:48.440216 slamcore_utils-0.1.5a0/slamcore_utils/utils.py
--rw-r--r--   0        0        0     5210 1970-01-01 00:00:00.000000 slamcore_utils-0.1.5a0/setup.py
--rw-r--r--   0        0        0     5056 1970-01-01 00:00:00.000000 slamcore_utils-0.1.5a0/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-05-31 17:55:25.837701 slamcore_utils-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0    14492 2023-05-31 17:55:25.837701 slamcore_utils-0.1.6/README.md
+-rw-r--r--   0        0        0     2332 2023-05-31 17:55:25.837701 slamcore_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/__init__.py
+-rw-r--r--   0        0        0     3053 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/arg_parser.py
+-rw-r--r--   0        0        0     1300 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/data_converter.py
+-rw-r--r--   0        0        0      679 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/dataset_dir_converter.py
+-rw-r--r--   0        0        0     1178 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/dataset_subdir_writer.py
+-rw-r--r--   0        0        0     2882 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/fs.py
+-rw-r--r--   0        0        0     3941 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/logging.py
+-rw-r--r--   0        0        0     5182 2023-05-31 17:55:25.881702 slamcore_utils-0.1.6/slamcore_utils/measurement_type.py
+-rw-r--r--   0        0        0     7047 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/openloris_converter.py
+-rw-r--r--   0        0        0     3306 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/progress_bar.py
+-rw-r--r--   0        0        0     1489 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/ros2/__init__.py
+-rw-r--r--   0        0        0     2021 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/ros2/ros2_converter_plugin.py
+-rw-r--r--   0        0        0     2350 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/ros2/ros2_utils.py
+-rw-r--r--   0        0        0     2284 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/ros_utils.py
+-rwxr-xr-x   0        0        0     2325 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/scripts/convert_openloris.py
+-rwxr-xr-x   0        0        0    18794 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/scripts/convert_rosbag2.py
+-rwxr-xr-x   0        0        0     8824 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/scripts/setup_dataset.py
+-rw-r--r--   0        0        0    15121 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/euroc_capture_info.json
+-rw-r--r--   0        0        0    24299 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/openlorismain_capture_info.json
+-rw-r--r--   0        0        0    24320 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/openlorismarket_capture_info.json
+-rw-r--r--   0        0        0    15153 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/tum1024_capture_info.json
+-rw-r--r--   0        0        0    15149 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/tum512_capture_info.json
+-rw-r--r--   0        0        0      936 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/share/setup_dataset.json
+-rw-r--r--   0        0        0      253 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/string.py
+-rw-r--r--   0        0        0    13762 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/test_utils.py
+-rw-r--r--   0        0        0     4256 2023-05-31 17:55:25.885702 slamcore_utils-0.1.6/slamcore_utils/utils.py
+-rw-r--r--   0        0        0    15757 1970-01-01 00:00:00.000000 slamcore_utils-0.1.6/PKG-INFO
```

### Comparing `slamcore_utils-0.1.5a0/LICENSE.md` & `slamcore_utils-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/pyproject.toml` & `slamcore_utils-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 [tool.poetry]
 name = "slamcore_utils"
-version = "0.1.5a"
+version = "0.1.6"
 description = "SLAMcore SLAM Utilities"
 authors = ["Nikos Koukis <nikolaos@slamcore.com>"]
 license = "BSD License"
 readme = "README.md"
 
 homepage = "https://github.com/slamcore/slamcore_utils"
 repository = "https://github.com/slamcore/slamcore_utils"
 classifiers = [
   "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: BSD License",
   "Operating System :: Unix",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6.8,<3.11"
 questionary = "^1.10.0"
 prompt-toolkit = ">3.0,<=3.0.23"
-numpy = "^1.19.5"
+numpy = [ { version = "^1.19.5", python = "<3.9" }, { version = "*", python = ">=3.9" } ]
 tqdm = { version = "^4.64.0", optional = true }
+pillow = { version = "^7.2.0", optional = true }
+lark = { version = "^1.1.5", optional = true }
+pyyaml = { version = "^6.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 black = { version = "*", allow-prereleases = true }
 isort = "^5.10.1"
 mock = "^4.0.3"
 pdbpp = "^0.10.3"
 mypy = ">=0.942"
 types-setuptools = "^57.4.12"
 pyright = "*"
 pyfakefs = "^4.5.6"
 pexpect = "^4.8.0"
+types-Pillow = "^9.5.0"
 
 [tool.poetry.scripts]
 slamcore-convert-openloris = "slamcore_utils.scripts.convert_openloris:main"
 slamcore-setup-dataset = "slamcore_utils.scripts.setup_dataset:main"
+slamcore-convert-rosbag2 = "slamcore_utils.scripts.convert_rosbag2:main"
 
 [tool.poetry.extras]
 tqdm = ["tqdm"]
+ros2 = ["pillow", "lark", "pyyaml"]
 
 [tool.isort]
 line_length = 95
 include_trailing_comma = true
 multi_line_output = 3
 
 [tool.black]
@@ -54,19 +61,33 @@
 include = '\.pyi?$'
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
-module = ["tqdm", "pytest", "pexpect"]
+module = [
+  "geometry_msgs.msg",
+  "numpy",
+  "pexpect",
+  "pytest",
+  "rclpy.serialization",
+  "rosbag2_py",
+  "rosidl_runtime_py.utilities",
+  "sensor_msgs.msg",
+  "tqdm",
+]
 ignore_missing_imports = true
 
 [tool.pyright]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.8"
 pythonPlatform = "Linux"
 
+[tool.ruff]
+line-length = 95
+target-version = "py38"
+
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/arg_parser.py` & `slamcore_utils-0.1.6/slamcore_utils/arg_parser.py`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/data_converter.py` & `slamcore_utils-0.1.6/slamcore_utils/data_converter.py`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/dataset_dir_converter.py` & `slamcore_utils-0.1.6/slamcore_utils/dataset_dir_converter.py`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/fs.py` & `slamcore_utils-0.1.6/slamcore_utils/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from shutil import rmtree
 
 from slamcore_utils.logging import logger
 
 """Filesystem-related utilities."""
 
+
 def get_ready_output_path(path: Path, overwrite_path: bool = False, logger=logger) -> Path:
     """
     Get a new valid path to write to. Depending on the `overwrite_path` flag it will either:
 
     - Remove all the contents of the given path (using `safe_rmtree`) and return the given path
       as is.
     - Or, it will use the specified path as a base to find the next suitable filename that's
```

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/logging.py` & `slamcore_utils-0.1.6/slamcore_utils/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from enum import Enum, auto
 from pathlib import Path
 
 from slamcore_utils.progress_bar import progress_bar
 
+
 class LoggingProfile(Enum):
     """Offers the available logging profiles that the slam_utils apps can run under.
 
     Add more if needed (e.g., log simultaneously to a file or to syslog) and adjust their
     behavior in the :py:func:`setup_pkg_logging` accordingly.
     """
 
@@ -46,14 +47,31 @@
     logger.setLevel(level)
     f = logging.Formatter(format_, datefmt="%H:%M:%S")
     ch = TqdmLoggingHandler()
     ch.setFormatter(f)
     logger.addHandler(ch)
 
 
+_verbosity_to_logging_lvls = {
+    0: logging.WARNING,
+    1: logging.INFO,
+    2: logging.DEBUG,
+}
+
+
+def verbotsity_to_logging_lvl(verbosity: int) -> int:
+    """Map CLI-provided verbosity count e.g., -vvv to logging module level."""
+    if verbosity > 2:
+        return logging.DEBUG
+    elif verbosity < 0:
+        raise RuntimeError(f"Invalid verbosity level provided -> {verbosity}")
+    else:
+        return _verbosity_to_logging_lvls[verbosity]
+
+
 def setup_pkg_logging(
     fname: str, profile: LoggingProfile = _LOGGING_PROFILE
 ) -> logging.Logger:
     """
     Setup a logger based on the filename of the current file.
 
     Usage::
@@ -110,9 +128,8 @@
     logger = logging.getLogger(name)
     _setup_logging(name, format_=format_, level=level)
 
     return logger
 
 
 _pkg_logger_name = Path(__file__).parent.name
-logger = logging.getLogger(_pkg_logger_name)
-setup_pkg_logging(_pkg_logger_name)
+logger = setup_pkg_logging(_pkg_logger_name)
```

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/openloris_converter.py` & `slamcore_utils-0.1.6/slamcore_utils/openloris_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from slamcore_utils.dataset_dir_converter import DatasetDirConverter
 from slamcore_utils.logging import logger
 from slamcore_utils.progress_bar import progress_bar
 
 
 class OpenLORISConverter(DatasetDirConverter):
-    """Convert a dataset from the OpenLORIS format to the SLAMcore Dataset Format."""
+    """Convert a dataset from the OpenLORIS format to the Slamcore Dataset Format."""
 
     def __init__(
         self,
         *,
         preserve_orig_timestamps: bool = False,
         **kargs,
     ):
```

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/progress_bar.py` & `slamcore_utils-0.1.6/slamcore_utils/progress_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 TL;DR: import `progress_bar`. This will resolve to tqdm.tqdm if available or _ProgressBar
        otherwise.
 """
 
 import importlib
 import sys
 import time
-from typing import Any, Iterable
+from typing import Any, Iterable, Optional, Type, cast
 
 
 class _ProgressBar:
-    def __init__(self, iterable: Iterable[Any] = None, total=None, *args, **kargs):
+    def __init__(self, iterable: Optional[Iterable[Any]] = None, total=None, *args, **kargs):
         """
         Poor man's Tqdm.
 
         This offers a minimal API with __iter__, and update as the two alternatives for
         updating the progress of a task. For a richer experience, just install Tqdm itself
 
         :param iterable: Iterable to decorate with a progressbar.
@@ -90,9 +90,11 @@
         sys.stdout.write(f"{s}{end}\r")
         sys.stdout.flush()
 
 
 try:
     tqdm = importlib.import_module("tqdm")
     progress_bar = tqdm.tqdm  # type: ignore
-except:
+except:  # noqa
     progress_bar = _ProgressBar
+
+progress_bar = cast(Type[_ProgressBar], progress_bar)
```

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/scripts/convert_openloris.py` & `slamcore_utils-0.1.6/slamcore_utils/scripts/convert_openloris.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import argparse
 from pathlib import Path
 
 from slamcore_utils.arg_parser import add_bool_argument, existing_dir
 from slamcore_utils.fs import get_ready_output_path
 from slamcore_utils.logging import logger
 from slamcore_utils.openloris_converter import OpenLORISConverter
+from slamcore_utils.utils import format_dict
 
 
 def main():
     """Main."""
 
     # argument parsing ------------------------------------------------------------------------
     parser = argparse.ArgumentParser(
@@ -47,21 +48,27 @@
 
     # overwrite output?
     output_dir = get_ready_output_path(
         output_dir, overwrite_path=overwrite_output, logger=logger
     )
 
     # announce to user ------------------------------------------------------------------------
-    s = (
-        "\n\nConverting OpenLORIS Dataset to internal SLAMcore format\n"
-        f"\t* Input directory:            {input_dir}\n"
-        f"\t* Output directory:           {output_dir}\n"
-        f"\t* Overwrite output directory: {overwrite_output}\n"
+    announce_items = {
+        "Input directory": input_dir,
+        "Output directory": output_dir,
+        "Overwrite output directory": overwrite_output,
+    }
+    logger.info(
+        format_dict(
+            header="Converting OpenLORIS Dataset to internal SLAMcore format",
+            items=announce_items,
+            prefix="\n\n",
+            suffix="\n",
+        )
     )
-    logger.info(s)
 
     # run conversion --------------------------------------------------------------------------
     converter = OpenLORISConverter(
         in_path=input_dir,
         out_path=output_dir,
         preserve_orig_timestamps=False,
     )
```

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/scripts/setup_dataset.py` & `slamcore_utils-0.1.6/slamcore_utils/scripts/setup_dataset.py`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/euroc_capture_info.json` & `slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/euroc_capture_info.json`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/openlorismain_capture_info.json` & `slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/openlorismain_capture_info.json`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/openlorismarket_capture_info.json` & `slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/openlorismarket_capture_info.json`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/tum1024_capture_info.json` & `slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/tum1024_capture_info.json`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/share/capture_infos/tum512_capture_info.json` & `slamcore_utils-0.1.6/slamcore_utils/share/capture_infos/tum512_capture_info.json`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/share/setup_dataset.json` & `slamcore_utils-0.1.6/slamcore_utils/share/setup_dataset.json`

 * *Files identical despite different names*

### Comparing `slamcore_utils-0.1.5a0/slamcore_utils/test_utils.py` & `slamcore_utils-0.1.6/slamcore_utils/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     def __call__(self, file: Path, expected_file: Path):
         """Compare two csv files.
 
         Assert that their contents are close. We assume that these files can be loaded via
         np.loadtxt.
         """
         try:
-            # load and try comparing as numeric arrays.
-            # will fail if the values in the CSV are not exclusively numeric
+            # load and try comparing as numeric arrays. Assume first row is a header and always
+            # skip it. Will fail if the values in the CSV are not exclusively numeric
             arr = np.loadtxt(fname=file, delimiter=",", skiprows=1)
             arr_expected = np.loadtxt(fname=expected_file, delimiter=",", skiprows=1)
             assert np.allclose(arr, arr_expected), (
                 "Output file contents don't match the expected contents."
                 f"Take a look at the following files: {file.absolute()} | {expected_file.absolute()}"
             )
         except ValueError:
@@ -193,21 +193,26 @@
                     Path(tempfile.gettempdir()) / f"slamcore_utils_{get_rand_string(len=5)}"
                 )
                 shutil.copytree(output, backup_dir)
                 to_restore_backup.append(Path(backup_dir))
             else:
                 to_remove.append(output)
 
-        s = "Will automatically remove the following files/directories\n\n"
-        s += "\n".join(map(str, to_remove))
-        s += "\n"
-        s += "\nWill preserve the following files/directories\n\n"
-        s += "\n".join(map(str, to_restore))
-        s += "\n"
-        logger.info(s)
+        s = ""
+        if to_remove:
+            s = "\nWill automatically remove the following files/directories\n\n \t- "
+            s += "\n \t- ".join(map(str, to_remove))
+        if to_restore:
+            s += "\n"
+            s += "\nWill preserve the following files/directories\n\n \t- "
+            s += "\n \t- ".join(map(str, to_restore))
+            s += "\n"
+
+        if s:
+            logger.info(f"\n{s}\n")
 
         try:
             # change directory? ---------------------------------------------------------------
             if cd_test_dir:
                 try:
                     oldpwd = Path(".").absolute()
                     os.chdir(data_path)
@@ -221,14 +226,22 @@
             # run it --------------------------------------------------------------------------
             cmd = [exec_path, *args]
             proc = subprocess.run(cmd, stdout=PIPE, stderr=PIPE, check=False)
             stdout, stderr = proc.stdout, proc.stderr
             stdout = stdout.decode("utf-8")
             stderr = stderr.decode("utf-8")
 
+            # assert error code ---------------------------------------------------------------
+            if proc.returncode != expected_return_code:
+                assert False, (
+                    "Got an unexpected error code, "
+                    f"{proc.returncode} instead of the expected {expected_return_code} - "
+                    f"stdout: {stdout} | stderr: {stderr}"
+                )
+
             # assert stdout/err ---------------------------------------------------------------
             if stdout_contains is not None:
                 for stdout_sample in stdout_contains:
                     assert stdout_sample in stdout, (
                         "Required stdout string not found, "
                         f"[{stdout}] should have contained [{stdout_sample}]"
                     )
@@ -236,22 +249,14 @@
             if stderr_contains is not None:
                 for stderr_sample in stderr_contains:
                     assert stderr_sample in stderr, (
                         "Required stderr string not found, "
                         f"[{stderr}] should have contained [{stderr_sample}]"
                     )
 
-            # assert error code ---------------------------------------------------------------
-            if proc.returncode != expected_return_code:
-                assert False, (
-                    "Got an unexpected error code, "
-                    f"{proc.returncode} instead of the expected {expected_return_code}\n\n"
-                    f"stdout:\n\n{stdout}\n\nstderr:\n\n{stderr}"
-                )
-
             # assert all the required files are actually there --------------------------------
             for output in outputs:
                 expected_output = output.parent / f"expected_{output.name}"
                 # make sure that the expected output files were generated
                 assert (
                     output.exists()
                 ), f"Output file/directory {output} was not generated as was expected"
```

