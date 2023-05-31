# Comparing `tmp/inputty-1.0.0.tar.gz` & `tmp/inputty-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inputty-1.0.0.tar", last modified: Tue May 30 11:45:26 2023, max compression
+gzip compressed data, was "inputty-1.0.1.tar", last modified: Wed May 31 08:48:42 2023, max compression
```

## Comparing `inputty-1.0.0.tar` & `inputty-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.0/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-30 11:45:26.441095 inputty-1.0.0/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.0/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.0/inputty/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-30 11:44:18.000000 inputty-1.0.0/inputty/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.0/inputty/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7598 2023-05-30 11:43:57.000000 inputty-1.0.0/inputty/src/input.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.0/inputty/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3230 2023-05-30 11:09:18.000000 inputty-1.0.0/inputty/tests/test_input.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-30 11:45:26.441095 inputty-1.0.0/inputty.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      898 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      303 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-30 11:45:26.000000 inputty-1.0.0/inputty.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-30 11:45:26.444428 inputty-1.0.0/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.0/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-31 08:48:42.580568 inputty-1.0.1/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.1/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      977 2023-05-31 08:48:42.580568 inputty-1.0.1/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.1/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-31 08:48:42.573901 inputty-1.0.1/inputty/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.1/inputty/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-31 08:43:46.000000 inputty-1.0.1/inputty/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-31 08:48:42.577235 inputty-1.0.1/inputty/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.1/inputty/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7787 2023-05-31 08:48:06.000000 inputty-1.0.1/inputty/src/input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-31 08:48:42.580568 inputty-1.0.1/inputty/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.1/inputty/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3230 2023-05-30 11:09:18.000000 inputty-1.0.1/inputty/tests/test_input.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      339 2023-05-31 08:29:56.000000 inputty-1.0.1/inputty/xxx.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-31 08:48:42.577235 inputty-1.0.1/inputty.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      977 2023-05-31 08:48:42.000000 inputty-1.0.1/inputty.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      318 2023-05-31 08:48:42.000000 inputty-1.0.1/inputty.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-31 08:48:42.000000 inputty-1.0.1/inputty.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-05-31 08:48:42.000000 inputty-1.0.1/inputty.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-31 08:48:42.580568 inputty-1.0.1/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.1/setup.py
```

### Comparing `inputty-1.0.0/LICENSE.txt` & `inputty-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inputty-1.0.0/PKG-INFO` & `inputty-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.0
+Version: 1.0.1
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,21 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.1 31 May 2023
+
+1. Implement __call__
+2. Refactor messages
+
+------
+
 Version 1.0.0 30 May 2023
 
 1. Major refactor
 2. Implement tests
 
 ------
```

### Comparing `inputty-1.0.0/inputty/src/input.py` & `inputty-1.0.1/inputty/src/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from termcolor import cprint
 import colorama
 
 colorama.init()
 
 MODULE_COLOUR = 'blue'
 ERROR_COLOUR = 'red'
+INVALID_SPEC_MSG = 'Invalid specification for process:'
+INVALID_INPUT_MSG = 'Invalid input.'
+USE_ONE_OF_MSG = 'Use one of'
+INTEGER_RANGE_MSG = 'Integer outside valid range:'
+
 RETURN = '<RTN>'
 INTEGER_SELECTION = '<INTEGERS>'
 INTEGER_BASE = 1
 
 __all__ = ['Input']
 
 
@@ -56,33 +61,37 @@
 
     process_response:
         Returns the method associated with a valid input.
 
     Example Usage
     -----
 
-
-    response = Input(prompt, processes).process_response()
+        Input(prompt, processes)()
+    or,
+        my_input = Input(prompt, processes)
+        my_input()
     """
     def __init__(self, prompt: str,
                  processes: dict[str, Tuple[object, List[object]]],
                  validation: dict[str, object] = {}):
-
         self.prompt = prompt
         self.processes = self._generate_processes(processes)
         self.validation = validation
         self.message_list = self._get_message_list(processes)
         self .response = None
         self.error_colour = ERROR_COLOUR
         # Are valid inputs to be included in the error message?
         self.include_valid_in_error = True
-        self._error_message = self._get_error_message('Invalid input.')
+        self._input_error_message = self._get_input_error_message()
 
         self.process_response = self.invoke
 
+    def __call__(self):
+        self.invoke()
+
     def invoke(self) -> object:
         # Return the result of a valid input
         response = self._get_input()
 
         self.response = response
         if response not in self.processes:
             return response
@@ -107,30 +116,30 @@
                     return RETURN
                 continue
 
             if response in self.processes:
                 return response
             elif self.validation:
                 return self.validate_input(response)
-            cprint(f"{self._error_message}", self.error_colour)
+            cprint(f"{self._input_error_message}", self.error_colour)
 
     def validate_input(self, response):
         # Return a valid input string having validated input.
         if 'integer' in self.validation:
             return self.validate_integer(response)
         return False
 
     def validate_integer(self, response):
         # Validate an integer  response.
         if not response.isnumeric():
             return False
         integer = int(response)
         min_, max_ = self.validation['integer']['min'], self.validation['integer']['max']
         if integer < min_ or integer > max_:
-            cprint(f"Integer outside valid range: {min_} to {max_}", ERROR_COLOUR)
+            cprint(f"{INTEGER_RANGE_MSG} {min_} to {max_}", ERROR_COLOUR)
             return False
         return response
 
     def _get_message_list(self, processes) -> List[str]:
         # Return a list of valid inputs for use in error message
         message_list = []
         for key in processes:
@@ -149,18 +158,18 @@
 
     @staticmethod
     def _validate_processes(processes):
         for key, item in processes.items():
             try:
                 _ = len(item)
             except TypeError:
-                err_msg = f'Invalid specification for process: {key}. No parameters.'
+                err_msg = f'{INVALID_SPEC_MSG} {key}. No parameters.'
                 raise TypeError(err_msg)
             if not isinstance(item[1], list):
-                err_msg = f'Invalid specification for process: {key}. Parameters not a list.'
+                err_msg = f'{INVALID_SPEC_MSG} {key}. Parameters not a list.'
                 raise TypeError(err_msg)
 
     @staticmethod
     def _get_case_processes(processes):
         case_processes = {}
         for key in processes:
             if not key.isnumeric() and key not in [INTEGER_SELECTION, RETURN]:
@@ -188,29 +197,29 @@
             return (INTEGER_BASE, process[2])
         else:
             return process[2]
 
     @staticmethod
     def _validate_integers(key, process):
         if len(process) <= 2:
-            err_msg = f'Invalid specification for process: {key}. No integer range.'
+            err_msg = f'{INVALID_SPEC_MSG} {key}. No integer range.'
             raise ValueError(err_msg)
         if isinstance(process[2], int):
             return
         if not isinstance(process[2], tuple):
-            err_msg = f'Invalid specification for process: {key}. Range not a tuple.'
+            err_msg = f'{INVALID_SPEC_MSG} {key}. Range not a tuple.'
             raise TypeError(err_msg)
         if len(process[2]) == 0:
-            err_msg = f'Invalid specification for process: {key}. Range empty.'
+            err_msg = f'{INVALID_SPEC_MSG} {key}. Range empty.'
             raise TypeError(err_msg)
 
-    def _get_error_message(self, error_text: str) -> str:
+    def _get_input_error_message(self) -> str:
         # Return the error message for the input
         if self.include_valid_in_error:
             valid_responses_list = self.message_list
             valid_responses = ', '.join(valid_responses_list)
             if len(valid_responses_list) >= 1:
-                return f'{error_text} Use one of {valid_responses}'
-        return error_text
+                return f'{INVALID_INPUT_MSG} {USE_ONE_OF_MSG} {valid_responses}'
+        return INVALID_INPUT_MSG
 
     def __str__(self) -> str:
         return f'Input: {self.prompt} {[key for key in self.processes]}'
```

### Comparing `inputty-1.0.0/inputty/tests/test_input.py` & `inputty-1.0.1/inputty/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `inputty-1.0.0/inputty.egg-info/PKG-INFO` & `inputty-1.0.1/inputty.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.0
+Version: 1.0.1
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,21 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.1 31 May 2023
+
+1. Implement __call__
+2. Refactor messages
+
+------
+
 Version 1.0.0 30 May 2023
 
 1. Major refactor
 2. Implement tests
 
 ------
```

### Comparing `inputty-1.0.0/setup.py` & `inputty-1.0.1/setup.py`

 * *Files identical despite different names*

