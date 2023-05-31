# Comparing `tmp/xt_st_common-0.4.1.tar.gz` & `tmp/xt_st_common-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.4.1.tar", max compression
+gzip compressed data, was "xt_st_common-0.5.0.tar", max compression
```

## Comparing `xt_st_common-0.4.1.tar` & `xt_st_common-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,33 @@
--rw-r--r--   0        0        0      606 2023-05-05 05:05:39.749835 xt_st_common-0.4.1/README.md
--rw-r--r--   0        0        0     1541 2023-05-05 05:05:39.749835 xt_st_common-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-05 05:05:39.749835 xt_st_common-0.4.1/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5039 2023-05-05 05:05:07.689646 xt_st_common-0.4.1/src/xt_st_common/components.py
--rw-r--r--   0        0        0     1784 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/config.py
--rw-r--r--   0        0        0     7200 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/database.py
--rw-r--r--   0        0        0    14615 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/file_manager.py
--rw-r--r--   0        0        0     6407 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0     5938 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/session.py
--rw-r--r--   0        0        0     4871 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1774 2023-05-05 05:05:07.693646 xt_st_common-0.4.1/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 xt_st_common-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-05-31 03:51:46.474738 xt_st_common-0.5.0/README.md
+-rw-r--r--   0        0        0     2603 2023-05-31 03:51:46.474738 xt_st_common-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-05-31 03:51:08.622162 xt_st_common-0.5.0/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-31 03:51:08.622162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-05-31 03:51:08.622162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-05-31 03:51:08.622162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-05-31 03:51:08.622162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-05-31 03:51:08.622162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-05-31 03:51:08.622162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-05-31 03:51:08.642162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-05-31 03:51:08.642162 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-05-31 03:51:46.474738 xt_st_common-0.5.0/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5004 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2371 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    21050 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6251 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-05-31 03:51:08.722163 xt_st_common-0.5.0/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.5.0/PKG-INFO
```

### Comparing `xt_st_common-0.4.1/src/xt_st_common/components.py` & `xt_st_common-0.5.0/src/xt_st_common/components.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,18 @@
     page_logo_width: int = 250,
     logout_url: str | None = None,
 ):
     """
     Display the page header including Title, Logo, and optional Logout button
     """
     base_url = settings.STREAMLIT_SERVER_BASE_URL_PATH
+    script_frame = st.empty()
     if logout_url is not None:
         # Load the css/icons for the button
         st.markdown(
-            f"""
-            <link rel="stylesheet"
-                  href="{base_url}/app/static/css/bootstrap-glyphicons.css"
-                  type='text/css' />"""
             """
             <style scoped type="text/css">
                 .btn-logout {
                     box-shadow:inset 0px 1px 0px 0px #ffffff;
                     background:linear-gradient(to bottom, #f9f9f9 5%, #e9e9e9 100%);
                     background-color:#f9f9f9;
                     border-radius:6px;
@@ -43,22 +40,24 @@
                     background:linear-gradient(to bottom, #e9e9e9 5%, #f9f9f9 100%);
                     background-color:#e9e9e9;
                 }
                 .btn-logout:active {
                     position:relative;
                     top:1px;
                 }
+                .main .block-container {
+                    padding-top: 3rem;
+                }
             </style>
             """,
             unsafe_allow_html=True,
         )
 
         # Define the button
-        logout_link = f"""<a id="logout-button" class="btn-logout" href={logout_url} role="button">
-<span class="glyphicon glyphicon-log-out"></span> Log out</a>"""
+        logout_link = f'<a id="logout-button" class="btn-logout" href={logout_url} role="button">🔐 Log out</a>'
     else:
         logout_link = ""
 
     page_title = "" if page_title is None else page_title
 
     page_logo = "" if page_logo is None else f"<img src='{page_logo}' width='{page_logo_width}px'>"
     # Display the page header including Title, Logo, and optional Logout button
@@ -87,18 +86,20 @@
                 border-radius: 20px;
                 margin-left: -15px;
                 padding: 0px 15px;
                 font-weight: bold;
                 vertical-align: super;
             }}
         </style>
+        """
+        + f"""
         <div class='xt_logo' >
             <span style='float: right;'>
-        {logout_link}"""
-        + f"""  <img src='{base_url}/app/static/media/XT_words_wrapped.png' width='200px'>
+            {logout_link}
+            <img src='{base_url}/app/static/media/XT_words_wrapped.png' width='200px'>
             </span>
             <span class='app_logo'>
         """
         + page_logo
         + page_title
         + """
          </span>
@@ -129,8 +130,9 @@
                     })
                     return true;
                 }
                 // Override the target so that we reload the current page rather than opening a new one
                 a.target = ""
             """
         )
-        streamlit_js_eval(js_expressions=logout_script, key="js-logout-script")
+        with script_frame:
+            streamlit_js_eval(js_expressions=logout_script, key="js-logout-script")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xt_st_common-0.4.1/src/xt_st_common/config.py` & `xt_st_common-0.5.0/src/xt_st_common/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,55 @@
+from enum import Enum
 from importlib.machinery import PathFinder
 from pathlib import Path
 from typing import Optional
 
-from pydantic import BaseSettings
+from pydantic import BaseSettings, SecretStr
 from pydantic.color import Color
 
 
+class StorageType(str, Enum):
+    MINIO = "MINIO"
+    MINIO_AWS = "MINIO_AWS"
+    NONE = "NONE"
+
+
 class StreamlitBaseSettings(BaseSettings):
     SIGNOUT_URL: Optional[str] = None
     CURRENT_PACKAGE = __name__.split(".")[0]
     BASE_PATH: str = str(Path(PathFinder().find_spec(CURRENT_PACKAGE).origin).parent)  # type: ignore
     DATA_DIR: str = str(Path.cwd() / "appdata")
     """Root directory for storing app data"""
+
+    ###############
+    # Storage Vars
+    ###############
+    STORAGE_TYPE: StorageType = StorageType.NONE
+    BUCKET_NAME: Optional[str] = None
+    BUCKET_PREFIX: Optional[str] = None
+    MINIO_SECRET_KEY: Optional[SecretStr] = None
+    MINIO_ACCESS_KEY: Optional[str] = None
+    MINIO_ENDPOINT: Optional[str] = None
+    MINIO_HTTPS: bool = True
+
+    APP_NAME: str = "my_app"
+    """Name of the app that be tagged in the DB"""
     APP_TAG_TEXT: str = "Development"
     """text that will appear next the application logo"""
     APP_TAG_BACKGROUND: Color = Color("#00a9ce")
     """background colour of the APP_TAG_TEXT"""
     DEBUG: bool = False
     """Enable debug information in the app"""
     DEBUG_MOCK_SESSION: bool = False
     """Mock the session headers returned when deployed to AWS"""
     USE_COGNITO: bool = False
     """Use AWS Cognito for Auth"""
     COGNITO_COOKIE: str = "AWSELBAuthSessionCookie"
     """If set cookies with this prefix will be deleted on signout"""
-    COGNITO_GROUPS: str = "app-fracg"
+    COGNITO_GROUPS: str = "ap-southeast-2_lC6GUKOej_CSIRO-EASI"
     """One of these comma separated groups must be present in the user's `cognito:groups`"""
     NO_ACCESS_MSG: str = "Error: You do not have permission to use this app."
     """Error message displayed when a user doesn't have permission to use the app"""
     STREAMLIT_SERVER_BASE_URL_PATH: str = ""
     """The base path for the URL where Streamlit should be served from"""
     MONGO_CONNECTION_STRING: str = ""
     """Mongo DB connection string"""
```

### Comparing `xt_st_common-0.4.1/src/xt_st_common/database.py` & `xt_st_common-0.5.0/src/xt_st_common/project_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,80 @@
 import logging
+from enum import Enum
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
-import streamlit as st
-from odmantic import Model, SyncEngine, query
-from pymongo import MongoClient
+from bson import ObjectId
+from pydantic import BaseModel, Field
 
-from .config import StreamlitBaseSettings
-from .storage import FileRef
+from xt_st_common.config import StreamlitBaseSettings
+from xt_st_common.storage import FileRef, storage_client
 
-# from streamlit.runtime.uploaded_file_manager import UploadedFile # FIXME: remove if unneeded?
+settings = StreamlitBaseSettings()
 
 
-# Initialize connection.
-# Uses st.experimental_singleton to only run once.
-@st.experimental_singleton
-def get_engine():
-    settings = StreamlitBaseSettings()
-    if settings.MONGO_CONNECTION_STRING is None:
-        raise ValueError("Can't get mongo engine when connection string is None.")
+class PyObjectId(ObjectId):
+    @classmethod
+    def __get_validators__(cls):
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, v):
+        if not ObjectId.is_valid(v):
+            raise ValueError("Invalid objectid")
+        return ObjectId(v)
+
+    @classmethod
+    def __modify_schema__(cls, field_schema):
+        field_schema.update(type="string")
+
+
+class ProjectState(str, Enum):
+    PROJECT_DELETE_CONFIRM = "proj_delete_confirm"
+    PROJECT_TO_DELETE = "proj_delete"
+    PROJECT_SUCCESS_MESSAGE = "proj_success_message"
+    PROJECT_WARNING_MESSAGE = "proj_warning_message"
+
+    FOLDER_TO_DELETE = "upload_delete_folder"
+    FOLDER_ADDED = "upload_folder_added"
+
+    UPLOAD_SUCCESS_MESSAGE = "upload_success_message"
+    UPLOAD_WARNING_MESSAGE = "upload_warning_message"
+    UPLOAD_DELETE_CONFIRM = "upload_delete_confirm"
 
-    client = MongoClient(settings.MONGO_CONNECTION_STRING)
-    return SyncEngine(client=client, database=settings.DATABASE_NAME)
+    FILE_DELETE_CONFIRM = "file_delete_confirm"
+    FILE_TO_DELETE = "file_to_delete"
+    FILE_SUCCESS_MESSAGE = "file_success_message"
+    FILE_WARNING_MESSAGE = "file_warning_message"
 
+    # FILE_MANAGER_UPLOAD = "file_manager_upload_file"
+    FILE_MANAGER_REPLACE_FILE = "file_manager_replace_file"
 
-class Project(Model):
+
+class Project(BaseModel):
+    id: Optional[PyObjectId] = Field(default_factory=PyObjectId, alias="_id")  # noqa: A003
     name: str
     description: str = ""
     public: bool = False
-    application: str = "mpl"  # Name of the application that creates the project
+    application: str = settings.APP_NAME
     files: List[FileRef] = []
     folders: List[str] = []
     owner: str = ""
     users: List[str] = []  # Users with access to this project
 
-    def exists(self, engine=None) -> bool:
-        if engine is None:
-            engine = get_engine()
-        return get_engine().count(Project, Project.id == self.id) > 0
-
-    def is_duplicate(self, engine=None) -> bool:
-        if engine is None:
-            engine = get_engine()
-        return (
-            engine.count(Project, (Project.id != self.id) & (Project.name == self.name) & (Project.owner == self.owner))
-            > 0
-        )
-
     def get_users_string(self):
         return ",".join(self.users)
 
     def get_folders_map(self):
-        fol_dict = {}
-        fol_dict["/"] = "Project Root"
+        fol_dict = {"/": "Project Root"}
         for folder in self.folders:
             parts = folder.strip("/").split("/")
             fol_dict[folder] = " - ".join(parts)
         return fol_dict
 
-    @classmethod
-    def list_owned(cls, engine, owner) -> List["Project"]:
-        return list(engine.find(cls, Project.owner == owner))
-
-    def save(self) -> "Project":
-        _ = get_engine().find_one(Project, Project.id == self.id)
-        _.update(self.dict(exclude_unset=True, exclude={"id"}))
-        return get_engine().save(_)
-
     def get_folder_path(self, folder):
         return f"{str(self.id)}/{self.name}/{folder}".strip("/")
 
     def get_files_in_folder(self, folder: str, include_subfolders=True, extensions=None, null_option=None):
         _files: Dict[str, Union[None, FileRef]] = {} if null_option is None else {null_option: None}
 
         path = self.get_folder_path(folder)
@@ -120,43 +124,39 @@
             if main_dict[key]:
                 children = []
                 self.populate_children(main_dict, key, children, key)
             nodes.append({"label": key, "value": key, "children": children})
 
         return nodes
 
-    def add_replace_file(self, data_file, folder: str, filename: str, save=False, content_type=None) -> FileRef:
+    def add_replace_file(self, data_file, folder: str, filename: str, content_type=None) -> FileRef:
         path = f"{self.get_folder_path(folder)}/{filename}".strip("/")
-        return self.add_replace_file_by_path(data_file, path, save, content_type=content_type)
+        return self.add_replace_file_by_path(data_file, path, content_type=content_type)
 
-    def add_replace_file_by_path(self, data_file, path: str, save=False, content_type=None) -> FileRef:
-        file_ref = st.session_state.storage_client.write_file(path, data_file, content_type)
+    def add_replace_file_by_path(self, data_file, path: str, content_type=None) -> FileRef:
+        file_ref = storage_client().write_file(path, data_file, content_type)
         replaced = False
         for idx, file in enumerate(self.files):
             if file.path == path:
                 self.files[idx] = file_ref
                 replaced = True
                 break
         if not replaced:
             self.files.append(file_ref)
-        if save:
-            self.save()
 
         return file_ref
 
-    def delete_file(self, file: FileRef, save=True):
-        st.session_state.storage_client.delete_file(file.path)
+    def delete_file(self, file: FileRef):
+        storage_client().delete_file(file.path)
         try:
             self.files.remove(file)
-            if save:
-                self.save()
         except ValueError:
             logging.warning(f"File {file.path} didn't exist and couldn't be deleted.")
 
-    def add_folders(self, folders_string: str, save: bool = False):
+    def add_folders(self, folders_string: str):
         folders = set(self.folders)
         new_folders = folders_string.split(",")
         count = 0
         for folder in new_folders:
             folder = folder.strip().replace(" ", "_").strip("/")
             folder_parts = folder.split("/")
             for idx, part in enumerate(folder_parts):
@@ -166,33 +166,21 @@
                     folders.add(f"{'/'.join(folder_parts[:idx+1])}")
                 count += 1
         try:
             self.folders = list(folders)
         except AttributeError:
             logging.warning("Weird odmatic error, attempting to ignore")
 
-        if save:
-            self.save()
-
         return count
 
-    def delete_folder(self, folder: str, save=False):
+    def delete_folder(self, folder: str):
         try:
             folder_path = self.get_folder_path(folder)
             self.folders.remove(folder)
             for file in [x for x in self.files if folder_path in x.path]:
                 self.delete_file(file)
-            if save:
-                self.save()
         except ValueError:
             logging.warning(f"Folder {folder} didn't exist and couldn't be deleted.")
 
-    def delete(self):
-        engine = get_engine()
-        engine.delete(self)
-
-    @classmethod
-    def list_accessable(cls, engine, user_email, owner, include_public=False) -> List["Project"]:
-        search_query = query.or_(cls.users == user_email, cls.owner == owner)
-        if include_public:
-            search_query = query.or_(Project.public == True, search_query)  # noqa
-        return list(engine.find(cls, search_query))
+    class Config:
+        anystr_strip_whitespace = True
+        # collection = "project"
```

### Comparing `xt_st_common-0.4.1/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.5.0/src/xt_st_common/fs_upload_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,17 +102,15 @@
         if path == "/" and len(root_dir) > 0:
             rmtree(root_dir)
             Path.mkdir(root_dir)
             return
 
         # Check path is a child of the expected root directory
         if not _is_child_path(fpath, root_dir):
-            raise PermissionError(
-                f"Attempting to remove file outside root directory: ['{path}']"
-            )
+            raise PermissionError(f"Attempting to remove file outside root directory: ['{path}']")
 
         # If path is a directory defer until later once all the files are removed
         # (can't remove a non-empty directory)
         if fpath.is_dir():
             dir_list.append(str(fpath))
         else:
             Path.unlink(fpath)
@@ -142,25 +140,21 @@
             Name of the zip when downloading will be `{dl_prefix}-Y-m-d_H.M.S.zip`
     """
     c1, c2 = st.columns(2)
 
     # Show file structure
     with c1:
         file_list = list_directory(data_dir + os.sep)
-        file_tree = [
-            {"label": "/", "value": "/", "children": create_file_tree(file_list)}
-        ]
+        file_tree = [{"label": "/", "value": "/", "children": create_file_tree(file_list)}]
         ts = tree_select(file_tree, expanded=["/"], check_model="all")
 
     # Show upload widget and other controls
     with c2:
         # File Upload
-        uploaded_files = st.file_uploader(
-            "Upload input file(s)", accept_multiple_files=True, type=accepted_ft
-        )
+        uploaded_files = st.file_uploader("Upload input file(s)", accept_multiple_files=True, type=accepted_ft)
         for uploaded_file in uploaded_files:
             save_path = Path(data_dir, uploaded_file.name)
             with Path.open(save_path, "wb") as w:
                 w.write(uploaded_file.getvalue())
 
         # File Download
         files_selected, dl_data = (False, "")
@@ -173,12 +167,10 @@
             st.download_button(
                 "Zip & Download",
                 data=dl_data,
                 file_name=f"{dl_prefix}-{datetime.now(tz=ZoneInfo(settings.TIMEZONE)).strftime('%Y-%m-%d_%H.%M.%S')}.zip",
                 disabled=not files_selected,
             )
         with r_btn:
-            if st.button(
-                "Delete Selected", disabled=not files_selected, type="primary"
-            ):
+            if st.button("Delete Selected", disabled=not files_selected, type="primary"):
                 _delete_files(ts["checked"], root_dir=data_dir)
                 st.experimental_rerun()
```

### Comparing `xt_st_common-0.4.1/src/xt_st_common/session.py` & `xt_st_common-0.5.0/src/xt_st_common/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 import jwt
 from streamlit.web.server.websocket_headers import _get_websocket_headers
 
 from xt_st_common.config import StreamlitBaseSettings
 
 settings = StreamlitBaseSettings()
@@ -38,15 +38,15 @@
             "Sec-Websocket-Protocol": "streamlit",
         }
         return headers
 
     return _get_websocket_headers()
 
 
-def decode_jwt(raw_jwt: str, algorithms: List[str] = None, options=None) -> dict:
+def decode_jwt(raw_jwt: str, algorithms: Optional[List[str]] = None, options=None) -> dict:
     """
     Decode a JWT and return its values as a dictionary
 
     `algorithms` defaults to `["ES256"]`
     `options` defaults to `{"verify_signature": False}`
     """
     if algorithms is None:
@@ -84,15 +84,15 @@
     """
     headers = get_session_headers()
     if headers is not None and "X-Goog-Authenticated-User-Email" in headers:
         return headers["X-Goog-Authenticated-User-Email"].split(":")[1]
     if headers is not None and "X-Amzn-Oidc-Data" in headers:
         return decode_jwt(headers["X-Amzn-Oidc-Data"])["email"]
     if allow_default:
-        return "default-user"
+        return "default-user@exploration.tools"
 
     raise KeyError("X-Goog-Authenticated-User-Email not found in headers")
 
 
 def get_oidc_groups() -> List[str]:
     """
     Attempts to retrieve the OIDC groups from the headers (e.g. cognito:groups)
```

### Comparing `xt_st_common-0.4.1/src/xt_st_common/storage.py` & `xt_st_common-0.5.0/src/xt_st_common/storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import logging
 import mimetypes
 import os
 from abc import ABC, abstractmethod
 from io import BytesIO
 from typing import Optional, Union
 
+import streamlit as st
 from minio import Minio
 from minio.credentials import IamAwsProvider, Provider
+from minio.credentials.providers import StaticProvider
 from minio.error import MinioException
 from minio.helpers import ObjectWriteResult
 from pydantic import BaseModel
 
+from xt_st_common.config import StorageType, StreamlitBaseSettings
+
 from .utils import sizeof_fmt
 
+settings = StreamlitBaseSettings()
+
 
 class FileRef(BaseModel):
     size: Optional[str]  # e.g. '3 KB'
     size_bytes: Optional[int]
     url: Optional[str] = None  # download url
     gs_uri: Optional[str] = None  # GSC Uri
     path: str  # path to current item (e.g. /folder1/someFile.txt)
@@ -56,23 +62,22 @@
     @abstractmethod
     def file_exists(self, file_path: str):
         pass
 
 
 class MinioStorageClient(StorageClient):
     def __init__(self, bucket: str, endpoint="s3.amazonaws.com", credentials: Provider = IamAwsProvider(), secure=True):
-        if len(bucket) > 0:
-            self.__bucket = bucket
-        else:
+        if not bucket:
             raise ValueError("bucket name must be set")
 
+        self.__bucket = bucket
         # Check environment variables have been set
         if isinstance(credentials, IamAwsProvider):
             for var in ["AWS_WEB_IDENTITY_TOKEN_FILE", "AWS_REGION", "AWS_ROLE_ARN"]:
-                if len(os.environ.get(var)) <= 0:
+                if os.environ.get(var) is None or len(str(os.environ.get(var))) <= 0:
                     raise ValueError("Environment Variable {var} missing")
 
         # Create the Minio Client
         __client = Minio(endpoint, credentials=credentials, secure=secure)
         exists = __client.bucket_exists(bucket)
         if not exists:
             __client.make_bucket(bucket)
@@ -141,7 +146,31 @@
             stats = self.__client.stat_object(self.__bucket, file_path)
             return stats is not None
         except MinioException as err:
             if hasattr(err, "code") and err.code == "NoSuchKey":
                 return False
             logging.error(str(err))
             raise err
+
+
+@st.cache_resource()
+def storage_client():
+    if settings.STORAGE_TYPE not in [StorageType.MINIO, StorageType.MINIO_AWS]:
+        raise ValueError("STORAGE_TYPE may not be blank when using the storage_client")
+    if settings.BUCKET_NAME is None:
+        raise ValueError("BUCKET_NAME may not be blank!")
+    if settings.STORAGE_TYPE == StorageType.MINIO_AWS:
+        return MinioStorageClient(settings.BUCKET_NAME)  # type: ignore
+    if settings.STORAGE_TYPE == StorageType.MINIO:
+        if settings.MINIO_ENDPOINT is None:
+            raise ValueError("MINIO_ENDPOINT may not be blank!")
+        if settings.MINIO_SECRET_KEY is None:
+            raise ValueError("MINIO_SECRET_KEY may not be blank!")
+        if settings.MINIO_ACCESS_KEY is None:
+            raise ValueError("MINIO_ACCESS_KEY may not be blank!")
+        return MinioStorageClient(
+            settings.BUCKET_NAME,
+            endpoint=settings.MINIO_ENDPOINT,
+            credentials=StaticProvider(settings.MINIO_ACCESS_KEY, settings.MINIO_SECRET_KEY.get_secret_value()),
+            secure=settings.MINIO_HTTPS,
+        )
+    raise NotImplementedError(f"Storage Type {settings.STORAGE_TYPE} not supported")
```

### Comparing `xt_st_common-0.4.1/src/xt_st_common/utils.py` & `xt_st_common-0.5.0/src/xt_st_common/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import csv
 from collections import defaultdict
+from enum import Enum
 from io import BytesIO
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
 import chardet
 import streamlit as st
 
 # from pydantic import BaseModel
 
 # from dask.distributed import Client
@@ -14,15 +15,14 @@
 # def get_dask_client():
 #     client = Client("tcp://127.0.0.1:8786")
 #     # client = Client()
 
 #     return client
 
 
-@st.cache
 def get_encoding_and_dialect(input_file: BytesIO):
     sample_bytes = 1048576  # 1 Megabyte
     _bytes = input_file.read(sample_bytes)
 
     result = chardet.detect(_bytes)
     charenc = result["encoding"]
 
@@ -31,15 +31,15 @@
 
     dialect = csv.Sniffer().sniff(str(_bytes))
     input_file.seek(0)
 
     return charenc, dialect
 
 
-def sizeof_fmt(num: Optional[Any], suffix="B") -> str:
+def sizeof_fmt(num: Optional[Union[float, int]], suffix="B") -> str:
     if num is None:
         return ""
     for unit in ["", "K", "M", "G", "T", "P", "E", "Z"]:
         if abs(num) < 1024.0:
             return "%3.1f%s%s" % (num, unit, suffix)
         num /= 1024.0
     return "%.1f%s%s" % (num, "Y", suffix)
@@ -63,9 +63,13 @@
     else:
         node, others = parts
         if node not in trunk:
             trunk[node] = defaultdict(dict, ((FILE_MARKER, []),))
         attach(others, trunk[node])
 
 
-def get_state(state_name, default=""):
-    return st.session_state[state_name] if state_name in st.session_state else default
+def get_state(state_name: Union[str, Enum], default: Optional[Any] = ""):
+    return st.session_state[str(state_name)] if str(state_name) in st.session_state else default
+
+
+def set_state(state_name: Union[str, Enum], value: Any):
+    st.session_state[str(state_name)] = value
```

### Comparing `xt_st_common-0.4.1/PKG-INFO` & `xt_st_common-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.4.1
+Version: 0.5.0
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
-Requires-Python: >=3.10,<4.0
+Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: databases
 Provides-Extra: storage
-Requires-Dist: chardet (>=5.1.0,<6.0.0)
+Requires-Dist: botocore (>=1.29.140) ; extra == "databases"
+Requires-Dist: chardet (>=4.0.0,<6.0)
 Requires-Dist: minio (>=7.1.14,<8.0.0) ; extra == "storage"
-Requires-Dist: odmantic (>=0.9.2,<0.10.0) ; extra == "databases"
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: plotly (>=4.14.3)
+Requires-Dist: pydantic (>=1.10.7)
 Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
-Requires-Dist: streamlit (>=1.21.0,<2.0.0)
+Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
+Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
+Requires-Dist: streamlit (>=1.22.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.4.1
+# XT-STREAMLIT - 0.5.0
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
-### Getting Started
+## Getting Started User
+TODO: Installation guide and pointer to API docs
 
-This project recommends using [nox](https://nox.thea.codes/) as a tool for managing test environments and running scripts
+## Getting Started Developer
+TODO: Poetry primer
+
+This project recommends using [poethepoet](https://poethepoet.natn.io/index.html) as a tool for running tasks. See `pypoetry.toml`
 
 In your base python environment
 ``` bash
 pip install pipx # Pipx is a tool for installing python tools globally
-pipx install nox # Installs nox as a global tool
-pipx inject nox nox-poetry # Injects nox-poetry into the pipx venv that nox uses
+pipx install poethepoet # Installs poe as a global tool
+poe --help # Will show all the available tasks defined for this project
 ```
```

