# Comparing `tmp/markpickle-1.3.0.tar.gz` & `tmp/markpickle-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markpickle-1.3.0.tar", max compression
+gzip compressed data, was "markpickle-1.4.0.tar", max compression
```

## Comparing `markpickle-1.3.0.tar` & `markpickle-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-05-26 20:14:01.644909 markpickle-1.3.0/LICENSE
--rw-r--r--   0        0        0     5763 2023-05-26 20:16:03.084691 markpickle-1.3.0/README.md
--rw-r--r--   0        0        0      574 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/__init__.py
--rw-r--r--   0        0        0     1225 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/__main__.py
--rw-r--r--   0        0        0     1543 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/binary_streams.py
--rw-r--r--   0        0        0       57 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/cli.py
--rw-r--r--   0        0        0     2298 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/config_class.py
--rw-r--r--   0        0        0    11510 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/deserialize.py
--rw-r--r--   0        0        0      359 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/meta.py
--rw-r--r--   0        0        0      568 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/mypy_types.py
--rw-r--r--   0        0        0       80 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/py.typed
--rw-r--r--   0        0        0     4817 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/python_to_tables.py
--rw-r--r--   0        0        0    14695 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/serialize.py
--rw-r--r--   0        0        0      737 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/simplify_types.py
--rw-r--r--   0        0        0     1032 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/split_file_code.py
--rw-r--r--   0        0        0     1252 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/third_party_tables.py
--rw-r--r--   0        0        0     1741 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/tool.py
--rw-r--r--   0        0        0      762 2023-05-26 20:14:01.648909 markpickle-1.3.0/markpickle/unicode_formatting.py
--rw-r--r--   0        0        0     3624 2023-05-26 20:14:01.648909 markpickle-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7278 1970-01-01 00:00:00.000000 markpickle-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 01:40:36.109373 markpickle-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6119 2023-05-31 01:40:36.109373 markpickle-1.4.0/README.md
+-rw-r--r--   0        0        0      574 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/__main__.py
+-rw-r--r--   0        0        0     1697 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/atx_as_dictionary.py
+-rw-r--r--   0        0        0     1543 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/binary_streams.py
+-rw-r--r--   0        0        0       57 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/cli.py
+-rw-r--r--   0        0        0     2298 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/config_class.py
+-rw-r--r--   0        0        0    12845 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/deserialize.py
+-rw-r--r--   0        0        0      412 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/meta.py
+-rw-r--r--   0        0        0      568 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/mypy_types.py
+-rw-r--r--   0        0        0       80 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/py.typed
+-rw-r--r--   0        0        0     4817 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/python_to_tables.py
+-rw-r--r--   0        0        0    14841 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/serialize.py
+-rw-r--r--   0        0        0      737 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/simplify_types.py
+-rw-r--r--   0        0        0     1032 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/split_file_code.py
+-rw-r--r--   0        0        0     1252 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/third_party_tables.py
+-rw-r--r--   0        0        0     1760 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/tool.py
+-rw-r--r--   0        0        0      813 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/unicode_formatting.py
+-rw-r--r--   0        0        0     3720 2023-05-31 01:40:36.109373 markpickle-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 markpickle-1.4.0/PKG-INFO
```

### Comparing `markpickle-1.3.0/LICENSE` & `markpickle-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/README.md` & `markpickle-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # markpickle
 
-Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown.
+Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
 For example this
 
 ```markdown
 - 1
 - 2
 ```
@@ -94,28 +94,32 @@
 
 [pytablewriter](https://pytablewriter.readthedocs.io/en/latest/pages/reference/writers/text/markup/md.html) also, dict to table, but supports many tabular formats.
 
 ### Deserializing to Python
 
 Most libraries turn markdown into document object model. Markdown-to-json is the most similar to markpickle's goal of turning a markdown document into a python data types, in this case nested dicts.
 
-[markdown-to-json](https://github.com/njvack/markdown-to-json)
+[markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle, but is somewhat broken, unmaintained and depends on the unmaintained commonmark library.
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
-## [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
+[beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
 ## Schema Validation for Markdown
 
 In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
 
 I haven't really found anything that says, for example, "This markdown document shall have one # Header and a 3 column table and nothing else."
 
 - [schema-markdown-js](https://craigahobbs.github.io/schema-markdown-js/language/) A json schema that happens to be using markdown as its syntax.
 
+## Credits
+
+I copied the ATX-dictionary-like header parsing from [markdown-to-json](https://github.com/njvack/markdown-to-json).
+
 ## Documentation
 
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
 ## Change Log
```

### Comparing `markpickle-1.3.0/markpickle/__init__.py` & `markpickle-1.4.0/markpickle/__init__.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/__main__.py` & `markpickle-1.4.0/markpickle/tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-"""
-CLI support
+r"""Command-line tool to validate and pretty-print Markdown as simple Python types
+
+Usage::
+
+    $ echo '-a\n-b\n-c' | python -m markpickle.tool
+    ["a", "b", "c"]
+
+Source code modeled after json.tool https://github.com/python/cpython/blob/3.11/Lib/json/tool.py
 """
 import argparse
-import json
 import sys
 from pathlib import Path
 
 import markpickle
 
-if __name__ == "__main__":
+
+def main():
     """CLI entry point"""
-    prog = "python -m markpickle"
-    description = "Command-line tool to convert some markdown to json"
+    prog = "python -m markpickle.tool"
+    description = "Command-line tool to validate and pretty-print Markdown as simple Python types"
     parser = argparse.ArgumentParser(prog=prog, description=description)
     parser.add_argument(
         "infile",
         nargs="?",
         type=argparse.FileType(encoding="utf-8"),
         help="a Markdown file to be pretty-printed",
         default=sys.stdin,
@@ -23,19 +29,29 @@
     parser.add_argument("outfile", nargs="?", type=Path, help="write the output of infile to outfile", default=None)
     options = parser.parse_args()
 
     dump_args = {}
 
     with options.infile as infile:
         try:
-            objs = (markpickle.load(infile),)
+            if options.json_lines:
+                objs = (markpickle.loads(line) for line in infile)
+            else:
+                objs = (markpickle.load(infile),)
 
             if options.outfile is None:
                 out = sys.stdout
             else:
                 out = options.outfile.open("w", encoding="utf-8")
             with out as outfile:
                 for obj in objs:
-                    json.dump(obj, outfile, **dump_args)
+                    markpickle.dump(obj, outfile, **dump_args)
                     outfile.write("\n")
-        except ValueError as e:
-            raise SystemExit(e)
+        except ValueError as error:
+            raise SystemExit(error) from error
+
+
+if __name__ == "__main__":
+    try:
+        main()
+    except BrokenPipeError as exc:
+        sys.exit(exc.errno)
```

### Comparing `markpickle-1.3.0/markpickle/binary_streams.py` & `markpickle-1.4.0/markpickle/binary_streams.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/config_class.py` & `markpickle-1.4.0/markpickle/config_class.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/deserialize.py` & `markpickle-1.4.0/markpickle/deserialize.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 Arbitrary strings might not pass or may pass but create values that still have unparsed markdown in them.
 """
 import datetime
 import io
 import logging
 import textwrap
+import urllib
 from typing import Any, Generator, Optional, cast
 
 import mistune
 
 import markpickle.python_to_tables as python_to_tables
+from markpickle.atx_as_dictionary import parse_outermost_dict
 from markpickle.binary_streams import extract_bytes
 from markpickle.config_class import Config
-from markpickle.mypy_types import DictTypes, ListTypes, ScalarTypes, SerializableTypes
+from markpickle.mypy_types import ListTypes, ScalarTypes, SerializableTypes
 
 
 def loads(value: str, config: Optional[Config] = None, object_hook=None) -> SerializableTypes:
     """
     Convert certain markdown strings into simple Python types
 
     >>> loads("- a\\n- b\\n - c\\n")
@@ -87,49 +89,58 @@
 
 
 def process_list(list_ast: Any, config: Config) -> Optional[ListTypes]:
     """Deserialize a markdown list in AST form"""
     current_list = []
     for token in list_ast["children"]:
         if token["type"] == "list_item":
-            if token["children"][0]["type"] == "block_text":
-                block_text = token["children"][0]
-                if block_text["children"][0]["type"] == "text":
-                    current_value = ",".join(text["text"] for text in block_text["children"])
-                    scalar = extract_scalar(current_value, config)
-                    current_list.append(scalar)
+            for child in token["children"]:
+                if child["type"] == "block_text":
+                    block_text = child
+                    if block_text["children"][0]["type"] == "text":
+                        # This fails if not all text!
+                        current_value = ",".join(str(text.get("text")) for text in block_text["children"])
+                        scalar = extract_scalar(current_value, config)
+                        current_list.append(scalar)
+                    elif block_text["children"][0]["type"] == "link":
+                        # Doesn't handle title or text
+                        url = urllib.parse.urlparse(block_text["children"][0]["link"])
+                        current_list.append(url)
+                    else:
+                        raise NotImplementedError(block_text["children"])
+                elif child["type"] == "list":
+                    current_list.append(process_list(child, config))
                 else:
-                    raise NotImplementedError()
-            else:
-                raise NotImplementedError()
+                    raise NotImplementedError(child["type"])
         else:
             raise NotImplementedError()
     return current_list
 
 
 def load_all(
     value: io.StringIO, config: Optional[Config] = None, object_hook=None
 ) -> Generator[SerializableTypes, None, None]:
     """Load multiple documents from a single stream"""
     part = io.StringIO()
-    has_data = False
+    has_data = True
     while True:
         line = value.readline()
-        if line is None:
+        if line is None or line == "":
             break
         if line.startswith("---") and not has_data:
             continue
         if line.startswith("---"):
             part.seek(0)
             yield load(part, config, object_hook)
             has_data = False
             part = io.StringIO()
             continue
         part.write(line)
         has_data = True
+    # last part
     if has_data:
         part.seek(0)
         yield load(part, config, object_hook)
 
 
 def loads_all(
     value: str, config: Optional[Config] = None, object_hook=None
@@ -147,96 +158,49 @@
             break
         part.write(line)
         has_data = True
     if has_data:
         yield loads(part.read(), config, object_hook)
 
 
-def load(value: io.StringIO, config: Optional[Config] = None, object_hook=None) -> SerializableTypes:
-    """
-    Convert certain markdown streams into simple Python types
-
-    >>> import io
-    >>> load(io.StringIO("- a\\n- b\\n - c\\n"))
-    ['a', 'b', 'c']
-    """
-    if not config:
-        config = Config()
-
-    # too much is RawText?
-    # d = Document([marks.read()])
-    # output = ast_renderer.get_ast(d)
-    # assert output
-
-    # Better!
-    # markdown = marko.Markdown(renderer=ASTRenderer)
-    # rerendered = markdown(marks.read())
-    # assert rerendered
-
-    string_value = value.read()
-    # TODO: maybe only do this if top level is block_code
-    string_value = textwrap.dedent(string_value)
-
-    # Empty document
-    if not string_value:
-        # Exists to improve round-tripping for unit tests
-        return cast(SerializableTypes, config.empty_string_is)
-
-    parser = mistune.create_markdown(renderer="ast")
-    result = parser.parse(string_value)
-
-    # Process a list
-    if len(result) == 1 and result[0]["type"] == "list":
-        return process_list(result[0], config)
-
-    possible_dict: DictTypes = {}
-    current_key = None
-
-    # Use this key when we find more text, ie a subsequent token that is just more text.
-    most_recent_key = None
-
-    # Iterate through tokens in the parsed result
-    for token in result:
+def process_list_of_tokens(list_of_tokens: list[dict[str, Any]], config: Config):
+    """Process a list of tokens to lists and scalars and so on."""
+    # Tokens that are not ATX-dict-like headers
+    return_value = None
+    for token in list_of_tokens:
         if token["type"] == "newline":
             # Whitespace, no impact on datatype
             continue
 
-        if token["type"] == "heading" and current_key is None:
-            # Dict key, value not found yet
-            if not all("text" in _ for _ in token["children"]):
-                print("uh oh")
-            current_key = ",".join([_["text"] for _ in token["children"]])
-            possible_dict[current_key] = None
-        elif token["type"] == "heading" and current_key is not None:
-            # New dict key, value not found yet
-            if not all("text" in _ for _ in token["children"]):
-                print("uh oh")
-            current_key = ",".join([_["text"] for _ in token["children"]])
-            possible_dict[current_key] = None
-        elif token["type"] == "list" and current_key is not None:
+        # if token["type"] == "heading" and current_key is None:
+        #     # Dict key, value not found yet
+        #     if not all("text" in _ for _ in token["children"]):
+        #         print("uh oh")
+        #     current_key = ",".join([_["text"] for _ in token["children"]])
+        #     possible_dict[current_key] = None
+        # elif token["type"] == "heading" and current_key is not None:
+        #     # New dict key, value not found yet
+        #     if not all("text" in _ for _ in token["children"]):
+        #         print("uh oh")
+        #     current_key = ",".join([_["text"] for _ in token["children"]])
+        #     possible_dict[current_key] = None
+        if token["type"] == "list":
             # Dict value of type list
             if token["children"][0]["type"] == "text":
-                possible_dict[current_key] = [
-                    ",".join(_["text"] for _ in item["children"]) for item in token["children"]
-                ]
-                most_recent_key = current_key
-                current_key = None
+                return_value = [",".join(_["text"] for _ in item["children"]) for item in token["children"]]
             elif token["children"][0]["type"] == "list_item":
-                possible_dict[current_key] = process_list(token, config)
-                most_recent_key = current_key
-                current_key = None
+                return_value = process_list(token, config)
             else:
                 raise NotImplementedError()
 
         elif (
             token["type"] == "paragraph"
             and token.get("children")
             and len(token["children"]) == 1
             and token["children"][0]["type"] in ("text", "image")
-            and not possible_dict
         ):
             if token["children"][0]["type"] == "image":
                 return extract_bytes(token["children"][0]["src"], config)
 
             # Root scalar
             current_text_value: str = token["children"][0]["text"]
             if current_text_value.count("|") >= 2 and config.tables_become_list_of_tuples:
@@ -245,68 +209,128 @@
             return extract_scalar(current_text_value, config)
 
         elif (
             token["type"] == "paragraph"
             and token.get("children")
             and len(token["children"]) == 1
             and token["children"][0]["type"] == "text"
-            and possible_dict
-            and current_key
         ):
             # Root scalar
             if token["children"][0]["type"] == "text":
                 current_value: str = token["children"][0]["text"]
                 scalar = extract_scalar(current_value, config)
             elif token["children"][0]["type"] == "image":
                 scalar = extract_bytes(token["children"][0]["src"], config)
             else:
                 raise NotImplementedError()
-            possible_dict[current_key] = scalar
-            most_recent_key = current_key
-            current_key = None
-        elif (
-            token["type"] == "paragraph"
-            and token.get("children")
-            # and len(token["children"]) == 1
-            # and token["children"][0]["type"] == "text"
-            and possible_dict
-            and most_recent_key
-            and not current_key
-        ):
-            series_of_children = token["children"]
-            most_recent_key = handle_series_of_children(config, most_recent_key, possible_dict, series_of_children)
-            current_key = None
-        elif token["type"] == "block_code" and possible_dict:
+            return_value = scalar
+        # what was this?
+        # elif (
+        #         token["type"] == "paragraph"
+        #         and token.get("children")
+        #         # and len(token["children"]) == 1
+        #         # and token["children"][0]["type"] == "text"
+        # ):
+        #     series_of_children = token["children"]
+        #     most_recent_key = handle_series_of_children(config, most_recent_key, outermost_dict, series_of_children)
+        #     current_key = None
+        elif token["type"] == "block_code":
             # Treat block code as just more text, no "styling"
             continuation_value: str = token["text"]
             scalar = extract_scalar(continuation_value, config)
             # continuation of text
-            if most_recent_key and not current_key:
-                possible_dict[most_recent_key] += "\n\n" + scalar
-                current_key = None
-            elif current_key:
-                possible_dict[current_key] = scalar
+            if return_value:
+                return_value += "\n\n" + scalar
             else:
-                raise TypeError("This shouldn't happen")
-        else:
-            raise NotImplementedError(token["type"])
+                return_value = scalar
+        elif token["type"] == "heading":
+            # handled elsewhere?
+            pass
+        # else:
+        #     raise NotImplementedError(token["type"])
+    return return_value
+
+
+def load(value: io.StringIO, config: Optional[Config] = None, object_hook=None) -> SerializableTypes:
+    """
+    Convert certain markdown streams into simple Python types
+
+    >>> import io
+    >>> load(io.StringIO("- a\\n- b\\n - c\\n"))
+    ['a', 'b', 'c']
+    """
+    if not config:
+        config = Config()
+
+    # too much is RawText?
+    # d = Document([marks.read()])
+    # output = ast_renderer.get_ast(d)
+    # assert output
+
+    # Better!
+    # markdown = marko.Markdown(renderer=ASTRenderer)
+    # rerendered = markdown(marks.read())
+    # assert rerendered
+
+    string_value = value.read()
+    # TODO: maybe only do this if top level is block_code
+    string_value = textwrap.dedent(string_value)
+
+    # Empty document
+    if not string_value:
+        # Exists to improve round-tripping for unit tests
+        return cast(SerializableTypes, config.empty_string_is)
+
+    parser = mistune.create_markdown(renderer="ast")
+    result = parser.parse(string_value)
+
+    # Process a list
+    if len(result) == 1 and result[0]["type"] == "list":
+        return process_list(result[0], config)
+
+    dict_wrapper = False
+    # handle ATX-dict-like headers
+    has_headers = any(True if item["type"] == "heading" else False for item in result)
+    if has_headers:
+        minimum = min(item["level"] if item["type"] == "heading" else 100000000 for item in result)
+        outermost_dict = parse_outermost_dict(result, minimum)
+        outermost_dict = walk_dict(outermost_dict, config)
+    else:
+        dict_wrapper = True
+        outermost_dict = {None: process_list_of_tokens(result, config)}
 
     # if possible_dict and possible_dict.get("python_type"):
     #     python_type = possible_dict.get("python_type")
     #     if constructor := globals().get(python_type):
     #         if hasattr(constructor, "__getstate__"):
     #             possible_dict = constructor.__setstate__(possible_dict)
     #         else:
     #             constructor(**possible_dict)
 
     # really? do I misunderstand this?
     if object_hook:
-        return object_hook(possible_dict)
+        return object_hook(outermost_dict)
 
-    return possible_dict
+    if dict_wrapper:
+        # Not ATX
+        return outermost_dict.get(None)
+    return outermost_dict
+
+
+def walk_dict(outermost_dict: dict[str, Any], config: Config):
+    """Process all lists of tokens found anywhere in this dictionary"""
+    if isinstance(outermost_dict, dict):
+        for current_key, list_or_dict_of_tokens in outermost_dict.items():
+            if isinstance(list_or_dict_of_tokens, list):
+                outermost_dict[current_key] = process_list_of_tokens(list_or_dict_of_tokens, config)
+            elif isinstance(list_or_dict_of_tokens, dict):
+                outermost_dict[current_key] = walk_dict(list_or_dict_of_tokens, config)
+            else:
+                raise NotImplementedError("Expected list or dict")
+    return outermost_dict
 
 
 def handle_series_of_children(config: Config, most_recent_key: str, possible_dict: dict[str, Any], series_of_children):
     """Handle a series of children, which may be text, images, or links."""
     for inner_token in series_of_children:
         if inner_token["type"] == "image":
             possible_dict[most_recent_key] += extract_bytes(inner_token["src"], config)
@@ -315,10 +339,9 @@
             continue
         if "text" not in inner_token:
             raise NotImplementedError("Not text like?")
         continuation_value: str = inner_token["text"]
         scalar = extract_scalar(continuation_value, config)
         # continuation of text
         possible_dict[most_recent_key] += "\n\n" + scalar
-        most_recent_key = most_recent_key
 
     return most_recent_key
```

### Comparing `markpickle-1.3.0/markpickle/mypy_types.py` & `markpickle-1.4.0/markpickle/mypy_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/python_to_tables.py` & `markpickle-1.4.0/markpickle/python_to_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/serialize.py` & `markpickle-1.4.0/markpickle/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 import datetime
 import io
 import logging
 import textwrap
 from typing import Callable, Optional, TextIO, Union
 
-import mdformat
-
 import markpickle.python_to_tables as python_to_tables
 import markpickle.simplify_types as simplify_types
 import markpickle.third_party_tables as third_party_tables
 from markpickle.binary_streams import bytes_to_markdown
 from markpickle.config_class import Config
 from markpickle.mypy_types import ScalarTypes, SerializableTypes
 
@@ -76,16 +74,17 @@
     if not config:
         config = Config()
     builder = io.StringIO()
     dump(value, builder, config=config, default=default)
 
     builder.seek(0)
     result = builder.read()
-    if config.serialize_run_formatter:
-        result = mdformat.text(result)
+    # Strips out ---, adds ##, flattens nested lists if they have the same bullet! Buggy!
+    # if config.serialize_run_formatter:
+    #     result = mdformat.text(result)
 
     # results in a copy! ugh!
     if result.endswith("\n"):
         result = result[0:-1]
     return result
 
 
@@ -246,14 +245,15 @@
                 builder.write(f"{indent * ' '}{config.list_bullet_style} {key}\n")
                 render_list(builder, item, config, indent + 1)
         elif isinstance(item, dict):
             builder.write(f"{'#' * header_level} {key}\n\n")
             if config.serialize_child_dict_as_table:
                 success = False
                 if config.serialize_tables_tabulate_style:
+                    # pylint: disable=broad-exception-caught
                     try:
                         table = third_party_tables.to_table_tablulate_style(item)
                         table = textwrap.indent(table, prefix=" " * (indent + 1))
                         builder.write(table)
                         success = True
                     except Exception:
                         success = False
@@ -267,15 +267,15 @@
         else:
             try:
                 table = third_party_tables.to_table_tablulate_style(item)
                 table = textwrap.indent(table, prefix=" " * (indent + 1))
                 builder.write(table)
             except Exception as ex:
                 logging.warning(f"Tabulate can't handle it either: {ex}")
-                raise NotImplementedError()
+                raise NotImplementedError() from ex
     return indent
 
 
 def render_list(
     builder: io.IOBase, value: list[SerializableTypes], config: Config, indent: int = 0, header_level: int = 1
 ) -> int:
     """
```

### Comparing `markpickle-1.3.0/markpickle/simplify_types.py` & `markpickle-1.4.0/markpickle/simplify_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/split_file_code.py` & `markpickle-1.4.0/markpickle/split_file_code.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/third_party_tables.py` & `markpickle-1.4.0/markpickle/third_party_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.3.0/markpickle/unicode_formatting.py` & `markpickle-1.4.0/markpickle/unicode_formatting.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,10 +19,14 @@
     # Convert underline markup
     # text = re.sub(r'--(.*?)--', r'\033[4m\g<1>\033[0m', text)
 
     return text
 
 
 if __name__ == "__main__":
-    text = "Some text in __bold__, *italic*, and --underline--"
-    converted_text = convert_markup_to_terminal(text)
-    print(converted_text)
+
+    def run() -> None:
+        text = "Some text in __bold__, *italic*, and --underline--"
+        converted_text = convert_markup_to_terminal(text)
+        print(converted_text)
+
+    run()
```

### Comparing `markpickle-1.3.0/pyproject.toml` & `markpickle-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [tool.poetry]
 name = "markpickle"
-version = "1.3.0"
+version = "1.4.0"
 description = "Lossy python to markdown serializer"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["serializer", "deserializer", "markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+
 ]
 include = [
     "markpickle/**/*.py",
     "markpickle/**/*.md",
     "markpickle/**/*.txt",
     "markpickle/**/*.html",
     "markpickle/**/*.jinja",
```

### Comparing `markpickle-1.3.0/PKG-INFO` & `markpickle-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markpickle
-Version: 1.3.0
+Version: 1.4.0
 Summary: Lossy python to markdown serializer
 Home-page: https://github.com/matthewdeanmartin/markpickle
 License: MIT
 Keywords: serializer,deserializer,markdown
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Classifier: Development Status :: 3 - Alpha
@@ -31,15 +31,15 @@
 Project-URL: Change Log, https://github.com/matthewdeanmartin/markpickle/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/matthewdeanmartin/markpickle
 Project-URL: Repository, https://github.com/matthewdeanmartin/markpickle
 Description-Content-Type: text/markdown
 
 # markpickle
 
-Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown.
+Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
 For example this
 
 ```markdown
 - 1
 - 2
 ```
@@ -129,28 +129,32 @@
 
 [pytablewriter](https://pytablewriter.readthedocs.io/en/latest/pages/reference/writers/text/markup/md.html) also, dict to table, but supports many tabular formats.
 
 ### Deserializing to Python
 
 Most libraries turn markdown into document object model. Markdown-to-json is the most similar to markpickle's goal of turning a markdown document into a python data types, in this case nested dicts.
 
-[markdown-to-json](https://github.com/njvack/markdown-to-json)
+[markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle, but is somewhat broken, unmaintained and depends on the unmaintained commonmark library.
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
-## [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
+[beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
 ## Schema Validation for Markdown
 
 In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
 
 I haven't really found anything that says, for example, "This markdown document shall have one # Header and a 3 column table and nothing else."
 
 - [schema-markdown-js](https://craigahobbs.github.io/schema-markdown-js/language/) A json schema that happens to be using markdown as its syntax.
 
+## Credits
+
+I copied the ATX-dictionary-like header parsing from [markdown-to-json](https://github.com/njvack/markdown-to-json).
+
 ## Documentation
 
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
 ## Change Log
```

