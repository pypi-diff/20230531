# Comparing `tmp/mecsimcalc-0.0.5.tar.gz` & `tmp/mecsimcalc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecsimcalc-0.0.5.tar", last modified: Thu May 18 07:57:43 2023, max compression
+gzip compressed data, was "mecsimcalc-0.1.0.tar", last modified: Wed May 31 21:39:58 2023, max compression
```

## Comparing `mecsimcalc-0.0.5.tar` & `mecsimcalc-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/mecsimcalc/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/mecsimcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/mecsimcalc/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/mecsimcalc/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/mecsimcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 07:57:43.000000 mecsimcalc-0.0.5/mecsimcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 07:57:43.875123 mecsimcalc-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-18 07:57:29.000000 mecsimcalc-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22654 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/mecsimcalc/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/spreadsheet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/mecsimcalc/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/mecsimcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 21:39:58.000000 mecsimcalc-0.1.0/mecsimcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:39:58.932139 mecsimcalc-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 21:39:47.000000 mecsimcalc-0.1.0/setup.py
```

### Comparing `mecsimcalc-0.0.5/LICENSE` & `mecsimcalc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mecsimcalc-0.0.5/PKG-INFO` & `mecsimcalc-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,145 +1,172 @@
-Metadata-Version: 2.1
-Name: mecsimcalc
-Version: 0.0.5
-Summary: Useful functions for MecSimCalc.com
-Author: MecSimCalc
-Author-email: <info@mecsimcalc.com>
-Keywords: python,MecSimCalc,Calculator,Simple
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-
-# Mecsimcalc 0.0.5 documentation
+# Mecsimcalc v0.1.0 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">decode_file_data</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL8C1-L30C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">input_to_file</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/general_utils.py#LL7C1-L31C61" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def decode_file_data(encoded_data, metadata = False)
+def input_to_file(input_file, metadata = False)
 ```
 
 #### Description:
 
-Converts a base64 encoded file into a file object and metadata
+Converts a base64 encoded string into a file object and metadata
 
 #### Arguments:
 
-| Argument           | Type                | Description                                                     |
-| ------------------ | ------------------- | --------------------------------------------------------------- |
-| **`encoded_data`** | **str**             | Base64 encoded file data                                        |
-| **`metadata`**     | **bool** (optional) | If True, function returns file and metadata (Defaults to False) |
+| Argument         | Type                | Description                                                |
+| ---------------- | ------------------- | ---------------------------------------------------------- |
+| **`input_file`** | **str**             | Base64 encoded string, prefixed with metadata              |
+| **`metadata`**   | **bool** (optional) | Flag to return metadata with the file. (Defaults to False) |
+
+#### Raises:
+
+| Exception        | Description                                                                        |
+| ---------------- | ---------------------------------------------------------------------------------- |
+| **`ValueError`** | If the input string doesn't contain ';base64,' to separate metadata and file data. |
 
 #### Returns:
 
-| Return Type             | Description                   | Condition         |
-| ----------------------- | ----------------------------- | ----------------- |
-| **`io.BytesIO`**        | The decoded file data         | metadata is False |
-| **`(io.BytesIO, str)`** | The decoded file and metadata | metadata is True  |
+| Return Type             | Description                                                              | Condition         |
+| ----------------------- | ------------------------------------------------------------------------ | ----------------- |
+| **`io.BytesIO`**        | The decoded file data (The thing you get when you open a file in Python) | metadata is False |
+| **`(io.BytesIO, str)`** | The decoded file data and its metadata                                   | metadata is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> file, metadata = decode_file_data(inputFile, metadata = True)
+>>> input_file = inputs['file']
+>>> file, metadata = input_to_file(input_file, metadata = True)
 >>> print(metadata)
 data:image/jpeg;base64,
 >>> type(file)
 <class '_io.BytesIO'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">download_text</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL182C1-L214C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">metadata_to_filetype</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/general_utils.py#LL34C1-L50C21" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+</div>
+
+```python
+def metadata_to_filetype(metadata):
+```
+
+#### Description:
+
+Extracts the file type from the metadata
+
+#### Arguments:
+
+| Argument       | Type    | Description                                                                                    |
+| -------------- | ------- | ---------------------------------------------------------------------------------------------- |
+| **`metadata`** | **str** | The metadata string in the form "Data:\<MIME type>;base64,"(returned from **`input_to_file`**) |
+
+#### Returns:
+
+| Return Type | Description                 |
+| ----------- | --------------------------- |
+| **`str`**   | The file type (e.g. "jpeg") |
+
+#### Example:
+
+```python
+>>> input_file = inputs['file']
+>>> file, metadata = input_to_file(input_file, metadata = True)
+>>> print(metadata)
+data:image/jpeg;base64,
+>>> download_file_type = metadata_to_filetype(metadata)
+>>> print(download_file_type)
+jpeg
+```
+
+## Text
+
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">string_to_file</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/text_utils.py#LL4C1-L34C85" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def download_text(
-    text: str,
-    filename: str = "myfile",
-    extension: str = ".txt",
-    download_text: str = "Download File",
-) -> str:
+def string_to_file(
+    text
+    filename= "myfile",
+    download_text = "Download File",
+)
 ```
 
 #### Description:
 
 Generates a downloadable text file containing the given text
 
 #### Arguments:
 
-| Argument            | Type               | Description                                                                   |
-| ------------------- | ------------------ | ----------------------------------------------------------------------------- |
-| **`text`**          | **str**            | The text to be downloaded                                                     |
-| **`filename`**      | **str** (optional) | The name of the file to be downloaded (Defaults to "myfile")                  |
-| **`extension`**     | **str** (optional) | The file extension of the file to be downloaded (Defaults to ".txt")          |
-| **`download_text`** | **str** (optional) | The text to be displayed on the download button (Defaults to "Download File") |
+| Argument            | Type               | Description                                                              |
+| ------------------- | ------------------ | ------------------------------------------------------------------------ |
+| **`text`**          | **str**            | Text to be downloaded                                                    |
+| **`filename`**      | **str** (optional) | Name of the download file. (Defaults to "myfile")                        |
+| **`download_text`** | **str** (optional) | Text to be displayed as the download link. (Defaults to "Download File") |
+
+#### Raises:
+
+| Exception       | Description                        |
+| --------------- | ---------------------------------- |
+| **`TypeError`** | If the input text is not a string. |
 
 #### Returns:
 
-| Return Type | Description                           |
-| ----------- | ------------------------------------- |
-| **`str`**   | The HTML code for the download button |
+| Return Type | Description        |
+| ----------- | ------------------ |
+| **`str`**   | HTML download link |
 
 #### Example:
 
 #### Python
 
 ```python
->>> downloadLink = download_text("Hello World!")
->>> return {"downloadLink": downloadLink}
+>>> download_link = string_to_file("Hello World!")
+>>> return {"download": download_link}
 ```
 
 #### Jinja2
 
 ```python
 # outputs.downloadLink is the html download link generated by the function
-{{ outputs.downloadLink }}
+{{ outputs.download }}
 ```
 
-## Tables/DataFrames
+## Spreadsheets
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">file_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL32C1-L52C14" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL9C1-L34C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def file_to_dataframe(file_data):
 ```
 
 #### Description:
 
-Converts a file object into a pandas DataFrame
+Converts a base64 encoded file data into a pandas DataFrame
 
 #### Arguments:
 
-| Argument        | Type           | Description                                          |
-| --------------- | -------------- | ---------------------------------------------------- |
-| **`file_data`** | **io.BytesIO** | Decoded file data (e.g. from **`decode_file_data`**) |
+| Argument        | Type           | Description                                       |
+| --------------- | -------------- | ------------------------------------------------- |
+| **`file_data`** | **io.BytesIO** | Decoded file data (e.g. from **`input_to_file`**) |
 
 #### Raises:
 
 | Exception                   | Description                                                                                                 |
 | --------------------------- | ----------------------------------------------------------------------------------------------------------- |
 | **`pd.errors.ParserError`** | If the file data cannot be converted to a DataFrame (i.e. file is not an Excel or CSV file or is corrupted) |
 
@@ -148,103 +175,107 @@
 | Return Type        | Description                      |
 | ------------------ | -------------------------------- |
 | **`pd.DataFrame`** | DataFrame created from file data |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> file = decode_file_data(inputFile)
->>> df = file_to_dataframe(file)
+>>> input_file = inputs['file']
+>>> decoded_file = input_to_file(input_file)
+>>> df = file_to_dataframe(decoded_file)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">input_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL55C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL35C1-L57C44" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def input_to_dataframe(file):
 ```
 
 #### Description:
 
 Converts a base64 encoded file data into a pandas DataFrame
 
 #### Arguments:
 
-| Argument   | Type    | Description              |
-| ---------- | ------- | ------------------------ |
-| **`file`** | **str** | Base64 encoded file data |
+| Argument            | Type     | Description                                                          |
+| ------------------- | -------- | -------------------------------------------------------------------- |
+| **`input_file`**    | **str**  | Base64 encoded file data                                             |
+| **`get_file_type`** | **bool** | If True, the function also returns the file type (Defaults to False) |
 
 #### Returns:
 
-| Return Type        | Description                      |
-| ------------------ | -------------------------------- |
-| **`pd.DataFrame`** | DataFrame created from file data |
+| Return Type               | Description                                      | Condition              |
+| ------------------------- | ------------------------------------------------ | ---------------------- |
+| **`pd.DataFrame`**        | DataFrame created from file data                 | get_file_type is False |
+| **`(pd.DataFrame, str)`** | Tuple containing the DataFrame and the file type | get_file_type is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> df = input_to_dataframe(inputFile)
+>>> input_file = inputs['file']
+>>> df, file_type = input_to_dataframe(input_file, get_file_type = True)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
+>>> print(file_type)
+csv
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL10C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL60C1-L119C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_dataframe(
     df,
     download = False,
-    DownloadText = "Download Table",
-    DownloadFileName = "mytable",
-    FileType = "csv",
+    download_text = "Download Table",
+    download_file_name = "mytable",
+    download_file_type = "csv",
 ):
 ```
 
 #### Description:
 
 Creates an HTML table and a download link for a given DataFrame
 
 #### Arguments:
 
-| Argument               | Type                | Description                                                             |
-| ---------------------- | ------------------- | ----------------------------------------------------------------------- |
-| **`df`**               | **pd.DataFrame**    | DataFrame to be converted                                               |
-| **`download`**         | **bool** (optional) | If True, function returns a download link (Defaults to False)           |
-| **`DownloadText`**     | **str** (optional)  | Text to be displayed as the download link (Defaults to "Download File") |
-| **`DownloadFileName`** | **str** (optional)  | Name of file when downloaded (Defaults to "myfile")                     |
-| **`FileType`**         | **str** (optional)  | File type of download (Defaults to "csv")                               |
+| Argument                 | Type                | Description                                                             |
+| ------------------------ | ------------------- | ----------------------------------------------------------------------- |
+| **`df`**                 | **pd.DataFrame**    | DataFrame to be converted                                               |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)           |
+| **`download_text`**      | **str** (optional)  | Text to be displayed as the download link (Defaults to "Download File") |
+| **`download_file_name`** | **str** (optional)  | Name of file when downloaded (Defaults to "myfile")                     |
+| **`download_file_type`** | **str** (optional)  | File type of downloaded file (Defaults to "csv")                        |
 
 #### Returns:
 
-| Return Type           | Description                 | Condition         |
-| --------------------- | --------------------------- | ----------------- |
-| **`str`**             | HTML table                  | download is False |
-| **`Tuple[str, str]`** | (HTML table, download link) | download is True  |
+| Return Type           | Description                      | Condition         |
+| --------------------- | -------------------------------- | ----------------- |
+| **`str`**             | HTML table                       | download is False |
+| **`Tuple[str, str]`** | (HTML table, HTML download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> inputFile = inputs['file']
->>> df = input_to_dataframe(inputFile)
->>> table, download = print_dataframe(df, download = True, DownloadFileName = "FunkyTable", DownloadText = "Download My Funky Table HERE!", FileType = "xlsx")
+>>> input_file = inputs['file']
+>>> df = input_to_dataframe(input_file)
+>>> table, download = print_dataframe(df, download = True, download_file_name = "FunkyTable", download_text = "Download My Funky Table HERE!", download_file_type = "xlsx")
 >>> return {
         "table":table,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
@@ -257,85 +288,87 @@
 # outputs.download is the download link
 Downloading Table
 {{ outputs.download }}
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">table_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL89C1-L105C35 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/table_utils.py#LL4C1-L26C54" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
+## Tables
+
 ```python
-def table_to_dataframe(columns: List[List[str]], column_headers: List[str]) -> pd.DataFrame:
+def table_to_dataframe(column_headers, rows) -> pd.DataFrame:
 ```
 
 #### Description:
 
-Creates a DataFrame from given columns and headers
+Create a DataFrame from given rows and column headers
 
 #### Arguments:
 
-| Argument             | Type                | Description                                                                        |
-| -------------------- | ------------------- | ---------------------------------------------------------------------------------- |
-| **`columns`**        | **List[List[str]]** | List of columns to be converted into a DataFrame. Each column is a list of strings |
-| **`column_headers`** | **List[str]**       | List of column headers                                                             |
+| Argument             | Type                | Description                                                                     |
+| -------------------- | ------------------- | ------------------------------------------------------------------------------- |
+| **`column_headers`** | **List[str]**       | List of column headers                                                          |
+| **`rows`**           | **List[List[str]]** | List of rows to be converted into a DataFrame. Each column is a list of strings |
 
 #### Returns:
 
-| Return Type        | Description                                |
-| ------------------ | ------------------------------------------ |
-| **`pd.DataFrame`** | DataFrame created from columns and headers |
+| Return Type        | Description                             |
+| ------------------ | --------------------------------------- |
+| **`pd.DataFrame`** | DataFrame created from headers and rows |
 
 #### Example:
 
 ```python
->>> columns = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
->>> df = table_to_dataframe(columns, column_headers)
+>>> rows = [["a", "b", "c"], ["d", "e", "f"]]
+>>> df = table_to_dataframe(column_headers, rows)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
 
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_table</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL216C1-L240C114" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/table_utils.py#LL29C1-L44C58" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-print_table(rows: List[List[str]], column_headers: List[str]):
+print_table(column_headers, rows):
 ```
 
 #### Description:
 
 Creates an HTML table from given rows and column headers
 
 #### Arguments:
 
 | Argument             | Type                | Description                                                                 |
 | -------------------- | ------------------- | --------------------------------------------------------------------------- |
-| **`rows`**           | **List[List[str]]** | List of rows to be converted into a table. Each column is a list of strings |
 | **`column_headers`** | **List[str]**       | List of column headers                                                      |
+| **`rows`**           | **List[List[str]]** | List of rows to be converted into a table. Each column is a list of strings |
 
 #### Returns:
 
 | Return Type | Description                              |
 | ----------- | ---------------------------------------- |
 | **`str`**   | HTML table created from rows and headers |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> rows = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
->>> table = print_table(rows, column_headers)
+>>> rows = [["a", "b", "c"], ["d", "e", "f"]]
+>>> table = print_table(column_headers, rows)
 >>> return {
         "table":table,
     }
 ```
 
 #### Output using Jinja2 Template:
 
@@ -344,99 +377,153 @@
 Displaying Table
 {{ outputs.table }}
 ```
 
 ## Images
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">file_to_PIL</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL13C1-L30C88" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+</div>
+
+```python
+def file_to_PIL(file):
+```
+
+#### Description:
+
+Transforms a file into a Pillow Image object
+
+#### Arguments:
+
+| Argument   | Type    | Description                                     |
+| ---------- | ------- | ----------------------------------------------- |
+| **`file`** | **str** | Decoded file data (returned from input_to_file) |
+
+#### Raises:
+
+| Exception Type   | Description                             |
+| ---------------- | --------------------------------------- |
+| **`ValueError`** | If the file does not contain image data |
+
+#### Returns:
+
+| Return Type | Description         |
+| ----------- | ------------------- |
+| **`Image`** | Pillow Image object |
+
+#### Example:
+
+#### Python Code:
+
+```python
+>>> input_file = inputs['file']
+>>> decoded_file = input_to_file(input_file)
+>>> image = file_to_PIL(decoded_file)
+>>> return {
+        "image":image,
+    }
+```
+
+#### Output using Jinja2 Template:
+
+```python
+# outputs.image is the Pillow Image object
+Displaying Image
+{{ outputs.image }}
+```
+
+<div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">input_to_PIL</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL70C1-L87C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL33C1-L57C15" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def input_to_PIL(file):
+def input_to_PIL(input_file, get_file_type=False):
 ```
 
 #### Description:
 
 Converts a base64 encoded file data into a pillow image
 
 #### Arguments:
 
-| Argument   | Type    | Description              |
-| ---------- | ------- | ------------------------ |
-| **`file`** | **str** | Base64 encoded file data |
+| Argument            | Type     | Description                                                          |
+| ------------------- | -------- | -------------------------------------------------------------------- |
+| **`input_file`**    | **str**  | Base64 encoded file data                                             |
+| **`get_file_type`** | **bool** | If True, the function also returns the file type (Defaults to False) |
 
 #### Returns:
 
-| Return Type                       | Description              |
-| --------------------------------- | ------------------------ |
-| **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) |
+| Return Type                       | Description              | Condition              |
+| --------------------------------- | ------------------------ | ---------------------- |
+| **`PIL.Image.Image`**             | Pillow Image object      | get_file_type is False |
+| **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) | get_file_type is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> img, metadata = input_to_PIL(inputFile)
->>> print(metadata)
-data:image/jpeg;base64,
->>> type(file)
+>>> input_file = inputs['file']
+>>> img, file_type = input_to_PIL(input_file, get_file_type=True)
+>>> print(file_type)
+jpeg
+>>> type(img)
 <class 'PIL.JpegImagePlugin.JpegImageFile'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_img</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL70C1-L129C1 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL60C1-L126C32" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_img(
     img,
-    metadata,
-    WIDTH = 200,
-    HEIGHT = 200,
-    OriginalSize = False,
+    width = 200,
+    height = 200,
+    original_size = False,
     download = False,
-    DownloadText = "Download Image",
-    ImageName= "myimg",
+    download_text = "Download Image",
+    download_file_name= "myimg",
+    download_file_type = "png",
 ):
 ```
 
 #### Description:
 
-Converts a pillow image into an HTML image and a download link
+Transforms a Pillow image into an HTML image, with an optional download link
 
 #### Arguments:
 
-| Argument           | Type                | Description                                                                        |
-| ------------------ | ------------------- | ---------------------------------------------------------------------------------- |
-| **`img`**          | **PIL.Image.Image** | Pillow image                                                                       |
-| **`metadata`**     | **str**             | Image metadata                                                                     |
-| **`WIDTH`**        | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
-| **`HEIGHT`**       | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
-| **`OriginalSize`** | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
-| **`download`**     | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
-| **`DownloadText`** | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
-| **`ImageName`**    | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
+| Argument                 | Type                | Description                                                                        |
+| ------------------------ | ------------------- | ---------------------------------------------------------------------------------- |
+| **`img`**                | **PIL.Image.Image** | Pillow image                                                                       |
+| **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
+| **`height`**             | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
+| **`original_size`**      | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
+| **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
+| **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
+| **`download_file_type`** | **str** (optional)  | The file type of the image when downloaded (Defaults to "png")                     |
 
 #### Returns:
 
 | Return Type           | Description                 | Condition         |
 | --------------------- | --------------------------- | ----------------- |
 | **`str`**             | HTML image                  | download is False |
 | **`Tuple[str, str]`** | (HTML image, download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> inputFile = inputs['file']
->>> img, metadata = input_to_PIL(inputFile)
->>> image, download = print_img(img, metadata, OriginalSize = True, download = True, DownloadText = "Download Image Here", ImageName = "myimage")
+>>> input_file = inputs['file']
+>>> img, metadata = input_to_PIL(input_file)
+>>> image, download = print_img(img,, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
 >>> return {
         "image":image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
@@ -447,65 +534,67 @@
 {{ outputs.image }}
 
 # outputs.download is the download link
 Downloading Image
 {{ outputs.download }}
 ```
 
+## Plots
+
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">print_plt</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL131C1-L180C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">print_plot</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/plotting_utils.py#LL8C1-L63C35" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def print_plt(
-    plt:,
+def print_plot(
+    plot_obj,
     width = 500,
     dpi= 100,
     download= False,
-    DownloadText = "Download Plot",
-    DownloadFileName = "myplot",
+    download_text = "Download Plot",
+    download_file_name = "myplot",
 )
 ```
 
 #### Description:
 
-Converts a matplotlib.pyplot or matplotlib.figure into an HTML image tag and optionally provides a download link for the image
+Converts a matplotlib.pyplot.axis or matplotlib.figure into an HTML image tag and optionally provides a download link for the image
 
 #### Arguments:
 
-| Argument               | Type                | Description                                                                 |
-| ---------------------- | ------------------- | --------------------------------------------------------------------------- |
-| **`plt`**              | **plt or figure**   | Matplotlib figure                                                           |
-| **`width`**            | **int** (optional)  | Output width of the image in pixels (Defaults to 500)                       |
-| **`dpi`**              | **int** (optional)  | Output dpi of the image in pixels (Defaults to 100)                         |
-| **`download`**         | **bool** (optional) | If True, function returns a download link (Defaults to False)               |
-| **`DownloadText`**     | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Plot") |
-| **`DownloadFileName`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myplot")           |
+| Argument                 | Type                | Description                                                                 |
+| ------------------------ | ------------------- | --------------------------------------------------------------------------- |
+| **`plot_obj`**           | **axes or figure**  | Matplotlib figure                                                           |
+| **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 500)                       |
+| **`dpi`**                | **int** (optional)  | Output dpi of the image in pixels (Defaults to 100)                         |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)               |
+| **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Plot") |
+| **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myplot")           |
 
 #### Returns:
 
-| Return Type           | Description                 | Condition         |
-| --------------------- | --------------------------- | ----------------- |
-| **`str`**             | HTML image                  | download is False |
-| **`Tuple[str, str]`** | (HTML image, download link) | download is True  |
+| Return Type           | Description                      | Condition         |
+| --------------------- | -------------------------------- | ----------------- |
+| **`str`**             | HTML image                       | download is False |
+| **`Tuple[str, str]`** | (HTML image, HTML download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
 >>> import matplotlib.pyplot as plt
 >>> import numpy as np
 >>> x = np.linspace(0, 2 * np.pi, 400)
 >>> y = np.sin(x)
 >>> fig, ax = plt.subplots()
 >>> ax.plot(x, y)
 >>> ax.set_title('A single plot')
->>> image, download = print_plt(fig, width = 500, dpi = 100, download = True, DownloadText = "Download Sin Function Plot", DownloadFileName = "sin(x)")
+>>> image, download = print_plot(fig, width = 500, dpi = 100, download = True, download_text = "Download Sin Function Plot", download_file_name = "sin(x)")
 >>> return {
         "image":image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
```

### Comparing `mecsimcalc-0.0.5/README.md` & `mecsimcalc-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,195 @@
-# Mecsimcalc 0.0.5 documentation
+Metadata-Version: 2.1
+Name: mecsimcalc
+Version: 0.1.0
+Summary: Useful functions for MecSimCalc.com
+Author: MecSimCalc
+Author-email: <info@mecsimcalc.com>
+Keywords: python,MecSimCalc,Calculator,Simple
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+
+# Mecsimcalc v0.1.0 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">decode_file_data</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL8C1-L30C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">input_to_file</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/general_utils.py#LL7C1-L31C61" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def decode_file_data(encoded_data, metadata = False)
+def input_to_file(input_file, metadata = False)
 ```
 
 #### Description:
 
-Converts a base64 encoded file into a file object and metadata
+Converts a base64 encoded string into a file object and metadata
 
 #### Arguments:
 
-| Argument           | Type                | Description                                                     |
-| ------------------ | ------------------- | --------------------------------------------------------------- |
-| **`encoded_data`** | **str**             | Base64 encoded file data                                        |
-| **`metadata`**     | **bool** (optional) | If True, function returns file and metadata (Defaults to False) |
+| Argument         | Type                | Description                                                |
+| ---------------- | ------------------- | ---------------------------------------------------------- |
+| **`input_file`** | **str**             | Base64 encoded string, prefixed with metadata              |
+| **`metadata`**   | **bool** (optional) | Flag to return metadata with the file. (Defaults to False) |
+
+#### Raises:
+
+| Exception        | Description                                                                        |
+| ---------------- | ---------------------------------------------------------------------------------- |
+| **`ValueError`** | If the input string doesn't contain ';base64,' to separate metadata and file data. |
 
 #### Returns:
 
-| Return Type             | Description                   | Condition         |
-| ----------------------- | ----------------------------- | ----------------- |
-| **`io.BytesIO`**        | The decoded file data         | metadata is False |
-| **`(io.BytesIO, str)`** | The decoded file and metadata | metadata is True  |
+| Return Type             | Description                                                              | Condition         |
+| ----------------------- | ------------------------------------------------------------------------ | ----------------- |
+| **`io.BytesIO`**        | The decoded file data (The thing you get when you open a file in Python) | metadata is False |
+| **`(io.BytesIO, str)`** | The decoded file data and its metadata                                   | metadata is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> file, metadata = decode_file_data(inputFile, metadata = True)
+>>> input_file = inputs['file']
+>>> file, metadata = input_to_file(input_file, metadata = True)
 >>> print(metadata)
 data:image/jpeg;base64,
 >>> type(file)
 <class '_io.BytesIO'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">download_text</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL182C1-L214C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">metadata_to_filetype</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/general_utils.py#LL34C1-L50C21" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+</div>
+
+```python
+def metadata_to_filetype(metadata):
+```
+
+#### Description:
+
+Extracts the file type from the metadata
+
+#### Arguments:
+
+| Argument       | Type    | Description                                                                                    |
+| -------------- | ------- | ---------------------------------------------------------------------------------------------- |
+| **`metadata`** | **str** | The metadata string in the form "Data:\<MIME type>;base64,"(returned from **`input_to_file`**) |
+
+#### Returns:
+
+| Return Type | Description                 |
+| ----------- | --------------------------- |
+| **`str`**   | The file type (e.g. "jpeg") |
+
+#### Example:
+
+```python
+>>> input_file = inputs['file']
+>>> file, metadata = input_to_file(input_file, metadata = True)
+>>> print(metadata)
+data:image/jpeg;base64,
+>>> download_file_type = metadata_to_filetype(metadata)
+>>> print(download_file_type)
+jpeg
+```
+
+## Text
+
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">string_to_file</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/text_utils.py#LL4C1-L34C85" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def download_text(
-    text: str,
-    filename: str = "myfile",
-    extension: str = ".txt",
-    download_text: str = "Download File",
-) -> str:
+def string_to_file(
+    text
+    filename= "myfile",
+    download_text = "Download File",
+)
 ```
 
 #### Description:
 
 Generates a downloadable text file containing the given text
 
 #### Arguments:
 
-| Argument            | Type               | Description                                                                   |
-| ------------------- | ------------------ | ----------------------------------------------------------------------------- |
-| **`text`**          | **str**            | The text to be downloaded                                                     |
-| **`filename`**      | **str** (optional) | The name of the file to be downloaded (Defaults to "myfile")                  |
-| **`extension`**     | **str** (optional) | The file extension of the file to be downloaded (Defaults to ".txt")          |
-| **`download_text`** | **str** (optional) | The text to be displayed on the download button (Defaults to "Download File") |
+| Argument            | Type               | Description                                                              |
+| ------------------- | ------------------ | ------------------------------------------------------------------------ |
+| **`text`**          | **str**            | Text to be downloaded                                                    |
+| **`filename`**      | **str** (optional) | Name of the download file. (Defaults to "myfile")                        |
+| **`download_text`** | **str** (optional) | Text to be displayed as the download link. (Defaults to "Download File") |
+
+#### Raises:
+
+| Exception       | Description                        |
+| --------------- | ---------------------------------- |
+| **`TypeError`** | If the input text is not a string. |
 
 #### Returns:
 
-| Return Type | Description                           |
-| ----------- | ------------------------------------- |
-| **`str`**   | The HTML code for the download button |
+| Return Type | Description        |
+| ----------- | ------------------ |
+| **`str`**   | HTML download link |
 
 #### Example:
 
 #### Python
 
 ```python
->>> downloadLink = download_text("Hello World!")
->>> return {"downloadLink": downloadLink}
+>>> download_link = string_to_file("Hello World!")
+>>> return {"download": download_link}
 ```
 
 #### Jinja2
 
 ```python
 # outputs.downloadLink is the html download link generated by the function
-{{ outputs.downloadLink }}
+{{ outputs.download }}
 ```
 
-## Tables/DataFrames
+## Spreadsheets
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">file_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL32C1-L52C14" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL9C1-L34C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def file_to_dataframe(file_data):
 ```
 
 #### Description:
 
-Converts a file object into a pandas DataFrame
+Converts a base64 encoded file data into a pandas DataFrame
 
 #### Arguments:
 
-| Argument        | Type           | Description                                          |
-| --------------- | -------------- | ---------------------------------------------------- |
-| **`file_data`** | **io.BytesIO** | Decoded file data (e.g. from **`decode_file_data`**) |
+| Argument        | Type           | Description                                       |
+| --------------- | -------------- | ------------------------------------------------- |
+| **`file_data`** | **io.BytesIO** | Decoded file data (e.g. from **`input_to_file`**) |
 
 #### Raises:
 
 | Exception                   | Description                                                                                                 |
 | --------------------------- | ----------------------------------------------------------------------------------------------------------- |
 | **`pd.errors.ParserError`** | If the file data cannot be converted to a DataFrame (i.e. file is not an Excel or CSV file or is corrupted) |
 
@@ -126,103 +198,107 @@
 | Return Type        | Description                      |
 | ------------------ | -------------------------------- |
 | **`pd.DataFrame`** | DataFrame created from file data |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> file = decode_file_data(inputFile)
->>> df = file_to_dataframe(file)
+>>> input_file = inputs['file']
+>>> decoded_file = input_to_file(input_file)
+>>> df = file_to_dataframe(decoded_file)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">input_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL55C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL35C1-L57C44" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def input_to_dataframe(file):
 ```
 
 #### Description:
 
 Converts a base64 encoded file data into a pandas DataFrame
 
 #### Arguments:
 
-| Argument   | Type    | Description              |
-| ---------- | ------- | ------------------------ |
-| **`file`** | **str** | Base64 encoded file data |
+| Argument            | Type     | Description                                                          |
+| ------------------- | -------- | -------------------------------------------------------------------- |
+| **`input_file`**    | **str**  | Base64 encoded file data                                             |
+| **`get_file_type`** | **bool** | If True, the function also returns the file type (Defaults to False) |
 
 #### Returns:
 
-| Return Type        | Description                      |
-| ------------------ | -------------------------------- |
-| **`pd.DataFrame`** | DataFrame created from file data |
+| Return Type               | Description                                      | Condition              |
+| ------------------------- | ------------------------------------------------ | ---------------------- |
+| **`pd.DataFrame`**        | DataFrame created from file data                 | get_file_type is False |
+| **`(pd.DataFrame, str)`** | Tuple containing the DataFrame and the file type | get_file_type is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> df = input_to_dataframe(inputFile)
+>>> input_file = inputs['file']
+>>> df, file_type = input_to_dataframe(input_file, get_file_type = True)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
+>>> print(file_type)
+csv
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL10C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL60C1-L119C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_dataframe(
     df,
     download = False,
-    DownloadText = "Download Table",
-    DownloadFileName = "mytable",
-    FileType = "csv",
+    download_text = "Download Table",
+    download_file_name = "mytable",
+    download_file_type = "csv",
 ):
 ```
 
 #### Description:
 
 Creates an HTML table and a download link for a given DataFrame
 
 #### Arguments:
 
-| Argument               | Type                | Description                                                             |
-| ---------------------- | ------------------- | ----------------------------------------------------------------------- |
-| **`df`**               | **pd.DataFrame**    | DataFrame to be converted                                               |
-| **`download`**         | **bool** (optional) | If True, function returns a download link (Defaults to False)           |
-| **`DownloadText`**     | **str** (optional)  | Text to be displayed as the download link (Defaults to "Download File") |
-| **`DownloadFileName`** | **str** (optional)  | Name of file when downloaded (Defaults to "myfile")                     |
-| **`FileType`**         | **str** (optional)  | File type of download (Defaults to "csv")                               |
+| Argument                 | Type                | Description                                                             |
+| ------------------------ | ------------------- | ----------------------------------------------------------------------- |
+| **`df`**                 | **pd.DataFrame**    | DataFrame to be converted                                               |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)           |
+| **`download_text`**      | **str** (optional)  | Text to be displayed as the download link (Defaults to "Download File") |
+| **`download_file_name`** | **str** (optional)  | Name of file when downloaded (Defaults to "myfile")                     |
+| **`download_file_type`** | **str** (optional)  | File type of downloaded file (Defaults to "csv")                        |
 
 #### Returns:
 
-| Return Type           | Description                 | Condition         |
-| --------------------- | --------------------------- | ----------------- |
-| **`str`**             | HTML table                  | download is False |
-| **`Tuple[str, str]`** | (HTML table, download link) | download is True  |
+| Return Type           | Description                      | Condition         |
+| --------------------- | -------------------------------- | ----------------- |
+| **`str`**             | HTML table                       | download is False |
+| **`Tuple[str, str]`** | (HTML table, HTML download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> inputFile = inputs['file']
->>> df = input_to_dataframe(inputFile)
->>> table, download = print_dataframe(df, download = True, DownloadFileName = "FunkyTable", DownloadText = "Download My Funky Table HERE!", FileType = "xlsx")
+>>> input_file = inputs['file']
+>>> df = input_to_dataframe(input_file)
+>>> table, download = print_dataframe(df, download = True, download_file_name = "FunkyTable", download_text = "Download My Funky Table HERE!", download_file_type = "xlsx")
 >>> return {
         "table":table,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
@@ -235,85 +311,87 @@
 # outputs.download is the download link
 Downloading Table
 {{ outputs.download }}
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">table_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL89C1-L105C35 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/table_utils.py#LL4C1-L26C54" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
+## Tables
+
 ```python
-def table_to_dataframe(columns: List[List[str]], column_headers: List[str]) -> pd.DataFrame:
+def table_to_dataframe(column_headers, rows) -> pd.DataFrame:
 ```
 
 #### Description:
 
-Creates a DataFrame from given columns and headers
+Create a DataFrame from given rows and column headers
 
 #### Arguments:
 
-| Argument             | Type                | Description                                                                        |
-| -------------------- | ------------------- | ---------------------------------------------------------------------------------- |
-| **`columns`**        | **List[List[str]]** | List of columns to be converted into a DataFrame. Each column is a list of strings |
-| **`column_headers`** | **List[str]**       | List of column headers                                                             |
+| Argument             | Type                | Description                                                                     |
+| -------------------- | ------------------- | ------------------------------------------------------------------------------- |
+| **`column_headers`** | **List[str]**       | List of column headers                                                          |
+| **`rows`**           | **List[List[str]]** | List of rows to be converted into a DataFrame. Each column is a list of strings |
 
 #### Returns:
 
-| Return Type        | Description                                |
-| ------------------ | ------------------------------------------ |
-| **`pd.DataFrame`** | DataFrame created from columns and headers |
+| Return Type        | Description                             |
+| ------------------ | --------------------------------------- |
+| **`pd.DataFrame`** | DataFrame created from headers and rows |
 
 #### Example:
 
 ```python
->>> columns = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
->>> df = table_to_dataframe(columns, column_headers)
+>>> rows = [["a", "b", "c"], ["d", "e", "f"]]
+>>> df = table_to_dataframe(column_headers, rows)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
 
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_table</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL216C1-L240C114" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/table_utils.py#LL29C1-L44C58" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-print_table(rows: List[List[str]], column_headers: List[str]):
+print_table(column_headers, rows):
 ```
 
 #### Description:
 
 Creates an HTML table from given rows and column headers
 
 #### Arguments:
 
 | Argument             | Type                | Description                                                                 |
 | -------------------- | ------------------- | --------------------------------------------------------------------------- |
-| **`rows`**           | **List[List[str]]** | List of rows to be converted into a table. Each column is a list of strings |
 | **`column_headers`** | **List[str]**       | List of column headers                                                      |
+| **`rows`**           | **List[List[str]]** | List of rows to be converted into a table. Each column is a list of strings |
 
 #### Returns:
 
 | Return Type | Description                              |
 | ----------- | ---------------------------------------- |
 | **`str`**   | HTML table created from rows and headers |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> rows = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
->>> table = print_table(rows, column_headers)
+>>> rows = [["a", "b", "c"], ["d", "e", "f"]]
+>>> table = print_table(column_headers, rows)
 >>> return {
         "table":table,
     }
 ```
 
 #### Output using Jinja2 Template:
 
@@ -322,99 +400,153 @@
 Displaying Table
 {{ outputs.table }}
 ```
 
 ## Images
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">file_to_PIL</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL13C1-L30C88" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+</div>
+
+```python
+def file_to_PIL(file):
+```
+
+#### Description:
+
+Transforms a file into a Pillow Image object
+
+#### Arguments:
+
+| Argument   | Type    | Description                                     |
+| ---------- | ------- | ----------------------------------------------- |
+| **`file`** | **str** | Decoded file data (returned from input_to_file) |
+
+#### Raises:
+
+| Exception Type   | Description                             |
+| ---------------- | --------------------------------------- |
+| **`ValueError`** | If the file does not contain image data |
+
+#### Returns:
+
+| Return Type | Description         |
+| ----------- | ------------------- |
+| **`Image`** | Pillow Image object |
+
+#### Example:
+
+#### Python Code:
+
+```python
+>>> input_file = inputs['file']
+>>> decoded_file = input_to_file(input_file)
+>>> image = file_to_PIL(decoded_file)
+>>> return {
+        "image":image,
+    }
+```
+
+#### Output using Jinja2 Template:
+
+```python
+# outputs.image is the Pillow Image object
+Displaying Image
+{{ outputs.image }}
+```
+
+<div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">input_to_PIL</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL70C1-L87C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL33C1-L57C15" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def input_to_PIL(file):
+def input_to_PIL(input_file, get_file_type=False):
 ```
 
 #### Description:
 
 Converts a base64 encoded file data into a pillow image
 
 #### Arguments:
 
-| Argument   | Type    | Description              |
-| ---------- | ------- | ------------------------ |
-| **`file`** | **str** | Base64 encoded file data |
+| Argument            | Type     | Description                                                          |
+| ------------------- | -------- | -------------------------------------------------------------------- |
+| **`input_file`**    | **str**  | Base64 encoded file data                                             |
+| **`get_file_type`** | **bool** | If True, the function also returns the file type (Defaults to False) |
 
 #### Returns:
 
-| Return Type                       | Description              |
-| --------------------------------- | ------------------------ |
-| **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) |
+| Return Type                       | Description              | Condition              |
+| --------------------------------- | ------------------------ | ---------------------- |
+| **`PIL.Image.Image`**             | Pillow Image object      | get_file_type is False |
+| **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) | get_file_type is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> img, metadata = input_to_PIL(inputFile)
->>> print(metadata)
-data:image/jpeg;base64,
->>> type(file)
+>>> input_file = inputs['file']
+>>> img, file_type = input_to_PIL(input_file, get_file_type=True)
+>>> print(file_type)
+jpeg
+>>> type(img)
 <class 'PIL.JpegImagePlugin.JpegImageFile'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_img</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL70C1-L129C1 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL60C1-L126C32" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_img(
     img,
-    metadata,
-    WIDTH = 200,
-    HEIGHT = 200,
-    OriginalSize = False,
+    width = 200,
+    height = 200,
+    original_size = False,
     download = False,
-    DownloadText = "Download Image",
-    ImageName= "myimg",
+    download_text = "Download Image",
+    download_file_name= "myimg",
+    download_file_type = "png",
 ):
 ```
 
 #### Description:
 
-Converts a pillow image into an HTML image and a download link
+Transforms a Pillow image into an HTML image, with an optional download link
 
 #### Arguments:
 
-| Argument           | Type                | Description                                                                        |
-| ------------------ | ------------------- | ---------------------------------------------------------------------------------- |
-| **`img`**          | **PIL.Image.Image** | Pillow image                                                                       |
-| **`metadata`**     | **str**             | Image metadata                                                                     |
-| **`WIDTH`**        | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
-| **`HEIGHT`**       | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
-| **`OriginalSize`** | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
-| **`download`**     | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
-| **`DownloadText`** | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
-| **`ImageName`**    | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
+| Argument                 | Type                | Description                                                                        |
+| ------------------------ | ------------------- | ---------------------------------------------------------------------------------- |
+| **`img`**                | **PIL.Image.Image** | Pillow image                                                                       |
+| **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
+| **`height`**             | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
+| **`original_size`**      | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
+| **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
+| **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
+| **`download_file_type`** | **str** (optional)  | The file type of the image when downloaded (Defaults to "png")                     |
 
 #### Returns:
 
 | Return Type           | Description                 | Condition         |
 | --------------------- | --------------------------- | ----------------- |
 | **`str`**             | HTML image                  | download is False |
 | **`Tuple[str, str]`** | (HTML image, download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> inputFile = inputs['file']
->>> img, metadata = input_to_PIL(inputFile)
->>> image, download = print_img(img, metadata, OriginalSize = True, download = True, DownloadText = "Download Image Here", ImageName = "myimage")
+>>> input_file = inputs['file']
+>>> img, metadata = input_to_PIL(input_file)
+>>> image, download = print_img(img,, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
 >>> return {
         "image":image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
@@ -425,65 +557,67 @@
 {{ outputs.image }}
 
 # outputs.download is the download link
 Downloading Image
 {{ outputs.download }}
 ```
 
+## Plots
+
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">print_plt</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL131C1-L180C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">print_plot</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/plotting_utils.py#LL8C1-L63C35" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def print_plt(
-    plt:,
+def print_plot(
+    plot_obj,
     width = 500,
     dpi= 100,
     download= False,
-    DownloadText = "Download Plot",
-    DownloadFileName = "myplot",
+    download_text = "Download Plot",
+    download_file_name = "myplot",
 )
 ```
 
 #### Description:
 
-Converts a matplotlib.pyplot or matplotlib.figure into an HTML image tag and optionally provides a download link for the image
+Converts a matplotlib.pyplot.axis or matplotlib.figure into an HTML image tag and optionally provides a download link for the image
 
 #### Arguments:
 
-| Argument               | Type                | Description                                                                 |
-| ---------------------- | ------------------- | --------------------------------------------------------------------------- |
-| **`plt`**              | **plt or figure**   | Matplotlib figure                                                           |
-| **`width`**            | **int** (optional)  | Output width of the image in pixels (Defaults to 500)                       |
-| **`dpi`**              | **int** (optional)  | Output dpi of the image in pixels (Defaults to 100)                         |
-| **`download`**         | **bool** (optional) | If True, function returns a download link (Defaults to False)               |
-| **`DownloadText`**     | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Plot") |
-| **`DownloadFileName`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myplot")           |
+| Argument                 | Type                | Description                                                                 |
+| ------------------------ | ------------------- | --------------------------------------------------------------------------- |
+| **`plot_obj`**           | **axes or figure**  | Matplotlib figure                                                           |
+| **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 500)                       |
+| **`dpi`**                | **int** (optional)  | Output dpi of the image in pixels (Defaults to 100)                         |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)               |
+| **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Plot") |
+| **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myplot")           |
 
 #### Returns:
 
-| Return Type           | Description                 | Condition         |
-| --------------------- | --------------------------- | ----------------- |
-| **`str`**             | HTML image                  | download is False |
-| **`Tuple[str, str]`** | (HTML image, download link) | download is True  |
+| Return Type           | Description                      | Condition         |
+| --------------------- | -------------------------------- | ----------------- |
+| **`str`**             | HTML image                       | download is False |
+| **`Tuple[str, str]`** | (HTML image, HTML download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
 >>> import matplotlib.pyplot as plt
 >>> import numpy as np
 >>> x = np.linspace(0, 2 * np.pi, 400)
 >>> y = np.sin(x)
 >>> fig, ax = plt.subplots()
 >>> ax.plot(x, y)
 >>> ax.set_title('A single plot')
->>> image, download = print_plt(fig, width = 500, dpi = 100, download = True, DownloadText = "Download Sin Function Plot", DownloadFileName = "sin(x)")
+>>> image, download = print_plot(fig, width = 500, dpi = 100, download = True, download_text = "Download Sin Function Plot", download_file_name = "sin(x)")
 >>> return {
         "image":image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
```

### Comparing `mecsimcalc-0.0.5/mecsimcalc.egg-info/PKG-INFO` & `mecsimcalc-0.1.0/mecsimcalc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,145 +1,195 @@
 Metadata-Version: 2.1
 Name: mecsimcalc
-Version: 0.0.5
+Version: 0.1.0
 Summary: Useful functions for MecSimCalc.com
 Author: MecSimCalc
 Author-email: <info@mecsimcalc.com>
 Keywords: python,MecSimCalc,Calculator,Simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Mecsimcalc 0.0.5 documentation
+# Mecsimcalc v0.1.0 documentation
 
 This library is designed to provide a set of functions for handling and converting various types of data, such as base64 encoded data, Pandas DataFrames, and Pillow images.
 
 - [GitHub Repository](https://github.com/MecSimCalc/MecSimCalc-utils)
 - [PyPi Page](https://pypi.org/project/mecsimcalc/)
 
 ## General
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">decode_file_data</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL8C1-L30C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">input_to_file</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/general_utils.py#LL7C1-L31C61" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def decode_file_data(encoded_data, metadata = False)
+def input_to_file(input_file, metadata = False)
 ```
 
 #### Description:
 
-Converts a base64 encoded file into a file object and metadata
+Converts a base64 encoded string into a file object and metadata
 
 #### Arguments:
 
-| Argument           | Type                | Description                                                     |
-| ------------------ | ------------------- | --------------------------------------------------------------- |
-| **`encoded_data`** | **str**             | Base64 encoded file data                                        |
-| **`metadata`**     | **bool** (optional) | If True, function returns file and metadata (Defaults to False) |
+| Argument         | Type                | Description                                                |
+| ---------------- | ------------------- | ---------------------------------------------------------- |
+| **`input_file`** | **str**             | Base64 encoded string, prefixed with metadata              |
+| **`metadata`**   | **bool** (optional) | Flag to return metadata with the file. (Defaults to False) |
+
+#### Raises:
+
+| Exception        | Description                                                                        |
+| ---------------- | ---------------------------------------------------------------------------------- |
+| **`ValueError`** | If the input string doesn't contain ';base64,' to separate metadata and file data. |
 
 #### Returns:
 
-| Return Type             | Description                   | Condition         |
-| ----------------------- | ----------------------------- | ----------------- |
-| **`io.BytesIO`**        | The decoded file data         | metadata is False |
-| **`(io.BytesIO, str)`** | The decoded file and metadata | metadata is True  |
+| Return Type             | Description                                                              | Condition         |
+| ----------------------- | ------------------------------------------------------------------------ | ----------------- |
+| **`io.BytesIO`**        | The decoded file data (The thing you get when you open a file in Python) | metadata is False |
+| **`(io.BytesIO, str)`** | The decoded file data and its metadata                                   | metadata is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> file, metadata = decode_file_data(inputFile, metadata = True)
+>>> input_file = inputs['file']
+>>> file, metadata = input_to_file(input_file, metadata = True)
 >>> print(metadata)
 data:image/jpeg;base64,
 >>> type(file)
 <class '_io.BytesIO'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">download_text</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL182C1-L214C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">metadata_to_filetype</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/general_utils.py#LL34C1-L50C21" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def download_text(
-    text: str,
-    filename: str = "myfile",
-    extension: str = ".txt",
-    download_text: str = "Download File",
-) -> str:
+def metadata_to_filetype(metadata):
+```
+
+#### Description:
+
+Extracts the file type from the metadata
+
+#### Arguments:
+
+| Argument       | Type    | Description                                                                                    |
+| -------------- | ------- | ---------------------------------------------------------------------------------------------- |
+| **`metadata`** | **str** | The metadata string in the form "Data:\<MIME type>;base64,"(returned from **`input_to_file`**) |
+
+#### Returns:
+
+| Return Type | Description                 |
+| ----------- | --------------------------- |
+| **`str`**   | The file type (e.g. "jpeg") |
+
+#### Example:
+
+```python
+>>> input_file = inputs['file']
+>>> file, metadata = input_to_file(input_file, metadata = True)
+>>> print(metadata)
+data:image/jpeg;base64,
+>>> download_file_type = metadata_to_filetype(metadata)
+>>> print(download_file_type)
+jpeg
+```
+
+## Text
+
+<div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">string_to_file</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/text_utils.py#LL4C1-L34C85" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+</div>
+
+```python
+def string_to_file(
+    text
+    filename= "myfile",
+    download_text = "Download File",
+)
 ```
 
 #### Description:
 
 Generates a downloadable text file containing the given text
 
 #### Arguments:
 
-| Argument            | Type               | Description                                                                   |
-| ------------------- | ------------------ | ----------------------------------------------------------------------------- |
-| **`text`**          | **str**            | The text to be downloaded                                                     |
-| **`filename`**      | **str** (optional) | The name of the file to be downloaded (Defaults to "myfile")                  |
-| **`extension`**     | **str** (optional) | The file extension of the file to be downloaded (Defaults to ".txt")          |
-| **`download_text`** | **str** (optional) | The text to be displayed on the download button (Defaults to "Download File") |
+| Argument            | Type               | Description                                                              |
+| ------------------- | ------------------ | ------------------------------------------------------------------------ |
+| **`text`**          | **str**            | Text to be downloaded                                                    |
+| **`filename`**      | **str** (optional) | Name of the download file. (Defaults to "myfile")                        |
+| **`download_text`** | **str** (optional) | Text to be displayed as the download link. (Defaults to "Download File") |
+
+#### Raises:
+
+| Exception       | Description                        |
+| --------------- | ---------------------------------- |
+| **`TypeError`** | If the input text is not a string. |
 
 #### Returns:
 
-| Return Type | Description                           |
-| ----------- | ------------------------------------- |
-| **`str`**   | The HTML code for the download button |
+| Return Type | Description        |
+| ----------- | ------------------ |
+| **`str`**   | HTML download link |
 
 #### Example:
 
 #### Python
 
 ```python
->>> downloadLink = download_text("Hello World!")
->>> return {"downloadLink": downloadLink}
+>>> download_link = string_to_file("Hello World!")
+>>> return {"download": download_link}
 ```
 
 #### Jinja2
 
 ```python
 # outputs.downloadLink is the html download link generated by the function
-{{ outputs.downloadLink }}
+{{ outputs.download }}
 ```
 
-## Tables/DataFrames
+## Spreadsheets
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">file_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL32C1-L52C14" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL9C1-L34C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def file_to_dataframe(file_data):
 ```
 
 #### Description:
 
-Converts a file object into a pandas DataFrame
+Converts a base64 encoded file data into a pandas DataFrame
 
 #### Arguments:
 
-| Argument        | Type           | Description                                          |
-| --------------- | -------------- | ---------------------------------------------------- |
-| **`file_data`** | **io.BytesIO** | Decoded file data (e.g. from **`decode_file_data`**) |
+| Argument        | Type           | Description                                       |
+| --------------- | -------------- | ------------------------------------------------- |
+| **`file_data`** | **io.BytesIO** | Decoded file data (e.g. from **`input_to_file`**) |
 
 #### Raises:
 
 | Exception                   | Description                                                                                                 |
 | --------------------------- | ----------------------------------------------------------------------------------------------------------- |
 | **`pd.errors.ParserError`** | If the file data cannot be converted to a DataFrame (i.e. file is not an Excel or CSV file or is corrupted) |
 
@@ -148,103 +198,107 @@
 | Return Type        | Description                      |
 | ------------------ | -------------------------------- |
 | **`pd.DataFrame`** | DataFrame created from file data |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> file = decode_file_data(inputFile)
->>> df = file_to_dataframe(file)
+>>> input_file = inputs['file']
+>>> decoded_file = input_to_file(input_file)
+>>> df = file_to_dataframe(decoded_file)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">input_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL55C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL35C1-L57C44" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def input_to_dataframe(file):
 ```
 
 #### Description:
 
 Converts a base64 encoded file data into a pandas DataFrame
 
 #### Arguments:
 
-| Argument   | Type    | Description              |
-| ---------- | ------- | ------------------------ |
-| **`file`** | **str** | Base64 encoded file data |
+| Argument            | Type     | Description                                                          |
+| ------------------- | -------- | -------------------------------------------------------------------- |
+| **`input_file`**    | **str**  | Base64 encoded file data                                             |
+| **`get_file_type`** | **bool** | If True, the function also returns the file type (Defaults to False) |
 
 #### Returns:
 
-| Return Type        | Description                      |
-| ------------------ | -------------------------------- |
-| **`pd.DataFrame`** | DataFrame created from file data |
+| Return Type               | Description                                      | Condition              |
+| ------------------------- | ------------------------------------------------ | ---------------------- |
+| **`pd.DataFrame`**        | DataFrame created from file data                 | get_file_type is False |
+| **`(pd.DataFrame, str)`** | Tuple containing the DataFrame and the file type | get_file_type is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> df = input_to_dataframe(inputFile)
+>>> input_file = inputs['file']
+>>> df, file_type = input_to_dataframe(input_file, get_file_type = True)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
+>>> print(file_type)
+csv
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL10C1-L67C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/spreadsheet_utils.py#LL60C1-L119C39" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_dataframe(
     df,
     download = False,
-    DownloadText = "Download Table",
-    DownloadFileName = "mytable",
-    FileType = "csv",
+    download_text = "Download Table",
+    download_file_name = "mytable",
+    download_file_type = "csv",
 ):
 ```
 
 #### Description:
 
 Creates an HTML table and a download link for a given DataFrame
 
 #### Arguments:
 
-| Argument               | Type                | Description                                                             |
-| ---------------------- | ------------------- | ----------------------------------------------------------------------- |
-| **`df`**               | **pd.DataFrame**    | DataFrame to be converted                                               |
-| **`download`**         | **bool** (optional) | If True, function returns a download link (Defaults to False)           |
-| **`DownloadText`**     | **str** (optional)  | Text to be displayed as the download link (Defaults to "Download File") |
-| **`DownloadFileName`** | **str** (optional)  | Name of file when downloaded (Defaults to "myfile")                     |
-| **`FileType`**         | **str** (optional)  | File type of download (Defaults to "csv")                               |
+| Argument                 | Type                | Description                                                             |
+| ------------------------ | ------------------- | ----------------------------------------------------------------------- |
+| **`df`**                 | **pd.DataFrame**    | DataFrame to be converted                                               |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)           |
+| **`download_text`**      | **str** (optional)  | Text to be displayed as the download link (Defaults to "Download File") |
+| **`download_file_name`** | **str** (optional)  | Name of file when downloaded (Defaults to "myfile")                     |
+| **`download_file_type`** | **str** (optional)  | File type of downloaded file (Defaults to "csv")                        |
 
 #### Returns:
 
-| Return Type           | Description                 | Condition         |
-| --------------------- | --------------------------- | ----------------- |
-| **`str`**             | HTML table                  | download is False |
-| **`Tuple[str, str]`** | (HTML table, download link) | download is True  |
+| Return Type           | Description                      | Condition         |
+| --------------------- | -------------------------------- | ----------------- |
+| **`str`**             | HTML table                       | download is False |
+| **`Tuple[str, str]`** | (HTML table, HTML download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> inputFile = inputs['file']
->>> df = input_to_dataframe(inputFile)
->>> table, download = print_dataframe(df, download = True, DownloadFileName = "FunkyTable", DownloadText = "Download My Funky Table HERE!", FileType = "xlsx")
+>>> input_file = inputs['file']
+>>> df = input_to_dataframe(input_file)
+>>> table, download = print_dataframe(df, download = True, download_file_name = "FunkyTable", download_text = "Download My Funky Table HERE!", download_file_type = "xlsx")
 >>> return {
         "table":table,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
@@ -257,85 +311,87 @@
 # outputs.download is the download link
 Downloading Table
 {{ outputs.download }}
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">table_to_dataframe</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL89C1-L105C35 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/table_utils.py#LL4C1-L26C54" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
+## Tables
+
 ```python
-def table_to_dataframe(columns: List[List[str]], column_headers: List[str]) -> pd.DataFrame:
+def table_to_dataframe(column_headers, rows) -> pd.DataFrame:
 ```
 
 #### Description:
 
-Creates a DataFrame from given columns and headers
+Create a DataFrame from given rows and column headers
 
 #### Arguments:
 
-| Argument             | Type                | Description                                                                        |
-| -------------------- | ------------------- | ---------------------------------------------------------------------------------- |
-| **`columns`**        | **List[List[str]]** | List of columns to be converted into a DataFrame. Each column is a list of strings |
-| **`column_headers`** | **List[str]**       | List of column headers                                                             |
+| Argument             | Type                | Description                                                                     |
+| -------------------- | ------------------- | ------------------------------------------------------------------------------- |
+| **`column_headers`** | **List[str]**       | List of column headers                                                          |
+| **`rows`**           | **List[List[str]]** | List of rows to be converted into a DataFrame. Each column is a list of strings |
 
 #### Returns:
 
-| Return Type        | Description                                |
-| ------------------ | ------------------------------------------ |
-| **`pd.DataFrame`** | DataFrame created from columns and headers |
+| Return Type        | Description                             |
+| ------------------ | --------------------------------------- |
+| **`pd.DataFrame`** | DataFrame created from headers and rows |
 
 #### Example:
 
 ```python
->>> columns = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
->>> df = table_to_dataframe(columns, column_headers)
+>>> rows = [["a", "b", "c"], ["d", "e", "f"]]
+>>> df = table_to_dataframe(column_headers, rows)
 >>> print(df)
    A  B  C
 0  a  b  c
 1  d  e  f
 
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_table</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL216C1-L240C114" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/table_utils.py#LL29C1-L44C58" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-print_table(rows: List[List[str]], column_headers: List[str]):
+print_table(column_headers, rows):
 ```
 
 #### Description:
 
 Creates an HTML table from given rows and column headers
 
 #### Arguments:
 
 | Argument             | Type                | Description                                                                 |
 | -------------------- | ------------------- | --------------------------------------------------------------------------- |
-| **`rows`**           | **List[List[str]]** | List of rows to be converted into a table. Each column is a list of strings |
 | **`column_headers`** | **List[str]**       | List of column headers                                                      |
+| **`rows`**           | **List[List[str]]** | List of rows to be converted into a table. Each column is a list of strings |
 
 #### Returns:
 
 | Return Type | Description                              |
 | ----------- | ---------------------------------------- |
 | **`str`**   | HTML table created from rows and headers |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> rows = [["a", "b", "c"], ["d", "e", "f"]]
 >>> column_headers = ["A", "B", "C"]
->>> table = print_table(rows, column_headers)
+>>> rows = [["a", "b", "c"], ["d", "e", "f"]]
+>>> table = print_table(column_headers, rows)
 >>> return {
         "table":table,
     }
 ```
 
 #### Output using Jinja2 Template:
 
@@ -344,99 +400,153 @@
 Displaying Table
 {{ outputs.table }}
 ```
 
 ## Images
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
+  <h3 style="margin: 5px; padding: 0;">file_to_PIL</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL13C1-L30C88" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+</div>
+
+```python
+def file_to_PIL(file):
+```
+
+#### Description:
+
+Transforms a file into a Pillow Image object
+
+#### Arguments:
+
+| Argument   | Type    | Description                                     |
+| ---------- | ------- | ----------------------------------------------- |
+| **`file`** | **str** | Decoded file data (returned from input_to_file) |
+
+#### Raises:
+
+| Exception Type   | Description                             |
+| ---------------- | --------------------------------------- |
+| **`ValueError`** | If the file does not contain image data |
+
+#### Returns:
+
+| Return Type | Description         |
+| ----------- | ------------------- |
+| **`Image`** | Pillow Image object |
+
+#### Example:
+
+#### Python Code:
+
+```python
+>>> input_file = inputs['file']
+>>> decoded_file = input_to_file(input_file)
+>>> image = file_to_PIL(decoded_file)
+>>> return {
+        "image":image,
+    }
+```
+
+#### Output using Jinja2 Template:
+
+```python
+# outputs.image is the Pillow Image object
+Displaying Image
+{{ outputs.image }}
+```
+
+<div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">input_to_PIL</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/input_utils.py#LL70C1-L87C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL33C1-L57C15" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def input_to_PIL(file):
+def input_to_PIL(input_file, get_file_type=False):
 ```
 
 #### Description:
 
 Converts a base64 encoded file data into a pillow image
 
 #### Arguments:
 
-| Argument   | Type    | Description              |
-| ---------- | ------- | ------------------------ |
-| **`file`** | **str** | Base64 encoded file data |
+| Argument            | Type     | Description                                                          |
+| ------------------- | -------- | -------------------------------------------------------------------- |
+| **`input_file`**    | **str**  | Base64 encoded file data                                             |
+| **`get_file_type`** | **bool** | If True, the function also returns the file type (Defaults to False) |
 
 #### Returns:
 
-| Return Type                       | Description              |
-| --------------------------------- | ------------------------ |
-| **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) |
+| Return Type                       | Description              | Condition              |
+| --------------------------------- | ------------------------ | ---------------------- |
+| **`PIL.Image.Image`**             | Pillow Image object      | get_file_type is False |
+| **`Tuple[PIL.Image.Image, str]`** | (pillow image, metadata) | get_file_type is True  |
 
 #### Example:
 
 ```python
->>> inputFile = inputs['file']
->>> img, metadata = input_to_PIL(inputFile)
->>> print(metadata)
-data:image/jpeg;base64,
->>> type(file)
+>>> input_file = inputs['file']
+>>> img, file_type = input_to_PIL(input_file, get_file_type=True)
+>>> print(file_type)
+jpeg
+>>> type(img)
 <class 'PIL.JpegImagePlugin.JpegImageFile'>
 ```
 
 <div style="display: flex; justify-content: space-between; align-items: center;">
   <h3 style="margin: 5px; padding: 0;">print_img</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL70C1-L129C1 style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/image_utils.py#LL60C1-L126C32" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
 def print_img(
     img,
-    metadata,
-    WIDTH = 200,
-    HEIGHT = 200,
-    OriginalSize = False,
+    width = 200,
+    height = 200,
+    original_size = False,
     download = False,
-    DownloadText = "Download Image",
-    ImageName= "myimg",
+    download_text = "Download Image",
+    download_file_name= "myimg",
+    download_file_type = "png",
 ):
 ```
 
 #### Description:
 
-Converts a pillow image into an HTML image and a download link
+Transforms a Pillow image into an HTML image, with an optional download link
 
 #### Arguments:
 
-| Argument           | Type                | Description                                                                        |
-| ------------------ | ------------------- | ---------------------------------------------------------------------------------- |
-| **`img`**          | **PIL.Image.Image** | Pillow image                                                                       |
-| **`metadata`**     | **str**             | Image metadata                                                                     |
-| **`WIDTH`**        | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
-| **`HEIGHT`**       | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
-| **`OriginalSize`** | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
-| **`download`**     | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
-| **`DownloadText`** | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
-| **`ImageName`**    | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
+| Argument                 | Type                | Description                                                                        |
+| ------------------------ | ------------------- | ---------------------------------------------------------------------------------- |
+| **`img`**                | **PIL.Image.Image** | Pillow image                                                                       |
+| **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 200)                              |
+| **`height`**             | **int** (optional)  | Output height of the image in pixels (Defaults to 200)                             |
+| **`original_size`**      | **bool** (optional) | If True, the HTML image will be displayed in its original size (Defaults to False) |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)                      |
+| **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Image")       |
+| **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myimg")                   |
+| **`download_file_type`** | **str** (optional)  | The file type of the image when downloaded (Defaults to "png")                     |
 
 #### Returns:
 
 | Return Type           | Description                 | Condition         |
 | --------------------- | --------------------------- | ----------------- |
 | **`str`**             | HTML image                  | download is False |
 | **`Tuple[str, str]`** | (HTML image, download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
->>> inputFile = inputs['file']
->>> img, metadata = input_to_PIL(inputFile)
->>> image, download = print_img(img, metadata, OriginalSize = True, download = True, DownloadText = "Download Image Here", ImageName = "myimage")
+>>> input_file = inputs['file']
+>>> img, metadata = input_to_PIL(input_file)
+>>> image, download = print_img(img,, original_size = True, download = True, download_text = "Download Image Here", download_file_name = "myimage", download_file_type = "jpeg")
 >>> return {
         "image":image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
@@ -447,65 +557,67 @@
 {{ outputs.image }}
 
 # outputs.download is the download link
 Downloading Image
 {{ outputs.download }}
 ```
 
+## Plots
+
 <div style="display: flex; justify-content: space-between; align-items: center;">
-  <h3 style="margin: 5px; padding: 0;">print_plt</h3>
-  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/output_utils.py#LL131C1-L180C1" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
+  <h3 style="margin: 5px; padding: 0;">print_plot</h3>
+  <a href="https://github.com/MecSimCalc/MecSimCalc-utils/blob/main/mecsimcalc/plotting_utils.py#LL8C1-L63C35" style="font-size: larger; margin-bottom: 2em; margin: 5px; padding: 0;"><strong>[Source]</strong></a>
 </div>
 
 ```python
-def print_plt(
-    plt:,
+def print_plot(
+    plot_obj,
     width = 500,
     dpi= 100,
     download= False,
-    DownloadText = "Download Plot",
-    DownloadFileName = "myplot",
+    download_text = "Download Plot",
+    download_file_name = "myplot",
 )
 ```
 
 #### Description:
 
-Converts a matplotlib.pyplot or matplotlib.figure into an HTML image tag and optionally provides a download link for the image
+Converts a matplotlib.pyplot.axis or matplotlib.figure into an HTML image tag and optionally provides a download link for the image
 
 #### Arguments:
 
-| Argument               | Type                | Description                                                                 |
-| ---------------------- | ------------------- | --------------------------------------------------------------------------- |
-| **`plt`**              | **plt or figure**   | Matplotlib figure                                                           |
-| **`width`**            | **int** (optional)  | Output width of the image in pixels (Defaults to 500)                       |
-| **`dpi`**              | **int** (optional)  | Output dpi of the image in pixels (Defaults to 100)                         |
-| **`download`**         | **bool** (optional) | If True, function returns a download link (Defaults to False)               |
-| **`DownloadText`**     | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Plot") |
-| **`DownloadFileName`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myplot")           |
+| Argument                 | Type                | Description                                                                 |
+| ------------------------ | ------------------- | --------------------------------------------------------------------------- |
+| **`plot_obj`**           | **axes or figure**  | Matplotlib figure                                                           |
+| **`width`**              | **int** (optional)  | Output width of the image in pixels (Defaults to 500)                       |
+| **`dpi`**                | **int** (optional)  | Output dpi of the image in pixels (Defaults to 100)                         |
+| **`download`**           | **bool** (optional) | If True, function returns a download link (Defaults to False)               |
+| **`download_text`**      | **str** (optional)  | The text to be displayed on the download link (Defaults to "Download Plot") |
+| **`download_file_name`** | **str** (optional)  | The name of the image file when downloaded (Defaults to "myplot")           |
 
 #### Returns:
 
-| Return Type           | Description                 | Condition         |
-| --------------------- | --------------------------- | ----------------- |
-| **`str`**             | HTML image                  | download is False |
-| **`Tuple[str, str]`** | (HTML image, download link) | download is True  |
+| Return Type           | Description                      | Condition         |
+| --------------------- | -------------------------------- | ----------------- |
+| **`str`**             | HTML image                       | download is False |
+| **`Tuple[str, str]`** | (HTML image, HTML download link) | download is True  |
 
 #### Example:
 
 #### Python Code:
 
 ```python
 >>> import matplotlib.pyplot as plt
 >>> import numpy as np
 >>> x = np.linspace(0, 2 * np.pi, 400)
 >>> y = np.sin(x)
 >>> fig, ax = plt.subplots()
 >>> ax.plot(x, y)
 >>> ax.set_title('A single plot')
->>> image, download = print_plt(fig, width = 500, dpi = 100, download = True, DownloadText = "Download Sin Function Plot", DownloadFileName = "sin(x)")
+>>> image, download = print_plot(fig, width = 500, dpi = 100, download = True, download_text = "Download Sin Function Plot", download_file_name = "sin(x)")
 >>> return {
         "image":image,
         "download":download,
     }
 ```
 
 #### Output using Jinja2 Template:
```

### Comparing `mecsimcalc-0.0.5/setup.py` & `mecsimcalc-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.5"
+VERSION = "0.1.0"
 DESCRIPTION = "Useful functions for MecSimCalc.com"
-LONG_DESCRIPTION = "Useful functions for MecSimCalc.com"
 
 # Setting up
 setup(
     name="mecsimcalc",
     version=VERSION,
     author="MecSimCalc",
     author_email="<info@mecsimcalc.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=["Pillow", "pandas", "matplotlib"],
+    install_requires=["Pillow", "pandas", "matplotlib", "openpyxl"],
     keywords=["python", "MecSimCalc", "Calculator", "Simple"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

