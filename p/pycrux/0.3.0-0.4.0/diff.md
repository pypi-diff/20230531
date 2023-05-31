# Comparing `tmp/pycrux-0.3.0.tar.gz` & `tmp/pycrux-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrux-0.3.0.tar", max compression
+gzip compressed data, was "pycrux-0.4.0.tar", max compression
```

## Comparing `pycrux-0.3.0.tar` & `pycrux-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-05-30 13:54:53.299492 pycrux-0.3.0/LICENSE
--rw-r--r--   0        0        0       85 2023-05-30 20:24:52.720158 pycrux-0.3.0/pycrux/__init__.py
--rw-r--r--   0        0        0     4154 2023-05-31 11:44:53.776004 pycrux-0.3.0/pycrux/crux.py
--rw-r--r--   0        0        0        0 2023-05-30 13:54:53.314684 pycrux-0.3.0/pycrux/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-30 13:54:53.314102 pycrux-0.3.0/pycrux/utils/config.py
--rw-r--r--   0        0        0      731 2023-05-30 14:16:53.108904 pycrux-0.3.0/pycrux/utils/logger.py
--rw-r--r--   0        0        0      959 2023-05-31 11:50:04.340155 pycrux-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 pycrux-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-30 13:54:53.299492 pycrux-0.4.0/LICENSE
+-rw-r--r--   0        0        0       85 2023-05-30 20:24:52.720158 pycrux-0.4.0/pycrux/__init__.py
+-rw-r--r--   0        0        0     4277 2023-05-31 11:57:07.825820 pycrux-0.4.0/pycrux/crux.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:54:53.314684 pycrux-0.4.0/pycrux/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-30 13:54:53.314102 pycrux-0.4.0/pycrux/utils/config.py
+-rw-r--r--   0        0        0      731 2023-05-30 14:16:53.108904 pycrux-0.4.0/pycrux/utils/logger.py
+-rw-r--r--   0        0        0      959 2023-05-31 11:57:26.270461 pycrux-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 pycrux-0.4.0/PKG-INFO
```

### Comparing `pycrux-0.3.0/LICENSE` & `pycrux-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrux-0.3.0/pycrux/crux.py` & `pycrux-0.4.0/pycrux/crux.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,19 +91,21 @@
         ]
 
         # Extension needs the starting dot.
         if ending[0] != ".":
             ending = "." + ending
 
         # Get all files with desired ending.
-        return [
+        fit_files_subdirs = [
             file
             for sub_folder in sub_folders
             for file in glob.glob(f"{sub_folder}/*{ending}")
         ]
+        fit_files_root = glob.glob(f"""{root}/*{ending}""")
+        return fit_files_root + fit_files_subdirs
 
     @staticmethod
     def _raise_if_file_does_not_exist(file: Path) -> None:
         if not file.is_file():
             raise FileNotFoundError(
                 f"No file exists at the location specified: {file.as_posix()}"
             )
```

### Comparing `pycrux-0.3.0/pycrux/utils/config.py` & `pycrux-0.4.0/pycrux/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.3.0/pycrux/utils/logger.py` & `pycrux-0.4.0/pycrux/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.3.0/pyproject.toml` & `pycrux-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycrux"
-version = "0.3.0"
+version = "0.4.0"
 description = "A python wrapper for crFitTool."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 homepage = "https://github.com/WahooFitness/pycrux"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pandas = "^2.0.2"
```

### Comparing `pycrux-0.3.0/PKG-INFO` & `pycrux-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrux
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python wrapper for crFitTool.
 Home-page: https://github.com/WahooFitness/pycrux
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

