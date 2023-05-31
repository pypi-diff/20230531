# Comparing `tmp/kaparoo_python_package-0.2.0.tar.gz` & `tmp/kaparoo_python_package-0.2.1.tar.gz`

## Comparing `kaparoo_python_package-0.2.0.tar` & `kaparoo_python_package-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/py.typed
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/exceptions.py
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/path.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/filesystem/types.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/utils/__init__.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/utils/optional.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/kaparoo/utils/singleton.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/LICENSE
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/README.md
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/py.typed
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/exceptions.py
+-rw-r--r--   0        0        0    21066 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/path.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/filesystem/types.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/utils/__init__.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/utils/optional.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/kaparoo/utils/singleton.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/README.md
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 kaparoo_python_package-0.2.1/PKG-INFO
```

### Comparing `kaparoo_python_package-0.2.0/kaparoo/filesystem/__init__.py` & `kaparoo_python_package-0.2.1/kaparoo/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.0/kaparoo/filesystem/path.py` & `kaparoo_python_package-0.2.1/kaparoo/filesystem/path.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 from kaparoo.filesystem.exceptions import DirectoryNotFoundError, NotAFileError
 
 if TYPE_CHECKING:
     from kaparoo.filesystem.types import StrPath
 
 
 def stringify_path(path: StrPath) -> str:
+    """Convert a path to a string representation."""
     return os.fspath(path)
 
 
 def stringify_paths(paths: Sequence[StrPath]) -> Sequence[str]:
+    """Convert a sequence of paths to a sequence of string representations."""
     return [stringify_path(p) for p in paths]
 
 
 @overload
 def check_if_path_exists(path: StrPath, *, stringify: Literal[False] = False) -> Path:
     ...
 
@@ -48,23 +50,22 @@
 
 @overload
 def check_if_path_exists(path: StrPath, *, stringify: bool) -> Path | str:
     ...
 
 
 def check_if_path_exists(path: StrPath, *, stringify: bool = False) -> Path | str:
-    """Check if a given path exists and return it as a Path object.
+    """Check if a given path exists and return it as a `Path` object.
 
     Args:
-        path (StrPath): The path to check for existence.
-        stringify (bool, optional): Whether to return the path as a string instead of a
-            Path object. Defaults to False.
+        path: The path to check for existence.
+        stringify: Whether to return the path as a string. Defaults to `False`.
 
     Returns:
-        The path as a Path object or a string, depending on the value of `stringify`.
+        The path as a `Path` object or a string, depending on the value of `stringify`.
 
     Raises:
         FileNotFoundError: If the path does not exist.
     """
 
     if not (path := Path(path)).exists():
         raise FileNotFoundError(f"no such path: {path}")
@@ -95,30 +96,29 @@
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_paths_exist(
     paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool = False
 ) -> Sequence[Path] | Sequence[str]:
-    """Check if multiple paths exist.
+    """Check if multiple paths exist and return them as a sequence of `Path` objects.
 
     Args:
-        paths (Sequence[StrPath]): A sequence of paths to check for existence.
-        root (StrPath|None, optional): The root directory to resolve relative paths.
-            If provided, the `paths` will be resolved relative to the `root` directory.
-            Defaults to None.
-        stringify (bool, optional): Whether to return a sequence of strings instead of
-            a sequence of Path objects. Defaults to False.
+        paths: A sequence of paths to check for existence.
+        root: The root directory to resolve relative paths. If provided, the `paths`
+            will be resolved relative to the `root` directory. Defaults to `None`.
+        stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
-        The paths that exist as a sequence of Path objects or a sequence of strings,
+        The paths as a sequence of `Path` objects or a sequence of strings,
             depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If the `root` directory does not exist.
+        NotADirectoryError: If `root` exists but is not a directory.
         FileNotFoundError: If any of the paths does not exist.
     """
 
     if root is not None:
         root = check_if_dir_exists(root)
         paths = [root / p for p in paths]
 
@@ -139,23 +139,22 @@
 
 @overload
 def check_if_file_exists(path: StrPath, *, stringify: bool) -> Path | str:
     ...
 
 
 def check_if_file_exists(path: StrPath, *, stringify: bool = False) -> Path | str:
-    """Check if a given path exists and is a file, and return it as a Path object.
+    """Check if a given path exists and is a file, and return it as a `Path` object.
 
     Args:
-        path (StrPath): The file path to check for existence.
-        stringify (bool, optional): Whether to return the path as a string instead of a
-            Path object. Defaults to False.
+        path: The file path to check for existence.
+        stringify: Whether to return the path as a string. Defaults to `False`.
 
     Returns:
-        The path as a Path object or a string, depending on the value of `stringify`.
+        The path as a `Path` object or a string, depending on the value of `stringify`.
 
     Raises:
         FileNotFoundError: If the path does not exist.
         NotAFileError: If the path exists but is not a file.
     """
 
     if not (path := Path(path)).exists():
@@ -189,30 +188,29 @@
 ) -> Sequence[Path] | Sequence[str]:
     ...
 
 
 def check_if_files_exist(
     paths: Sequence[StrPath], *, root: StrPath | None = None, stringify: bool = False
 ) -> Sequence[Path] | Sequence[str]:
-    """Check if multiple files exist.
+    """Check if multiple files exist and return them as a sequence of `Path` objects.
 
     Args:
-        paths (Sequence[StrPath]): A sequence of file paths to check for existence.
-        root (StrPath|None, optional): The root directory to resolve relative paths.
-            If provided, the `paths` will be resolved relative to the `root` directory.
-            Defaults to None.
-        stringify (bool, optional): Whether to return a sequence of strings instead of
-            a sequence of Path objects. Defaults to False.
+        paths: A sequence of file paths to check for existence.
+        root: The root directory to resolve relative paths. If provided, the `paths`
+            will be resolved relative to the `root` directory. Defaults to `None`.
+        stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
-        The file paths as a sequence of Path objects or a sequence of strings,
+        The file paths as a sequence of `Path` objects or a sequence of strings,
             depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If the `root` directory does not exist.
+        NotADirectoryError: If `root` exists but is not a directory.
         FileNotFoundError: If any of the file paths does not exist.
         NotAFileError: If any of the paths exists but is not a file.
     """  # noqa: E501
 
     if root is not None:
         root = check_if_dir_exists(root)
         paths = [root / p for p in paths]
@@ -242,32 +240,29 @@
 ) -> Path | str:
     ...
 
 
 def check_if_dir_exists(
     path: StrPath, *, make: bool | int = False, stringify: bool = False
 ) -> Path | str:
-    """Check if a given path exists and is a directory, and return it as a Path object.
+    """Check if a given path exists and is a directory, and return it as a `Path` object.
 
     Args:
-        path (StrPath): The directory path to check for existence.
-        make (bool|int, optional): Whether to create the directory if it does not exist.
-            If an int is provided, use it as the octal mode for the directory.
-            Defaults to False.
-        stringify (bool, optional): Whether to return the path as a string instead of a
-            Path object. Defaults to False.
+        path: The directory path to check for existence.
+        make: Whether to create the directory if it does not exist. If an `int` is provided,
+            use it as the octal mode for the directory. Defaults to `False`.
+        stringify: Whether to return the path as a string. Defaults to `False`.
 
     Returns:
-        The path as a Path object or a string, depending on the value of `stringify`.
+        The path as a `Path` object or a string, depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If the path does not exist and `make` is False.
-            Note that `DirectoryNotFoundError` inherits from `FileNotFoundError`.
         NotADirectoryError: If the path exists but is not a directory.
-    """
+    """  # noqa: E501
 
     if not (path := Path(path)).exists():
         if make is False:
             raise DirectoryNotFoundError(f"no such directory: {path}")
         path.mkdir(mode=511 if make is True else make, parents=True)  # 511 == 0o777
     elif not path.is_dir():
         raise NotADirectoryError(f"not a directory: {path}")
@@ -311,39 +306,37 @@
 def check_if_dirs_exist(
     paths: Sequence[StrPath],
     *,
     root: StrPath | None = None,
     make: bool | int = False,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
-    """Check if multiple directories exist.
+    """Check if multiple directories exist and return them as a sequence of `Path` objects.
 
     Args:
-        paths (Sequence[StrPath]): A sequence of directory paths to check for existence.
-        root (StrPath|None, optional): The root directory to resolve relative paths.
-            If provided, the `paths` will be resolved relative to the `root` directory.
-            Defaults to None.
-        make (bool|int, optional): Whether to create the directory if it does not exist.
-            If an int is provided, use it as the octal mode for the directory.
-            Defaults to False.
-        stringify (bool, optional): Whether to return a sequence of strings instead of
-            a sequence of Path objects. Defaults to False.
+        paths: A sequence of directory paths to check for existence.
+        root: The root directory to resolve relative paths. If provided, the `paths`
+            will be resolved relative to the `root` directory. Defaults to `None`.
+        make: Whether to create the directory if it does not exist. If an `int` is provided,
+            use it as the octal mode for the directory. Defaults to `False`.
+        stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
-        The directory paths as a sequence of Path objects or a sequence of strings,
+        The directory paths as a sequence of `Path` objects or a sequence of strings,
             depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If the `root` directory does not exist
         DirectoryNotFoundError: If any of the directory paths does not exist.
+        NotADirectoryError: If `root` exists but is not a directory.
         NotADirectoryError: If any of the paths exists but is not a directory.
-    """
+    """  # noqa: E501
 
     if root is not None:
-        root = check_if_dir_exists(root, make=make)
+        root = check_if_dir_exists(root)
         paths = [root / p for p in paths]
 
     paths = [check_if_dir_exists(p, make=make) for p in paths]
 
     return stringify_paths(paths) if stringify else paths
 
 
@@ -398,33 +391,32 @@
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files or directories in a given directory.
 
     Args:
-        root (StrPath): The directory to search for paths.
-        pattern (str, optional): A glob pattern to match the paths against. Defaults to
-            None and automatically uses "*" to list all paths included in the `root`.
-        num_samples (int, optional): A maximum number of paths to return. If given and
-            its value is smaller than the total number of paths, only the `num_samples`
-            paths of the total are randomly selected and returned. Hence, even using the
-            same `num_samples`, may return a different result. Defaults to None.
-        ignores (Sequence[StrPath], optional): A sequence of paths to ignore. If any path
-            in `ignores` does not start with `root`, it is treated as a relative path.
-            For example, `any/path` is treated as `root/any/path`. Defaults to None.
-        condition (Callable[[Path], bool], optional): A predicate that takes a Path object
-            and decides whether to include the path in the results. Defaults to None.
-        recursive (bool, optional): Whether to search for paths recursively in
-            subdirectories of the `root` directory. Defaults to True.
-        stringify (bool, optional): Whether to return a sequence of strings instead of a
-            sequence of Path objects. Defaults to False.
+        root: The directory to search for paths.
+        pattern: A glob pattern to match the paths against. Defaults to `None` and
+            automatically uses "*" to list all paths included in the `root` directory.
+        num_samples: A maximum number of paths to return. If given and its value is
+            smaller than the total number of paths, only the `num_samples` paths of the
+            total are randomly selected and returned. Hence, even using the same value
+            of `num_samples`, may return a different result. Defaults to `None`.
+        ignores: A sequence of paths to ignore. If any path in `ignores` does not start
+            with `root`, it is treated as a relative path. For example, `any/path` is
+            treated as `root/any/path`. Defaults to `None`.
+        condition: A predicate that takes a `Path` object and decides whether to include
+            the path in the results. Defaults to `None`.
+        recursive: Whether to search for paths recursively in subdirectories of the
+            `root` directory. Defaults to `True`.
+        stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
-        The paths that match the specified criteria as a sequence of Path objects or a
+        The paths that match the specified criteria as a sequence of `Path` objects or a
             sequence of strings, depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If `root` does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
         ValueError: If `num_samples` is not a positive int.
     """  # noqa: E501
@@ -513,39 +505,37 @@
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of files in a given directory.
 
     Args:
-        root (StrPath): The directory to search for paths.
-        pattern (str, optional): A glob pattern to match the paths against. Defaults to
-            None and automatically uses "*" to list all paths included in the `root`.
-        num_samples (int, optional): A maximum number of paths to return. If given and
-            its value is smaller than the total number of paths, only the `num_samples`
-            paths of the total are randomly selected and returned. Hence, even using the
-            same `num_samples`, may return a different result. Defaults to None.
-        ignores (Sequence[StrPath], optional): A sequence of paths to ignore. If any path
-            in `ignores` does not start with `root`, it is treated as a relative path.
-            For example, `any/path` is treated as `root/any/path`. Defaults to None.
-        condition (Callable[[Path], bool], optional): A predicate that takes a Path object
-            and decides whether to include the path in the results. Defaults to None.
-        recursive (bool, optional): Whether to search for paths recursively in
-            subdirectories of the `root` directory. Defaults to True.
-        stringify (bool, optional): Whether to return a sequence of strings instead of a
-            sequence of Path objects. Defaults to False.
+        root: The directory to search for paths.
+        pattern: A glob pattern to match the paths against. Defaults to `None` and
+            automatically uses "*" to list all paths included in the `root` directory.
+        num_samples: A maximum number of paths to return. If given and its value is
+            smaller than the total number of paths, only the `num_samples` paths of the
+            total are randomly selected and returned. Hence, even using the same value
+            of `num_samples`, may return a different result. Defaults to `None`.
+        ignores: A sequence of paths to ignore. If any path in `ignores` does not start
+            with `root`, it is treated as a relative path. For example, `any/path` is
+            treated as `root/any/path`. Defaults to `None`.
+        condition: A predicate that takes a `Path` object and decides whether to include
+            the path in the results. Defaults to `None`.
+        recursive: Whether to search for paths recursively in subdirectories of the
+            `root` directory. Defaults to `True`.
+        stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
-        The file paths that match the specified criteria as a sequence of Path objects
+        The file paths that match the specified criteria as a sequence of `Path` objects
             or a sequence of strings, depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If `root` does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
-        FileNotFoundError: If no paths match the specified `pattern`.
         ValueError: If `num_samples` is not a positive int.
     """  # noqa: E501
 
     if not callable(condition):
         file_condition = lambda p: p.is_file()  # noqa: E731
     else:
         file_condition = lambda p: p.is_file() and condition(p)  # type: ignore[misc] # noqa: E501, E731
@@ -614,39 +604,37 @@
     condition: Callable[[Path], bool] | None = None,
     recursive: bool = True,
     stringify: bool = False,
 ) -> Sequence[Path] | Sequence[str]:
     """Get paths of directories in a given directory.
 
     Args:
-        root (StrPath): The directory to search for paths.
-        pattern (str, optional): A glob pattern to match the paths against. Defaults to
-            None and automatically uses "*" to list all paths included in the `root`.
-        num_samples (int, optional): A maximum number of paths to return. If given and
-            its value is smaller than the total number of paths, only the `num_samples`
-            paths of the total are randomly selected and returned. Hence, even using the
-            same `num_samples`, may return a different result. Defaults to None.
-        ignores (Sequence[StrPath], optional): A sequence of paths to ignore. If any path
-            in `ignores` does not start with `root`, it is treated as a relative path.
-            For example, `any/path` is treated as `root/any/path`. Defaults to None.
-        condition (Callable[[Path], bool], optional): A predicate that takes a Path object
-            and decides whether to include the path in the results. Defaults to None.
-        recursive (bool, optional): Whether to search for paths recursively in
-            subdirectories of the `root` directory. Defaults to True.
-        stringify (bool, optional): Whether to return a sequence of strings instead of a
-            sequence of Path objects. Defaults to False.
+        root: The directory to search for paths.
+        pattern: A glob pattern to match the paths against. Defaults to `None` and
+            automatically uses "*" to list all paths included in the `root` directory.
+        num_samples: A maximum number of paths to return. If given and its value is
+            smaller than the total number of paths, only the `num_samples` paths of the
+            total are randomly selected and returned. Hence, even using the same value
+            of `num_samples`, may return a different result. Defaults to `None`.
+        ignores: A sequence of paths to ignore. If any path in `ignores` does not start
+            with `root`, it is treated as a relative path. For example, `any/path` is
+            treated as `root/any/path`. Defaults to `None`.
+        condition: A predicate that takes a `Path` object and decides whether to include
+            the path in the results. Defaults to `None`.
+        recursive: Whether to search for paths recursively in subdirectories of the
+            `root` directory. Defaults to `True`.
+        stringify: Whether to return a sequence of strings. Defaults to `False`.
 
     Returns:
-        The directory paths that match the specified criteria as a sequence of Path objects
-            or a sequence of strings, depending on the value of `stringify`.
+        The directory paths that match the specified criteria as a sequence of `Path`
+            objects or a sequence of strings, depending on the value of `stringify`.
 
     Raises:
         DirectoryNotFoundError: If `root` does not exist.
         NotADirectoryError: If `root` exists but is not a directory.
-        FileNotFoundError: If no paths match the specified `pattern`.
         ValueError: If `num_samples` is not a positive int.
     """  # noqa: E501
 
     if not callable(condition):
         dir_condition = lambda p: p.is_dir()  # noqa: E731
     else:
         dir_condition = lambda p: p.is_dir() and condition(p)  # type: ignore[misc] # noqa: E501, E731
```

### Comparing `kaparoo_python_package-0.2.0/kaparoo/utils/optional.py` & `kaparoo_python_package-0.2.1/kaparoo/utils/optional.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 
 
 def unwrap_or_default(
     optional: T | None,
     default: T,
     callback: Callable[[T], T] | None = None,
 ) -> T:
-    """Unwraps an optional value or returns a default value.
+    """Unwrap an optional value or returns a default value.
 
     If the `optional` value is not `None`, it is returned. Otherwise, the `default`
     value is returned. Optionally, a `callback` function can be provided to transform
     the resulting value.
 
     Args:
         optional: The optional value to unwrap.
         default: The default value to return if `optional` is `None`.
         callback: A function to transform the resulting value. Defaults to None.
 
     Returns:
         The unwrapped value or the default value.
-
     """
+
     if optional is not None:
         result = optional
     else:
         result = default
 
     if callable(callback):
         result = callback(result)
@@ -40,28 +40,29 @@
 
 
 def unwrap_or_factory(
     optional: T | None,
     factory: Callable[[], T],
     callback: Callable[[T], T] | None = None,
 ) -> T:
-    """Unwraps an optional value or returns a value created by a factory function.
+    """Unwrap an optional value or returns a value created by a factory function.
 
     If the `optional` value is not `None`, it is returned. Otherwise, a value is created
     by calling the `factory` function. Optionally, a `callback` function can be provided
     to transform the resulting value.
 
     Args:
         optional: The optional value to unwrap.
         factory: A factory function to create a value if `optional` is `None`.
         callback: A function to transform the resulting value. Defaults to None.
 
     Returns:
        The unwrapped value or the value created by the factory function.
     """
+
     if optional is not None:
         result = optional
     else:
         result = factory()
 
     if callable(callback):
         result = callback(result)
```

### Comparing `kaparoo_python_package-0.2.0/kaparoo/utils/singleton.py` & `kaparoo_python_package-0.2.1/kaparoo/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.0/.gitignore` & `kaparoo_python_package-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.0/LICENSE` & `kaparoo_python_package-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.0/README.md` & `kaparoo_python_package-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.0/pyproject.toml` & `kaparoo_python_package-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaparoo_python_package-0.2.0/PKG-INFO` & `kaparoo_python_package-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaparoo-python-package
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package for (personally) common and useful features.
 Project-URL: GitHub, https://www.github.com/kaparoo/python-package
 Author-email: Jaewoo Park <kaparoo2001@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jaewoo Park
```

