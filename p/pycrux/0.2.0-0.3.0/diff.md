# Comparing `tmp/pycrux-0.2.0.tar.gz` & `tmp/pycrux-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrux-0.2.0.tar", max compression
+gzip compressed data, was "pycrux-0.3.0.tar", max compression
```

## Comparing `pycrux-0.2.0.tar` & `pycrux-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-05-30 13:54:53.299492 pycrux-0.2.0/LICENSE
--rw-r--r--   0        0        0       85 2023-05-30 20:24:52.720158 pycrux-0.2.0/pycrux/__init__.py
--rw-r--r--   0        0        0     3494 2023-05-31 10:55:02.634701 pycrux-0.2.0/pycrux/crux.py
--rw-r--r--   0        0        0        0 2023-05-30 13:54:53.314684 pycrux-0.2.0/pycrux/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-30 13:54:53.314102 pycrux-0.2.0/pycrux/utils/config.py
--rw-r--r--   0        0        0      731 2023-05-30 14:16:53.108904 pycrux-0.2.0/pycrux/utils/logger.py
--rw-r--r--   0        0        0      925 2023-05-31 11:12:08.018004 pycrux-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 pycrux-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-30 13:54:53.299492 pycrux-0.3.0/LICENSE
+-rw-r--r--   0        0        0       85 2023-05-30 20:24:52.720158 pycrux-0.3.0/pycrux/__init__.py
+-rw-r--r--   0        0        0     4154 2023-05-31 11:44:53.776004 pycrux-0.3.0/pycrux/crux.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:54:53.314684 pycrux-0.3.0/pycrux/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-30 13:54:53.314102 pycrux-0.3.0/pycrux/utils/config.py
+-rw-r--r--   0        0        0      731 2023-05-30 14:16:53.108904 pycrux-0.3.0/pycrux/utils/logger.py
+-rw-r--r--   0        0        0      959 2023-05-31 11:50:04.340155 pycrux-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 pycrux-0.3.0/PKG-INFO
```

### Comparing `pycrux-0.2.0/LICENSE` & `pycrux-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrux-0.2.0/pycrux/crux.py` & `pycrux-0.3.0/pycrux/crux.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,28 @@
     def read_fit(
         self, fit_file, to_log: bool = False, ending: str = ".records.csv"
     ) -> pd.DataFrame:
         """Return the records for a given .fit file."""
         self.crfittool(fit_file=fit_file, to_log=to_log)
         return pd.read_csv(fit_file + ending)
 
+    def read_fit_recursively(
+        self, root: str, to_log: bool = True, ending: str = ".records.csv"
+    ) -> dict[str, pd.DataFrame]:
+        """Runs read_fit on all .fit files found recursively inside the root folder."""
+        fit_files = self.get_all_files_in_folder(root)
+        dict_of_dataframes: dict[str, pd.DataFrame] = {}
+        for fit_file in fit_files:
+            try:
+                df = self.read_fit(fit_file=fit_file, to_log=to_log, ending=ending)
+                dict_of_dataframes[fit_file] = df
+            except Exception as e:
+                logger.error(f"Could not parse {fit_file}: {e}")
+        return dict_of_dataframes
+
     # TODO: Add a `safe` flag that when true does not run crux if the corresponding
     #       records exist already.
     def crfittool(self, fit_file: str, to_log: bool = False) -> CompletedProcess[str]:
         """Run crFitTool."""
         file = Path(os.path.expanduser(fit_file))
         self._raise_if_file_does_not_exist(file)
```

### Comparing `pycrux-0.2.0/pycrux/utils/config.py` & `pycrux-0.3.0/pycrux/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.2.0/pycrux/utils/logger.py` & `pycrux-0.3.0/pycrux/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pycrux-0.2.0/pyproject.toml` & `pycrux-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [tool.poetry]
 name = "pycrux"
-version = "0.2.0"
+version = "0.3.0"
 description = "A python wrapper for crFitTool."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 homepage = "https://github.com/WahooFitness/pycrux"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pandas = "^2.0.2"
+pdoc = "^13.1.1"
+rich = "^13.3.5"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 ruff = "^0.0.253"
 black = "^23.1.0"
 pyclean = "^2.2.0"
 pre-commit = "^3.1.1"
```

