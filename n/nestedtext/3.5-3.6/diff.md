# Comparing `tmp/nestedtext-3.5.tar.gz` & `tmp/nestedtext-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestedtext-3.5.tar", last modified: Fri Nov  4 16:34:59 2022, max compression
+gzip compressed data, was "nestedtext-3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nestedtext-3.5.tar` & `nestedtext-3.6.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1092 2020-09-26 21:45:10.833811 nestedtext-3.5/LICENSE
--rw-r--r--   0        0        0     3871 2022-11-04 16:26:00.929920 nestedtext-3.5/README.rst
--rw-r--r--   0        0        0      212 2022-11-04 16:26:00.928920 nestedtext-3.5/nestedtext/__init__.py
--rw-r--r--   0        0        0    77542 2022-11-04 15:57:07.194800 nestedtext-3.5/nestedtext/nestedtext.py
--rw-r--r--   0        0        0     1051 2022-11-04 16:26:00.927920 nestedtext-3.5/pyproject.toml
--rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 nestedtext-3.5/PKG-INFO
+-rw-r--r--   0        0        0     5573 2023-05-31 03:28:22.230022 nestedtext-3.6/README.rst
+-rw-r--r--   0        0        0      212 2023-05-31 03:28:22.229022 nestedtext-3.6/nestedtext/__init__.py
+-rw-r--r--   0        0        0      454 2022-12-12 20:16:48.827895 nestedtext-3.6/nestedtext/__init__.pyi
+-rw-r--r--   0        0        0    82755 2023-05-23 23:28:50.403675 nestedtext-3.6/nestedtext/nestedtext.py
+-rw-r--r--   0        0        0     2528 2022-12-13 07:26:30.385323 nestedtext-3.6/nestedtext/nestedtext.pyi
+-rw-r--r--   0        0        0        0 2022-12-12 18:21:38.584487 nestedtext-3.6/nestedtext/py.typed
+-rw-r--r--   0        0        0     1027 2023-05-31 03:28:22.228022 nestedtext-3.6/pyproject.toml
+-rw-r--r--   0        0        0     6510 1970-01-01 00:00:00.000000 nestedtext-3.6/PKG-INFO
```

### Comparing `nestedtext-3.5/nestedtext/nestedtext.py` & `nestedtext-3.6/nestedtext/nestedtext.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 scalar text (strings).
 
 It is easily created, modified, or viewed with a text editor and easily
 understood and used by both programmers and non-programmers.
 """
 
 # MIT License {{{1
-# Copyright (c) 2020-22 Ken and Kale Kundert
+# Copyright (c) 2020-2023 Ken and Kale Kundert
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -57,15 +57,15 @@
     # but the resulting NestedText files are not compliant with the spec.
     # Use of this feature is highly discouraged.
 
 
 # Utility functions {{{1
 # convert_returns {{{2
 def convert_returns(text):
-    return text.replace('\r\n', '\n').replace('\r', '\n')
+    return text.replace("\r\n", "\n").replace("\r", "\n")
 
 
 # Unspecified {{{2
 # class that is used as a default in functions to signal nothing was given
 class _Unspecified:
     def __bool__(self):  # pragma: no cover
         return False
@@ -147,15 +147,15 @@
         ...     print(nt.loads(content))
         ... except nt.NestedTextError as e:
         ...     print(str(e))
         2: duplicate key: name1.
 
     You can also use the *report* method to print the message directly. This is
     appropriate if you are using *inform* for your messaging as it follows
-    *inform*'s conventions::
+    *inform*’s conventions::
 
         >> try:
         ..     print(nt.loads(content))
         .. except nt.NestedTextError as e:
         ..     e.report()
         error: 2: duplicate key: name1.
             ❬name1: value2❭
@@ -206,16 +206,16 @@
 
     .. code-block:: python
 
         >>> try:
         ...     print(nt.loads(content))
         ... except nt.NestedTextError as e:
         ...     template = None
-        ...     if e.template == 'duplicate key: {}.':
-        ...         template = 'llave duplicada: {}.'
+        ...     if e.template == "duplicate key: {}.":
+        ...         template = "llave duplicada: {}."
         ...     print(e.render(template=template))
         2: llave duplicada: name1.
 
     '''
 
 
 # NotSuitableForInline {{{2
@@ -240,65 +240,65 @@
 
 # report {{{2
 def report(message, line, *args, colno=None, **kwargs):
     message = full_stop(message)
     culprits = get_culprit()
     codicil = [kwargs.get("codicil", "")]
     if culprits:
-        kwargs['source'] = culprits[0]
+        kwargs["source"] = culprits[0]
     if line:
         # line numbers are always 0 based unless included in a message to user
         include_prev_line = not (
-            line.prev_line is None or kwargs.pop('suppress_prev_line', False)
+            line.prev_line is None or kwargs.pop("suppress_prev_line", False)
         )
         if colno is not None:
             # build codicil that shows both the line and the preceding line
             if include_prev_line:
-                codicil += [f'{line.prev_line.lineno+1:>4} ❬{line.prev_line.text}❭']
+                codicil += [f"{line.prev_line.lineno+1:>4} ❬{line.prev_line.text}❭"]
             else:
                 codicil += []
             # replace tabs with → so that arrow points to right location.
             text = line.text.replace("\t", "→")
             codicil += [
-                f'{line.lineno+1:>4} ❬{text}❭',
-                '      ' + (colno*' ') + '▲',
+                f"{line.lineno+1:>4} ❬{text}❭",
+                "      " + (colno*" ") + "▲",
             ]
-            kwargs['codicil'] = '\n'.join(cull(codicil))
-            kwargs['colno'] = colno
+            kwargs["codicil"] = "\n".join(cull(codicil))
+            kwargs["colno"] = colno
         else:
-            kwargs['codicil'] = f'{line.lineno+1:>4} ❬{line.text}❭'
-        kwargs['culprit'] = get_culprit(line.lineno+1)
-        kwargs['line'] = line.text
-        kwargs['lineno'] = line.lineno
+            kwargs["codicil"] = f"{line.lineno+1:>4} ❬{line.text}❭"
+        kwargs["culprit"] = get_culprit(line.lineno + 1)
+        kwargs["line"] = line.text
+        kwargs["lineno"] = line.lineno
         if include_prev_line:
-            kwargs['prev_line'] = line.prev_line.text
+            kwargs["prev_line"] = line.prev_line.text
     else:
-        kwargs['culprit'] = culprits  # pragma: no cover
+        kwargs["culprit"] = culprits  # pragma: no cover
     raise NestedTextError(template=message, *args, **kwargs)
 
 
 # unrecognized_line {{{2
 def unrecognized_line(line):
     # line will not be recognized if there is invalid white space in indentation
-    first_non_space = line.text.lstrip(' ')[0]
+    first_non_space = line.text.lstrip(" ")[0]
     index_of_first_non_space = line.text.index(first_non_space)
-    if first_non_space.strip() == '':
+    if first_non_space.strip() == "":
         # first non-space is a white space character
         # treat it as invalid indentation
         desc = unicodedata.name(first_non_space, "")
         if desc:
-            desc = f' ({desc})'
+            desc = f" ({desc})"
         report(
-            f'invalid character in indentation: {first_non_space!r}{desc}.',
+            f"invalid character in indentation: {first_non_space!r}{desc}.",
             line,
             colno = index_of_first_non_space,
-            codicil = 'Only simple spaces are allowed in indentation.'
+            codicil = "Only simple spaces are allowed in indentation."
         )
     else:
-        report('unrecognized line.', line, colno=index_of_first_non_space)
+        report("unrecognized line.", line, colno=index_of_first_non_space)
 
 
 # Lines class {{{2
 class Lines:
     # constructor {{{3
     def __init__(self, lines):
         self.lines = lines
@@ -308,83 +308,83 @@
             self.next_line = next(self.generator, None)
             if self.next_line and self.next_line.kind not in ["blank", "comment"]:
                 return
 
     # Line class {{{3
     class Line(Info):
         def render(self, col=None):
-            result = [f'{self.lineno+1:>4} ❬{self.text}❭']
+            result = [f"{self.lineno+1:>4} ❬{self.text}❭"]
             if col is not None:
-                result += ['      ' + (col*' ') + '▲']
-            return '\n'.join(result)
+                result += ["      " + (col*" ") + "▲"]
+            return "\n".join(result)
 
         def __str__(self):
             return self.text
 
         def __repr__(self):
             return self.__class__.__name__ + f"({self.lineno+1}: ❬{self.text}❭)"
 
     # read_lines() {{{3
     def read_lines(self):
         prev_line = None
         last_line = None
         for lineno, line in enumerate(self.lines):
             key = None
             value = None
-            line = line.rstrip('\n')
+            line = line.rstrip("\n")
 
             # compute indentation
-            stripped = line.lstrip(' ')
+            stripped = line.lstrip(" ")
             depth = len(line) - len(stripped)
 
             # determine line type and extract values
             if stripped == "":
                 kind = "blank"
                 value = None
                 depth = None
             elif stripped[:1] == "#":
                 kind = "comment"
                 value = line[1:].strip()
                 depth = None
-            elif stripped == '-' or stripped.startswith('- '):
+            elif stripped == "-" or stripped.startswith("- "):
                 kind = "list item"
                 value = stripped[2:]
-            elif stripped == '>' or stripped.startswith('> '):
+            elif stripped == ">" or stripped.startswith("> "):
                 kind = "string item"
                 value = line[depth+2:]
-            elif stripped == ':' or stripped.startswith(': '):
+            elif stripped == ":" or stripped.startswith(": "):
                 kind = "key item"
                 value = line[depth+2:]
-            elif stripped[0:1] in ['[', '{'] and support_inlines:
+            elif stripped[0:1] in ["[", "{"] and support_inlines:
                 tag = stripped[0:1]
-                kind = 'inline dict' if tag == '{' else 'inline list'
+                kind = "inline dict" if tag == "{" else "inline list"
                 value = line[depth:]
             else:
                 matches = dict_item_recognizer.fullmatch(stripped)
                 if matches:
                     kind = "dict item"
-                    key = matches.group('key')
-                    value = matches.group('value')
+                    key = matches.group("key")
+                    value = matches.group("value")
                     if value is None:
-                        value = ''
+                        value = ""
                 else:
                     kind = "unrecognized"
                     value = line
 
             # bundle information about line
             this_line = self.Line(
                 text = line,
                 lineno = lineno,
                 kind = kind,
                 depth = depth,
                 key = key,
                 value = value,
                 prev_line = prev_line,
             )
-            if kind.endswith(' item') or kind.startswith('inline '):
+            if kind.endswith(" item") or kind.startswith("inline "):
                 # Create prev_line, which differs from last_line in that it
                 # is a copy of the line without a prev_line attribute of its
                 # own. This avoids keeping a chain of all previous lines. In
                 # contrast, last line is the actual this_line from the previous
                 # iteration.  Also, it is a data line, not a comment or blank.
                 prev_line = self.Line(
                     text = this_line.text,
@@ -393,18 +393,18 @@
                     depth = this_line.depth,
                     lineno = this_line.lineno,
                 )
 
                 # add this line as next_line in prev_line if this is a continued
                 # multiline string.
                 if (
-                    last_line and
-                    depth == last_line.depth and
-                    kind == last_line.kind and
-                    kind in ['key item', 'string item']
+                    last_line                 and
+                    depth == last_line.depth  and
+                    kind == last_line.kind    and
+                    kind in ["key item", "string item"]
                 ):
                     last_line.next_line = this_line
 
             last_line = this_line
             yield this_line
 
     # type_of_next() {{{3e
@@ -455,38 +455,35 @@
 
     # indentation_error {{{3
     def indentation_error(self, line, depth):
         assert line.depth != depth
         prev_line = line.prev_line
         codicil = None
         if not line.prev_line and depth == 0:
-            msg = 'top-level content must start in column 1.'
+            msg = "top-level content must start in column 1."
         elif (
-            prev_line and
-            prev_line.value and
-            prev_line.depth < line.depth and
-            prev_line.kind in ['list item', 'dict item']
+            prev_line                     and
+            prev_line.value               and
+            prev_line.depth < line.depth  and
+            prev_line.kind in ["list item", "dict item"]
         ):
-            if prev_line.value.strip() == '':
-                obs = ', which in this case consists only of whitespace'
+            if prev_line.value.strip() == "":
+                obs = ", which in this case consists only of whitespace"
             else:
-                obs = ''
-            msg = 'invalid indentation.'
+                obs = ""
+            msg = "invalid indentation."
             codicil = join(
                 "An indent may only follow a dictionary or list item that does",
                 f"not already have a value{obs}.",
                 wrap = True
             )
-        elif (
-            prev_line and
-            prev_line.depth > line.depth
-        ):
-            msg = 'invalid indentation, partial dedent.'
+        elif prev_line and prev_line.depth > line.depth:
+            msg = "invalid indentation, partial dedent."
         else:
-            msg = 'invalid indentation.'
+            msg = "invalid indentation."
         report(join(msg, wrap=True), line, colno=depth, codicil=codicil)
 
 
 # KeyPolicy class {{{2
 # Used to hold and implement the on_dup policy for dictionaries.
 class KeyPolicy:
     @classmethod
@@ -494,46 +491,47 @@
         if callable(on_dup):
             # if on_dup is a function, convert it to a data structure that will
             # hold state during the load
             on_dup = {_OnDupCallback: on_dup}
         cls.on_dup = on_dup
 
     @classmethod
-    def add_to_dictionary(cls, dictionary, key, value, keys, line=None, colno=None):
-        if key in dictionary:
-            # found duplicate key
-            if cls.on_dup is None or cls.on_dup == 'error':
-                report('duplicate key: {}.', line, key, colno=colno)
-            if cls.on_dup == 'ignore':
-                return
-            if isinstance(cls.on_dup, dict):
-                dup_handler = cls.on_dup.pop(_OnDupCallback)
-                cls.on_dup.update(
-                    dict(value=value, dictionary=dictionary, keys=keys)
-                )
-                try:
-                    key = dup_handler(key=key, state=cls.on_dup)
-                    if key is None:
-                        return
-                except KeyError:
-                    report('duplicate key: {}.', line, key, colno=colno)
-                cls.on_dup[_OnDupCallback] = dup_handler  # restore dup_handler
-            elif cls.on_dup != 'replace':
-                raise NotImplementedError(f'{cls.on_dup}: unknown value for on_dup.')
-        dictionary[key] = value
+    def process_duplicate(cls, dictionary, key, keys, line=None, colno=None):
+        if cls.on_dup is None or cls.on_dup == "error":
+            report("duplicate key: {}.", line, key, colno=colno)
+        if cls.on_dup == "ignore":
+            return None
+        if isinstance(cls.on_dup, dict):
+            dup_handler = cls.on_dup.pop(_OnDupCallback)
+            cls.on_dup.update(
+                dict(dictionary=dictionary, keys=keys)
+            )
+            try:
+                key = dup_handler(key=key, state=cls.on_dup)
+                if key is None:
+                    return None
+            except KeyError:
+                report("duplicate key: {}.", line, key, colno=colno)
+            cls.on_dup[_OnDupCallback] = dup_handler  # restore dup_handler
+        elif cls.on_dup != "replace":  # pragma: no cover
+            raise AssertionError(
+                f"{cls.on_dup}: unexpected value for on_dup."
+            ) from None
+        return key
 
 
 # Location class {{{2
 class Location:
     """Holds information about the location of a token.
 
     Returned from :func:`load` and :func:`loads` as the values in a *keymap*.
     Objects of this class holds the line and column numbers of the key and value
     tokens.
     """
+
     def __init__(self, line=None, col=None, key_line=None, key_col=None):
         self.line = line
         self.key_line = key_line
         self.col = col
         self.key_col = key_col
 
     def __repr__(self):
@@ -547,62 +545,80 @@
         key_col = self.key_col
         if key_col is None:
             key_col = self.col
         components.append(f"key_colno={key_col}")
         return f"{self.__class__.__name__}({', '.join(components)})"
 
     # as_tuple() {{{3
-    def as_tuple(self, kind='value'):
+    def as_tuple(self, kind="value"):
         """
         Returns the location of either the value or the key token as a tuple
         that contains the line number and the column number.  The line and
         column numbers are 0 based.
 
         Args:
             kind (str):
                 Specify either “key” or “value” depending on which token is
                 desired.
         """
-        if kind == 'key':
+        if kind == "key":
             line = self.key_line
             col = self.key_col
             if line is None:
                 line = self.line
             if col is None:
                 col = self.col
         else:
             line = self.line
             col = self.col
         return line.lineno, col
 
     # as_line() {{{3
-    def as_line(self, kind='value'):
+    def as_line(self, kind="value"):
         """
         Returns a string containing two lines that identify the token in
         context.  The first line contains the line number and text of the line
         that contains the token.  The second line contains a pointer to the
         token.
 
         Args:
             kind (str):
                 Specify either “key” or “value” depending on which token is
                 desired.
         """
-        if kind == 'key':
+        if kind == "key":
             line = self.key_line
             col = self.key_col
             if line is None:
                 line = self.line
             if col is None:
                 col = self.col
         else:
             line = self.line
             col = self.col
         return line.render(col)
 
+    # _get_original_key() {{{3
+    def _get_original_key(self, key, strict):
+        try:
+            line = self.key_line
+            if line.kind == "key item":
+                # is multiline key (key fragment is actually held in line.text)
+                key_frags = [line.text[line.depth+2:]]
+                while line.next_line:
+                    line = line.next_line
+                    key_frags.append(line.text[line.depth+2:])
+                key = "\n".join(key_frags)
+            else:
+                if line.kind != "list item":
+                    key = line.key
+            return key
+        except AttributeError:
+            # this occurs for list indexes
+            return key
 
 # Inline class {{{2
 class Inline:
     # a recursive descent parser to interpret inline lists and dictionaries
 
     # constructor() {{{3
     def __init__(self, line, keys, loader):
@@ -610,122 +626,123 @@
         self.loader = loader
         self.text = line.value
         self.max_index = len(self.text)
         self.starting_col = line.depth
         try:
             self.values, self.keymap, index = self.parse_inline_value(keys, 0)
         except IndexError:
-            self.inline_error(
-                "line ended without closing delimiter", self.max_index
-            )
+            self.inline_error("line ended without closing delimiter", self.max_index)
         if index < self.max_index:
             extra = self.text[index:]
             self.inline_error(
                 f"extra {plural(extra):character} after closing delimiter: ‘{{}}’.",
                 index, extra
             )
         assert index == self.max_index
 
     # parse_inline_value() {{{3
     def parse_inline_value(self, keys, index, forbidden_chars=None):
-        if self.text[index] == '{':
+        if self.text[index] == "{":
             return self.parse_inline_dict(keys, index)
-        elif self.text[index] == '[':
+        elif self.text[index] == "[":
             return self.parse_inline_list(keys, index)
         else:
             return self.parse_inline_str(keys, index, forbidden_chars)
 
     # parse_inline_dict() {{{3
     def parse_inline_dict(self, keys, index):
         starting_index = index
-        assert self.text[index] == '{'
+        assert self.text[index] == "{"
         index += 1
         values = {}
         need_another = False
 
-        while self.text[index] != '}':
+        while self.text[index] != "}":
             prev_index = index
             orig_key, value, location, index = self.parse_inline_dict_item(keys, index)
             key = self.loader.normalize_key(orig_key, keys)
-            KeyPolicy.add_to_dictionary(values, key, value, keys, self.line, prev_index)
-            self.loader._add_keymap(keys + (key,), location)
+            if key in values:
+                key = KeyPolicy.process_duplicate(values, key, keys, self.line, prev_index)
+            if key is not None:
+                values[key] = value
+                self.loader._add_keymap(keys + (key,), location)
             need_another = False
-            if self.text[index] not in ',}':
+            if self.text[index] not in ",}":
                 self.inline_error(
                     "expected ‘,’ or ‘}}’, found ‘{}’", index, self.text[index]
                 )
-            if self.text[index] == ',':
+            if self.text[index] == ",":
                 index += 1
                 need_another = True
         if need_another:
             self.inline_error("expected value", index)
         return (
             values,
             self.location(starting_index),
             self.adjust_index(index+1)
         )
 
     # parse_inline_dict_item() {{{3
     def parse_inline_dict_item(self, keys, index):
-        forbidden_chars = '{}[],:'
+        forbidden_chars = "{}[],:"
         key_index = self.adjust_index(index)
         if self.text[index] in forbidden_chars:
-            key = ''
+            key = ""
         else:
             key, _, index = self.parse_inline_value(keys, index, forbidden_chars)
-        if self.text[index] != ':':
+        if self.text[index] != ":":
             self.inline_error(
                 "expected ‘:’, found ‘{}’", index, self.text[index], culprit=key
             )
         index = self.adjust_index(index+1)
-        if self.text[index] in ',}':
-            value = ''
+        if self.text[index] in ",}":
+            value = ""
             loc = self.location(index)
         else:
             value, loc, index = self.parse_inline_value(keys, index, forbidden_chars)
         self.add_key_location(loc, key_index)
         return key, value, loc, index
 
     # parse_inline_list() {{{3
     def parse_inline_list(self, keys, index):
-        forbidden_chars = '{}[],'
+        forbidden_chars = "{}[],"
         starting_index = index
-        assert self.text[index] == '['
+        assert self.text[index] == "["
         index += 1
 
         # handle empty list
-        if self.text[index] == ']':
+        if self.text[index] == "]":
             return [], self.location(starting_index), self.adjust_index(index+1)
 
         key = 0
         values = []
-        value = ''
+        value = ""
         loc = self.location(index)
         while True:
             new_keys = keys + (key,)
             c = self.text[index]
-            if c in ',]':
+            if c in ",]":
                 values.append(value)
                 self.loader._add_keymap(new_keys, loc)
                 key += 1
-                if c == ']':
+                if c == "]":
                     return (
                         values,
                         self.location(starting_index),
                         self.adjust_index(index+1)
                     )
                 index += 1
                 loc = self.location(index)
                 index = self.adjust_index(index)
-                value = ''
+                value = ""
             elif value:
                 self.inline_error(
                     "expected ‘,’ or ‘]’, found ‘{}’", index, self.text[index]
                 )
-            elif c in '}],':
+            elif c in "}],":
                 self.inline_error("expected value", index)
             else:
                 value, loc, index = self.parse_inline_value(
                     new_keys, index, forbidden_chars
                 )
 
     # parse_inline_str() {{{3
@@ -734,22 +751,22 @@
         while self.text[index] not in forbidden_chars:
             index = self.adjust_index(index+1)
         value = self.text[starting_index:index].strip()
         return value, self.location(starting_index), index
 
     # adjust_index() {{{3
     def adjust_index(self, index):
-        # if desired index points to white space, shift right until it doesn't
-        while index < self.max_index and self.text[index] in ' \t':
+        # if desired index points to white space, shift right until it doesn’t
+        while index < self.max_index and self.text[index] in " \t":
             index += 1
         return index
 
     # location() {{{3
     def location(self, index, **kwargs):
-        kwargs['line'] = self.line
+        kwargs["line"] = self.line
         return Location(col=index + self.starting_col, **kwargs)
 
     # add_key_location() {{{3
     def add_key_location(self, loc, key_index):
         loc.key_col = key_index + self.starting_col
 
     # inline_error {{{3
@@ -780,53 +797,63 @@
 
 # NestedTextLoader class {{{2
 class NestedTextLoader:
     # __init__() {{{3
     def __init__(self, lines, top, source, on_dup, keymap, normalize_key):
         KeyPolicy.set_policy(on_dup)
         self.source = source
-        self.keymap = {} if keymap is True else keymap
+        self.keymap = keymap
+        assert self.keymap is None or is_mapping(self.keymap)
         self.normalize_key = normalize_key if normalize_key else lambda k, ks: k
 
         with set_culprit(source):
             lines = self.lines = Lines(lines)
             next_is = lines.type_of_next()
 
-            if top in ['any', any]:
+            if top in ["any", any]:
                 if next_is is None:
                     self.values, self.keymap = None, None
                 else:
                     self.values, self.keymap = self._read_value(0, ())
                 return
 
-            if top in ['dict', dict]:
+            if top in ["dict", dict]:
                 if next_is in ["dict item", "key item", "inline dict"]:
                     self.values, self.keymap = self._read_value(0, ())
                 elif next_is is None:
                     self.values, self.keymap = {}, None
                 else:
-                    report('content must start with key or brace ({{).', lines.get_next())
+                    report(
+                        "content must start with key or brace ({{).",
+                        lines.get_next()
+                    )
                 return
 
-            if top in ['list', list]:
+            if top in ["list", list]:
                 if next_is in ["list item", "inline list"]:
                     self.values, self.keymap = self._read_value(0, ())
                 elif next_is is None:
                     self.values, self.keymap = [], None
                 else:
-                    report('content must start with dash (-) or bracket ([).', lines.get_next())
+                    report(
+                        "content must start with dash (-) or bracket ([).",
+                        lines.get_next(),
+                    )
                 return
 
-            if top in ['str', str]:
+            if top in ["str", str]:
                 if next_is == "string item":
                     self.values, self.keymap = self._read_value(0, ())
                 elif next_is is None:
                     self.values, self.keymap = "", None
                 else:
-                    report('content must start with greater-than sign (>).', lines.get_next())
+                    report(
+                        "content must start with greater-than sign (>).",
+                        lines.get_next(),
+                    )
                 return
 
             raise NotImplementedError(top)
 
     # get_decoded() {{{3
     def get_decoded(self):
         return self.values
@@ -901,59 +928,75 @@
                 # case it must be indented.
                 depth_of_next = lines.depth_of_next()
                 if depth_of_next > depth:
                     value, loc = self._read_value(depth_of_next, new_keys)
                     loc.key_line = line
                     loc.key_col = depth
                 else:
-                    value = ''
+                    value = ""
                     loc = Location(line=line, key_col=depth, col=depth + 1)
                 values.append(value)
                 self._add_keymap(new_keys, loc)
             index += 1
 
         return values, Location(line=first_line, col=first_line.depth)
 
     # _read_dict() {{{3
     def _read_dict(self, depth, keys):
         lines = self.lines
         values = {}
         first_line = lines.next_line
+
+        # process all items in dictionary
         while lines.still_within_level(depth):
             line = lines.get_next()
+            key_line = line
+            key_col = depth
+
+            # error checking
             if line.depth != depth:
                 lines.indentation_error(line, depth)
             if line.kind not in ["dict item", "key item"]:
                 report("expected dictionary item.", line, colno=depth)
-            key_line = line
-            key_col = depth
+
+            # process key
             if line.kind == "key item":
                 # multiline key
                 original_key = self._read_key(line, depth)
                 value = None
             else:
                 # key and value on a single line
                 original_key = line.key
                 value = line.value
             key = self.normalize_key(original_key, keys)
-
+            if key in values:
+                # found duplicate key
+                key = KeyPolicy.process_duplicate(values, key, keys, line, depth)
+                if key is None:
+                    continue
             new_keys = keys + (key,)
+
+            # process value
             if value:
-                loc = Location(line=line, col=depth+len(key)+2)
+                # this is a single-line item, value was found above
+                loc = Location(line=line, col=depth + len(key) + 2)
             else:
+                # value is on subsequent lines
                 depth_of_next = lines.depth_of_next()
                 if depth_of_next > depth:
+                    # read indented values
                     value, loc = self._read_value(depth_of_next, new_keys)
                 elif line.kind == "dict item":
-                    value = ''
-                    loc = Location(line=line, col=depth+len(key)+1)
+                    # found the next key in this dictionary, so value is empty
+                    value = ""
+                    loc = Location(line=line, col=depth + len(key) + 1)
                 else:
-                    report('multiline key requires a value.', line, None, colno=depth)
+                    report("multiline key requires a value.", line, None, colno=depth)
 
-            KeyPolicy.add_to_dictionary(values, key, value, keys, line, depth)
+            values[key] = value
             loc.key_line = key_line
             loc.key_col = key_col
             self._add_keymap(new_keys, loc)
         return values, Location(line=first_line, col=first_line.depth)
 
     # _read_key() {{{3
     def _read_key(self, line, depth):
@@ -983,16 +1026,15 @@
         lines = self.lines
         line = lines.get_next()
         return Inline(line, keys, self).get_values()
 
 
 # loads {{{2
 def loads(
-    content, top="dict", *,
-    source=None, on_dup=None, keymap=None, normalize_key=None
+    content, top="dict", *, source=None, on_dup=None, keymap=None, normalize_key=None
 ):
     # description {{{3
     r'''
     Loads *NestedText* from string.
 
     Args:
         content (str):
@@ -1025,16 +1067,14 @@
 
             key:
                 The new key (duplicates an existing key).
 
             state:
                 A dictionary containing other possibly helpful information:
 
-                value:
-                    The value associated with the duplicate key.
                 dictionary:
                     The entire dictionary as it is at the moment the duplicate
                     key is found.  You should not change it.
                 keys:
                     The keys that identify the dictionary.
 
                 This dictionary is created as *loads* is called and deleted as
@@ -1042,19 +1082,17 @@
                 on subsequent calls to this function during the load operation.
 
             This function should return a new key.  If the key duplicates an
             existing key, the value associated with that key is replaced.  If
             *None* is returned, this key is ignored.  If a *KeyError* is
             raised, the duplicate key is reported as an error.
 
-            Be aware that de-duplication does not play nicely with keymaps when
-            used to access values using the original keys as it is not possible
-            to use the original keys to distinguish between the duplicate
-            key-sets.  If an error occurs in the value of one of the duplicates,
-            it may be reported as occurring in one of the others.
+            Be aware that key de-duplication occurs after key normalization.  As
+            such you should generate keys during de-duplication that are
+            consistent with your normalization scheme.
 
         keymap (dict):
             Specify an empty dictionary or nothing at all for the value of
             this argument.  If you give an empty dictionary it will be filled
             with location information for the values that are returned.  Upon
             return the dictionary maps a tuple containing the keys for the value
             of interest to the location of that value in the *NestedText* source
@@ -1086,48 +1124,48 @@
 
         .. code-block:: python
 
             >>> import nestedtext as nt
 
             >>> contents = """
             ... name: Kristel Templeton
-            ... sex: female
+            ... gender: female
             ... age: 74
             ... """
 
             >>> try:
             ...     data = nt.loads(contents, "dict")
             ... except nt.NestedTextError as e:
             ...     e.terminate()
 
             >>> print(data)
-            {'name': 'Kristel Templeton', 'sex': 'female', 'age': '74'}
+            {'name': 'Kristel Templeton', 'gender': 'female', 'age': '74'}
 
         *loads()* takes an optional argument, *source*. If specified, it is
         added to any error messages. It is often used to designate the source
         of *NestedText* document. For example, if *contents* were read from a
         file, *source* would be the file name.  Here is a typical example of
         reading *NestedText* from a file:
 
         .. code-block:: python
 
-            >>> filename = 'examples/duplicate-keys.nt'
+            >>> filename = "examples/duplicate-keys.nt"
             >>> try:
-            ...     with open(filename, encoding='utf-8') as f:
+            ...     with open(filename, encoding="utf-8") as f:
             ...         addresses = nt.loads(f.read(), source=filename)
             ... except nt.NestedTextError as e:
             ...     print(e.render())
             ...     print(*e.get_codicil(), sep="\n")
             examples/duplicate-keys.nt, 5: duplicate key: name.
                4 ❬name:❭
                5 ❬name:❭
                   ▲
 
         Notice in the above example the encoding is explicitly specified as
-        'utf-8'.  *NestedText* files should always be read and written using
+        "utf-8".  *NestedText* files should always be read and written using
         *utf-8* encoding.
 
         The following examples demonstrate the various ways of handling
         duplicate keys:
 
         .. code-block:: python
 
@@ -1140,57 +1178,58 @@
             ... """
 
             >>> print(nt.loads(content))
             Traceback (most recent call last):
             ...
             nestedtext.nestedtext.NestedTextError: 3: duplicate key: key.
 
-            >>> print(nt.loads(content, on_dup='ignore'))
+            >>> print(nt.loads(content, on_dup="ignore"))
             {'key': 'value 1', 'name': 'value 4'}
 
-            >>> print(nt.loads(content, on_dup='replace'))
+            >>> print(nt.loads(content, on_dup="replace"))
             {'key': 'value 3', 'name': 'value 5'}
 
             >>> def de_dup(key, state):
             ...     if key not in state:
             ...         state[key] = 1
             ...     state[key] += 1
             ...     return f"{key} — #{state[key]}"
 
             >>> print(nt.loads(content, on_dup=de_dup))
             {'key': 'value 1', 'key — #2': 'value 2', 'key — #3': 'value 3', 'name': 'value 4', 'name — #2': 'value 5'}
 
     '''
 
     # code {{{3
-    lines = convert_returns(content).split('\n')
+    lines = convert_returns(content).split("\n")
     loader = NestedTextLoader(lines, top, source, on_dup, keymap, normalize_key)
     return loader.get_decoded()
 
 
 # load {{{2
 def load(f, top="dict", *, on_dup=None, keymap=None, normalize_key=None):
     # description {{{3
-    r'''
+    r"""
     Loads *NestedText* from file or stream.
 
     Is the same as :func:`loads` except the *NextedText* is accessed by reading
     a file rather than directly from a string. It does not keep the full
     contents of the file in memory and so is more memory efficient with large
     files.
 
     Args:
         f (str, os.PathLike, io.TextIOBase, collections.abc.Iterator):
             The file to read the *NestedText* content from.  This can be
             specified either as a path (e.g. a string or a `pathlib.Path`),
-            as a text IO object (e.g. an open file), or as an iterator.  If a
-            path is given, the file will be opened, read, and closed.  If an IO
-            object is given, it will be read and not closed; utf-8 encoding
-            should be used..  If an iterator is given, it should generate full
-            lines in the same manner that iterating on a file descriptor would.
+            as a text IO object (e.g. an open file, or 0 for stdin), or as an
+            iterator.  If a path is given, the file will be opened, read, and
+            closed.  If an IO object is given, it will be read and not closed;
+            utf-8 encoding should be used..  If an iterator is given, it should
+            generate full lines in the same manner that iterating on a file
+            descriptor would.
         kwargs:
             See :func:`loads` for optional arguments.
 
     Returns:
         The extracted data.
         See :func:`loads` description of the return value.
 
@@ -1201,371 +1240,414 @@
     Examples:
 
         Load from a path specified as a string:
 
         .. code-block:: python
 
             >>> import nestedtext as nt
-            >>> print(open('examples/groceries.nt').read())
+            >>> print(open("examples/groceries.nt").read())
             groceries:
               - Bread
               - Peanut butter
               - Jam
             <BLANKLINE>
 
-            >>> nt.load('examples/groceries.nt')
+            >>> nt.load("examples/groceries.nt")
             {'groceries': ['Bread', 'Peanut butter', 'Jam']}
 
         Load from a `pathlib.Path`:
 
         .. code-block:: python
 
             >>> from pathlib import Path
-            >>> nt.load(Path('examples/groceries.nt'))
+            >>> nt.load(Path("examples/groceries.nt"))
             {'groceries': ['Bread', 'Peanut butter', 'Jam']}
 
         Load from an open file object:
 
         .. code-block:: python
 
-            >>> with open('examples/groceries.nt') as f:
+            >>> with open("examples/groceries.nt") as f:
             ...     nt.load(f)
             ...
             {'groceries': ['Bread', 'Peanut butter', 'Jam']}
 
-    '''
+    """
 
     # code {{{3
     # Do not invoke the read method as that would read in the entire contents of
     # the file, possibly consuming a lot of memory. Instead pass the file
     # pointer into _read_all(), it will iterate through the lines, discarding
     # them once they are no longer needed, which reduces the memory usage.
 
     if isinstance(f, collections.abc.Iterator):
-        source = getattr(f, 'name', None)
+        source = getattr(f, "name", None)
         loader = NestedTextLoader(f, top, source, on_dup, keymap, normalize_key)
         return loader.get_decoded()
     else:
         source = str(f)
-        with open(f, encoding='utf-8') as fp:
+        with open(f, encoding="utf-8") as fp:
             loader = NestedTextLoader(fp, top, source, on_dup, keymap, normalize_key)
             return loader.get_decoded()
 
 
 # NestedText Writer {{{1
 # Converts Python data hierarchies to NestedText.
 
 # add_leader {{{2
 def add_leader(s, leader):
     # split into separate lines
     # add leader to each non-blank line
     # add right-stripped leader to each blank line
     # rejoin and return
-    return '\n'.join(
+    return "\n".join(
         leader + line if line else leader.rstrip()
-        for line in s.split('\n')
+        for line in s.split("\n")
     )
 
 
 # add_prefix {{{2
 def add_prefix(prefix, suffix):
     # A simple formatting of dict and list items will result in a space
     # after the colon or dash if the value is placed on next line.
     # This, function simply eliminates that space.
     if not suffix or suffix.startswith("\n"):
         return prefix + suffix
     return prefix + " " + suffix
 
 
-# Keys class {{{2
-class Keys:
-    def __init__(self, key, value, dumper):
-        self.dumper = dumper
-        self.orig_keys = dumper.keys
-        self.orig_values = dumper.values
-        dumper.keys = dumper.keys + (key,)
-        dumper.values = dumper.values + (id(value),)
-
-    def __enter__(self):
-        pass
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.dumper.keys = self.orig_keys
-        self.dumper.values = self.orig_values
+# grow {{{2
+# add object to end of a tuple
+def grow(base, ext):
+    return base + (ext,)
 
 
 # NestedTextDumper class {{{2
 class NestedTextDumper:
     # constructor {{{3
-    def __init__(self, width, inline_level, sort_keys, indent, converters, default):
+    def __init__(
+        self, width, inline_level, sort_keys, indent, converters, default, map_keys
+    ):
         assert indent > 0
         self.width = width
         self.inline_level = inline_level
         self.indent = indent
         self.converters = converters
+        self.map_keys = map_keys
         self.default = default
-        self.keys = ()
-        self.values = ()
 
         # define key sorting function {{{4
         if sort_keys:
-            def sort(keys):
-                return sorted(keys, key=sort_keys if callable(sort_keys) else None)
+            if callable(sort_keys):
+                def sort(items, keys):
+                    return sorted(items, key=lambda k: sort_keys(k, keys))
+            else:
+                def sort(items, keys):
+                    return sorted(items)
         else:
-            def sort(keys):
-                return keys
-        self.sort_keys = sort
+            def sort(items, keys):
+                return items
+        self.sort = sort
 
         # define object type identification functions {{{4
-        if default == 'strict':
+        if default == "strict":
             self.is_a_dict = lambda obj: isinstance(obj, dict)
             self.is_a_list = lambda obj: isinstance(obj, list)
             self.is_a_str = lambda obj: isinstance(obj, str)
             self.is_a_scalar = lambda obj: False
         else:
             self.is_a_dict = is_mapping
             self.is_a_list = is_collection
             self.is_a_str = is_str
             self.is_a_scalar = lambda obj: obj is None or isinstance(obj, (bool, int, float))
             if is_str(default):
                 raise NotImplementedError(default)
 
-    # convert {{{3
-    def convert(self, obj):
-        converters = self.converters
-        converter = getattr(obj, '__nestedtext_converter__', None)
-        converter = converters.get(type(obj)) if converters else converter
-        if converter:
-            try:
-                return converter(obj)
-            except TypeError:
-                # is bound method
-                return converter()
-        elif converter is False:
-            raise NestedTextError(
-                obj,
-                template = f"unsupported type ({type(obj).__name__}).",
-                culprit = self.keys,
-            ) from None
-        return obj
-
     # render_key {{{3
-    def render_key(self, key):
-        key = self.convert(key)
+    def render_key(self, key, keys):
+        key = self.convert(key, keys)
         if self.is_a_scalar(key):
             if key is None:
                 key = ""
             else:
                 key = str(key)
         if not self.is_a_str(key) and callable(self.default):
             key = self.default(key)
         if not self.is_a_str(key):
             raise NestedTextError(
-                key,
-                template = 'keys must be strings.',
-                culprit = self.keys
+                key, template="keys must be strings.", culprit=keys
             ) from None
         return convert_returns(key)
 
     # render_dict_item {{{3
-    def render_dict_item(self, key, value, level):
+    def render_dict_item(self, key, value, keys, values):
         multiline_key_required = (
             not key
-            or '\n' in key
+            or "\n" in key
             or key.strip() != key
             or (key[:1] in "#[{" and support_inlines)
             or key[:2] in ["- ", "> ", ": "]
-            or ': ' in key
+            or ": " in key
         )
         if multiline_key_required:
             key = "\n".join(": "+l if l else ":" for l in key.split("\n"))
             if is_str(value):
                 # force use of multiline value with multiline keys
                 value = convert_returns(value)
                 return key + "\n" + add_leader(value, self.indent*" " + "> ")
             else:
-                return key + self.render_content(value, level + 1)
+                return key + self.render_value(value, keys, values)
         else:
-            return add_prefix(key + ":", self.render_content(value, level + 1))
+            return add_prefix(key + ":", self.render_value(value, keys, values))
 
     # render_inline_value {{{3
-    def render_inline_value(self, obj, exclude):
-        obj = self.convert(obj)
+    def render_inline_value(self, obj, exclude, keys, values):
+        obj = self.convert(obj, keys)
         if self.is_a_dict(obj):
-            return self.render_inline_dict(obj)
+            return self.render_inline_dict(obj, keys, values)
         if self.is_a_list(obj):
-            return self.render_inline_list(obj)
-        return self.render_inline_scalar(obj, exclude)
+            return self.render_inline_list(obj, keys, values)
+        return self.render_inline_scalar(obj, exclude, keys, values)
 
     # render_inline_dict {{{3
-    def render_inline_dict(self, obj):
-        exclude = set('\n\r[]{}:,')
-        rendered = {}
+    def render_inline_dict(self, obj, keys, values):
+        exclude = set("\n\r[]{}:,")
+        rendered = []
         for k, v in obj.items():
-            with Keys(k, v, self):
-                v = self.render_inline_value(obj[k], exclude=exclude)
-                k = self.render_inline_scalar(k, exclude=exclude)
-                rendered[k] = v
-        items = []
-        for k in self.sort_keys(rendered):
-            items.append(f'{k}: {rendered[k]}')
-        return '{' + ', '.join(items) + '}'
+            new_keys = grow(keys, k)
+            new_values = grow(values, id(v))
+            key = self.render_key(k, new_keys)
+            mapped_key = self.map_key(key, new_keys)
+            v = obj[k]
+            rendered_value = self.render_inline_value(
+                v, exclude, new_keys, new_values
+            )
+            rendered_key = self.render_inline_scalar(
+                mapped_key, exclude, new_keys, new_values
+            )
+            rendered.append((mapped_key, key, f"{rendered_key}: {rendered_value}",))
+        items = [v for mk, k, v in self.sort(rendered, keys)]
+        return ''.join(["{", ", ".join(items), "}"])
 
     # render_inline_list {{{3
-    def render_inline_list(self, obj):
-        items = []
-        for v in obj:
-            v = self.render_inline_value(v, exclude=set('\n\r[]{},'))
-            items.append(v)
-        if len(items) == 1 and not items[0]:
-            return '[ ]'
-        content = ', '.join(items)
-        leading_delimiter = '[ ' if content[0:1] == ',' else '['
-        return leading_delimiter + content + ']'
+    def render_inline_list(self, obj, keys, values):
+        rendered_values = []
+        for i, v in enumerate(obj):
+            rendered_value = self.render_inline_value(
+                v, set("\n\r[]{},"), grow(keys, i), grow(values, id(v))
+            )
+            rendered_values.append(rendered_value)
+        if len(rendered_values) == 1 and not rendered_values[0]:
+            return "[ ]"
+        content = ", ".join(rendered_values)
+        leading_delimiter = "[ " if content[0:1] == "," else "["
+        return leading_delimiter + content + "]"
 
     # render_inline_scalar {{{3
-    def render_inline_scalar(self, obj, exclude):
-        obj = self.convert(obj)
+    def render_inline_scalar(self, obj, exclude, keys, values):
+        obj = self.convert(obj, keys)
         if self.is_a_str(obj):
             value = obj
         elif self.is_a_scalar(obj):
-            value = '' if obj is None else str(obj)
+            value = "" if obj is None else str(obj)
         elif self.default and callable(self.default):
             try:
                 obj = self.default(obj)
             except TypeError:
                 raise NestedTextError(
                     obj,
                     template = f"unsupported type ({type(obj).__name__}).",
-                    culprit = self.keys
+                    culprit = keys
                 ) from None
-            return self.render_inline_value(obj, exclude)
+            return self.render_inline_value(obj, exclude, keys, values)
         else:
             raise NotSuitableForInline from None
 
         if exclude & set(value):
             raise NotSuitableForInline from None
         if value.strip() != value:
             raise NotSuitableForInline from None
         return value
 
-    # is_cyclic_reference {{{3
-    def check_for_cyclic_reference(self, obj):
-        if id(obj) in self.values[:-1]:
-            raise NestedTextError(
-                obj,
-                template = 'circular reference.',
-                culprit=self.keys
-            )
-
     # render content {{{3
-    def render_content(self, obj, level):
-        assert level >= 0
+    def render_value(self, obj, keys, values):
+        level = len(keys)
         error = None
-        content = ''
-        obj = self.convert(obj)
+        content = ""
+        obj = self.convert(obj, keys)
         need_indented_block = is_collection(obj)
 
         if self.is_a_dict(obj):
-            self.check_for_cyclic_reference(obj)
+            self.check_for_cyclic_reference(obj, keys, values)
             try:
                 if level < self.inline_level:
                     raise NotSuitableForInline from None
                 if obj and (self.width <= 0 or len(obj) > self.width/5):
                     raise NotSuitableForInline from None
-                content = self.render_inline_dict(obj)
+                content = self.render_inline_dict(obj, keys, values)
                 if obj and (len(content) > self.width):
                     raise NotSuitableForInline from None
             except NotSuitableForInline:
-                rendered = {}
+                rendered = []
                 for k, v in obj.items():
-                    with Keys(k, v, self):
-                        key = self.render_key(k)
-                        v = self.render_dict_item(key, obj[k], level)
-                        rendered[key] = v
-                content = "\n".join(rendered[k] for k in self.sort_keys(rendered))
+                    new_keys = grow(keys, k)
+                    new_values = grow(values, id(v))
+                    key = self.render_key(k, new_keys)
+                    mapped_key = self.map_key(key, new_keys)
+                    rendered_value = self.render_dict_item(
+                        mapped_key, obj[k], new_keys, new_values
+                    )
+                    rendered.append((mapped_key, key, rendered_value))
+                content = "\n".join(v for mk, k, v in self.sort(rendered, keys))
         elif self.is_a_list(obj):
-            self.check_for_cyclic_reference(obj)
+            self.check_for_cyclic_reference(obj, keys, values)
             try:
                 if level < self.inline_level:
                     raise NotSuitableForInline from None
                 if obj and (self.width <= 0 or len(obj) > self.width/3):
                     raise NotSuitableForInline from None
-                content = self.render_inline_list(obj)
+                content = self.render_inline_list(obj, keys, values)
                 if obj and (len(content) > self.width):
                     raise NotSuitableForInline from None
             except NotSuitableForInline:
                 content = []
                 for i, v in enumerate(obj):
-                    with Keys(i, v, self):
-                        content.append(
-                            add_prefix("-", self.render_content(v, level+1))
-                        )
+                    v = self.render_value(v, grow(keys, i), grow(values, id(v)))
+                    content.append(add_prefix("-", v))
                 content = "\n".join(content)
 
         elif self.is_a_str(obj):
             text = convert_returns(obj)
             if "\n" in text or level == 0:
-                content = add_leader(text, '> ')
+                content = add_leader(text, "> ")
                 need_indented_block = True
             else:
                 content = text
         elif self.is_a_scalar(obj):
             if obj is None:
-                content = ''
+                content = ""
             else:
                 content = str(obj)
+                if level == 0:
+                    content = add_leader(content, "> ")
+                    need_indented_block = True
         elif self.default and callable(self.default):
             try:
                 obj = self.default(obj)
             except TypeError:
                 error = f"unsupported type ({type(obj).__name__})."
             else:
-                content = self.render_content(obj, level+1)
+                content = self.render_value(obj, keys, values)
         else:
             error = f"unsupported type ({type(obj).__name__})."
 
         if need_indented_block and content and level:
             content = "\n" + add_leader(content, self.indent*" ")
 
         if error:
-            raise NestedTextError(obj, template=error, culprit=self.keys) from None
+            raise NestedTextError(obj, template=error, culprit=keys) from None
 
         return content
 
+    # check_for_cyclic_reference {{{3
+    def check_for_cyclic_reference(self, obj, keys, values):
+        if id(obj) in values[:-1]:
+            raise NestedTextError(
+                obj, template="circular reference.", culprit=keys
+            )
+
+    # convert {{{3
+    # apply externally supplied converter to convert value to string
+    def convert(self, obj, keys):
+        converters = self.converters
+        converter = getattr(obj, "__nestedtext_converter__", None)
+        converter = converters.get(type(obj)) if converters else converter
+        if converter:
+            try:
+                return converter(obj)
+            except TypeError:
+                # is bound method
+                return converter()
+        elif converter is False:
+            raise NestedTextError(
+                obj,
+                template = f"unsupported type ({type(obj).__name__}).",
+                culprit = keys,
+            ) from None
+        return obj
+
+    # map_key {{{3
+    # apply externally supplied mapping to convert key to desired form
+    def map_key(self, key, keys):
+        mapper = self.map_keys
+        if not mapper:
+            return key
+        if callable(mapper):
+            new_key = mapper(key, keys[:-1])
+            if new_key is None:
+                return key
+            return new_key
+        elif is_mapping(mapper):
+            try:
+                loc = mapper.get(keys)
+                if loc:
+                    return loc._get_original_key(key, strict=False)
+                else:
+                    return key
+            except AttributeError:    # pragma: no cover
+                raise AssertionError(
+                    "if map_keys is a dictionary, it must be a keymap"
+                ) from None
+        else:  # pragma: no cover
+            raise AssertionError(
+                "map_keys must be a callable or a dictionary"
+            ) from None
+
 
 # dumps {{{2
 def dumps(
     obj,
     *,
     width = 0,
     inline_level = 0,
     sort_keys = False,
     indent = 4,
     converters = None,
+    map_keys = None,
     default = None,
 ):
     # description {{{3
-    """Recursively convert object to *NestedText* string.
+    '''Recursively convert object to *NestedText* string.
 
     Args:
         obj:
             The object to convert to *NestedText*.
 
         width (int):
             Enables inline lists and dictionaries if greater than zero and if
             resulting line would be less than or equal to given width.
 
         inline_level (int):
             Recursion depth must be equal to this value or greater to be
             eligible for inlining.
 
         sort_keys (bool or func):
-            Dictionary items are sorted by their key if *sort_keys* is true.
-            If a function is passed in, it is used as the key function.
+            Dictionary items are sorted by their key if *sort_keys* is *True*.
+            In this case, keys at all level are sorted alphabetically.  If
+            *sort_keys* is *False*, the natural order of dictionaries is
+            retained.
+
+            If a function is passed in, it is expected to return the sort key.
+            The function is passed two tuples, each consists only of strings.
+            The first contains the mapped key, the original key, and the
+            rendered item.  So it takes the form::
+
+                ('<mapped_key>', '<orig_key>', '<mapped_key>: <value>')
+
+            The second contains the keys of the parent.
 
         indent (int):
             The number of spaces to use to represent a single level of
             indentation.  Must be one or greater.
 
         converters (dict):
             A dictionary where the keys are types and the values are converter
@@ -1589,18 +1671,24 @@
             are supported, including *None*, *bool*, *int*, *float*, and *list*-
             and *dict*-like objects.  In this case Booleans are rendered as
             “True” and “False” and None is rendered as an empty string.  If
             *default* is a function, it acts as the default converter.  If
             it raises a TypeError, the value is reported as an
             unsupported type.
 
-        _level (int):
-            The number of indentation levels.  When dumps is invoked recursively
-            this is used to increment the level and so the indent.  This argument
-            is use internally and should not be specified by the user.
+        map_keys (func or keymap):
+            This argument is used to modify the way keys are rendered.  It may
+            be a keymap that was created by :func:`load` or :func:`loads`, in
+            which case keys are rendered into their original form, before any
+            normalization or de-duplication was performed by the load functions.
+
+            It may also be a function that takes two arguments: the key after
+            any needed conversion has been performed, and the tuple of parent
+            keys.  The value returned is used as the key and so must be a
+            string.  If no value is returned, the key is not modified.
 
     Returns:
         The *NestedText* content without a trailing newline.  *NestedText* files
         should end with a newline, but unlike :func:`dump`, this function does
         not output that newline.  You will need to explicitly add that newline
         when writing the output :func:`dumps` to a file.
 
@@ -1610,25 +1698,25 @@
     Examples:
 
         .. code-block:: python
 
             >>> import nestedtext as nt
 
             >>> data = {
-            ...     'name': 'Kristel Templeton',
-            ...     'sex': 'female',
-            ...     'age': '74',
+            ...     "name": "Kristel Templeton",
+            ...     "gender": "female",
+            ...     "age": "74",
             ... }
 
             >>> try:
             ...     print(nt.dumps(data))
             ... except nt.NestedTextError as e:
             ...     print(str(e))
             name: Kristel Templeton
-            sex: female
+            gender: female
             age: 74
 
         The *NestedText* format only supports dictionaries, lists, and strings.
         By default, *dumps* is configured to be rather forgiving, so it will
         render many of the base Python data types, such as *None*, *bool*,
         *int*, *float* and list-like types such as *tuple* and *set* by
         converting them to the types supported by the format.  This implies that
@@ -1636,45 +1724,45 @@
         values being transformed. You can restrict *dumps* to only supporting
         the native types of *NestedText* by passing `default="strict"` to
         *dumps*.  Doing so means that values that are not dictionaries, lists,
         or strings generate exceptions.
 
         .. code-block:: python
 
-            >>> data = {'key': 42, 'value': 3.1415926, 'valid': True}
+            >>> data = {"key": 42, "value": 3.1415926, "valid": True}
 
             >>> try:
             ...     print(nt.dumps(data))
             ... except nt.NestedTextError as e:
             ...     print(str(e))
             key: 42
             value: 3.1415926
             valid: True
 
             >>> try:
-            ...     print(nt.dumps(data, default='strict'))
+            ...     print(nt.dumps(data, default="strict"))
             ... except nt.NestedTextError as e:
             ...     print(str(e))
             key: unsupported type (int).
 
         Alternatively, you can specify a function to *default*, which is used
         to convert values to recognized types.  It is used if no suitable
         converter is available.  Typical values are *str* and *repr*.
 
         .. code-block:: python
 
             >>> class Color:
             ...     def __init__(self, color):
             ...         self.color = color
             ...     def __repr__(self):
-            ...         return f'Color({self.color!r})'
+            ...         return f"Color({self.color!r})"
             ...     def __str__(self):
             ...         return self.color
 
-            >>> data['house'] = Color('red')
+            >>> data["house"] = Color("red")
             >>> print(nt.dumps(data, default=repr))
             key: 42
             value: 3.1415926
             valid: True
             house: Color('red')
 
             >>> print(nt.dumps(data, default=str))
@@ -1690,15 +1778,15 @@
 
             >>> class Color:
             ...     def __init__(self, color):
             ...         self.color = color
             ...     def __nestedtext_converter__(self):
             ...         return self.color.title()
 
-            >>> data['house'] = Color('red')
+            >>> data["house"] = Color("red")
             >>> print(nt.dumps(data))
             key: 42
             value: 3.1415926
             valid: True
             house: Red
 
         You can also specify a dictionary of converters. The dictionary maps the
@@ -1707,22 +1795,22 @@
         .. code-block:: python
 
             >>> class Info:
             ...     def __init__(self, **kwargs):
             ...         self.__dict__ = kwargs
 
             >>> converters = {
-            ...     bool: lambda b: 'yes' if b else 'no',
+            ...     bool: lambda b: "yes" if b else "no",
             ...     int: hex,
-            ...     float: lambda f: f'{f:0.3}',
+            ...     float: lambda f: f"{f:0.3}",
             ...     Color: lambda c: c.color,
             ...     Info: lambda i: i.__dict__,
             ... }
 
-            >>> data['attributes'] = Info(readable=True, writable=False)
+            >>> data["attributes"] = Info(readable=True, writable=False)
 
             >>> try:
             ...    print(nt.dumps(data, converters=converters))
             ... except nt.NestedTextError as e:
             ...     print(str(e))
             key: 0x2a
             value: 3.14
@@ -1737,15 +1825,15 @@
 
         If the dictionary maps a type to *None*, then the default behavior is
         used for that type. If it maps to *False*, then an exception is raised.
 
         .. code-block:: python
 
             >>> converters = {
-            ...     bool: lambda b: 'yes' if b else 'no',
+            ...     bool: lambda b: "yes" if b else "no",
             ...     int: hex,
             ...     float: False,
             ...     Color: lambda c: c.color,
             ...     Info: lambda i: i.__dict__,
             ... }
 
             >>> try:
@@ -1762,66 +1850,121 @@
         .. code-block:: python
 
             >>> import arrow
             >>> from inform import cull
             >>> import quantiphy
 
             >>> class Dollars(quantiphy.Quantity):
-            ...     units = '$'
-            ...     form = 'fixed'
+            ...     units = "$"
+            ...     form = "fixed"
             ...     prec = 2
             ...     strip_zeros = False
             ...     show_commas = True
 
             >>> converters = {
             ...     dict: cull,
-            ...     arrow.Arrow: lambda d: d.format('D MMMM YYYY'),
+            ...     arrow.Arrow: lambda d: d.format("D MMMM YYYY"),
             ...     quantiphy.Quantity: lambda q: str(q)
             ... }
 
             >>> transaction = dict(
-            ...     date = arrow.get('2013-05-07T22:19:11.363410-07:00'),
-            ...     description = "Incoming wire from Publisher's Clearing House",
+            ...     date = arrow.get("2013-05-07T22:19:11.363410-07:00"),
+            ...     description = "Incoming wire from Publisher’s Clearing House",
             ...     debit = 0,
             ...     credit = Dollars(12345.67)
             ... )
 
             >>> print(nt.dumps(transaction, converters=converters))
             date: 7 May 2013
-            description: Incoming wire from Publisher's Clearing House
+            description: Incoming wire from Publisher’s Clearing House
             credit: $12,345.67
 
         Both *default* and *converters* may be used together. *converters* has
         priority over the built-in types and *default*.  When a function is
         specified as *default*, it is always applied as a last resort.
-    """
+
+        Use the *map_keys* argument to format the keys as you wish.  For
+        example, you may wish to render the keys at the first level of hierarchy
+        in upper case:
+
+        .. code-block:: python
+
+            >>> def map_keys(key, parent_keys):
+            ...     if len(parent_keys) == 0:
+            ...         return key.upper()
+
+            >>> print(nt.dumps(transaction, converters=converters, map_keys=map_keys))
+            DATE: 7 May 2013
+            DESCRIPTION: Incoming wire from Publisher’s Clearing House
+            CREDIT: $12,345.67
+
+        It can also be used map the keys back to their original form when
+        round-tripping a dataset when using key normalization or key
+        de-duplication:
+
+        .. code-block:: python
+
+            >>> content = """
+            ... Michael Jordan:
+            ...     occupation: basketball player
+            ... Michael Jordan:
+            ...     occupation: actor
+            ... Michael Jordan:
+            ...     occupation: football player
+            ... """
+
+            >>> def de_dup(key, state):
+            ...     if key not in state:
+            ...         state[key] = 1
+            ...     state[key] += 1
+            ...     return f"{key}  ⟪#{state[key]}⟫"
+
+            >>> keymap = {}
+            >>> people = nt.loads(content, dict, on_dup=de_dup, keymap=keymap)
+            >>> print(nt.dumps(people))
+            Michael Jordan:
+                occupation: basketball player
+            Michael Jordan  ⟪#2⟫:
+                occupation: actor
+            Michael Jordan  ⟪#3⟫:
+                occupation: football player
+
+            >>> print(nt.dumps(people, map_keys=keymap))
+            Michael Jordan:
+                occupation: basketball player
+            Michael Jordan:
+                occupation: actor
+            Michael Jordan:
+                occupation: football player
+
+    '''
 
     # code {{{3
     dumper = NestedTextDumper(
-        width, inline_level, sort_keys, indent, converters, default
+        width, inline_level, sort_keys, indent, converters, default, map_keys
     )
-    return dumper.render_content(obj, 0)
+    return dumper.render_value(obj, (), ())
 
 
 # dump {{{2
 def dump(obj, dest, **kwargs):
     # description {{{3
     """Write the *NestedText* representation of the given object to the given file.
 
     Args:
         obj:
             The object to convert to *NestedText*.
         dest (str, os.PathLike, io.TextIOBase):
             The file to write the *NestedText* content to.  The file can be
             specified either as a path (e.g. a string or a `pathlib.Path`) or
-            as a text IO instance (e.g. an open file).  If a path is given, the
-            will be opened, written, and closed.  If an IO object is given, it
-            must have been opened in a mode that allows writing (e.g.
-            ``open(path, 'w')``), if applicable.  It will be written and not
-            closed.
+            as a text IO instance (e.g. an open file, or 1 for stdout).  If a
+            path is given, the will be opened, written, and closed.  If an IO
+            object is given, it must have been opened in a mode that allows
+            writing (e.g.  ``open(path, "w")``), if applicable.  It will be
+            written and not closed.
 
             The name used for the file is arbitrary but it is tradition to use a
             .nt suffix.  If you also wish to further distinguish the file type
             by giving the schema, it is recommended that you use two suffixes,
             with the suffix that specifies the schema given first and .nt given
             last. For example: flicker.sig.nt.
         kwargs:
@@ -1841,57 +1984,57 @@
 
         .. code-block:: python
 
             >>> import nestedtext as nt
             >>> from inform import fatal, os_error
 
             >>> data = {
-            ...     'name': 'Kristel Templeton',
-            ...     'sex': 'female',
-            ...     'age': '74',
+            ...     "name": "Kristel Templeton",
+            ...     "gender": "female",
+            ...     "age": "74",
             ... }
 
             >>> try:
-            ...     with open('data.nt', 'w', encoding='utf-8') as f:
+            ...     with open("data.nt", "w", encoding="utf-8") as f:
             ...         nt.dump(data, f)
             ... except nt.NestedTextError as e:
             ...     e.terminate()
             ... except OSError as e:
             ...     fatal(os_error(e))
 
         This example writes to a file specified by file name.  In general, the
         file name and extension are arbitrary. However, by convention a
-        '.nt' suffix is generally used for *NestedText* files.
+        ‘.nt’ suffix is generally used for *NestedText* files.
 
         .. code-block:: python
 
             >>> try:
-            ...     nt.dump(data, 'data.nt')
+            ...     nt.dump(data, "data.nt")
             ... except nt.NestedTextError as e:
             ...     e.terminate()
             ... except OSError as e:
             ...     fatal(os_error(e))
 
     """
 
     # code {{{3
     content = dumps(obj, **kwargs)
 
     try:
-        dest.write(content + '\n')
+        dest.write(content + "\n")
     except AttributeError:
         # Avoid nested try-except blocks, since they lead to chained exceptions
-        # (e.g. if the file isn't found, etc.) that unnecessarily complicate the
+        # (e.g. if the file isn’t found, etc.) that unnecessarily complicate the
         # stack trace.
         pass
     else:
         return
 
-    with open(dest, 'w', encoding='utf-8') as f:
-        f.write(content + '\n')
+    with open(dest, "w", encoding="utf-8") as f:
+        f.write(content + "\n")
 
 
 # NestedText Utilities {{{1
 # Extras that are useful when using NestedText.
 
 # get_value_from_keys {{{2
 def get_value_from_keys(obj, keys):
@@ -1915,28 +2058,28 @@
 
             >>> contents = """
             ... names:
             ...     given: Fumiko
             ...     surname: Purvis
             ... """
 
-            >>> data = nt.loads(contents, 'dict')
+            >>> data = nt.loads(contents, "dict")
 
-            >>> get_value_from_keys(data, ('names', 'given'))
+            >>> get_value_from_keys(data, ("names", "given"))
             'Fumiko'
 
     '''
     for key in keys:
         obj = obj[key]
     return obj
 
 
 # get_lines_from_keys {{{2
-def get_lines_from_keys(obj, keys, keymap, kind='value', sep=None):
-    """
+def get_lines_from_keys(obj, keys, keymap, kind="value", sep=None):
+    '''
     Get line numbers from normalized keys.
 
     This function returns the line numbers of the key or value selected by
     *keys*.  It is used when reporting an error in a value that is possibly a
     multiline string.  If the location contained in a keymap were used the user
     would only see the line number of the first line, which may confuse some
     users into believing the error is actually contained in the first line.
@@ -1972,20 +2115,20 @@
         sep:
             The separator string. If given a string is returned and *sep* is
             inserted between two line numbers.  Otherwise a tuple is returned.
 
     Example:
         >>> import nestedtext as nt
 
-        >>> doc = '''
+        >>> doc = """
         ... key:
         ...     > this is line 1
         ...     > this is line 2
         ...     > this is line 3
-        ... '''
+        ... """
 
         >>> data = nt.loads(doc, keymap=(keymap:={}))
         >>> keys = ("key",)
         >>> lines = nt.get_lines_from_keys(data, keys, keymap, sep="-")
         >>> text = doc.splitlines()
         >>> print(
         ...     f"Lines {lines}:",
@@ -1993,28 +2136,28 @@
         ...     sep="\\n"
         ... )
         Lines 3-5:
             > this is line 1
             > this is line 2
             > this is line 3
 
-    """
+    '''
     line, col = keymap[keys].as_tuple(kind)
     value = get_value_from_keys(obj, keys)
-    if kind == 'value':
+    if kind == "value":
         num_lines = len(value.splitlines()) if is_str(value) else 1
     else:
         key = keys[-1]
         num_lines = len(key.splitlines()) if is_str(key) else 1
     if sep is None:
-        return (line, line+num_lines)
+        return (line, line + num_lines)
     if num_lines > 1:
-        return join(line+1, line+num_lines, sep=sep)
+        return join(line + 1, line + num_lines, sep=sep)
     else:
-        return str(line+1)
+        return str(line + 1)
 
 
 # get_original_keys {{{2
 def get_original_keys(keys, keymap, strict=False):
     '''
     Get original keys from normalized keys.
 
@@ -2049,58 +2192,42 @@
             ... Names:
             ...     Given: Fumiko
             ... """
 
             >>> def normalize_key(key, keys):
             ...     return key.lower()
 
-            >>> data = nt.loads(contents, 'dict', normalize_key=normalize_key, keymap=(keymap:={}))
+            >>> data = nt.loads(contents, "dict", normalize_key=normalize_key, keymap=(keymap:={}))
 
-            >>> print(get_original_keys(('names', 'given'), keymap))
+            >>> print(get_original_keys(("names", "given"), keymap))
             ('Names', 'Given')
 
-            >>> print(get_original_keys(('names', 'surname'), keymap))
+            >>> print(get_original_keys(("names", "surname"), keymap))
             ('Names', 'surname')
 
-            >>> keys = get_original_keys(('names', 'surname'), keymap, strict=True)
+            >>> keys = get_original_keys(("names", "surname"), keymap, strict=True)
             Traceback (most recent call last):
             ...
             KeyError: ('names', 'surname')
 
     '''
-    original_keys = []
+    original_keys = ()
     for i in range(len(keys)):
         try:
             loc = keymap[tuple(keys[:i+1])]
-            line = loc.key_line
-            if line.kind == 'key item':
-                # is multiline key (key fragment is actually held in line.text)
-                key = [line.text[line.depth+2:]]
-                while line.next_line:
-                    line = line.next_line
-                    key.append(line.text[line.depth+2:])
-                key = '\n'.join(key)
-            else:
-                if line.kind == 'list item':
-                    key = keys[i]
-                else:
-                    key = line.key
-            original_keys.append(key)
-        except AttributeError:
-            # this occurs for list indexes
-            original_keys.append(keys[i])
+            original_keys += loc._get_original_key(keys[i], strict),
         except (KeyError, IndexError):
             if strict:
                 raise
-            original_keys.append(keys[i])
-    return tuple(original_keys)
+            original_keys += keys[i],
+    return original_keys
 
 
 # join_keys {{{2
-def join_keys(keys, sep=', ', keymap=None, strict=False):
+def join_keys(keys, sep=", ", keymap=None, strict=False):
     '''
     Joins the keys into a string.
 
     Args:
         keys:
             A tuple of keys.
         sep:
@@ -2129,32 +2256,33 @@
             ... Names:
             ...     Given: Fumiko
             ... """
 
             >>> def normalize_key(key, keys):
             ...     return key.lower()
 
-            >>> data = nt.loads(contents, 'dict', normalize_key=normalize_key, keymap=(keymap:={}))
+            >>> data = nt.loads(contents, "dict", normalize_key=normalize_key, keymap=(keymap:={}))
 
-            >>> join_keys(('names', 'given'))
+            >>> join_keys(("names", "given"))
             'names, given'
 
-            >>> join_keys(('names', 'given'), sep='.')
+            >>> join_keys(("names", "given"), sep=".")
             'names.given'
 
-            >>> join_keys(('names', 'given'), keymap=keymap)
+            >>> join_keys(("names", "given"), keymap=keymap)
             'Names, Given'
 
-            >>> join_keys(('names', 'surname'), keymap=keymap)
+            >>> join_keys(("names", "surname"), keymap=keymap)
             'Names, surname'
 
-            >>> join_keys(('names', 'surname'), keymap=keymap, strict=True)
+            >>> join_keys(("names", "surname"), keymap=keymap, strict=True)
             Traceback (most recent call last):
                 ...
             KeyError: ('names', 'surname')
 
     '''
     if keymap:
         keys = get_original_keys(keys, keymap, strict=strict)
     return sep.join(str(k) for k in keys)
 
+
 # vim: set sw=4 sts=4 tw=80 fo=croqj foldmethod=marker et spell:
```

### Comparing `nestedtext-3.5/pyproject.toml` & `nestedtext-3.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [project]
 name = "nestedtext"
-version = "3.5"
+version = "3.6"
 description = "human readable and writable data interchange format"
 readme = "README.rst"
-license = {file = "LICENSE"}
-keywords = ["data", "serialzation", "json", "yaml"]
+keywords = ["data", "serialization", "json", "yaml"]
 authors = [
     {name = "Ken Kundert"},
     {name = "Kale Kundert"},
-    {email = "inform@nurdletech.com"}
+    {email = "nestedtext@nurdletech.com"}
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Topic :: Text Processing :: Markup",
     "Topic :: Utilities",
 ]
 requires-python = ">=3.6"
 dependencies = [
-    "inform>=1.25",
+    "inform>=1.28",
 ]
 
 [project.urls]
 homepage = "https://nestedtext.org"
 documentation = "https://nestedtext.org"
 repository = "https://github.com/kenkundert/nestedtext"
 changelog = "https://github.com/KenKundert/nestedtext/blob/master/doc/releases.rst"
```

