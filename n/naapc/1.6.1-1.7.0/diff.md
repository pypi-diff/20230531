# Comparing `tmp/naapc-1.6.1.tar.gz` & `tmp/naapc-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naapc-1.6.1.tar", last modified: Tue May 30 00:29:29 2023, max compression
+gzip compressed data, was "naapc-1.7.0.tar", last modified: Wed May 31 11:43:33 2023, max compression
```

## Comparing `naapc-1.6.1.tar` & `naapc-1.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.258334 naapc-1.6.1/
--rwxrwxrwx   0 ei        (1000) ei        (1000)     1067 2023-05-29 12:45:29.000000 naapc-1.6.1/LICENSE
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-30 00:29:29.256334 naapc-1.6.1/PKG-INFO
--rwxrwxrwx   0 ei        (1000) ei        (1000)     4642 2023-05-29 13:32:11.000000 naapc-1.6.1/README.md
--rwxrwxrwx   0 ei        (1000) ei        (1000)     1003 2023-05-30 00:28:46.000000 naapc-1.6.1/pyproject.toml
--rwxrwxrwx   0 ei        (1000) ei        (1000)       38 2023-05-30 00:29:29.258334 naapc-1.6.1/setup.cfg
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.123611 naapc-1.6.1/src/
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.179113 naapc-1.6.1/src/naapc/
--rwxrwxrwx   0 ei        (1000) ei        (1000)      129 2023-05-30 00:28:46.000000 naapc-1.6.1/src/naapc/__init__.py
--rwxrwxrwx   0 ei        (1000) ei        (1000)     5995 2023-05-29 13:12:19.000000 naapc-1.6.1/src/naapc/nconfig.py
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6711 2023-05-30 00:28:30.000000 naapc-1.6.1/src/naapc/ndict.py
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.236334 naapc-1.6.1/src/naapc.egg-info/
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/PKG-INFO
--rwxrwxrwx   0 ei        (1000) ei        (1000)      271 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        1 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        7 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/requires.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        6 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/top_level.txt
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.245335 naapc-1.6.1/test/
--rwxrwxrwx   0 ei        (1000) ei        (1000)    16019 2023-05-29 13:20:42.000000 naapc-1.6.1/test/test.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.530043 naapc-1.7.0/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1067 2023-05-29 12:45:29.000000 naapc-1.7.0/LICENSE
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-31 11:43:31.529041 naapc-1.7.0/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     4642 2023-05-29 13:32:11.000000 naapc-1.7.0/README.md
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1003 2023-05-31 11:41:06.000000 naapc-1.7.0/pyproject.toml
+-rwxrwxrwx   0 ei        (1000) ei        (1000)       38 2023-05-31 11:43:31.530043 naapc-1.7.0/setup.cfg
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.395327 naapc-1.7.0/src/
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.453014 naapc-1.7.0/src/naapc/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      129 2023-05-31 11:41:06.000000 naapc-1.7.0/src/naapc/__init__.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     5995 2023-05-29 13:12:19.000000 naapc-1.7.0/src/naapc/nconfig.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6980 2023-05-31 11:40:32.000000 naapc-1.7.0/src/naapc/ndict.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.509041 naapc-1.7.0/src/naapc.egg-info/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      271 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        1 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        7 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/requires.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        6 2023-05-31 11:43:31.000000 naapc-1.7.0/src/naapc.egg-info/top_level.txt
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-31 11:43:31.518042 naapc-1.7.0/test/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)    16019 2023-05-29 13:20:42.000000 naapc-1.7.0/test/test.py
```

### Comparing `naapc-1.6.1/LICENSE` & `naapc-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `naapc-1.6.1/PKG-INFO` & `naapc-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.6.1
+Version: 1.7.0
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naapc-1.6.1/README.md` & `naapc-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `naapc-1.6.1/pyproject.toml` & `naapc-1.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["wheel", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naapc"
-version = "1.6.1"
+version = "1.7.0"
 description = "Nested Automated Argument Parsing Configuration (NAAPC)."
 readme = "README.md"
 authors = [{name = "Bai Huanyu", email = "eiphnix@gmail.com"}]
 license = {file = "LICENSE"}
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -19,15 +19,15 @@
 dependencies = ["pyyaml"]
 requires-python = "==3.10.*"
 
 [project.urls]
 repository = "https://github.com/eiphy/naapc"
 
 [tool.bumpver]
-current_version = "1.6.1"
+current_version = "1.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `naapc-1.6.1/src/naapc/nconfig.py` & `naapc-1.7.0/src/naapc/nconfig.py`

 * *Files identical despite different names*

### Comparing `naapc-1.6.1/src/naapc/ndict.py` & `naapc-1.7.0/src/naapc/ndict.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,17 @@
         if isinstance(dictionary, ndict):
             self._d = dictionary.raw_dict
         elif isinstance(dictionary, dict):
             self._d = dictionary
         else:
             raise TypeError(f"Unexpected type {type(dictionary)}.")
 
-        assert isinstance(delimiter, str), f"delimiter must be str, but recieved {type(delimiter)}"
+        assert isinstance(
+            delimiter, str
+        ), f"delimiter must be str, but recieved {type(delimiter)}"
         self.delimiter = delimiter
         self._update_flatten()
 
     @classmethod
     def from_flatten_dict(cls, flatten_dict: dict, delimiter=";") -> ndict:
         """Generate nested from flattened dictionary.
         The delimiter must be the same!
@@ -70,15 +72,19 @@
                 if missing_method == "ignore":
                     continue
                 elif missing_method == "false":
                     return False
                 elif missing_method == "error":
                     raise KeyError(f"Wrong path: {path}.")
 
-            if isinstance(v, str) and v.startswith("!QUERY") and not eval(v[6:].strip()):
+            if (
+                isinstance(v, str)
+                and v.startswith("!QUERY")
+                and not eval(v[6:].strip())
+            ):
                 return False
             if self[path] != v:
                 return False
         return True
 
     ### internal manipulation ###
     def _update_flatten(self) -> None:
@@ -129,36 +135,41 @@
     @property
     def flatten_dict(self):
         return deepcopy(self._flatten_dict)
 
     @property
     def flatten_dict_split(self):
         return deepcopy(
-            [ndict.from_flatten_dict({p: v}).raw_dict for p, v in self.flatten_dict.items()]
+            [
+                ndict.from_flatten_dict({p: v}).raw_dict
+                for p, v in self.flatten_dict.items()
+            ]
         )
 
     @property
     def paths(self):
         return deepcopy(self._paths)
 
     @property
     def size(self):
         return len(self._flatten_dict)
 
     ### setters & updators ###
-    def update(self, d, ignore_missing_path=False):
+    def update(self, d, ignore_missing_path=False, ignore_none=True):
         if isinstance(d, dict):
             d = ndict(d, delimiter=self.delimiter)._flatten_dict
         elif isinstance(d, ndict):
             d = d._flatten_dict
         else:
             raise TypeError(f"Unexpected type {type(d)}")
 
         for path, v in d.items():
-            if path not in self.paths and ignore_missing_path:
+            if (path not in self.paths and ignore_missing_path) or (
+                ignore_none and v is None
+            ):
                 continue
             self[path] = v
 
     ### iterations ###
     def items(self):
         return self._d.items()
 
@@ -184,17 +195,18 @@
                 del reduce(getitem, path[:-1], self._d)[path[-1]]
             self._update_flatten()
 
     def __getitem__(self, path: str) -> Any:
         if path not in self._paths:
             raise KeyError(path)
         if self.delimiter not in path:
-            return self._d[path]
+            v = self._d[path]
         path = path.split(self.delimiter)
-        return reduce(getitem, path, self._d)
+        v = reduce(getitem, path, self._d)
+        return v
 
     def __len__(self) -> int:
         return len(self._d)
 
     def __setitem__(self, path: str, value) -> None:
         if self.delimiter not in path:
             self._d[path] = value
@@ -207,13 +219,13 @@
                 v = v[node]
             v[path[-1]] = value
         self._update_flatten()
 
     def __str__(self) -> str:
         return json.dumps(self._d, sort_keys=False, indent=2)
 
-    def __eq__(self, other) -> bool:
-        assert isinstance(other, ndict), f"Unexpected type {type(other)}"
-        return self._flatten_dict == other._flatten_dict
+    def __eq__(self, other: NestedOrDict) -> bool:
+        assert isinstance(other, (ndict, dict)), f"Unexpected type {type(other)}"
+        return self._flatten_dict == ndict(other, self.delimiter)._flatten_dict
 
 
 NestedOrDict = Union[ndict, dict]
```

### Comparing `naapc-1.6.1/src/naapc.egg-info/PKG-INFO` & `naapc-1.7.0/src/naapc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.6.1
+Version: 1.7.0
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naapc-1.6.1/test/test.py` & `naapc-1.7.0/test/test.py`

 * *Files identical despite different names*

