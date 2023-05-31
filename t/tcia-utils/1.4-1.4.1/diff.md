# Comparing `tmp/tcia_utils-1.4.tar.gz` & `tmp/tcia_utils-1.4.1.tar.gz`

## Comparing `tcia_utils-1.4.tar` & `tcia_utils-1.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    51536 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.4/LICENSE
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 tcia_utils-1.4/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tcia_utils-1.4/pyproject.toml
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 tcia_utils-1.4/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    51403 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 tcia_utils-1.4.1/PKG-INFO
```

### Comparing `tcia_utils-1.4/src/tcia_utils/datacite.py` & `tcia_utils-1.4.1/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4/src/tcia_utils/nbia.py` & `tcia_utils-1.4.1/src/tcia_utils/nbia.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,43 +133,46 @@
 ####### getToken()
 # Retrieves security token to access APIs that require authorization
 # Provides interactive prompts for user/pw if they're not specified as parameters
 # Use getToken() for querying restricted collections with "Search API"
 # Use getToken(api_url = "nlst") for "Advanced API" queries of National Lung Screening Trial
 # Sets expiration time for tokens (2 hours from creation)
 
-def getToken(user = "", pw = "", api_url = ""):
+def getToken(user = "", pw = "", api_url = ""): 
 
     global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers
 
     # token URLs
-    token_url = "https://services.cancerimagingarchive.net/nbia-api/oauth/token?username="
-    nlst_token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token?username="
+    if api_url == "nlst":
+        token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token"
+    else:
+        token_url = "https://nbia.cancerimagingarchive.net/nbia-api/oauth/token"
 
     # set user name and password
     if user == "":
         print("Enter User: ")
         userName = input()
     else:
         userName = user
     if pw == "" and user != "nbia_guest":
         passWord = getpass.getpass(prompt = 'Enter Password: ')
     else:
         passWord = pw
 
     # create API token
-    if api_url == "nlst":
-        # create nlst token
-        url = nlst_token_url + userName + "&password=" + passWord + "&grant_type=password&client_id=nbiaRestAPIClient&client_secret=ItsBetweenUAndMe"
-    else:
-        # create regular token
-        url = token_url + userName + "&password=" + passWord + "&grant_type=password&client_id=nbiaRestAPIClient&client_secret=ItsBetweenUAndMe"
-
     try:
-        data = requests.get(url)
+        params = {
+        'client_id': 'nbiaRestAPIClient',
+        'client_secret' : 'ItsBetweenUAndMe',
+        'grant_type': 'password',
+        'username' : userName,
+        'password': passWord
+        }
+        
+        data = requests.post(token_url, data = params)
         data.raise_for_status()
         access_token = data.json()["access_token"]
         # track expiration status/time (2 hours from creation)
         current_time = datetime.now()
         if api_url == "nlst":
             nlst_token_exp_time = current_time + timedelta(hours=2)
             nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
```

### Comparing `tcia_utils-1.4/src/tcia_utils/pathdb.py` & `tcia_utils-1.4.1/src/tcia_utils/pathdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         df = pd.DataFrame(extracted_data)
         return df
     elif format == "csv":
         df = pd.DataFrame(extracted_data)
         today = datetime.now().strftime("%Y-%m-%d")
         filename = f"pathologyCollections-{today}.csv"
         df.to_csv(filename, index=False)
+        _log.info(f"File saved to {filename}.")
     else:
         return extracted_data
         
 ###################
 # getImages()
 # use "query" parameter to search collection names or enter a specific collection ID
 # returns JSON, but format parameter can be set to "df" for dataframe
```

### Comparing `tcia_utils-1.4/.gitignore` & `tcia_utils-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4/LICENSE` & `tcia_utils-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.4/README.md` & `tcia_utils-1.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,23 @@
 # Installation
 ```
 pip install tcia_utils
 ```
 
 # Usage
 
-To import functions related to the NBIA software, which holds TCIA's DICOM data:
+To import functions related to the NBIA software, which holds TCIA's DICOM radiology data:
 ```
 from tcia_utils import nbia
 ```
 
+To import functions related to the PathDB software, which holds TCIA's histopathology data:
+```
+from tcia_utils import pathdb
+```
+
 To import functions related to Datacite, which holds metadata and Digital Object Identifiers (DOIs) for TCIA datasets:
 ```
 from tcia_utils import datacite
 ```
 
 Example notebooks demonstrating tcia_utils functionality can be found at https://github.com/kirbyju/TCIA_Notebooks.
```

### Comparing `tcia_utils-1.4/pyproject.toml` & `tcia_utils-1.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.4"
+version = "1.4.1"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.4/PKG-INFO` & `tcia_utils-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.4
+Version: 1.4.1
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,23 @@
 # Installation
 ```
 pip install tcia_utils
 ```
 
 # Usage
 
-To import functions related to the NBIA software, which holds TCIA's DICOM data:
+To import functions related to the NBIA software, which holds TCIA's DICOM radiology data:
 ```
 from tcia_utils import nbia
 ```
 
+To import functions related to the PathDB software, which holds TCIA's histopathology data:
+```
+from tcia_utils import pathdb
+```
+
 To import functions related to Datacite, which holds metadata and Digital Object Identifiers (DOIs) for TCIA datasets:
 ```
 from tcia_utils import datacite
 ```
 
 Example notebooks demonstrating tcia_utils functionality can be found at https://github.com/kirbyju/TCIA_Notebooks.
```

