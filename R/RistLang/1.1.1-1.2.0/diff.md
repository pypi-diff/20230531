# Comparing `tmp/RistLang-1.1.1.tar.gz` & `tmp/RistLang-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RistLang-1.1.1.tar", last modified: Fri May 19 10:37:52 2023, max compression
+gzip compressed data, was "RistLang-1.2.0.tar", last modified: Wed May 31 09:40:55 2023, max compression
```

## Comparing `RistLang-1.1.1.tar` & `RistLang-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:37:52.216957 RistLang-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-19 10:37:31.000000 RistLang-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-19 10:37:52.216957 RistLang-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-19 10:37:31.000000 RistLang-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:37:52.216957 RistLang-1.1.1/RistLang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 10:37:52.000000 RistLang-1.1.1/RistLang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:37:52.216957 RistLang-1.1.1/ristpy/
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-19 10:37:31.000000 RistLang-1.1.1/ristpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-19 10:37:31.000000 RistLang-1.1.1/ristpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-19 10:37:31.000000 RistLang-1.1.1/ristpy/walkers.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 10:37:52.216957 RistLang-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-19 10:37:31.000000 RistLang-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:55.310464 RistLang-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-31 09:40:33.000000 RistLang-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-31 09:40:55.310464 RistLang-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-31 09:40:33.000000 RistLang-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:55.310464 RistLang-1.2.0/RistLang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 09:40:55.000000 RistLang-1.2.0/RistLang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:55.310464 RistLang-1.2.0/ristpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-05-31 09:40:33.000000 RistLang-1.2.0/ristpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-31 09:40:33.000000 RistLang-1.2.0/ristpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-31 09:40:33.000000 RistLang-1.2.0/ristpy/walkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:40:55.310464 RistLang-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-31 09:40:33.000000 RistLang-1.2.0/setup.py
```

### Comparing `RistLang-1.1.1/LICENSE` & `RistLang-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RistLang-1.1.1/PKG-INFO` & `RistLang-1.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: RistLang
-Version: 1.1.1
-Summary: A module for compiling RistLang
-Home-page: https://github.com/RistPy/PyRist
-License: MIT
-Project-URL: Issue tracker, https://github.com/RistPy/PyRist/issues
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RistPy
 A programming language made by me ([@Rishiraj0100](https://GitHub.com/Rishiraj0100))
 ```
 R  - Rist
 I  - Is
 S  - Short
 T  - Text
@@ -110,34 +92,25 @@
 foo{}
 
 # asynchronous func
 ?bar{} # ? + <name_of_func>
 ```
 ### Dict 
 How can I make dict as `{}` is used as `()`
-#### Working With Dict
-To make dict to things are here
-`()` and `<>`
+#### Working With Dictionaries and sets
+Dictionaries and Sets, in this language are enclosed within parentheses
+`()`
+
 For example
+
 ```rist
 ("hi": "hello")
 ("hello": ("wor": "ld"))
-<"hi": "hi">
-
-# mixed
-<
-  1: <
-    2: (
-      3: 4
-    ),
-    5: 6
-  >,
-  7: 8
->
 ```
+
 ### Tuples and lists
 #### Making a List 
 ```rist
 [1,2]
 [
   1,
   2
@@ -147,24 +120,15 @@
 ```rist
 {1,2}
 {
   1,
   2
 }
 ```
-### Function Return TypeHints
-How do I use `def myfunc() -> None:` in rist as `>` symbol
-is used in dict?
 
-`>` is used for dictionary but however, typehints
-doesn't gets converted, it's like `} -> Any:`
-```rist
-SomeFunc${} -> None:
-  pass
-```
 ### Comments 
 To use comments in this language, use `#`, Just like Python
 
 For example:-
 ```rist
 # Some comment
 ```
@@ -185,21 +149,22 @@
 $l    # list
 $p    # pass
 $t    # type
 $b    # break
 $n    # input
 $p    # print
 $u    # tuple
+$wh   # while
 $yi   # yield
 $ex   # except
 $la   # lambda
 $o    # locals
+$ret  # return
 $fi   # finally
 $g    # globals
-$ret  # return
 $co   # continue
 $m    # __import__
 $r    # ristpy.rist
 $eval # run rist code
 $re   # regex library (re)
 ```
 
@@ -227,14 +192,119 @@
 ```
 False
 True
 True
 False
 ```
 
+## MultiFile Project
+For Multiple File projects, make a file named `ristconf.json`
+
+Format of the file is
+```json
+{
+  "main": "<main file>",
+  "dirs": [
+    "<directories to use>"
+  ],
+  "ignore": [
+    "<files to ignore>"
+  ],
+  "snippets": {
+    "<macro name>": [
+      "line1",
+      "line2"
+    ]
+  },
+  "snippets_py": {
+    "<macro name>": [
+      "line1",
+      "line2"
+    ]
+  }
+}
+```
+Here `main` key is required while others are optional
+
+A sample file is given here
+```json{
+  "main": "main.rist",
+  "dirs": ["dir_example"],
+  "ignore": ["not_to_compile.rist"],
+  "snippets": {
+    "a": [
+      "$p{0}",
+      "$p{1}",
+      "$p{2}"
+    ]
+  },
+  "snippets_py": {
+    "b": [
+      "print(3)",
+      "print(4)",
+      "print(5)"
+    ]
+  }
+}
+```
+Now the question arises, what is the `snippets` key given here.
+
+Here you can create macros which you can directly import in rist files
+
+## Working with macros
+Syntax
+```json
+{
+  "snippets": {
+    "<name of macro>": [
+      "Line 1, (in rist)",
+      "Line 2, (in rist)",
+      "and so on...(in rist)"
+    ]
+  },
+  "snippets_py": {
+    "<name of macro>": [
+      "Line 1, (in Python)",
+      "Line 2, (in Python)",
+      "and so on...(in Python)"
+    ]
+  }
+}
+```
+For example
+```json
+{
+  "main": "main.rist",
+  "snippets": {
+    "a": [
+      "$p{0}",
+      "$p{1}",
+      "$p{2}"
+    ]
+  },
+  "snippets_py": {
+    "b": [
+      "print(3)",
+      "print(4)"
+    ]
+  }
+}
+```
+You can use it by `%- <name of macro> -%`
+
+```rist
+%- a -%
+
+# inside function
+func${}:
+  %- b -%
+
+```
+> Note: Nothing other should be there in the lines containing `%-` syntax
+
 ## Encryptions/Decryptions
 Encryptions and Decryptions too comes with rist.
 You can encrypt anything with rist!
 
 ### Encrypting from shell
 If you want to encrypt something, then just run this in your shell
 ```
```

### Comparing `RistLang-1.1.1/RistLang.egg-info/PKG-INFO` & `RistLang-1.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RistLang
-Version: 1.1.1
+Version: 1.2.0
 Summary: A module for compiling RistLang
 Home-page: https://github.com/RistPy/PyRist
 License: MIT
 Project-URL: Issue tracker, https://github.com/RistPy/PyRist/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -110,34 +110,25 @@
 foo{}
 
 # asynchronous func
 ?bar{} # ? + <name_of_func>
 ```
 ### Dict 
 How can I make dict as `{}` is used as `()`
-#### Working With Dict
-To make dict to things are here
-`()` and `<>`
+#### Working With Dictionaries and sets
+Dictionaries and Sets, in this language are enclosed within parentheses
+`()`
+
 For example
+
 ```rist
 ("hi": "hello")
 ("hello": ("wor": "ld"))
-<"hi": "hi">
-
-# mixed
-<
-  1: <
-    2: (
-      3: 4
-    ),
-    5: 6
-  >,
-  7: 8
->
 ```
+
 ### Tuples and lists
 #### Making a List 
 ```rist
 [1,2]
 [
   1,
   2
@@ -147,24 +138,15 @@
 ```rist
 {1,2}
 {
   1,
   2
 }
 ```
-### Function Return TypeHints
-How do I use `def myfunc() -> None:` in rist as `>` symbol
-is used in dict?
 
-`>` is used for dictionary but however, typehints
-doesn't gets converted, it's like `} -> Any:`
-```rist
-SomeFunc${} -> None:
-  pass
-```
 ### Comments 
 To use comments in this language, use `#`, Just like Python
 
 For example:-
 ```rist
 # Some comment
 ```
@@ -185,21 +167,22 @@
 $l    # list
 $p    # pass
 $t    # type
 $b    # break
 $n    # input
 $p    # print
 $u    # tuple
+$wh   # while
 $yi   # yield
 $ex   # except
 $la   # lambda
 $o    # locals
+$ret  # return
 $fi   # finally
 $g    # globals
-$ret  # return
 $co   # continue
 $m    # __import__
 $r    # ristpy.rist
 $eval # run rist code
 $re   # regex library (re)
 ```
 
@@ -227,14 +210,119 @@
 ```
 False
 True
 True
 False
 ```
 
+## MultiFile Project
+For Multiple File projects, make a file named `ristconf.json`
+
+Format of the file is
+```json
+{
+  "main": "<main file>",
+  "dirs": [
+    "<directories to use>"
+  ],
+  "ignore": [
+    "<files to ignore>"
+  ],
+  "snippets": {
+    "<macro name>": [
+      "line1",
+      "line2"
+    ]
+  },
+  "snippets_py": {
+    "<macro name>": [
+      "line1",
+      "line2"
+    ]
+  }
+}
+```
+Here `main` key is required while others are optional
+
+A sample file is given here
+```json{
+  "main": "main.rist",
+  "dirs": ["dir_example"],
+  "ignore": ["not_to_compile.rist"],
+  "snippets": {
+    "a": [
+      "$p{0}",
+      "$p{1}",
+      "$p{2}"
+    ]
+  },
+  "snippets_py": {
+    "b": [
+      "print(3)",
+      "print(4)",
+      "print(5)"
+    ]
+  }
+}
+```
+Now the question arises, what is the `snippets` key given here.
+
+Here you can create macros which you can directly import in rist files
+
+## Working with macros
+Syntax
+```json
+{
+  "snippets": {
+    "<name of macro>": [
+      "Line 1, (in rist)",
+      "Line 2, (in rist)",
+      "and so on...(in rist)"
+    ]
+  },
+  "snippets_py": {
+    "<name of macro>": [
+      "Line 1, (in Python)",
+      "Line 2, (in Python)",
+      "and so on...(in Python)"
+    ]
+  }
+}
+```
+For example
+```json
+{
+  "main": "main.rist",
+  "snippets": {
+    "a": [
+      "$p{0}",
+      "$p{1}",
+      "$p{2}"
+    ]
+  },
+  "snippets_py": {
+    "b": [
+      "print(3)",
+      "print(4)"
+    ]
+  }
+}
+```
+You can use it by `%- <name of macro> -%`
+
+```rist
+%- a -%
+
+# inside function
+func${}:
+  %- b -%
+
+```
+> Note: Nothing other should be there in the lines containing `%-` syntax
+
 ## Encryptions/Decryptions
 Encryptions and Decryptions too comes with rist.
 You can encrypt anything with rist!
 
 ### Encrypting from shell
 If you want to encrypt something, then just run this in your shell
 ```
```

### Comparing `RistLang-1.1.1/ristpy/__init__.py` & `RistLang-1.2.0/ristpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,22 +74,27 @@
   flags = _ParsedFlags()
   for attr in attrs.keys():
     setattr(flags, attr, attrs[attr])
 
   return flags
 
 def rist(arg: str, fp: bool = True, flags: RistFlags = C, **kwargs) -> str:
+  macros = kwargs.pop("macros", {})
+  macro_py = kwargs.pop("macros_py", {})
+  for n, snippet in macros.items():
+    assert n not in macro_py, "Name of all the snippets should be unique"
+    macro_py[n] = rist(snippet, False, C, file=f"<macro_{n}>", macro_py=macro_py).splitlines()
   flags = _parse_flags(flags)
   if fp:
     with open(arg, 'r') as f:
       code = f.read()
     fname = arg
   else:
     code = arg
-    fname = '<unknown.rist>'
+    fname = kwargs.pop("file", "<unknown.rist>")
 
   class _Token:
     def __init__(
       self,
       name: str,
       value: Union[str, int],
       line: int,
@@ -111,34 +116,32 @@
   class __Interpreter:
     __rules: List[Tuple[str, str]] = [
       ('COMMENT', r'#.*'),
       ('DOCSTRING', r'"""'),
       ('DOCSTRING', r"'''"),
       ('STRING', r'((".*?")(?<!(\\)))'),
       ('STRING', r"(('.*?')(?<!(\\)))"),
+      ('MACRO', r"^(\s)*\%\-(\s)*{NAME}(\s)*\-\%(\s)*$"),
       ('FROM', r'^(\s)*\+@(\s*)([.]?{ATTRIBUTED_NAME}|{NAME})(\s*)@\+(\s*)({ATTRIBUTED_NAME}|\*|\{)'),
       ('IMPORT', r'^(\s)*@\+(\s*){ATTRIBUTED_NAME}'),
       ('ERR_IMPORT', r'\+@ ({ATTRIBUTED_NAME}|{NAME}) @\+ ({ATTRIBUTED_NAME}|\*|\{)'),
       ('ERR_IMPORT', r'@\+ {ATTRIBUTED_NAME}'),
       ('FUNCDEF', r'(\$)?{NAME}\$\{'),
-      ('PREDEFS', r'\$(ret|re|co|yi|pa|b|i|p|d|t|n|m|s|u|o|g|r|eval|ei|la|y|fi|ex|e|l|x|f)'),
+      ('PREDEFS', r'\$(ret|re|co|yi|pa|b|i|p|d|t|n|m|s|u|o|g|r|eval|ei|la|y|fi|ex|e|l|x|f|wh)'),
       ('AT', '@{ATTRIBUTED_NAME}'),
       ('ARROW', r'\}( )?\-\>( )?{ATTRIBUTED_NAME}?'),
-      ('GTORLT', r'__(\<|\>)'),
       ('AWAIT', r'\?(\s+)?'),
-      ('LARROW', r'\<'),
-      ('RARROW', r'\>'),
       ('NUMBER', r'\d+\.\d+'),
       ('NUMBER', r'\d+'),
       ('ATTRIBUTED_NAME', r'{NAME}?([.]*(?=[a-zA-Z_])([a-zA-Z0-9_]*))+'),
       ('NAME', r'[a-zA-Z_][a-zA-Z0-9_]*'),
       ('TABSPACE', '\t'),
       ('SPACE', ' '),
       ('OPERATOR', r'[\+\*\-\/%]'),       # arithmetic operators
-      ('OPERATOR', r'==|!='),             # comparison operators
+      ('OPERATOR', r'==|!=|\<|\>'),             # comparison operators
       ('OPERATOR', r'\|\||\||&|&&'),      # boolean operators
       ('OPERATOR', r'\.\.\.|\.\.'),       # range operators
       ('OPERATOR', r'!'),
       ('ASSIGN', '='),
       ('LPAREN', r'\('),
       ('RPAREN', r'\)'),
       ('LBRACK', r'\['),
@@ -234,14 +237,16 @@
   
     @classmethod
     def interprete(cls, s, f) -> str:
       self = cls()
       tokens = []
       line_num = 0
       lines = s.splitlines()
+      under = ""
+      under_info = {}
       for line_num, line in enumerate(lines, 1):
         line = line.rstrip()
         if not line:
           tokens.append(_Token('NEWLINE', "\n", line_num, 1))
           continue
         line_tokens = list(self.__interprete_line(line, line_num, f))
         if line_tokens:
@@ -250,53 +255,92 @@
 
       if self.under_docstring:
         err = SyntaxError(f"EOF while scanning docstring literal")
         kwrds = dict(filename=f, lineno=len(lines), offset=len(lines[-1]), text=lines[-1])
         for k, v in kwrds.items():
           setattr(err, k, v)
         raise err
-
+      
       ntoks = []
+      i_n=[0,0]
+      el = 0
       for tok in tokens:
-        if tok.name == "LCBRACK" and tok.value == "{":
-          ntoks.append(_Token("LPAREN", "(", tok.line, tok.coloumn))
+        if tok.line!=i_n[0]:
+          i_n = [tok.line, 0]
+        if tok.name not in ("STRING", "DOCSTRING", "COMMENT"):
+          for i in tok.value:
+            i_n[-1]+=1
+            if i not in "[{()}]":
+              continue
+            if i in ")}]":
+              if (not under) or under[-1]!=i:
+                err = SyntaxError(f"Unmatched '{i}'" if not under else f"Got '{i}', while expecting '{under[-1]}'")
+                kwrds = dict(filename=f, lineno=tok.line, offset=i_n[-1], text=lines[tok.line-1])
+                for k, v in kwrds.items(): setattr(err, k, v)
+                raise err
+
+              under = under[:-1]
+              under_info = under_info["par"]
+            if i in "[{(":
+              under+={"[":"]","{":"}","(":")"}[i]
+              under_info["par"] = {**under_info}
+              under_info["line"] = tok.line
+              under_info["offset"] = i_n[-1]
+              
+        tok.under=under
+        l_n = tok.line + el
+        if tok.name == "MACRO":
+          indent, n = tok.value.split("%-")
+          n = n.split("-%")[0].strip()
+          assert n in macro_py, f"Snippet '{n}' not found!"
+          v = indent + f"\n{indent}".join(macro_py[n])
+          el+=len(v.splitlines())-1
+          ntoks.append(_Token(f"MACRO_{n}", v, tok.line, 0))
+        elif tok.name == "LCBRACK" and tok.value == "{":
+          ntoks.append(_Token("LPAREN", "(", l_n, tok.coloumn))
         elif tok.name == "RCBRACK" and tok.value == "}":
-          ntoks.append(_Token("RPAREN", ")", tok.line, tok.coloumn))
+          ntoks.append(_Token("RPAREN", ")", l_n, tok.coloumn))
         elif tok.name == "FUNCDEF":
           if tok.value.startswith("$"):val="async def "+tok.value[1:]
           else:val="def "+tok.value
           val=val.replace("${","(")
-          ntoks.append(_Token("FUNCDEF", val, tok.line, tok.coloumn))
-        elif (tok.name == "LPAREN" and tok.value == "(") or (tok.name == "LARROW" and tok.value == "<"):
-          ntoks.append(_Token("LCBRACK", "{", tok.line, tok.coloumn))
-        elif (tok.name == "RPAREN" and tok.value == ")") or (tok.name == "RARROW" and tok.value == ">"):
-          ntoks.append(_Token("RCBRACK", "}", tok.line, tok.coloumn))
+          ntoks.append(_Token("FUNCDEF", val, l_n, tok.coloumn))
+        elif tok.name == "LPAREN" and tok.value == "(":
+          ntoks.append(_Token("LCBRACK", "{", l_n, tok.coloumn))
+        elif tok.name == "RPAREN" and tok.value == ")":
+          ntoks.append(_Token("RCBRACK", "}", l_n, tok.coloumn))
         elif tok.name=="PREDEFS":
           r="__import__('ristpy').rist"
           e="(lambda code:__import__('ristpy').execute(code,[2])"
           x="(lambda a,b:((not (a and b)) and (a or b)))"
           extra={"o":"locals","g":"globals","r":r,"eval":e,"e":"else","ei":"elif","la":"lambda","x":x,"y":"try","fi":"finally","ex":"except"}
           ex2={"b":"break","f":"for","re":"__import__('re')","ret":"return","co":"continue","yi":"yield","pa":"pass"}
           ntoks.append(_Token("PREDEFS",
-            {'i':"int",'p':"print",'d':"dict",'l':"list",'t':"type",'n':"input",'m':"__import__",'s':"str",'u':"tuple",**extra,**ex2}[tok.value[1:]],
-            tok.line,tok.coloumn
+            {'i':"int",'p':"print",'d':"dict",'l':"list",'t':"type",'n':"input",'m':"__import__",'s':"str",'u':"tuple","wh":"while",**extra,**ex2}[tok.value[1:]],
+            l_n,tok.coloumn
           ))
         elif tok.name == "ARROW":
-          ntoks.append(_Token(tok.name, ")"+tok.value[1:], tok.line, tok.coloumn))
+          ntoks.append(_Token(tok.name, ")"+tok.value[1:], l_n, tok.coloumn))
         elif tok.name == "AWAIT":
-          ntoks.append(_Token(tok.name, "await ", tok.line, tok.coloumn))
+          ntoks.append(_Token(tok.name, "await ", l_n, tok.coloumn))
         elif tok.name == "FROM":
-          ntoks.append(_Token(tok.name, tok.value.replace("+@","from").replace("@+","import").replace("{","("), tok.line, tok.coloumn))
+          ntoks.append(_Token(tok.name, tok.value.replace("+@","from").replace("@+","import").replace("{","("), l_n, tok.coloumn))
         elif tok.name == "IMPORT":
-          ntoks.append(_Token(tok.name, tok.value.replace("@+","import"), tok.line, tok.coloumn))
-        elif tok.name == "GTORLT" and tok.value.startswith('__'):
-          ntoks.append(_Token(tok.name, tok.value[-1], tok.line, tok.coloumn))
+          ntoks.append(_Token(tok.name, tok.value.replace("@+","import"), l_n, tok.coloumn))
         else:
           ntoks.append(tok)
+          
+        ntoks[-1].under = under
 
+      if under:
+        err = SyntaxError(f"Unexpected EOF")
+        kwrds = dict(filename=f, lineno=under_info["line"], offset=under_info["offset"], text=lines[under_info["line"]-1])
+        for k, v in kwrds.items():
+          setattr(err, k, v)
+        raise err
       code = "".join(list(str(t) for t in ntoks))
   
       return code
   
   class __CompiledCode(str):
     @classmethod
     def setup(cls, code: str, fname: str = '<unknown>') -> None:
```

### Comparing `RistLang-1.1.1/ristpy/__main__.py` & `RistLang-1.2.0/ristpy/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 import json
+import atexit
+import signal
 import argparse
 
 from ristpy import rist, execute, E, W, encrypt, decrypt
 
 
 def init(parser, args):
   if "ristconf.json" not in os.listdir():
@@ -13,36 +15,54 @@
   except Exception as e:
     raise e
 
   main=conf.get("main") or ""
   assert bool(main) is True, "A setting named 'main' should must be in the config file"
   assert main.endswith(".rist"), "Your main file should must be a rist file"
   mf=main if "/" in main else "./"+main
+  macros = conf.get("snippets", {})
+  for name, snippet in macros.items():
+    if type(snippet) is list: macros[name] = "\n".join(snippet)
+      
+  macros_py = conf.get("snippets_py", {})
+  for name, snippet in macros_py.items():
+    if type(snippet) is list:
+      snippet = "\n".join(snippet)
+    macros_py[name] = snippet.splitlines()
+    
+  
+  for n, snippet in macros.items():
+    assert n not in macros_py, "Name of all the snippets should be unique"
+    macros_py[n] = rist(snippet, False, file=f"<macro_{n}>", macro_py=macros_py).splitlines()
+
   dirs=conf.get("dirs") or []
   ign=conf.get("ignore") or []
   ign.append(mf)
   if "." not in dirs: dirs.append(".")
   pyfiles=[]
   def rm():
     for f in pyfiles:
       try:os.remove(f)
       except:continue
   try:
     def mk(f):
       nonlocal pyfiles
       if f not in ign:
         pyfiles.append(f[:-4]+"py")
-        rist(f, flags=W, compile_to=f[:-4]+"py")
+        rist(f, flags=W, compile_to=f[:-4]+"py", macros_py={**macros_py})
     for dir in dirs:
       if not dir.endswith("/"): dir+="/"
       for file in os.listdir(dir):
         if file.endswith(".rist"):
           file=dir+file
           mk(file)
     mk(main)
+    atexit.register(rm)
+    signal.signal(signal.SIGTERM, rm)
+    signal.signal(signal.SIGINT, rm)
     os.system(f'python3 {main[:-4]+"py"}')
   except Exception as e:
     rm()
     raise e
   finally:
     rm()
```

### Comparing `RistLang-1.1.1/ristpy/walkers.py` & `RistLang-1.2.0/ristpy/walkers.py`

 * *Files identical despite different names*

### Comparing `RistLang-1.1.1/setup.py` & `RistLang-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-version = "1.1.1"
+version = "1.2.0"
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 if version.endswith(('a', 'b', 'rc')):
   # append version identifier based on commit count
   try:
```

