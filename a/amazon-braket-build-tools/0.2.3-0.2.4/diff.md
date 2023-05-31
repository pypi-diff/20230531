# Comparing `tmp/amazon-braket-build-tools-0.2.3.tar.gz` & `tmp/amazon-braket-build-tools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-build-tools-0.2.3.tar", last modified: Mon May 29 16:04:11 2023, max compression
+gzip compressed data, was "amazon-braket-build-tools-0.2.4.tar", last modified: Wed May 31 16:04:21 2023, max compression
```

## Comparing `amazon-braket-build-tools-0.2.3.tar` & `amazon-braket-build-tools-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.720320 amazon-braket-build-tools-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 16:04:11.000000 amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.720320 amazon-braket-build-tools-0.2.3/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/src/braket/_build_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/src/braket/_build_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:04:11.724320 amazon-braket-build-tools-0.2.3/src/braket/flake8_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-05-29 16:03:57.000000 amazon-braket-build-tools-0.2.3/src/braket/flake8_plugins/braket_checkstyle_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:04:21.432592 amazon-braket-build-tools-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-31 16:04:10.000000 amazon-braket-build-tools-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 16:04:10.000000 amazon-braket-build-tools-0.2.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 16:04:21.432592 amazon-braket-build-tools-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-31 16:04:10.000000 amazon-braket-build-tools-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 16:04:10.000000 amazon-braket-build-tools-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 16:04:21.436592 amazon-braket-build-tools-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-31 16:04:10.000000 amazon-braket-build-tools-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:04:21.432592 amazon-braket-build-tools-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:04:21.432592 amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 16:04:21.000000 amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-31 16:04:21.000000 amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:04:21.000000 amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 16:04:21.000000 amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-31 16:04:21.000000 amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 16:04:21.000000 amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:04:21.432592 amazon-braket-build-tools-0.2.4/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:04:21.432592 amazon-braket-build-tools-0.2.4/src/braket/_build_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 16:04:10.000000 amazon-braket-build-tools-0.2.4/src/braket/_build_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:04:21.432592 amazon-braket-build-tools-0.2.4/src/braket/flake8_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-05-31 16:04:10.000000 amazon-braket-build-tools-0.2.4/src/braket/flake8_plugins/braket_checkstyle_plugin.py
```

### Comparing `amazon-braket-build-tools-0.2.3/LICENSE` & `amazon-braket-build-tools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.3/PKG-INFO` & `amazon-braket-build-tools-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.3/README.md` & `amazon-braket-build-tools-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.3/setup.cfg` & `amazon-braket-build-tools-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.3/setup.py` & `amazon-braket-build-tools-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-build-tools-0.2.3/src/amazon_braket_build_tools.egg-info/PKG-INFO` & `amazon-braket-build-tools-0.2.4/src/amazon_braket_build_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-build-tools
-Version: 0.2.3
+Version: 0.2.4
 Summary: A set of build tools for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-build-tools
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `amazon-braket-build-tools-0.2.3/src/braket/_build_tools/_version.py` & `amazon-braket-build-tools-0.2.4/src/braket/_build_tools/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # language governing permissions and limitations under the License.
 
 """Version information.
 
 Version number (major.minor.patch[-label])
 """
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

### Comparing `amazon-braket-build-tools-0.2.3/src/braket/flake8_plugins/braket_checkstyle_plugin.py` & `amazon-braket-build-tools-0.2.4/src/braket/flake8_plugins/braket_checkstyle_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,27 +24,32 @@
     DESCRIPTION = "DESCRIPTION"
     ARGUMENTS = "ARGUMENTS"
     RETURN_FIRST_LINE = "RETURN_FIRST_LINE"
     RETURN_REST = "RETURN_REST"
     MISC = "MISC"
 
 
+class ArgType(str, Enum):
+    DEFAULT = "DEFAULT"
+    KEYWORD = "KEYWORD"
+
+
 @dataclass
 class DocContext:
     """
     This is the context object for parsing the function definition. We record all the information
     we need about the function and the current state of parsing.
     """
 
     found_args: bool = False
     found_return: bool = False
     found_description: bool = False
     in_sub_list: bool = False
     current_section: DocSection = DocSection.DESCRIPTION
-    current_arg: int = 0
+    previous_arg: Tuple[int, ArgType] = None
     found_arg_list: Set = None
     args_indent: int = 0
     return_indent: int = 0
     invalid_indents: int = 0
     first_invalid_indent_line: str = None
 
 
@@ -186,21 +191,23 @@
             context.current_section = DocSection.RETURN_REST
         elif context.current_section == DocSection.RETURN_REST:
             self._check_indent(context.return_indent, doc_line, context)
 
     def _check_argument_info(
         self, regex_matches: re.Match, context: DocContext, node: ast.FunctionDef
     ) -> None:
-        arg_indent, arg_name, arg_type, arg_description = regex_matches.groups()
-        arg_index = _get_argument_with_name(arg_name, node)
+        arg_indent, arg_name, arg_hint, arg_description = regex_matches.groups()
+        arg_index, arg_type = _get_argument_with_name(arg_name, node)
         self._check_argument_indent(arg_indent, arg_name, arg_index, context, node)
         if arg_index is None:
             return
-        self._check_argument_docs(arg_name, arg_type, arg_description, arg_index, context, node)
-        context.current_arg = arg_index + 1
+        self._check_argument_docs(
+            arg_name, arg_hint, arg_description, arg_index, arg_type, context, node
+        )
+        context.previous_arg = (arg_index, arg_type)
 
     def _check_argument_indent(
         self,
         arg_indent: str,
         arg_name: str,
         arg_index: int,
         context: DocContext,
@@ -211,51 +218,83 @@
                 self.add_problem(node=node, code="BCS007", arguments=arg_name)
         elif len(arg_indent) != context.args_indent + 4:
             _invalid_indent_found(arg_name, context)
 
     def _check_argument_docs(
         self,
         arg_name: str,
-        arg_type: str,
+        arg_hint: str,
         arg_description: str,
         arg_index: int,
+        arg_type: ArgType,
         context: DocContext,
         node: ast.FunctionDef,
     ) -> None:
         if context.found_arg_list is None:
-            context.found_arg_list = {arg_index}
-        elif arg_index in context.found_arg_list:
+            context.found_arg_list = {(arg_index, arg_type)}
+        elif (arg_index, arg_type) in context.found_arg_list:
             self.add_problem(node=node, code="BCS009", arguments=arg_name)
             return
         else:
-            context.found_arg_list.add(arg_index)
-        if context.current_arg == 0 and arg_index != context.current_arg:
+            context.found_arg_list.add((arg_index, arg_type))
+
+        self._check_argument_order(arg_name, arg_index, arg_type, context, node)
+
+        if arg_hint is None:
+            self.add_problem(node=node, code="BCS004", arguments=arg_name)
+        else:
+            self._check_annotation(arg_name, arg_hint, arg_index, arg_type, node)
+
+        if (arg_description is None or len(arg_description.strip()) < 2) and (
+            len(arg_name) + len(arg_hint) < 70
+        ):
+            self.add_problem(node=node, code="BCS008", arguments=arg_name)
+
+    def _check_argument_order(
+        self,
+        arg_name: str,
+        arg_index: int,
+        arg_type: ArgType,
+        context: DocContext,
+        node: ast.FunctionDef,
+    ) -> None:
+        expected_index = 0
+        if context.previous_arg is None:
             if node.args.args[0].arg in self.RESERVED_ARGS:
-                context.current_arg = 1
-        if arg_index != context.current_arg:
+                expected_index = 1
+        elif arg_type == context.previous_arg[1]:
+            expected_index = context.previous_arg[0] + 1
+        if arg_index != expected_index:
             self.add_problem(node=node, code="BCS015", arguments=arg_name)
-        if arg_type is None:
-            self.add_problem(node=node, code="BCS004", arguments=arg_name)
-        elif node.args.args[arg_index].annotation:
-            documented_type = _remove_all_spaces(arg_type[1:-1])
-            annotation_doc = _remove_all_spaces(
-                self._annotation_to_doc_str(node.args.args[arg_index].annotation)
-            )
+
+    def _check_annotation(
+        self,
+        arg_name: str,
+        arg_hint: str,
+        arg_index: int,
+        arg_type: ArgType,
+        node: ast.FunctionDef,
+    ) -> None:
+        annotation = None
+        if arg_type == ArgType.DEFAULT:
+            if node.args.args[arg_index].annotation:
+                annotation = node.args.args[arg_index].annotation
+        elif arg_type == ArgType.KEYWORD:
+            if node.args.kwonlyargs[arg_index].annotation:
+                annotation = node.args.kwonlyargs[arg_index].annotation
+        if annotation:
+            documented_type = _remove_all_spaces(arg_hint[1:-1])
+            annotation_doc = _remove_all_spaces(self._annotation_to_doc_str(annotation))
             if not _are_type_strings_same(annotation_doc, documented_type):
                 self.add_problem(
                     node=node,
                     code="BCS005",
                     arguments=(arg_name, annotation_doc, documented_type),
                 )
 
-        if (arg_description is None or len(arg_description.strip()) < 2) and (
-            len(arg_name) + len(arg_type) < 70
-        ):
-            self.add_problem(node=node, code="BCS008", arguments=arg_name)
-
     # flake8: noqa: C901
     def _annotation_to_doc_str(self, annotation) -> str:
         if isinstance(annotation, ast.Name):
             return annotation.id
         if isinstance(annotation, ast.Attribute):
             return annotation.attr
         if isinstance(annotation, ast.Subscript):
@@ -323,15 +362,21 @@
             and node.args.kwarg is None
             and node.args.vararg is None
         ):
             self.add_problem(node=node, code="BCS019", arguments=node.name)
             return
         if context.found_arg_list:
             for index, arg in enumerate(node.args.args):
-                if index not in context.found_arg_list and arg.arg not in self.RESERVED_ARGS:
+                if (
+                    index,
+                    ArgType.DEFAULT,
+                ) not in context.found_arg_list and arg.arg not in self.RESERVED_ARGS:
+                    self.add_problem(node=node, code="BCS011", arguments=arg.arg)
+            for index, arg in enumerate(node.args.kwonlyargs):
+                if (index, ArgType.KEYWORD) not in context.found_arg_list:
                     self.add_problem(node=node, code="BCS011", arguments=arg.arg)
 
     def _verify_return(self, context: DocContext, node: ast.FunctionDef) -> None:
         if context.found_return:
             if not node.returns:
                 self.add_problem(node=node, code="BCS020", arguments=node.name)
         else:
@@ -386,19 +431,24 @@
 def _get_first_doc(node: ast.FunctionDef):
     for body_node in node.body:
         if isinstance(body_node, ast.Expr) and isinstance(body_node.value, ast.Str):
             return body_node.value
     return None
 
 
-def _get_argument_with_name(arg_name: str, node: ast.FunctionDef) -> Optional[int]:
+def _get_argument_with_name(
+    arg_name: str, node: ast.FunctionDef
+) -> Tuple[Optional[int], Optional[ArgType]]:
     for index, arg in enumerate(node.args.args):
         if arg_name == arg.arg:
-            return index
-    return None
+            return index, ArgType.DEFAULT
+    for index, arg in enumerate(node.args.kwonlyargs):
+        if arg_name == arg.arg:
+            return index, ArgType.KEYWORD
+    return None, None
 
 
 def _function_requires_documentation(node: ast.FunctionDef) -> bool:
     if node.name.startswith("_"):
         return False
     if node.body is None or len(node.body) == 0:
         return False
```

