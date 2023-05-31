# Comparing `tmp/kaparoo_python_package-0.1.0.tar.gz` & `tmp/kaparoo_python_package-0.2.0.tar.gz`

## Comparing `kaparoo_python_package-0.1.0.tar` & `kaparoo_python_package-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/py.typed
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/filesystem/path.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/utils/optional.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/kaparoo/utils/singleton.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/LICENSE
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/README.md
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/py.typed
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/path.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/utils/singleton.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/README.md
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/PKG-INFO
```

### Comparing `kaparoo_python_package-0.1.0/kaparoo/filesystem/__init__.py` & `kaparoo_python_package-0.2.0/kaparoo/filesystem/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # -*- coding: utf-8 -*-
 
 __all__ = (
     # exceptions
     "NotAFileError",
     "DirectoryNotFoundError",
     # path utils
+    "stringify_path",
+    "stringify_paths",
     "check_if_path_exists",
+    "check_if_paths_exist",
     "check_if_file_exists",
+    "check_if_files_exist",
     "check_if_dir_exists",
+    "check_if_dirs_exist",
     "get_paths",
     "get_file_paths",
     "get_dir_paths",
     # type aliases
     "StrPath",
 )
 
 from kaparoo.filesystem.exceptions import DirectoryNotFoundError, NotAFileError
 from kaparoo.filesystem.path import (
     check_if_dir_exists,
+    check_if_dirs_exist,
     check_if_file_exists,
+    check_if_files_exist,
     check_if_path_exists,
+    check_if_paths_exist,
     get_dir_paths,
     get_file_paths,
     get_paths,
+    stringify_path,
+    stringify_paths,
 )
 from kaparoo.filesystem.types import StrPath
```

### Comparing `kaparoo_python_package-0.1.0/kaparoo/filesystem/path.py` & `kaparoo_python_package-0.2.0/kaparoo/filesystem/path.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 __all__ = (
+    "stringify_path",
+    "stringify_paths",
     "check_if_path_exists",
+    "check_if_paths_exist",
     "check_if_file_exists",
+    "check_if_files_exist",
     "check_if_dir_exists",
+    "check_if_dirs_exist",
     "get_paths",
     "get_file_paths",
     "get_dir_paths",
 )
 
+import os
 import random
 from collections.abc import Callable, Sequence
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal, overload
 
 from kaparoo.filesystem.exceptions import DirectoryNotFoundError, NotAFileError
 
 if TYPE_CHECKING:
     from kaparoo.filesystem.types import StrPath
 
 
+def stringify_path(path: StrPath) -> str:
+    return os.fspath(path)
+
+
+def stringify_paths(paths: Sequence[StrPath]) -> Sequence[str]:
+    return [stringify_path(p) for p in paths]
+
+
 @overload
 def check_if_path_exists(path: StrPath, *, stringify: Literal[False] = False) -> Path:
     ...
 
 
 @overload
 def check_if_path_exists(path: StrPath, *, stringify: Literal[True]) -> str:
@@ -51,15 +65,70 @@
     Raises:
         FileNotFoundError: If the path does not exist.
     """
 
     if not (path := Path(path)).exists():
         raise FileNotFoundError(f"no such path: {path}")
 
-    return str(path) if stringify else path
+    return stringify_path(path) if stringify else path
+
+
+@overload
+def check_if_paths_exist(
+    paths: Sequence[StrPath],
+    *,
+    root: StrPath | None = None,
+    stringify: Literal[False] = False,
+) -> Sequence[Path]:
+    ...
+
+
+@overload
+def check_if_paths_exist(
+    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: Literal[True]
+) -> Sequence[str]:
+    ...
+
+
+@overload
+def check_if_paths_exist(
+    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool
+) -> Sequence[Path] | Sequence[str]:
+    ...
+
+
+def check_if_paths_exist(
+    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool = False
+) -> Sequence[Path] | Sequence[str]:
+    """Check if multiple paths exist.
+
+    Args:
+        paths (Sequence[StrPath]): A sequence of paths to check for existence.
+        root (StrPath|None, optional): The root directory to resolve relative paths.
+            If provided, the `paths` will be resolved relative to the `root` directory.
+            Defaults to None.
+        stringify (bool, optional): Whether to return a sequence of strings instead of
+            a sequence of Path objects. Defaults to False.
+
+    Returns:
+        The paths that exist as a sequence of Path objects or a sequence of strings,
+            depending on the value of `stringify`.
+
+    Raises:
+        DirectoryNotFoundError: If the `root` directory does not exist.
+        FileNotFoundError: If any of the paths does not exist.
+    """
+
+    if root is not None:
+        root = check_if_dir_exists(root)
+        paths = [root / p for p in paths]
+
+    paths = [check_if_path_exists(p) for p in paths]
+
+    return stringify_paths(paths) if stringify else paths
 
 
 @overload
 def check_if_file_exists(path: StrPath, *, stringify: Literal[False] = False) -> Path:
     ...
 
 
@@ -90,29 +159,91 @@
     """
 
     if not (path := Path(path)).exists():
         raise FileNotFoundError(f"no such file: {path}")
     elif not path.is_file():
         raise NotAFileError(f"not a file: {path}")
 
-    return str(path) if stringify else path
+    return stringify_path(path) if stringify else path
+
+
+@overload
+def check_if_files_exist(
+    paths: Sequence[StrPath],
+    *,
+    root: StrPath | None = None,
+    stringify: Literal[False] = False,
+) -> Sequence[Path]:
+    ...
+
+
+@overload
+def check_if_files_exist(
+    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: Literal[True]
+) -> Sequence[str]:
+    ...
+
+
+@overload
+def check_if_files_exist(
+    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool
+) -> Sequence[Path] | Sequence[str]:
+    ...
+
+
+def check_if_files_exist(
+    paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool = False
+) -> Sequence[Path] | Sequence[str]:
+    """Check if multiple files exist.
+
+    Args:
+        paths (Sequence[StrPath]): A sequence of file paths to check for existence.
+        root (StrPath|None, optional): The root directory to resolve relative paths.
+            If provided, the `paths` will be resolved relative to the `root` directory.
+            Defaults to None.
+        stringify (bool, optional): Whether to return a sequence of strings instead of
+            a sequence of Path objects. Defaults to False.
+
+    Returns:
+        The file paths as a sequence of Path objects or a sequence of strings,
+            depending on the value of `stringify`.
+
+    Raises:
+        DirectoryNotFoundError: If the `root` directory does not exist.
+        FileNotFoundError: If any of the file paths does not exist.
+        NotAFileError: If any of the paths exists but is not a file.
+    """  # noqa: E501
+
+    if root is not None:
+        root = check_if_dir_exists(root)
+        paths = [root / p for p in paths]
+
+    paths = [check_if_file_exists(p) for p in paths]
+
+    return stringify_paths(paths) if stringify else paths
 
 
 @overload
-def check_if_dir_exists(path: StrPath, *, stringify: Literal[False] = False) -> Path:
+def check_if_dir_exists(
+    path: StrPath, *, make: bool | int = False, stringify: Literal[False] = False
+) -> Path:
     ...
 
 
 @overload
-def check_if_dir_exists(path: StrPath, *, stringify: Literal[True]) -> str:
+def check_if_dir_exists(
+    path: StrPath, *, make: bool | int = False, stringify: Literal[True]
+) -> str:
     ...
 
 
 @overload
-def check_if_dir_exists(path: StrPath, *, stringify: bool) -> Path | str:
+def check_if_dir_exists(
+    path: StrPath, *, make: bool | int = False, stringify: bool
+) -> Path | str:
     ...
 
 
 def check_if_dir_exists(
     path: StrPath, *, make: bool | int = False, stringify: bool = False
 ) -> Path | str:
     """Check if a given path exists and is a directory, and return it as a Path object.
@@ -131,71 +262,145 @@
     Raises:
         DirectoryNotFoundError: If the path does not exist and `make` is False.
             Note that `DirectoryNotFoundError` inherits from `FileNotFoundError`.
         NotADirectoryError: If the path exists but is not a directory.
     """
 
     if not (path := Path(path)).exists():
-        if make is not False:
-            path.mkdir(parents=True)
-            if make is not True:  # `make` AS IS int
-                path.chmod(mode=make)
-        raise DirectoryNotFoundError(f"no such directory: {path}")
+        if make is False:
+            raise DirectoryNotFoundError(f"no such directory: {path}")
+        path.mkdir(mode=511 if make is True else make, parents=True)  # 511 == 0o777
     elif not path.is_dir():
         raise NotADirectoryError(f"not a directory: {path}")
 
-    return str(path) if stringify else path
+    return stringify_path(path) if stringify else path
+
+
+@overload
+def check_if_dirs_exist(
+    paths: Sequence[StrPath],
+    *,
+    root: StrPath | None = None,
+    make: bool | int = False,
+    stringify: Literal[False] = False,
+) -> Sequence[Path]:
+    ...
+
+
+@overload
+def check_if_dirs_exist(
+    paths: Sequence[StrPath],
+    *,
+    root: StrPath | None = None,
+    make: bool | int = False,
+    stringify: Literal[True],
+) -> Sequence[str]:
+    ...
+
+
+@overload
+def check_if_dirs_exist(
+    paths: Sequence[StrPath],
+    *,
+    root: StrPath | None = None,
+    make: bool | int = False,
+    stringify: bool,
+) -> Sequence[Path] | Sequence[str]:
+    ...
+
+
+def check_if_dirs_exist(
+    paths: Sequence[StrPath],
+    *,
+    root: StrPath | None = None,
+    make: bool | int = False,
+    stringify: bool = False,
+) -> Sequence[Path] | Sequence[str]:
+    """Check if multiple directories exist.
+
+    Args:
+        paths (Sequence[StrPath]): A sequence of directory paths to check for existence.
+        root (StrPath|None, optional): The root directory to resolve relative paths.
+            If provided, the `paths` will be resolved relative to the `root` directory.
+            Defaults to None.
+        make (bool|int, optional): Whether to create the directory if it does not exist.
+            If an int is provided, use it as the octal mode for the directory.
+            Defaults to False.
+        stringify (bool, optional): Whether to return a sequence of strings instead of
+            a sequence of Path objects. Defaults to False.
+
+    Returns:
+        The directory paths as a sequence of Path objects or a sequence of strings,
+            depending on the value of `stringify`.
+
+    Raises:
+        DirectoryNotFoundError: If the `root` directory does not exist
+        DirectoryNotFoundError: If any of the directory paths does not exist.
+        NotADirectoryError: If any of the paths exists but is not a directory.
+    """
+
+    if root is not None:
+        root = check_if_dir_exists(root, make=make)
+        paths = [root / p for p in paths]
+
+    paths = [check_if_dir_exists(p, make=make) for p in paths]
+
+    return stringify_paths(paths) if stringify else paths
 
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def get_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files or directories in a given directory.
 
     Args:
         root (StrPath): The directory to search for paths.
         pattern (str, optional): A glob pattern to match the paths against. Defaults to
@@ -205,106 +410,112 @@
             paths of the total are randomly selected and returned. Hence, even using the
             same `num_samples`, may return a different result. Defaults to None.
         ignores (Sequence[StrPath], optional): A sequence of paths to ignore. If any path
             in `ignores` does not start with `root`, it is treated as a relative path.
             For example, `any/path` is treated as `root/any/path`. Defaults to None.
         condition (Callable[[Path], bool], optional): A predicate that takes a Path object
             and decides whether to include the path in the results. Defaults to None.
+        recursive (bool, optional): Whether to search for paths recursively in
+            subdirectories of the `root` directory. Defaults to True.
         stringify (bool, optional): Whether to return a sequence of strings instead of a
             sequence of Path objects. Defaults to False.
 
     Returns:
         The paths that match the specified criteria as a sequence of Path objects or a
             sequence of strings, depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If `root` does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
-        FileNotFoundError: If no paths match the specified `pattern`.
         ValueError: If `num_samples` is not a positive int.
     """  # noqa: E501
 
     root = check_if_dir_exists(root)
 
     if not isinstance(pattern, str):
         pattern = "*"
 
-    paths = [p for p in root.glob(pattern)]
-
-    if callable(condition):
-        paths = [p for p in paths if condition(p)]
+    matched = root.rglob(pattern) if recursive else root.glob(pattern)
+    paths = [p for p in matched]
 
-    if not paths:
-        raise FileNotFoundError(f'no path matches "{pattern}" at {root}')
+    if root in paths:
+        paths.remove(root)
 
     if not ignores:
         ignores = []
 
     for ignore in ignores:
         ignore_path = Path(ignore)
         if root not in ignore_path.parents:
             ignore_path = root / ignore_path
 
         if ignore_path in paths:
             paths.remove(ignore_path)
 
+    if callable(condition):
+        paths = [p for p in paths if condition(p)]
+
     if isinstance(num_samples, int) and num_samples < len(paths):
         if num_samples <= 0:
             raise ValueError("`num_samples` must be a positive int")
         paths = random.sample(paths, num_samples)
 
-    return [str(p) for p in paths] if stringify else paths
+    return stringify_paths(paths) if stringify else paths
 
 
 @overload
 def get_file_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def get_file_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def get_file_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def get_file_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files in a given directory.
 
     Args:
         root (StrPath): The directory to search for paths.
         pattern (str, optional): A glob pattern to match the paths against. Defaults to
@@ -314,20 +525,22 @@
             paths of the total are randomly selected and returned. Hence, even using the
             same `num_samples`, may return a different result. Defaults to None.
         ignores (Sequence[StrPath], optional): A sequence of paths to ignore. If any path
             in `ignores` does not start with `root`, it is treated as a relative path.
             For example, `any/path` is treated as `root/any/path`. Defaults to None.
         condition (Callable[[Path], bool], optional): A predicate that takes a Path object
             and decides whether to include the path in the results. Defaults to None.
+        recursive (bool, optional): Whether to search for paths recursively in
+            subdirectories of the `root` directory. Defaults to True.
         stringify (bool, optional): Whether to return a sequence of strings instead of a
             sequence of Path objects. Defaults to False.
 
     Returns:
-        The paths that match the specified criteria as a sequence of Path objects or a
-            sequence of strings, depending on the value of `stringify`.
+        The file paths that match the specified criteria as a sequence of Path objects
+            or a sequence of strings, depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If `root` does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
         FileNotFoundError: If no paths match the specified `pattern`.
         ValueError: If `num_samples` is not a positive int.
     """  # noqa: E501
@@ -339,66 +552,71 @@
 
     file_paths = get_paths(
         root,
         pattern=pattern,
         num_samples=num_samples,
         ignores=ignores,
         condition=file_condition,
+        recursive=recursive,
         stringify=stringify,
     )
 
     return file_paths
 
 
 @overload
 def get_dir_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: Literal[False] = False,
 ) -> Sequence[Path]:
     ...
 
 
 @overload
 def get_dir_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: Literal[True],
 ) -> Sequence[str]:
     ...
 
 
 @overload
 def get_dir_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: bool,
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def get_dir_paths(
     root: StrPath,
     *,
     pattern: str | None = None,
     num_samples: int | None = None,
     ignores: Sequence[StrPath] | None = None,
     condition: Callable[[Path], bool] | None = None,
+    recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of directories in a given directory.
 
     Args:
         root (StrPath): The directory to search for paths.
         pattern (str, optional): A glob pattern to match the paths against. Defaults to
@@ -408,20 +626,22 @@
             paths of the total are randomly selected and returned. Hence, even using the
             same `num_samples`, may return a different result. Defaults to None.
         ignores (Sequence[StrPath], optional): A sequence of paths to ignore. If any path
             in `ignores` does not start with `root`, it is treated as a relative path.
             For example, `any/path` is treated as `root/any/path`. Defaults to None.
         condition (Callable[[Path], bool], optional): A predicate that takes a Path object
             and decides whether to include the path in the results. Defaults to None.
+        recursive (bool, optional): Whether to search for paths recursively in
+            subdirectories of the `root` directory. Defaults to True.
         stringify (bool, optional): Whether to return a sequence of strings instead of a
             sequence of Path objects. Defaults to False.
 
     Returns:
-        The paths that match the specified criteria as a sequence of Path objects or a
-            sequence of strings, depending on the value of `stringify`.
+        The directory paths that match the specified criteria as a sequence of Path objects
+            or a sequence of strings, depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If `root` does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
         FileNotFoundError: If no paths match the specified `pattern`.
         ValueError: If `num_samples` is not a positive int.
     """  # noqa: E501
@@ -433,11 +653,12 @@
 
     dir_paths = get_paths(
         root,
         pattern=pattern,
         num_samples=num_samples,
         ignores=ignores,
         condition=dir_condition,
+        recursive=recursive,
         stringify=stringify,
     )
 
     return dir_paths
```

### Comparing `kaparoo_python_package-0.1.0/kaparoo/utils/singleton.py` & `kaparoo_python_package-0.2.0/kaparoo/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.1.0/.gitignore` & `kaparoo_python_package-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.1.0/LICENSE` & `kaparoo_python_package-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.1.0/README.md` & `kaparoo_python_package-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.1.0/pyproject.toml` & `kaparoo_python_package-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.1.0/PKG-INFO` & `kaparoo_python_package-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python-package
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

