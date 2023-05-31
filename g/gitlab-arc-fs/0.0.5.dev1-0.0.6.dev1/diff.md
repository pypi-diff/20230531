# Comparing `tmp/gitlab_arc_fs-0.0.5.dev1.tar.gz` & `tmp/gitlab_arc_fs-0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_arc_fs-0.0.5.dev1.tar", last modified: Fri Mar 10 09:38:12 2023, max compression
+gzip compressed data, was "gitlab_arc_fs-0.0.6.dev1.tar", last modified: Wed May 31 07:45:17 2023, max compression
```

## Comparing `gitlab_arc_fs-0.0.5.dev1.tar` & `gitlab_arc_fs-0.0.6.dev1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-03-10 09:38:12.896633 gitlab_arc_fs-0.0.5.dev1/
--rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-03-10 09:38:12.896633 gitlab_arc_fs-0.0.5.dev1/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      185 2023-03-10 07:57:09.000000 gitlab_arc_fs-0.0.5.dev1/README.md
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-03-10 09:38:12.896633 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/
--rw-rw-r--   0 julian    (1000) julian    (1000)       55 2023-03-10 07:57:35.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/__init__.py
--rw-rw-r--   0 julian    (1000) julian    (1000)     6900 2023-03-10 07:57:52.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/gitlab_filestream.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    25417 2023-03-10 09:37:25.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/gitlab_fs.py
--rw-rw-r--   0 julian    (1000) julian    (1000)     1015 2023-03-10 07:57:35.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/opener.py
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-03-10 09:38:12.896633 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs.egg-info/
--rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-03-10 09:38:12.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs.egg-info/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      354 2023-03-10 09:38:12.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs.egg-info/SOURCES.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-03-10 09:38:12.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs.egg-info/dependency_links.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       53 2023-03-10 09:38:12.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs.egg-info/entry_points.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       60 2023-03-10 09:38:12.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs.egg-info/requires.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       14 2023-03-10 09:38:12.000000 gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs.egg-info/top_level.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-03-10 09:38:12.896633 gitlab_arc_fs-0.0.5.dev1/setup.cfg
--rw-rw-r--   0 julian    (1000) julian    (1000)      712 2023-03-10 09:37:16.000000 gitlab_arc_fs-0.0.5.dev1/setup.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      185 2023-02-27 10:58:22.000000 gitlab_arc_fs-0.0.6.dev1/README.md
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/
+-rw-rw-r--   0 julian    (1000) julian    (1000)      336 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      424 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/SOURCES.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/dependency_links.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       53 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/entry_points.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       60 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/requires.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       14 2023-05-31 07:45:17.000000 gitlab_arc_fs-0.0.6.dev1/gitlab_arc_fs.egg-info/top_level.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/setup.cfg
+-rw-rw-r--   0 julian    (1000) julian    (1000)      768 2023-05-31 07:00:27.000000 gitlab_arc_fs-0.0.6.dev1/setup.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.780414 gitlab_arc_fs-0.0.6.dev1/src/
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/
+-rw-rw-r--   0 julian    (1000) julian    (1000)       72 2023-05-31 06:59:25.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/__init__.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     8611 2023-05-31 06:59:34.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_filestream.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    28273 2023-05-31 06:59:29.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_fs.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    11153 2023-05-31 07:05:11.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/lfs_file.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     1046 2023-05-31 07:00:16.000000 gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/opener.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-05-31 07:45:17.784414 gitlab_arc_fs-0.0.6.dev1/tests/
+-rw-rw-r--   0 julian    (1000) julian    (1000)    10257 2023-05-30 12:58:02.000000 gitlab_arc_fs-0.0.6.dev1/tests/test_gitlab_fs.py
```

### Comparing `gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/gitlab_filestream.py` & `gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_filestream.py`

 * *Files 16% similar despite different names*

```diff
@@ -118,34 +118,69 @@
         Returns:
             True (bool):    if the file is a lfs file
             False (bool):   if the file is not a lfs file
             None:           if the file is not found
             TODO: Annotate the new return type here. Aso use it everywhere.
         """
         async with semaphore, session.get(url,
+                                          allow_redirects=False,
                                           headers={"PRIVATE-TOKEN":
                                                    self.token,
-                                                   'Accept-Encoding':
-                                                   'None'}) as resp:
-            history = resp.history
-            status = resp.status
+                                                   }) as resp:
             headers = resp.headers
-            logging.debug(f"Begining download of {url}\n")
-            # await asyncio.sleep(10)
-        if status >= 300:
+            status = resp.status
+            redirected = False
+        if status in {301, 302}:
+            redirect_url = headers.get('Location')
+            async with semaphore, session.get(redirect_url,
+                                              allow_redirects=False,
+                                              headers={"PRIVATE-TOKEN":
+                                                       self.token,
+                                                       }) as resp:
+
+                status = resp.status
+                headers = resp.headers
+                redirected = True
+        logging.debug(f"Begining download of {url}\n")
+        # await asyncio.sleep(10)
+        if status >= 302:
             if status == 404:
                 logging.warning(f"Attention: File with URL {url} "
                                 f"was not found")
-                logging.warning("Maybe there is a typo in the ISA file or the "
-                                "filename.\n")
                 return None
-        if len(history) == 0:
+        if not redirected:
             size = headers['X-Gitlab-Size']
         else:
-            size = headers['Content-Length']
+            try:
+                size = headers['Content-Length']
+            # For some reason unkown to men, I only get the content
+            # length in some cases. To retrieve the filesize anyway,
+            # read the size from the content of the header files
+            # (since we got redirected before, it must be a pointer file)
+            except KeyError:
+                url = url.replace("&lfs=true", "")
+                async with semaphore, session.get(url,
+                                                  allow_redirects=False,
+                                                  headers={"PRIVATE-TOKEN":
+                                                           self.token,
+                                                           }) as resp:
+                    try:
+                        content = await resp.text()
+                        lines = content.split("\n")
+                        for line in lines:
+                            try:  # empty lines
+                                (key, value) = line.split(" ", 2)
+                                if key == "size":
+                                    size = value
+                            except Exception as ex:  # NOQA
+                                pass
+                    except aiohttp.ClientError:
+                        size = 0
+                        # TODO: log stuff here
+
         fileinfo = {"name": path.parts[-1],
                     "size": size}
         return fileinfo
 
     def get_file_stream(self,
                         path: str,
                         repo_id: int,
```

### Comparing `gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/gitlab_fs.py` & `gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/gitlab_fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 from fs.base import FS
 from fs.info import Info
+from fs.mode import Mode
 from fs.errors import ResourceNotFound, DirectoryExpected,\
                       ResourceReadOnly, Unsupported,\
                       FileExpected  # NOQA
 from pathlib import Path
 import asyncio
 import aiohttp
-import urllib3
+import urllib3 # NOQA
 import threading
 import os # NOQA
-
 import requests
+import io
+# from dotenv import load_dotenv
+# from os import getenv
 
+try:
+    from .lfs_file import LFSFile
+except ImportError:
+    from lfs_file import LFSFile
 
 try:
     from .gitlab_filestream import FileStreamHandler
 except ImportError:
     from gitlab_filestream import FileStreamHandler
 
 
 class RunThread(threading.Thread):
     """
+    Class to run an asynchronus function
+    in a new thread.
+
     Sligthly changed verion of this answer on
     SO:
     https://stackoverflow.com/a/63072524
     Credits to Mark:
     https://stackoverflow.com/users/2606953/mark
     """
     def __init__(self, func, args):
@@ -34,27 +44,29 @@
         super().__init__()
 
     def run(self):
         self.result = asyncio.run(self.func(*self.args))
 
 
 class GitlabFS(FS):
-    """A readonly PyFileSystem extension for gitlab"""
+    """A readonly PyFileSystem2 extension for gitlab"""
 
     def __init__(self,
                  token: str,
                  server_url: str):
         super().__init__()
         self.server_url = server_url
         self.hostname = server_url.replace("https://", "")
         self.token = token
 
         self.fstream = FileStreamHandler(server_url,
                                          token)
 
+        # Remember already accessed repositories to avoid
+        # requesting the same repository tree multiple times.
         self.accesed_repositories = set()
 
         # Get the initial (toplevel) directory structure.
         # This is essentially a list of directories which represent
         # all Arcs a user has access to with a given token.
         # The repository metadatastructures themselves are constructed
         # upon changing in into the directory.
@@ -74,55 +86,70 @@
 
         # Create a metadata dictionary for all repositories as
         # well as for the root directory ("/").
         # {Path: {"info": Info}
         self.info_dict = {}
         self._build_repository_info()
 
-    def _build_repository_info(self):
-        """Build info for all accesible repositories (toplevel)"""
+    def _build_repository_info(self) -> None:
+        """
+        Build info from self.repos_dictionary for all accesible repositories
+        (toplevel) and save this info in self.info_dict.
+
+        """
         for (path, details) in self.repos_dictionary.items():
             name = path.parts[-1]
             created = details.get('created_at')
 
             info = {"basic": {"name": name, "is_dir": True},
                     "details": {"accessed": None,
                                 "created": created,
                                 "metadata_changed": None,
                                 "modified": None,
                                 "size": None,
                                 "type": 1}}
             self.info_dict.update({path: Info(info)})
 
-    def _build_directory_info(self, path: str):
+    def _check_ressource(self, path):
+        """
+        """
+        (id, repo) = self._get_repo_id_path(str(path))
+        if path in self.repo_trees_dict.get(id):
+            return True
+        return False
+
+    def _build_directory_info(self, path: str) -> None:
         """
         Builds the directory info for a given path, which
         is the path of a directory INSIDE of a repository.
         The metadata information will be collected for all
         files in the directory.
-        Will set metadata as self.metadata_dict[path].
+        Will set metadata as self.info_dict[path].
         If path is the path to a file, will raise DirectoryExpected.
 
         Args:
             path (str): The path to the directory or file
                         to retrieve information about.
 
         Returns:
             None
 
         Raises:
             DirectoryExpected: If the path is not a directory.
         """
         if not self.isdir(path):
-            raise DirectoryExpected(path)
+            if not self._check_ressource(path):
+                raise ResourceNotFound(path)
+            else:
+                raise DirectoryExpected(path)
 
         # Check if the info of the non-file information
         # (i.e. the directory tree information) of the
         # with path corresponding repository is already build.
-        (id, root_path) = self._get_repo_id_path(path)
+        (id, root_path) = self._get_repo_id_path(str(path))
         if id not in self.repo_trees_dict:
             self._construct_tree_dict(id, root_path)
 
         repo_tree = self.repo_trees_dict[id]
         for (pth, raw_info) in repo_tree.items():
             if (str(pth.parent) == path or str(pth) == path)\
                                               and self.isdir(pth):
@@ -132,15 +159,15 @@
                                     "created": None,
                                     "metadata_changed": None,
                                     "modified": None,
                                     "size": None,
                                     "type": 1}}
                 self.info_dict.update({pth: Info(info)})
 
-        # TODO: Add the rest of the info object
+        # Retrieve information about all files under path.
         raw_info_dict = self.run_async(self._retrieve_metadata, path)
         for (pth, info_raw) in raw_info_dict.items():
             name = info_raw['name']
             size = int(info_raw["size"])
             info = {"basic": {"name": name, "is_dir": False},
                     "details": {"accessed": None,
                                 "created": None,
@@ -153,37 +180,33 @@
     async def _retrieve_metadata(self, path: str, semaphore: int = None)\
             -> dict:
         """
         This function asynchronously retrieves the (needed) metadata
         by asynchronously sending HTTP-request to the Gitlab-API.
 
         NOTE: This function should only be called from within
-              _build_repository_tree.
+              _build_directory_info.
 
         Args:
             path (str): The path to the repository / directory to retrieve
                         information about.
             semaphore (int): Number to limit concurrency to.
 
         Returns:
-            paths_lfs (dict): Dictionary of the filepaths to all files in the
-                              (sub)directory specified by path as keys.
-                              And wheter they are lfs files (True) or not
-                              (False) as values. If the file was not fount on
-                              gitlab, the value is None.
+            paths_info (dict): TODO: Add return details.
 
         Raises:
             No internal exception handling.
          """
         if semaphore is None:
             semaphore = 10
 
         if path != "/":
             path = path.strip("/")
-        repo_id, repo_path = self._get_repo_id_path(path)
+        repo_id, repo_path = self._get_repo_id_path(str(path))
         semaphore = asyncio.BoundedSemaphore(semaphore)
         paths = self._gather_file_paths(path)
         urls = [self.fstream.construct_url(
             str(path),
             repo_id,
             repo_path)
             for path in paths]
@@ -212,16 +235,16 @@
         a path to a file, return [path].
 
         Args:
             path (str): The path to directory or file to gather the paths from.
 
         Returns:
             directory_list:             A list of paths to (non dir) files
-            (list[pathlib.PosixPath])   which lay under the (sub)directory
-                                        specified path.
+            (list[pathlib.PosixPath])   which lay in the directory
+                                        specified by path.
 
         Raises:
             No internal exception handling.
         """
         # If we are in the root directory, return only the
         # toplevel ARC-View.
         # This information ist stored in self.repos_dictionary.
@@ -231,15 +254,15 @@
             return path_list
         else:
             path = path.strip('/')
 
         path = Path(path)
         # Get the repository id and path.
         # Build the repository tree, if necessary.
-        (id, repo_path) = self._get_repo_id_path(path)
+        (id, repo_path) = self._get_repo_id_path(str(path))
         if id not in self.repo_trees_dict:
             self._construct_tree_dict(id, repo_path)
 
         # Return path, if path is the path to a file.
         repo_tree = self.repo_trees_dict.get(id)
         if not repo_tree.get(path).get("is_dir"):
             return [path]
@@ -249,25 +272,44 @@
             parent = path_key.parent
             isdir = repo_tree.get(path_key).get("is_dir")
             if parent == path and not isdir:
                 path_list.append(path_key)
 
         return path_list
 
-    def _get_repo_id_path(self, path: str):
+    def _get_repo_id_path(self, path: str) -> tuple:
+        """
+        Returns a tuple containing the ID and repository path of the with
+        repository corresonding with path.
+
+        Args:
+            path (str): path do a directory or file (inside a repository).
+
+        Returns:
+            TODO: check return values inside tuple.
+            (ID: int, path: pathlib.Posixpath): A tuple of the repository id
+                                                and repository path
+                                                corresponding with path.
+        """
+        # Set alternative root paths names to the root path.
+        if path == "." or path == "./":
+            path = "/"
+        # Remove trailing / leading slash.
+        if path != "/":
+            path = path.strip("/")
         path = Path(path)
         root_path = path.parts[0]
         try:
             id = self.repos_dictionary.get(Path(root_path)).get("id")
         except (KeyError, AttributeError):
             id = None
             root_path = None
         return (id, root_path)
 
-    def _get_accessable_repositories(self):
+    def _get_accessable_repositories(self) -> dict:
         """
         Gets information about the repository which are accessible with
         the given token.
 
         Args: None
 
         Returns:
@@ -327,44 +369,46 @@
                 # TODO: Add some retry functionality here.
             except requests.exceptions.RequestException as e:
                 print("Recieved request exception:")
                 raise SystemExit(e)
             data.extend(r.json())
 
         for dict in data:
-            dict["path_without_namespace"] = Path(dict.get("path"))
-            dict["path_formated"] = Path(dict.pop("path_with_namespace")
-                                         .replace("/", "-"))
+            # dict["path_without_namespace"] = Path(dict.get("path"))
+            path = dict.get("name_with_namespace")
+            formated_path = path.replace(" / ", "-").replace(" ", "_")
+            dict["path_formated"] = Path(formated_path)
+            # dict["path_formated"] = Path(dict.pop("path_with_namespace")
+            #                              .replace("/", "-"))
             dict.update({"is_repository": True,
                          "is_dir": True})
 
         # Adding the root directory.
         data.append({"path_formated": Path("/"),
                      "path": Path("/"),
                      "is_repository": False,
                      "is_dir": True})
-
         return data
 
-    def _build_repo_dict(self):
+    def _build_repo_dict(self) -> None:
         """
-        Construct the directory dict structure from the self.directory_tree.
-        Sets the structure as self.directory_dict.
+        Construct the directory dict structure from self.repo_list.
+        Sets the structure as self.repos_dictionary.
 
         Args: None
         Returns: None
         Raises: No internal exception handling.
         """
         for el in self.repo_list:
             key = el.get("path_formated")
             value = el
             self.repos_dictionary.update({key: value})
 
     def _construct_tree_dict(self, repo_id: int,
-                             repo_path: str):
+                             repo_path: str) -> None:
         # TODO: Type annotation
         # TODO: Add datetime
         # TODO: Maybe extract everything with requests to gitlab_filestream
         """
         Builds self.repos_dictionary for a given repository(id).
 
         Args:
@@ -399,15 +443,15 @@
                                    "order_by": "id",
                                    "sort": "asc",
                                    "per_page": 100})
             r.raise_for_status()
         except requests.HTTPError as e:
             print("Bad status code:", r.status_code)
             print("Exiting program")
-            raise SystemExit(e)
+            raise e
         except requests.exceptions.Timeout:
             print("Timout error")
             # TODO: Add some retry functionality here.
         except requests.exceptions.RequestException as e:
             print("Recieved request exception")
             print("Exiting program")
             raise SystemExit(e)
@@ -460,34 +504,40 @@
         repo_path = Path(repo_path)
         info = {"is_dir": True, "name": name}
         directory_dict.update({repo_path: info})
 
         self.repo_trees_dict.update({repo_id: directory_dict})
         self.accesed_repositories.add(repo_id)
 
-    def getinfo(self, path: str, namespaces=None):
+    def getinfo(self, path: str, namespaces=None) -> Info:
         """
+        TODO: Docstings
         """
+        if path in [".", "./", ""]:
+            path = "/"
         if path != "/":
             path = path.strip("/")
 
         # Ceck if the given path is a path to a repository.
         # If so, the metadata information is already available
         # in self.info_dict.
         if self.isrepository(path):
             try:
                 return self.info_dict[Path(path)]
             except KeyError:
-                raise ResourceNotFound
+                raise ResourceNotFound(path)
 
         # Check in the repository corresponding to the path
         # was already accessed.
-        (id, repo_path) = self._get_repo_id_path(path)
+        (id, repo_path) = self._get_repo_id_path(str(path))
         if id not in self.accesed_repositories:
-            self._construct_tree_dict(id, repo_path)
+            try:
+                self._construct_tree_dict(id, repo_path)
+            except requests.exceptions.HTTPError:
+                raise ResourceNotFound(path)
 
         # Check if metadata for the given path is available already.
         path = Path(path)
         info = self.info_dict.get(path)
         # If not, retrieve the metadata for all files in the given path.
         # If path is the path to a file, then for all files in the same
         # directory
@@ -524,14 +574,18 @@
         Returns:
             directory_list (list): list of names, relative to path.
 
         Raises:
             fs.errors.DirectoryExpected: If ``path`` is not a directory.
             fs.errors.ResourceNotFound: If ``path`` does not exist.
         """
+        # Set alternative root paths names to the root path.
+        if path == "." or path == "./":
+            path = "/"
+        # Remove trailing / leading slash.
         if path != "/":
             path = path.strip("/")
 
         directory_list = []
 
         # handling of the top-level directory (the view on different ARCs)
         if path == "/":
@@ -541,20 +595,20 @@
             return directory_list
 
         # Get the root directory of the given path (which will be an
         # repository). Get the repository id. With this, check if the
         # given path is already in self.repos_dictionary.
         # If not, try to build it.
         is_repository = self.isrepository(path)
-        (id, root_path) = self._get_repo_id_path(path)
+        (id, root_path) = self._get_repo_id_path(str(path))
 
         # If the root path is not in self.repos_dictionary, it can't be
         # a repository which the user has acces to.
         if id is None:
-            raise ResourceNotFound
+            raise ResourceNotFound(path)
         # Check if the repository described by root path was already build.
         if id not in self.repo_trees_dict:
             self._construct_tree_dict(id, root_path)
 
         # Check if the path is a valid directory or repository
         # TODO: Revisit this after getinfo and isdir are implemented.
         if (self.repo_trees_dict.get(id).get(Path(path)) is None and
@@ -569,15 +623,18 @@
         directory_list = [pth.name for pth in paths_list
                           if pth.parent == Path(path)]
 
         return directory_list
 
     def isrepository(self, path: str) -> bool:
         """
+        TODO: Docstings
         """
+        if path in [".", "./", ""]:
+            path = "/"
         if path != "/":
             path = path.strip('/')
         root_path = Path(path).parts[0]
         is_repository = False
         if root_path == path:
             is_repository = True
         return is_repository
@@ -589,14 +646,17 @@
         Arguments:
             path (str): A path on the filesystem.
 
         Returns:
             bool: `True` if ``path`` maps to a directory.
 
         """
+        # Set alternative root paths names to the root path.
+        if path in [".", "./", ""]:
+            path = "/"
         path = Path(path)
         # Check if the path is a repository (and therefore a directory).
         if path in self.repos_dictionary:
             return True
         # Check if the repository corresponding to the given path is
         # already build.
         (id, root_path) = self._get_repo_id_path(str(path))
@@ -615,49 +675,59 @@
 
         if repo_tree.get(path).get("is_dir"):
             return True
 
         return False
 
     def openbin(self, path, mode='r', buffering=-1, **options)\
-            -> urllib3.response.HTTPResponse:
+            -> io.IOBase:
         """
         Returns a file like object that can be opened.
         Args:
             path (str): The path to open.
             mode (str): The mode to open the file with. Only read is supported.
             buffering: -
         Returns:
-            fp (tempfile.TemporaryFile): A temporary, seekable file object.
-            or
             resp (resp.Response): A Response object for a filestream.
         Raises: No internal exception handling.
-        NOTE: Only supports read mode ('r')
         TODO: Possibly implement buffering
         TODO: Improve error handling. Maybe get inspired from one of the
               built-in filesystems.
               See https://github.com/PyFilesystem/fs.dropboxfs
         """
         with self._lock:
+            try:
+                parsedMode = Mode(mode)
+                parsedMode.validate_bin()
+            except ValueError as e:
+                raise e
             if path != "/":
                 path = path.strip("/")
             if self.isdir(path):
-                raise FileExpected
-            if mode != 'r':
-                print("Only read operations are supported!")
+                raise FileExpected(path)
+            if parsedMode.reading:
+                (repo_id, repo_path) = self._get_repo_id_path(str(path))
+                r = self.fstream.get_file_stream(path, repo_id, repo_path)
+                return r.raw
+            if parsedMode.exclusive or parsedMode.writing or parsedMode.create:
+                repo_id, repo_path = self._get_repo_id_path(str(path))
+                namespace = self._get_namespace(repo_path)
+                path = "/".join(part for part in Path(path).parts[1:])
+                file = LFSFile(path, self.token,
+                               self.hostname,
+                               namespace,
+                               repo_id)
+                return file
+            else:
                 raise Unsupported
 
-        (repo_id, repo_path) = self._get_repo_id_path(path)
-
-        r = self.fstream.get_file_stream(path, repo_id, repo_path)
-
-        return r.raw
-
     def run_async(self, func, *args):
         """
+        TODO: Docstrings
+        TODO: return values
         Sligthly changed verion of this answer on
         SO:
         https://stackoverflow.com/a/63072524
         Credits to Mark:
         https://stackoverflow.com/users/2606953/mark
         """
         try:
@@ -668,14 +738,24 @@
             thread = RunThread(func, args)
             thread.start()
             thread.join()
             return thread.result
         else:
             return asyncio.run(func(*args))
 
+    def _get_namespace(self, path: str):
+        """_summary_
+
+        Args:
+            id (_type_): _description_
+        """
+        namespace = self.repos_dictionary.get(Path(path))\
+            .get("path_with_namespace")
+        return namespace
+
     def makedir():
         pass
 
     def remove():
         pass
 
     def removedir():
```

### Comparing `gitlab_arc_fs-0.0.5.dev1/gitlab_arc_fs/opener.py` & `gitlab_arc_fs-0.0.6.dev1/src/gitlab_arc_fs/opener.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,37 @@
 
 import fs # NOQA
 
 from fs.opener import Opener
 from fs.opener.errors import OpenerError # NOQA
 from fs.base import FS
 
-from gitlab_arc_fs import gitlab_fs  # NOQA
+try:
+    from .gitlab_fs import GitlabFS
+except ImportError:
+    from gitlab_fs import GitlabFS
 
 
 class GitlabFSOpener(Opener):
     """
     The Gitlab FSOpener class represents a gitlab fsopener.
     TODO: Implement error handling.
     """
     protocols = ['gitlab']
 
-    def open_fs(self, fs_url, parse_result, writeable=False,
+    def open_fs(self, fs_url, parse_result, writeable=True,
                 create=True, cwd=None) -> FS:
         private_token = parse_result.username
         print(parse_result)
 
         url = urllib.parse.urlparse(parse_result.resource)
 
         serverURL = url.scheme + '://' + url.netloc
         namespace = url.path
 
         print(serverURL, namespace)
 
         if "ref" in parse_result.params:
             ref = parse_result.params['ref']
-            return gitlab_fs.GitlabFS(private_token, serverURL, namespace, ref)
+            return GitlabFS(private_token, serverURL, namespace, ref)
 
-        return gitlab_fs.GitlabFS(private_token, serverURL, namespace)
+        return GitlabFS(private_token, serverURL, namespace)
```

### Comparing `gitlab_arc_fs-0.0.5.dev1/setup.py` & `gitlab_arc_fs-0.0.6.dev1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,11 +14,12 @@
     entry_points={
         'fs.opener': [
             'gitlab = gitlab_fs.opener:GitlabFSOpener',
         ]
     },
     license="MY LICENSE",
     packages=['gitlab_arc_fs'],
-    version="0.0.5.dev1",
+    package_dir={'gitlab_arc_fs': 'src/gitlab_arc_fs'},
+    version="0.0.6.dev1",
     url="https://git.bwcloud.uni-freiburg.de/julian.weidhase/GitlabFS",
     python_requires='>=3.8'
 )
```

