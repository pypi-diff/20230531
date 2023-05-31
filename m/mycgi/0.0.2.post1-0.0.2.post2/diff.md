# Comparing `tmp/mycgi-0.0.2.post1.tar.gz` & `tmp/mycgi-0.0.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Ron\mycgi\dist\.tmp-lpq68e5k\mycgi-0.0.2.post1.tar", last modified: Fri Apr 28 18:16:41 2023, max compression
+gzip compressed data, was "C:\Ron\mycgi\dist\.tmp-tjl0ppf6\mycgi-0.0.2.post2.tar", last modified: Wed May 31 18:44:38 2023, max compression
```

## Comparing `mycgi-0.0.2.post1.tar` & `mycgi-0.0.2.post2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:16:41.786794 mycgi-0.0.2.post1/
--rw-rw-rw-   0        0        0      568 2023-04-19 14:17:36.000000 mycgi-0.0.2.post1/LICENSE.txt
--rw-rw-rw-   0        0        0     6691 2023-04-28 18:16:41.766085 mycgi-0.0.2.post1/PKG-INFO
--rw-rw-rw-   0        0        0     5602 2023-04-27 17:38:57.000000 mycgi-0.0.2.post1/README.md
--rw-rw-rw-   0        0        0      592 2023-04-28 18:13:25.000000 mycgi-0.0.2.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 18:16:41.786794 mycgi-0.0.2.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 18:16:41.693997 mycgi-0.0.2.post1/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 18:16:41.763866 mycgi-0.0.2.post1/src/mycgi.egg-info/
--rw-rw-rw-   0        0        0     6691 2023-04-28 18:16:41.000000 mycgi-0.0.2.post1/src/mycgi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-04-28 18:16:41.000000 mycgi-0.0.2.post1/src/mycgi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:16:41.000000 mycgi-0.0.2.post1/src/mycgi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-28 18:16:41.000000 mycgi-0.0.2.post1/src/mycgi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 18:16:41.000000 mycgi-0.0.2.post1/src/mycgi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10049 2023-04-19 16:56:00.000000 mycgi-0.0.2.post1/src/mycgi.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:44:38.317920 mycgi-0.0.2.post2/
+-rw-rw-rw-   0        0        0      568 2023-04-19 14:17:36.000000 mycgi-0.0.2.post2/LICENSE.txt
+-rw-rw-rw-   0        0        0     7096 2023-05-31 18:44:38.316923 mycgi-0.0.2.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     6007 2023-05-31 18:19:02.000000 mycgi-0.0.2.post2/README.md
+-rw-rw-rw-   0        0        0      592 2023-05-31 18:42:28.000000 mycgi-0.0.2.post2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 18:44:38.318920 mycgi-0.0.2.post2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 18:44:38.305920 mycgi-0.0.2.post2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 18:44:38.315919 mycgi-0.0.2.post2/src/mycgi.egg-info/
+-rw-rw-rw-   0        0        0     7096 2023-05-31 18:44:38.000000 mycgi-0.0.2.post2/src/mycgi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-31 18:44:38.000000 mycgi-0.0.2.post2/src/mycgi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 18:44:38.000000 mycgi-0.0.2.post2/src/mycgi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-31 18:44:38.000000 mycgi-0.0.2.post2/src/mycgi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 18:44:38.000000 mycgi-0.0.2.post2/src/mycgi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10055 2023-05-31 18:42:54.000000 mycgi-0.0.2.post2/src/mycgi.py
```

### Comparing `mycgi-0.0.2.post1/LICENSE.txt` & `mycgi-0.0.2.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mycgi-0.0.2.post1/PKG-INFO` & `mycgi-0.0.2.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycgi
-Version: 0.0.2.post1
+Version: 0.0.2.post2
 Summary: A Python3 replacement for the deprecated cgi module
 Author-email: Ronald Aaronson <ronaldaaronson@gmail.com>
 License: Copyright 2023, Ronald Aaronson
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -19,46 +19,46 @@
 Keywords: cgi,replacement
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-mycgi - A Python3 Replacement for the Deprecated `cgi` Module
-=============================================================
+# mycgi - A Python3 Replacement for the Deprecated `cgi` Module
 
-This module uses the `python-multipart` package for handling non-JSON-encoded POST and PUT requests.
+Other than using different class names (`mycgi.Form` instead of `cgi.FieldStorage` and `mycgi.Field` instead of `cgi.FieldStorage`) this module should be quite backward-compatible with the `mycgi` module. Additionally, JSON-encoded PUT and POST requests are supported.
 
-Some Usage Examples
--------------------
+Note that this module depends on the `python-multipart` package for handling POST and PUT requests that are not JSON-encoded.
+
+## Some Usage Examples
 
 ```
 # Instead of:
 #from cgi import FieldStorage
 # Use:
 from mycgi import Form
 
 form = Form()
 
-# Field 'name' is a text input field:
-name = form.getvalue('name') # This will be a list if the form has multiple 'name' fields
-name = form.getfirst('name') # This will be a single string
-names = form.getlist('name') # This will be a list of strings
+# name is a text input field:
+name = form.getvalue('name') # this will be a list if the form has multiple 'name' fields
+# or: name = form.getfirst('name')
+# or: names = form.getlist('name')
 
-# Field 'spreadsheet' is a file input field:
+# spreadsheet is a file input field:
 fileitem = form['spreadsheet']
-filename = fileitem.filename # The name of the uploaded file
+# The name of the uploaded file:
+filename = fileitem.filename
 # Get the file contents as bytes 3 different ways:
 contents = fileitem.file.read()
 contents = fileitem.value
 contents = form.getvalue('spreadsheet')
 ```
 
-Documentation
--------------
+## Documentation
 
 The initializer for the `mycgi.Form` class is:
 
 ```
     def __init__(self, environ=os.environ, fp=None, keep_blank_values=False):
         """
         Initialize a Form instance.
@@ -82,30 +82,35 @@
 
 A `mycgi.Form` instance is a specialized dictionary whose keys are the field names and whose values are either a `mycgi.Field`
 instance or a list of these instances. A `mycgi.Field` instance has the following attributes:
 
 1. `name`:     The form field name.
 2. `filename`: If this field is for an uploaded file, then the uploaded filename, else None.
 3. `value`:    The form field value (or an uploaded file's contents as bytes).
-4. `file`:     If the field value is a string or byte string, then a stream that can be read to get the field's value, else None.
+4. `file`:     If the field value is a string or byte string,then a stream that can be read to get the field's value, else None.
+
+The `mycgi.Form` class supports the `getvalue`, `getlist` and `getfirst` methods that behave identically to the like-named methods of the deprecated `cgi.FieldStorage` class and which make it unnecessary to access the `mycgi.Field` instances, although doing so can be useful for processing file uploads.
+
+### JSON-encoded PUT and POST requests
+
+Also supported are POST and PUT requests where the data is a JSON-encoded dictionary.
 
-**Also supported are POST and PUT requests where the data is a JSON-encoded dictionary.**
+### WSGI Application Usage
 
 To use `mycgi.Form` with a WSGI application:
 
 ```
 from mycgi import Form
 
 def wsgiApp(environ, start_response):
     form = Form(environ=environ, fp=environ['wsgi.input'])
     ...
 ```
 
-Tests to Further Demonstrate `mycgi` Usage
-----------------------------------------
+## Tests To Demonstrate `mycgi` Usage
 
 ```
 from mycgi import Form
 import io
 
 # Test a GET request:
 form = Form(environ={'QUERY_STRING': 'x=1&x=2&y=3'})
@@ -123,17 +128,16 @@
 assert form['y'].name == 'y'
 assert form['y'].filename is None
 assert form['y'].value == '3'
 assert form['y'].file.read() == '3'
 
 # Test a multipart POST request:
 # We have here a text input field named 'act' whose value is 'abc' and two
-# file input fields named 'the_file' where a file named 'test.txt' has been
-# selected for the first occurence and no file selected for the second
-# occurrence:
+# file input fields named 'the_file' where a file has been selected for only the
+# first occurence:
 
 # The following definition of fp is on a single line:
 fp = io.BytesIO(b'------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="act"\r\n\r\nTest\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="the_file"; filename="test.txt"\r\nContent-Type: text/plain\r\n\r\nabc\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="the_file"; filename=""\r\nContent-Type: application/octet-stream\r\n\r\n\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp--\r\n')
 
 environ = {
     'CONTENT_LENGTH': '431',
     'CONTENT_TYPE': 'multipart/form-data; boundary=----WebKitFormBoundarytQ0DkMXsDqxwxBlp',
```

### Comparing `mycgi-0.0.2.post1/README.md` & `mycgi-0.0.2.post2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-mycgi - A Python3 Replacement for the Deprecated `cgi` Module
-=============================================================
+# mycgi - A Python3 Replacement for the Deprecated `cgi` Module
 
-This module uses the `python-multipart` package for handling non-JSON-encoded POST and PUT requests.
+Other than using different class names (`mycgi.Form` instead of `cgi.FieldStorage` and `mycgi.Field` instead of `cgi.FieldStorage`) this module should be quite backward-compatible with the `mycgi` module. Additionally, JSON-encoded PUT and POST requests are supported.
 
-Some Usage Examples
--------------------
+Note that this module depends on the `python-multipart` package for handling POST and PUT requests that are not JSON-encoded.
+
+## Some Usage Examples
 
 ```
 # Instead of:
 #from cgi import FieldStorage
 # Use:
 from mycgi import Form
 
 form = Form()
 
-# Field 'name' is a text input field:
-name = form.getvalue('name') # This will be a list if the form has multiple 'name' fields
-name = form.getfirst('name') # This will be a single string
-names = form.getlist('name') # This will be a list of strings
+# name is a text input field:
+name = form.getvalue('name') # this will be a list if the form has multiple 'name' fields
+# or: name = form.getfirst('name')
+# or: names = form.getlist('name')
 
-# Field 'spreadsheet' is a file input field:
+# spreadsheet is a file input field:
 fileitem = form['spreadsheet']
-filename = fileitem.filename # The name of the uploaded file
+# The name of the uploaded file:
+filename = fileitem.filename
 # Get the file contents as bytes 3 different ways:
 contents = fileitem.file.read()
 contents = fileitem.value
 contents = form.getvalue('spreadsheet')
 ```
 
-Documentation
--------------
+## Documentation
 
 The initializer for the `mycgi.Form` class is:
 
 ```
     def __init__(self, environ=os.environ, fp=None, keep_blank_values=False):
         """
         Initialize a Form instance.
@@ -57,30 +57,35 @@
 
 A `mycgi.Form` instance is a specialized dictionary whose keys are the field names and whose values are either a `mycgi.Field`
 instance or a list of these instances. A `mycgi.Field` instance has the following attributes:
 
 1. `name`:     The form field name.
 2. `filename`: If this field is for an uploaded file, then the uploaded filename, else None.
 3. `value`:    The form field value (or an uploaded file's contents as bytes).
-4. `file`:     If the field value is a string or byte string, then a stream that can be read to get the field's value, else None.
+4. `file`:     If the field value is a string or byte string,then a stream that can be read to get the field's value, else None.
+
+The `mycgi.Form` class supports the `getvalue`, `getlist` and `getfirst` methods that behave identically to the like-named methods of the deprecated `cgi.FieldStorage` class and which make it unnecessary to access the `mycgi.Field` instances, although doing so can be useful for processing file uploads.
+
+### JSON-encoded PUT and POST requests
+
+Also supported are POST and PUT requests where the data is a JSON-encoded dictionary.
 
-**Also supported are POST and PUT requests where the data is a JSON-encoded dictionary.**
+### WSGI Application Usage
 
 To use `mycgi.Form` with a WSGI application:
 
 ```
 from mycgi import Form
 
 def wsgiApp(environ, start_response):
     form = Form(environ=environ, fp=environ['wsgi.input'])
     ...
 ```
 
-Tests to Further Demonstrate `mycgi` Usage
-----------------------------------------
+## Tests To Demonstrate `mycgi` Usage
 
 ```
 from mycgi import Form
 import io
 
 # Test a GET request:
 form = Form(environ={'QUERY_STRING': 'x=1&x=2&y=3'})
@@ -98,17 +103,16 @@
 assert form['y'].name == 'y'
 assert form['y'].filename is None
 assert form['y'].value == '3'
 assert form['y'].file.read() == '3'
 
 # Test a multipart POST request:
 # We have here a text input field named 'act' whose value is 'abc' and two
-# file input fields named 'the_file' where a file named 'test.txt' has been
-# selected for the first occurence and no file selected for the second
-# occurrence:
+# file input fields named 'the_file' where a file has been selected for only the
+# first occurence:
 
 # The following definition of fp is on a single line:
 fp = io.BytesIO(b'------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="act"\r\n\r\nTest\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="the_file"; filename="test.txt"\r\nContent-Type: text/plain\r\n\r\nabc\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="the_file"; filename=""\r\nContent-Type: application/octet-stream\r\n\r\n\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp--\r\n')
 
 environ = {
     'CONTENT_LENGTH': '431',
     'CONTENT_TYPE': 'multipart/form-data; boundary=----WebKitFormBoundarytQ0DkMXsDqxwxBlp',
```

### Comparing `mycgi-0.0.2.post1/pyproject.toml` & `mycgi-0.0.2.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mycgi"
-version = "0.0.2.post1"
+version = "0.0.2.post2"
 description = "A Python3 replacement for the deprecated cgi module"
 readme = "README.md"
 authors = [{ name = "Ronald Aaronson", email = "ronaldaaronson@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `mycgi-0.0.2.post1/src/mycgi.egg-info/PKG-INFO` & `mycgi-0.0.2.post2/src/mycgi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycgi
-Version: 0.0.2.post1
+Version: 0.0.2.post2
 Summary: A Python3 replacement for the deprecated cgi module
 Author-email: Ronald Aaronson <ronaldaaronson@gmail.com>
 License: Copyright 2023, Ronald Aaronson
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
@@ -19,46 +19,46 @@
 Keywords: cgi,replacement
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-mycgi - A Python3 Replacement for the Deprecated `cgi` Module
-=============================================================
+# mycgi - A Python3 Replacement for the Deprecated `cgi` Module
 
-This module uses the `python-multipart` package for handling non-JSON-encoded POST and PUT requests.
+Other than using different class names (`mycgi.Form` instead of `cgi.FieldStorage` and `mycgi.Field` instead of `cgi.FieldStorage`) this module should be quite backward-compatible with the `mycgi` module. Additionally, JSON-encoded PUT and POST requests are supported.
 
-Some Usage Examples
--------------------
+Note that this module depends on the `python-multipart` package for handling POST and PUT requests that are not JSON-encoded.
+
+## Some Usage Examples
 
 ```
 # Instead of:
 #from cgi import FieldStorage
 # Use:
 from mycgi import Form
 
 form = Form()
 
-# Field 'name' is a text input field:
-name = form.getvalue('name') # This will be a list if the form has multiple 'name' fields
-name = form.getfirst('name') # This will be a single string
-names = form.getlist('name') # This will be a list of strings
+# name is a text input field:
+name = form.getvalue('name') # this will be a list if the form has multiple 'name' fields
+# or: name = form.getfirst('name')
+# or: names = form.getlist('name')
 
-# Field 'spreadsheet' is a file input field:
+# spreadsheet is a file input field:
 fileitem = form['spreadsheet']
-filename = fileitem.filename # The name of the uploaded file
+# The name of the uploaded file:
+filename = fileitem.filename
 # Get the file contents as bytes 3 different ways:
 contents = fileitem.file.read()
 contents = fileitem.value
 contents = form.getvalue('spreadsheet')
 ```
 
-Documentation
--------------
+## Documentation
 
 The initializer for the `mycgi.Form` class is:
 
 ```
     def __init__(self, environ=os.environ, fp=None, keep_blank_values=False):
         """
         Initialize a Form instance.
@@ -82,30 +82,35 @@
 
 A `mycgi.Form` instance is a specialized dictionary whose keys are the field names and whose values are either a `mycgi.Field`
 instance or a list of these instances. A `mycgi.Field` instance has the following attributes:
 
 1. `name`:     The form field name.
 2. `filename`: If this field is for an uploaded file, then the uploaded filename, else None.
 3. `value`:    The form field value (or an uploaded file's contents as bytes).
-4. `file`:     If the field value is a string or byte string, then a stream that can be read to get the field's value, else None.
+4. `file`:     If the field value is a string or byte string,then a stream that can be read to get the field's value, else None.
+
+The `mycgi.Form` class supports the `getvalue`, `getlist` and `getfirst` methods that behave identically to the like-named methods of the deprecated `cgi.FieldStorage` class and which make it unnecessary to access the `mycgi.Field` instances, although doing so can be useful for processing file uploads.
+
+### JSON-encoded PUT and POST requests
+
+Also supported are POST and PUT requests where the data is a JSON-encoded dictionary.
 
-**Also supported are POST and PUT requests where the data is a JSON-encoded dictionary.**
+### WSGI Application Usage
 
 To use `mycgi.Form` with a WSGI application:
 
 ```
 from mycgi import Form
 
 def wsgiApp(environ, start_response):
     form = Form(environ=environ, fp=environ['wsgi.input'])
     ...
 ```
 
-Tests to Further Demonstrate `mycgi` Usage
-----------------------------------------
+## Tests To Demonstrate `mycgi` Usage
 
 ```
 from mycgi import Form
 import io
 
 # Test a GET request:
 form = Form(environ={'QUERY_STRING': 'x=1&x=2&y=3'})
@@ -123,17 +128,16 @@
 assert form['y'].name == 'y'
 assert form['y'].filename is None
 assert form['y'].value == '3'
 assert form['y'].file.read() == '3'
 
 # Test a multipart POST request:
 # We have here a text input field named 'act' whose value is 'abc' and two
-# file input fields named 'the_file' where a file named 'test.txt' has been
-# selected for the first occurence and no file selected for the second
-# occurrence:
+# file input fields named 'the_file' where a file has been selected for only the
+# first occurence:
 
 # The following definition of fp is on a single line:
 fp = io.BytesIO(b'------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="act"\r\n\r\nTest\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="the_file"; filename="test.txt"\r\nContent-Type: text/plain\r\n\r\nabc\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp\r\nContent-Disposition: form-data; name="the_file"; filename=""\r\nContent-Type: application/octet-stream\r\n\r\n\r\n------WebKitFormBoundarytQ0DkMXsDqxwxBlp--\r\n')
 
 environ = {
     'CONTENT_LENGTH': '431',
     'CONTENT_TYPE': 'multipart/form-data; boundary=----WebKitFormBoundarytQ0DkMXsDqxwxBlp',
```

### Comparing `mycgi-0.0.2.post1/src/mycgi.py` & `mycgi-0.0.2.post2/src/mycgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__version__ = '0.0.2'
+__version__ = '0.0.2.post2'
 
 import multipart
 import os
 import sys
 import json
 from urllib.parse import parse_qs, unquote_plus
 import io
```

