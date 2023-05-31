# Comparing `tmp/str_style-0.1.0.tar.gz` & `tmp/str_style-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "str_style-0.1.0.tar", max compression
+gzip compressed data, was "str_style-1.0.0.tar", max compression
```

## Comparing `str_style-0.1.0.tar` & `str_style-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-05-24 14:31:39.676679 str_style-0.1.0/LICENSE
--rw-r--r--   0        0        0     1200 2023-05-24 14:31:39.676679 str_style-0.1.0/README.md
--rw-r--r--   0        0        0      467 2023-05-24 14:31:39.676679 str_style-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-24 14:31:39.676679 str_style-0.1.0/strstyle/__init__.py
--rw-r--r--   0        0        0     1517 2023-05-24 14:31:39.680678 str_style-0.1.0/strstyle/str_style.py
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 str_style-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-31 11:20:10.440295 str_style-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2474 2023-05-31 11:20:10.440295 str_style-1.0.0/README.md
+-rw-r--r--   0        0        0      733 2023-05-31 11:20:10.440295 str_style-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-31 11:20:10.440295 str_style-1.0.0/strstyle/__init__.py
+-rw-r--r--   0        0        0     1850 2023-05-31 11:20:10.440295 str_style-1.0.0/strstyle/__main__.py
+-rw-r--r--   0        0        0     2305 2023-05-31 11:20:10.440295 str_style-1.0.0/strstyle/str_style.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 str_style-1.0.0/PKG-INFO
```

### Comparing `str_style-0.1.0/LICENSE` & `str_style-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `str_style-0.1.0/strstyle/str_style.py` & `str_style-1.0.0/strstyle/str_style.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,114 @@
-def _paint(color_code: str, str_body: str) -> str:
-    return f'\033[{color_code}m{str_body}\033[0m'
+def bold(str_body: str) -> str:
+    return f'\033[01m{str_body}\033[0m'
+
+
+def disabled(str_body: str) -> str:
+    return f'\033[02m{str_body}\033[0m'
+
+
+def italic(str_body: str) -> str:
+    return f'\033[03m{str_body}\033[0m'
+
+
+def underline(str_body: str) -> str:
+    return f'\033[04m{str_body}\033[0m'
+
+
+def sharp(str_body: str) -> str:
+    return f'\033[07m{str_body}\033[0m'
+
+
+def invisible(str_body: str) -> str:
+    return f'\033[08m{str_body}\033[0m'
+
+
+def strike_through(str_body: str) -> str:
+    return f'\033[09m{str_body}\033[0m'
+
+
+def double_underline(str_body: str) -> str:
+    return f'\033[21m{str_body}\033[0m'
 
 
 def black(str_body: str) -> str:
-    return _paint('30', str_body)
+    return f'\033[30m{str_body}\033[0m'
 
 
 def red(str_body: str) -> str:
-    return _paint('31', str_body)
+    return f'\033[31m{str_body}\033[0m'
 
 
 def green(str_body: str) -> str:
-    return _paint('32', str_body)
+    return f'\033[32m{str_body}\033[0m'
 
 
 def orange(str_body: str) -> str:
-    return _paint('33', str_body)
+    return f'\033[33m{str_body}\033[0m'
 
 
 def blue(str_body: str) -> str:
-    return _paint('34', str_body)
+    return f'\033[34m{str_body}\033[0m'
 
 
 def purple(str_body: str) -> str:
-    return _paint('35', str_body)
+    return f'\033[35m{str_body}\033[0m'
 
 
 def cyan(str_body: str) -> str:
-    return _paint('36', str_body)
+    return f'\033[36m{str_body}\033[0m'
 
 
-def lightgrey(str_body: str) -> str:
-    return _paint('37', str_body)
+def light_grey(str_body: str) -> str:
+    return f'\033[37m{str_body}\033[0m'
 
 
-def darkgrey(str_body: str) -> str:
-    return _paint('90', str_body)
+def red_background(str_body: str) -> str:
+    return f'\033[41m{str_body}\033[0m'
 
 
-def lightred(str_body: str) -> str:
-    return _paint('91', str_body)
+def green_background(str_body: str) -> str:
+    return f'\033[42m{str_body}\033[0m'
 
 
-def yellow(str_body: str) -> str:
-    return _paint('93', str_body)
+def yellow_background(str_body: str) -> str:
+    return f'\033[43m{str_body}\033[0m'
 
 
-def lightblue(str_body: str) -> str:
-    return _paint('94', str_body)
+def blue_background(str_body: str) -> str:
+    return f'\033[44m{str_body}\033[0m'
 
 
-def pink(str_body: str) -> str:
-    return _paint('95', str_body)
+def purple_background(str_body: str) -> str:
+    return f'\033[45m{str_body}\033[0m'
 
 
-def lightcyan(str_body: str) -> str:
-    return _paint('96', str_body)
+def cyan_background(str_body: str) -> str:
+    return f'\033[46m{str_body}\033[0m'
 
 
-def bold(str_body: str) -> str:
-    return _paint('01', str_body)
+def light_grey_background(str_body: str) -> str:
+    return f'\033[47m{str_body}\033[0m'
 
 
-def disabled(str_body: str) -> str:
-    return _paint('02', str_body)
+def dark_grey(str_body: str) -> str:
+    return f'\033[90m{str_body}\033[0m'
 
 
-def underline(str_body: str) -> str:
-    return _paint('04', str_body)
+def light_red(str_body: str) -> str:
+    return f'\033[91m{str_body}\033[0m'
 
 
-def reverse(str_body: str) -> str:
-    return _paint('07', str_body)
+def yellow(str_body: str) -> str:
+    return f'\033[93m{str_body}\033[0m'
 
 
-def invisible(str_body: str) -> str:
-    return _paint('08', str_body)
+def light_blue(str_body: str) -> str:
+    return f'\033[94m{str_body}\033[0m'
+
+
+def pink(str_body: str) -> str:
+    return f'\033[95m{str_body}\033[0m'
 
 
-def strikethrough(str_body: str) -> str:
-    return _paint('09', str_body)
+def light_cyan(str_body: str) -> str:
+    return f'\033[96m{str_body}\033[0m'
```

### Comparing `str_style-0.1.0/PKG-INFO` & `str_style-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,116 @@
 Metadata-Version: 2.1
 Name: str-style
-Version: 0.1.0
+Version: 1.0.0
 Summary: 
+Home-page: https://github.com/esharf/str-style
 License: MIT
+Keywords: style,collor
 Author: esharf
 Author-email: 57587340+esharf@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Bug Tracker, https://github.com/esharfr/str-style/issues
+Project-URL: Repository, https://github.com/esharf/str-style
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/str-style.svg)](https://badge.fury.io/py/str-style) [![GuardRails badge](https://api.guardrails.io/v2/badges/184958?token=4d9cc37be41ca42f0bc2daa171df4f9a3c2ec046a8f510df251890dd9cdd98d2)](https://dashboard.guardrails.io/gh/esharf/repos/184958) [![codecov](https://codecov.io/gh/esharf/str-style/branch/master/graph/badge.svg?token=X35CF3HYU0)](https://codecov.io/gh/esharf/str-style)
 # str-style
 
 str-style is a Python package that provides string styling functions to enhance the visual appearance of text.
 
 #### Usage
 
-To use the str-style package, follow these steps:
+To use the str-style package in CLI, yoiu simply need to run the following:
+```bash
+str-style red Hello world
+```
+
+This will print the string "<span style="color: red">Hello world</span>" with red styling applied.
+
+To use the str-style package in your own python script, follow these steps:
 
 1. Import the desired styling function(s) from strstyle module.
 2. Apply the styling function(s) to your string(s) to modify their appearance.
 Here's an example of how to use the red styling function:
 ```python
 >>> from strstyle import red
 >>> print(red('Hello world'))
 ```
 
 This will print the string "<span style="color: red">Hello world</span>" with red styling applied.
 
-#### Available Styling Functions
+#### Available CLI Styling
+- bold
+- disabled
+- italic
+- underline
+- sharp
+- invisible
+- strike-through
+- double-underline
 - black
 - red
 - green
 - orange
 - blue
 - purple
 - cyan
-- lightgrey
-- darkgrey
-- lightred
+- light-grey
+- red-background
+- green-background
+- yellow-background
+- blue-background
+- purple-background
+- cyan-background
+- light-grey-background
+- dark-grey
+- light-red
 - yellow
-- lightblue
+- light-blue
 - pink
-- lightcyan
+- light-cyan
+
+#### Available Styling Functions
 - bold
 - disabled
+- italic
 - underline
-- reverse
+- sharp
 - invisible
-- strikethrough
+- strike_through
+- double_underline
+- black
+- red
+- green
+- orange
+- blue
+- purple
+- cyan
+- light_grey
+- red_background
+- green_background
+- yellow_background
+- blue_background
+- purple_background
+- cyan_background
+- light_grey_background
+- dark_grey
+- light_red
+- yellow
+- light_blue
+- pink
+- light_cyan
 
 
 #### Contributing
 Contributions to str-style are welcome! If you encounter any issues, have suggestions, or want to contribute improvements, please feel free to open an [issue](https://github.com/esharf/str-style/issues) or submit a [pull request](https://github.com/esharf/str-style/pulls).
 
 #### License
-This package is licensed under the MIT License. See the [LICENSE](/LICENSE) file for more details.
-
+This package is licensed under the MIT License. See the [LICENSE](https://github.com/esharf/str-style/blob/master/LICENSE) file for more details.
```

