# Comparing `tmp/nestedtext-3.6.tar.gz` & `tmp/nestedtext-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestedtext-3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nestedtext-3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nestedtext-3.6.tar` & `nestedtext-3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     5573 2023-05-31 03:28:22.230022 nestedtext-3.6/README.rst
--rw-r--r--   0        0        0      212 2023-05-31 03:28:22.229022 nestedtext-3.6/nestedtext/__init__.py
--rw-r--r--   0        0        0      454 2022-12-12 20:16:48.827895 nestedtext-3.6/nestedtext/__init__.pyi
--rw-r--r--   0        0        0    82755 2023-05-23 23:28:50.403675 nestedtext-3.6/nestedtext/nestedtext.py
--rw-r--r--   0        0        0     2528 2022-12-13 07:26:30.385323 nestedtext-3.6/nestedtext/nestedtext.pyi
--rw-r--r--   0        0        0        0 2022-12-12 18:21:38.584487 nestedtext-3.6/nestedtext/py.typed
--rw-r--r--   0        0        0     1027 2023-05-31 03:28:22.228022 nestedtext-3.6/pyproject.toml
--rw-r--r--   0        0        0     6510 1970-01-01 00:00:00.000000 nestedtext-3.6/PKG-INFO
+-rw-r--r--   0        0        0     8359 2024-04-28 01:02:55.499774 nestedtext-3.7/README.rst
+-rw-r--r--   0        0        0      403 2024-04-28 01:02:55.498774 nestedtext-3.7/nestedtext/__init__.py
+-rw-r--r--   0        0        0      454 2022-12-12 20:16:48.827895 nestedtext-3.7/nestedtext/__init__.pyi
+-rw-r--r--   0        0        0    98718 2024-04-28 00:46:53.910605 nestedtext-3.7/nestedtext/nestedtext.py
+-rw-r--r--   0        0        0     3319 2024-02-25 02:01:36.227667 nestedtext-3.7/nestedtext/nestedtext.pyi
+-rw-r--r--   0        0        0        0 2022-12-12 18:21:38.584487 nestedtext-3.7/nestedtext/py.typed
+-rw-r--r--   0        0        0     1027 2024-04-28 01:02:55.497774 nestedtext-3.7/pyproject.toml
+-rw-r--r--   0        0        0     9296 1970-01-01 00:00:00.000000 nestedtext-3.7/PKG-INFO
```

### Comparing `nestedtext-3.6/nestedtext/nestedtext.py` & `nestedtext-3.7/nestedtext/nestedtext.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 scalar text (strings).
 
 It is easily created, modified, or viewed with a text editor and easily
 understood and used by both programmers and non-programmers.
 """
 
 # MIT License {{{1
-# Copyright (c) 2020-2023 Ken and Kale Kundert
+# Copyright (c) 2020-2024 Ken and Kale Kundert
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -47,21 +47,14 @@
     Info,
 )
 import collections.abc
 import re
 import unicodedata
 
 
-# Globals {{{1
-support_inlines = True
-    # By disabling inlines it is possible to have keys that start with [ or {,
-    # but the resulting NestedText files are not compliant with the spec.
-    # Use of this feature is highly discouraged.
-
-
 # Utility functions {{{1
 # convert_returns {{{2
 def convert_returns(text):
     return text.replace("\r\n", "\n").replace("\r", "\n")
 
 
 # Unspecified {{{2
@@ -144,14 +137,17 @@
         ... """).strip()
 
         >>> try:
         ...     print(nt.loads(content))
         ... except nt.NestedTextError as e:
         ...     print(str(e))
         2: duplicate key: name1.
+               1 ❬name1: value1❭
+               2 ❬name1: value2❭
+                  ▲
 
     You can also use the *report* method to print the message directly. This is
     appropriate if you are using *inform* for your messaging as it follows
     *inform*’s conventions::
 
         >> try:
         ..     print(nt.loads(content))
@@ -210,14 +206,17 @@
         ...     print(nt.loads(content))
         ... except nt.NestedTextError as e:
         ...     template = None
         ...     if e.template == "duplicate key: {}.":
         ...         template = "llave duplicada: {}."
         ...     print(e.render(template=template))
         2: llave duplicada: name1.
+               1 ❬name1: value1❭
+               2 ❬name1: value2❭
+                  ▲
 
     '''
 
 
 # NotSuitableForInline {{{2
 # this is only intended for internal use
 class NotSuitableForInline(Exception):
@@ -296,28 +295,37 @@
     else:
         report("unrecognized line.", line, colno=index_of_first_non_space)
 
 
 # Lines class {{{2
 class Lines:
     # constructor {{{3
-    def __init__(self, lines):
+    def __init__(self, lines, support_inlines):
         self.lines = lines
+        self.support_inlines = support_inlines
         self.generator = self.read_lines()
+        self.first_value_line = None
+        self.last_comment_line = None
+            # a location is needed for the top of the data, keys = ()
+            # use the first value given, if the data is not empty
+            # use last comment given if data is empty
         self.next_line = True
         while self.next_line:
             self.next_line = next(self.generator, None)
             if self.next_line and self.next_line.kind not in ["blank", "comment"]:
                 return
 
     # Line class {{{3
     class Line(Info):
         def render(self, col=None):
             result = [f"{self.lineno+1:>4} ❬{self.text}❭"]
             if col is not None:
+                l = len(self.text)
+                if l < col:
+                    col = l
                 result += ["      " + (col*" ") + "▲"]
             return "\n".join(result)
 
         def __str__(self):
             return self.text
 
         def __repr__(self):
@@ -350,15 +358,15 @@
                 value = stripped[2:]
             elif stripped == ">" or stripped.startswith("> "):
                 kind = "string item"
                 value = line[depth+2:]
             elif stripped == ":" or stripped.startswith(": "):
                 kind = "key item"
                 value = line[depth+2:]
-            elif stripped[0:1] in ["[", "{"] and support_inlines:
+            elif stripped[0:1] in ["[", "{"] and self.support_inlines:
                 tag = stripped[0:1]
                 kind = "inline dict" if tag == "{" else "inline list"
                 value = line[depth:]
             else:
                 matches = dict_item_recognizer.fullmatch(stripped)
                 if matches:
                     kind = "dict item"
@@ -379,36 +387,42 @@
                 key = key,
                 value = value,
                 prev_line = prev_line,
             )
             if kind.endswith(" item") or kind.startswith("inline "):
                 # Create prev_line, which differs from last_line in that it
                 # is a copy of the line without a prev_line attribute of its
-                # own. This avoids keeping a chain of all previous lines. In
-                # contrast, last line is the actual this_line from the previous
-                # iteration.  Also, it is a data line, not a comment or blank.
+                # own. This avoids keeping a chain of all previous lines.
+                #
+                # In contrast, last_line is the actual this_line from the previous
+                # non-blank/comment iteration
                 prev_line = self.Line(
                     text = this_line.text,
                     value = this_line.value,
                     kind = this_line.kind,
                     depth = this_line.depth,
                     lineno = this_line.lineno,
                 )
 
                 # add this line as next_line in prev_line if this is a continued
-                # multiline string.
+                # multiline key or multiline string.
                 if (
                     last_line                 and
                     depth == last_line.depth  and
                     kind == last_line.kind    and
                     kind in ["key item", "string item"]
                 ):
                     last_line.next_line = this_line
 
-            last_line = this_line
+            if kind in ['blank', 'comment']:
+                self.last_comment_line = this_line
+            else:
+                last_line = this_line
+                if not self.first_value_line:
+                    self.first_value_line = this_line
             yield this_line
 
     # type_of_next() {{{3e
     def type_of_next(self):
         if self.next_line:
             return self.next_line.kind
 
@@ -552,54 +566,127 @@
     def as_tuple(self, kind="value"):
         """
         Returns the location of either the value or the key token as a tuple
         that contains the line number and the column number.  The line and
         column numbers are 0 based.
 
         Args:
-            kind (str):
+            kind:
                 Specify either “key” or “value” depending on which token is
                 desired.
         """
         if kind == "key":
             line = self.key_line
             col = self.key_col
             if line is None:
                 line = self.line
             if col is None:
                 col = self.col
         else:
+            assert kind == "value"
             line = self.line
             col = self.col
         return line.lineno, col
 
     # as_line() {{{3
-    def as_line(self, kind="value"):
+    def as_line(self, kind="value", offset=0):
         """
         Returns a string containing two lines that identify the token in
         context.  The first line contains the line number and text of the line
         that contains the token.  The second line contains a pointer to the
         token.
 
         Args:
-            kind (str):
+            kind:
                 Specify either “key” or “value” depending on which token is
                 desired.
+            offset:
+                If *offset* is None, the error pointer is not added to the line.
+                If *offset* is an integer, the pointer is moved to the right by
+                this many characters.  The default is 0.
+                If *offset* is a tuple, it must have two values.  The first is
+                the row offset and the second is the column offset.  This is
+                useful for annotating errors in multiline strings.
+
+        Raises:
+            *IndexError* if row offset is out of range.
         """
+        # get the line and the column number of the key or value
         if kind == "key":
             line = self.key_line
             col = self.key_col
             if line is None:
                 line = self.line
             if col is None:
                 col = self.col
         else:
+            assert kind == "value"
             line = self.line
             col = self.col
-        return line.render(col)
+
+        if not line:  # this occurs if input is completely empty
+            return ""
+
+        # process the offset
+        if offset is None:
+            return line.render()
+        col_offset = offset
+        try:
+            row_offset, col_offset = offset
+            while row_offset > 0:
+                line = line.next_line
+                row_offset -= 1
+                if line is None:
+                    raise IndexError(offset[0])
+        except TypeError:
+            pass
+
+        return line.render(col + col_offset)
+
+    # get_line_numbers() {{{3
+    def get_line_numbers(self, kind="value", sep=None):
+        """
+        Returns the line numbers of a token either as a pair of integers or as a
+        string.
+
+        Args:
+            kind:
+                Specify either “key” or “value” depending on which token is
+                desired.
+            sep:
+                The separator string.
+
+                If given a string is returned and *sep* is inserted between two
+                line numbers.  In this case the line numbers start at 1.
+
+                If *sep* is not given, a tuple of integers is returned.  In this
+                case the line numbers start at 0, but the second number returned
+                is the last line number plus 1.  This form is suitable to use
+                with the Python slice function to extract the lines from the
+                *NestedText* source.
+        """
+        if kind == "key":
+            line = self.key_line
+            if line is None:
+                line = self.line
+        else:
+            assert kind == "value"
+            line = self.line
+
+        # find line numbers
+        first_lineno = line.lineno
+        while line:
+            last_lineno = line.lineno
+            line = line.next_line
+
+        if sep is None:
+            return (first_lineno, last_lineno + 1)
+        if first_lineno != last_lineno:
+            return join(first_lineno+1, last_lineno+1, sep=sep)
+        return str(first_lineno+1)
 
     # _get_original_key() {{{3
     def _get_original_key(self, key, strict):
         try:
             line = self.key_line
             if line.kind == "key item":
                 # is multiline key (key fragment is actually held in line.text)
@@ -794,23 +881,33 @@
         name = self.__class__.__name__
         return f"{name}({self.text!r})"
 
 
 # NestedTextLoader class {{{2
 class NestedTextLoader:
     # __init__() {{{3
-    def __init__(self, lines, top, source, on_dup, keymap, normalize_key):
+    def __init__(self, lines, top, source, on_dup, keymap, normalize_key, dialect):
         KeyPolicy.set_policy(on_dup)
         self.source = source
         self.keymap = keymap
         assert self.keymap is None or is_mapping(self.keymap)
         self.normalize_key = normalize_key if normalize_key else lambda k, ks: k
+        if dialect and "i" in dialect:
+            support_inlines = False
+        else:
+            support_inlines = True
 
         with set_culprit(source):
-            lines = self.lines = Lines(lines)
+            lines = self.lines = Lines(lines, support_inlines)
+            if keymap is not None:
+                # add a location for the top-level of the data set
+                if lines.first_value_line:
+                    keymap[()] = Location(line=lines.first_value_line, col=0)
+                else:
+                    keymap[()] = Location(line=lines.last_comment_line, col=0)
             next_is = lines.type_of_next()
 
             if top in ["any", any]:
                 if next_is is None:
                     self.values, self.keymap = None, None
                 else:
                     self.values, self.keymap = self._read_value(0, ())
@@ -1026,15 +1123,22 @@
         lines = self.lines
         line = lines.get_next()
         return Inline(line, keys, self).get_values()
 
 
 # loads {{{2
 def loads(
-    content, top="dict", *, source=None, on_dup=None, keymap=None, normalize_key=None
+    content,
+    top = "dict",
+    *,
+    source = None,
+    on_dup = None,
+    keymap = None,
+    normalize_key = None,
+    dialect = None
 ):
     # description {{{3
     r'''
     Loads *NestedText* from string.
 
     Args:
         content (str):
@@ -1104,14 +1208,28 @@
 
         normalize_key (func):
             A function that takes two arguments; the original key for a value
             and the tuple of normalized keys for its parent values.  It then
             transforms the given key into the desired normalized form.  Only
             called on dictionary keys, so the key will always be a string.
 
+        dialect (str):
+            Specifies support for particular variations in *NestedText*.
+
+            In general you are discouraged from using a dialect as it can result
+            in *NestedText* documents that are not compliant with the standard.
+
+            The following deviant dialects are supported.
+
+            *support inlines*:
+                If "i" is included in *dialect*, support for inline lists and
+                dictionaries is dropped.  The default is "I", which enables
+                support for inlines.  The main effect of disabling inlines in
+                the load functions is that keys may begin with ``[`` or ``{``.
+
     Returns:
         The extracted data.  The type of the return value is specified by the
         top argument.  If top is “any”, then the return value will match that of
         top-level data container in the input content. If content is empty, an
         empty data value of the type specified by top is returned. If top is
         “any” None is returned.
 
@@ -1150,19 +1268,18 @@
 
             >>> filename = "examples/duplicate-keys.nt"
             >>> try:
             ...     with open(filename, encoding="utf-8") as f:
             ...         addresses = nt.loads(f.read(), source=filename)
             ... except nt.NestedTextError as e:
             ...     print(e.render())
-            ...     print(*e.get_codicil(), sep="\n")
             examples/duplicate-keys.nt, 5: duplicate key: name.
-               4 ❬name:❭
-               5 ❬name:❭
-                  ▲
+                   4 ❬name:❭
+                   5 ❬name:❭
+                      ▲
 
         Notice in the above example the encoding is explicitly specified as
         "utf-8".  *NestedText* files should always be read and written using
         *utf-8* encoding.
 
         The following examples demonstrate the various ways of handling
         duplicate keys:
@@ -1177,14 +1294,17 @@
             ... name: value 5
             ... """
 
             >>> print(nt.loads(content))
             Traceback (most recent call last):
             ...
             nestedtext.nestedtext.NestedTextError: 3: duplicate key: key.
+                   2 ❬key: value 1❭
+                   3 ❬key: value 2❭
+                      ▲
 
             >>> print(nt.loads(content, on_dup="ignore"))
             {'key': 'value 1', 'name': 'value 4'}
 
             >>> print(nt.loads(content, on_dup="replace"))
             {'key': 'value 3', 'name': 'value 5'}
 
@@ -1197,20 +1317,31 @@
             >>> print(nt.loads(content, on_dup=de_dup))
             {'key': 'value 1', 'key — #2': 'value 2', 'key — #3': 'value 3', 'name': 'value 4', 'name — #2': 'value 5'}
 
     '''
 
     # code {{{3
     lines = convert_returns(content).split("\n")
-    loader = NestedTextLoader(lines, top, source, on_dup, keymap, normalize_key)
+    loader = NestedTextLoader(
+        lines, top, source, on_dup, keymap, normalize_key, dialect
+    )
     return loader.get_decoded()
 
 
 # load {{{2
-def load(f, top="dict", *, on_dup=None, keymap=None, normalize_key=None):
+def load(
+    f,
+    top = "dict",
+    *,
+    source = None,
+    on_dup = None,
+    keymap = None,
+    normalize_key = None,
+    dialect = None
+):
     # description {{{3
     r"""
     Loads *NestedText* from file or stream.
 
     Is the same as :func:`loads` except the *NextedText* is accessed by reading
     a file rather than directly from a string. It does not keep the full
     contents of the file in memory and so is more memory efficient with large
@@ -1276,21 +1407,30 @@
     # code {{{3
     # Do not invoke the read method as that would read in the entire contents of
     # the file, possibly consuming a lot of memory. Instead pass the file
     # pointer into _read_all(), it will iterate through the lines, discarding
     # them once they are no longer needed, which reduces the memory usage.
 
     if isinstance(f, collections.abc.Iterator):
-        source = getattr(f, "name", None)
-        loader = NestedTextLoader(f, top, source, on_dup, keymap, normalize_key)
+        if not source:
+            source = getattr(f, "name", None)
+        loader = NestedTextLoader(
+            f, top, source, on_dup, keymap, normalize_key, dialect
+        )
         return loader.get_decoded()
     else:
-        source = str(f)
+        if not source:
+            if f == 0:
+                source = '<stdin>'
+            else:
+                source = str(f)
         with open(f, encoding="utf-8") as fp:
-            loader = NestedTextLoader(fp, top, source, on_dup, keymap, normalize_key)
+            loader = NestedTextLoader(
+                fp, top, source, on_dup, keymap, normalize_key, dialect
+            )
             return loader.get_decoded()
 
 
 # NestedText Writer {{{1
 # Converts Python data hierarchies to NestedText.
 
 # add_leader {{{2
@@ -1321,23 +1461,34 @@
     return base + (ext,)
 
 
 # NestedTextDumper class {{{2
 class NestedTextDumper:
     # constructor {{{3
     def __init__(
-        self, width, inline_level, sort_keys, indent, converters, default, map_keys
+        self,
+        width,
+        inline_level,
+        sort_keys,
+        indent,
+        converters,
+        default,
+        map_keys,
+        dialect
     ):
         assert indent > 0
         self.width = width
         self.inline_level = inline_level
         self.indent = indent
         self.converters = converters
         self.map_keys = map_keys
         self.default = default
+        self.support_inlines = True
+        if dialect and "i" in dialect:
+            self.support_inlines = False
 
         # define key sorting function {{{4
         if sort_keys:
             if callable(sort_keys):
                 def sort(items, keys):
                     return sorted(items, key=lambda k: sort_keys(k, keys))
             else:
@@ -1356,15 +1507,15 @@
             self.is_a_scalar = lambda obj: False
         else:
             self.is_a_dict = is_mapping
             self.is_a_list = is_collection
             self.is_a_str = is_str
             self.is_a_scalar = lambda obj: obj is None or isinstance(obj, (bool, int, float))
             if is_str(default):
-                raise NotImplementedError(default)
+                raise NotImplementedError(default)  # pragma: no cover
 
     # render_key {{{3
     def render_key(self, key, keys):
         key = self.convert(key, keys)
         if self.is_a_scalar(key):
             if key is None:
                 key = ""
@@ -1380,26 +1531,29 @@
 
     # render_dict_item {{{3
     def render_dict_item(self, key, value, keys, values):
         multiline_key_required = (
             not key
             or "\n" in key
             or key.strip() != key
-            or (key[:1] in "#[{" and support_inlines)
+            or key[:1] == "#"
+            or (key[:1] in "[{" and self.support_inlines)
             or key[:2] in ["- ", "> ", ": "]
             or ": " in key
         )
         if multiline_key_required:
             key = "\n".join(": "+l if l else ":" for l in key.split("\n"))
+            if self.is_a_dict(value) or self.is_a_list(value):
+                return key + self.render_value(value, keys, values)
             if is_str(value):
                 # force use of multiline value with multiline keys
                 value = convert_returns(value)
-                return key + "\n" + add_leader(value, self.indent*" " + "> ")
             else:
-                return key + self.render_value(value, keys, values)
+                value = self.render_value(value, keys, values)
+            return key + "\n" + add_leader(value, self.indent*" " + "> ")
         else:
             return add_prefix(key + ":", self.render_value(value, keys, values))
 
     # render_inline_value {{{3
     def render_inline_value(self, obj, exclude, keys, values):
         obj = self.convert(obj, keys)
         if self.is_a_dict(obj):
@@ -1475,14 +1629,16 @@
         content = ""
         obj = self.convert(obj, keys)
         need_indented_block = is_collection(obj)
 
         if self.is_a_dict(obj):
             self.check_for_cyclic_reference(obj, keys, values)
             try:
+                if not self.support_inlines:
+                    raise NotSuitableForInline from None
                 if level < self.inline_level:
                     raise NotSuitableForInline from None
                 if obj and (self.width <= 0 or len(obj) > self.width/5):
                     raise NotSuitableForInline from None
                 content = self.render_inline_dict(obj, keys, values)
                 if obj and (len(content) > self.width):
                     raise NotSuitableForInline from None
@@ -1497,14 +1653,16 @@
                         mapped_key, obj[k], new_keys, new_values
                     )
                     rendered.append((mapped_key, key, rendered_value))
                 content = "\n".join(v for mk, k, v in self.sort(rendered, keys))
         elif self.is_a_list(obj):
             self.check_for_cyclic_reference(obj, keys, values)
             try:
+                if not self.support_inlines:
+                    raise NotSuitableForInline from None
                 if level < self.inline_level:
                     raise NotSuitableForInline from None
                 if obj and (self.width <= 0 or len(obj) > self.width/3):
                     raise NotSuitableForInline from None
                 content = self.render_inline_list(obj, keys, values)
                 if obj and (len(content) > self.width):
                     raise NotSuitableForInline from None
@@ -1610,14 +1768,15 @@
     width = 0,
     inline_level = 0,
     sort_keys = False,
     indent = 4,
     converters = None,
     map_keys = None,
     default = None,
+    dialect = None
 ):
     # description {{{3
     '''Recursively convert object to *NestedText* string.
 
     Args:
         obj:
             The object to convert to *NestedText*.
@@ -1682,14 +1841,30 @@
             normalization or de-duplication was performed by the load functions.
 
             It may also be a function that takes two arguments: the key after
             any needed conversion has been performed, and the tuple of parent
             keys.  The value returned is used as the key and so must be a
             string.  If no value is returned, the key is not modified.
 
+        dialect (str):
+            Specifies support for particular variations in *NestedText*.
+
+            In general you are discouraged from using a dialect as it can result
+            in *NestedText* documents that are not compliant with the standard.
+
+            The following deviant dialects are supported.
+
+            *support inlines*:
+                If "i" is included in *dialect*, support for inline lists and
+                dictionaries is dropped.  The default is "I", which enables
+                support for inlines.  The main effect of disabling inlines in
+                the dump functions is that empty lists and dictionaries are
+                output using an empty value, which is normally interpreted by
+                *NestedText* as an empty string.
+
     Returns:
         The *NestedText* content without a trailing newline.  *NestedText* files
         should end with a newline, but unlike :func:`dump`, this function does
         not output that newline.  You will need to explicitly add that newline
         when writing the output :func:`dumps` to a file.
 
     Raises:
@@ -1936,15 +2111,16 @@
             Michael Jordan:
                 occupation: football player
 
     '''
 
     # code {{{3
     dumper = NestedTextDumper(
-        width, inline_level, sort_keys, indent, converters, default, map_keys
+        width, inline_level, sort_keys, indent, converters, default,
+        map_keys, dialect
     )
     return dumper.render_value(obj, (), ())
 
 
 # dump {{{2
 def dump(obj, dest, **kwargs):
     # description {{{3
@@ -2033,23 +2209,29 @@
         f.write(content + "\n")
 
 
 # NestedText Utilities {{{1
 # Extras that are useful when using NestedText.
 
 # get_value_from_keys {{{2
-def get_value_from_keys(obj, keys):
+def get_value_from_keys(data, keys):
+    # description {{{3
     '''
     Get value from keys.
 
+    Deprecated in version 3.7 and is to be removed in future versions.
+    :func:`get_value_from_keys` is replaced :func:`get_value`, which is
+    identical.
+
     Args:
-        obj:
+        data:
             Your data set as returned by :meth:`load` or :meth:`loads`.
         keys:
-            A tuple of keys taken from a *keymap*.
+            The sequence of normalized keys that identify a value in the
+            dataset.
 
     Returns:
         The value that corresponds to a tuple of keys from a keymap.
 
     Examples:
 
         .. code-block:: python
@@ -2064,24 +2246,30 @@
 
             >>> data = nt.loads(contents, "dict")
 
             >>> get_value_from_keys(data, ("names", "given"))
             'Fumiko'
 
     '''
+
+    # code {{{3
     for key in keys:
-        obj = obj[key]
-    return obj
+        data = data[key]
+    return data
 
 
 # get_lines_from_keys {{{2
-def get_lines_from_keys(obj, keys, keymap, kind="value", sep=None):
+def get_lines_from_keys(data, keys, keymap, kind="value", sep=None):
+    # description {{{3
     '''
     Get line numbers from normalized keys.
 
+    Deprecated in version 3.7 and is to be removed in future versions.
+    Use :func:`get_line_numbers` as a replacement.
+
     This function returns the line numbers of the key or value selected by
     *keys*.  It is used when reporting an error in a value that is possibly a
     multiline string.  If the location contained in a keymap were used the user
     would only see the line number of the first line, which may confuse some
     users into believing the error is actually contained in the first line.
     Using this function gives both the starting and ending line number so the
     user focuses on the whole string and not just the first line.
@@ -2099,15 +2287,15 @@
     If the value is requested and it is a composite (a dictionary or list), the
     line on which it ends cannot be easily determined, so the value is treated
     as if it consists of a single line.  This is considered tolerable as it is
     expected that this function is primarily used to return the line number of
     leaf values, which are always strings.
 
     Args:
-        obj:
+        data:
             Your data set as returned by :meth:`load` or :meth:`loads`.
         keys:
             The collection of keys that identify a value in the dataset.
         keymap:
             The keymap returned from :meth:`load` or :meth:`loads`.
         kind (str):
             Specify either “key” or “value” depending on which token is
@@ -2137,34 +2325,42 @@
         ... )
         Lines 3-5:
             > this is line 1
             > this is line 2
             > this is line 3
 
     '''
+
+    # code {{{3
+    if type(keys) is not tuple:
+        keys = tuple(keys)
+
     line, col = keymap[keys].as_tuple(kind)
-    value = get_value_from_keys(obj, keys)
+    value = get_value_from_keys(data, keys)
     if kind == "value":
         num_lines = len(value.splitlines()) if is_str(value) else 1
     else:
         key = keys[-1]
         num_lines = len(key.splitlines()) if is_str(key) else 1
     if sep is None:
         return (line, line + num_lines)
     if num_lines > 1:
         return join(line + 1, line + num_lines, sep=sep)
-    else:
-        return str(line + 1)
+    return str(line + 1)
 
 
 # get_original_keys {{{2
 def get_original_keys(keys, keymap, strict=False):
+    # description {{{3
     '''
     Get original keys from normalized keys.
 
+    Deprecated in version 3.7 and is to be removed in future versions.
+    Use :func:`get_keys` as a replacement.
+
     This function is used when the *normalize_key* argument is used with
     :meth:`load` or :meth:`loads` to transform the keys to a standard form.
     Given a set of normalized keys that point to a particular value in the
     returned dataset, this function returns the original keys for that value.
 
     Args:
         keys:
@@ -2206,31 +2402,37 @@
 
             >>> keys = get_original_keys(("names", "surname"), keymap, strict=True)
             Traceback (most recent call last):
             ...
             KeyError: ('names', 'surname')
 
     '''
+
+    # code {{{3
     original_keys = ()
     for i in range(len(keys)):
         try:
             loc = keymap[tuple(keys[:i+1])]
             original_keys += loc._get_original_key(keys[i], strict),
         except (KeyError, IndexError):
             if strict:
                 raise
             original_keys += keys[i],
     return original_keys
 
 
 # join_keys {{{2
 def join_keys(keys, sep=", ", keymap=None, strict=False):
+    # description {{{3
     '''
     Joins the keys into a string.
 
+    Deprecated in version 3.7 and is to be removed in future versions.
+    Use :func:`get_keys` as a replacement.
+
     Args:
         keys:
             A tuple of keys.
         sep:
             The separator string. It is inserted between each key during the join.
         keymap:
             The keymap returned from :meth:`load` or :meth:`loads`. It is
@@ -2276,13 +2478,285 @@
 
             >>> join_keys(("names", "surname"), keymap=keymap, strict=True)
             Traceback (most recent call last):
                 ...
             KeyError: ('names', 'surname')
 
     '''
+
+    # code {{{3
     if keymap:
         keys = get_original_keys(keys, keymap, strict=strict)
     return sep.join(str(k) for k in keys)
 
 
+# get_keys {{{2
+def get_keys(keys, keymap, *, original=True, strict=True, sep=None):
+    # description {{{3
+    '''
+    Returns a key sequence given a normalized key sequence.
+
+    Keys in the dataset output by the load functions are referred to as
+    normalized keys, even though no key normalization may have occurred.  This
+    distinguishes them from the original keys, which are the keys given in the
+    NestedText document read by the load functions.  The original keys are
+    mapped to normalized keys by the *normalize_key* argument to the load
+    function.  If normalization is not performed, the normalized keys are
+    the same as the original keys.
+
+    By default this function returns the original key sequence that corresponds
+    to *keys*, a normalized key sequence.
+
+    Args:
+        keys:
+            The sequence of normalized keys that identify a value in the
+            dataset.
+        keymap:
+            The keymap returned from :meth:`load` or :meth:`loads`.
+        original:
+            If true, return keys as originally given in the NestedText document
+            (pre-normalization). Otherwise return keys as they exist in the
+            dataset (post-normalization).  The value of this argument has no
+            effect if the keys were not normalized.
+        strict:
+            *strict* controls what happens if the given keys are not found in
+            *keymap*.
+
+            The various options can be helpful when reporting errors on key
+            sequences that do not exist in the data set.  Since they are not in
+            the dataset, the original keys are not available.
+
+            True or "error":
+                A *KeyError* is raised.
+            False or "all":
+                All keys given in *keys* are returned.
+            "found":
+                Only the initial available keys are returned.
+            "missing":
+                Only the missing final keys are returned.
+
+            When returning keys, the initial available keys are converted to
+            their original form if *original* is true,  The missing keys are
+            always returned as given.
+
+    Returns:
+        A tuple containing the desired keys.
+
+    Examples:
+
+        .. code-block:: python
+
+            >>> import nestedtext as nt
+
+            >>> contents = """
+            ... Names:
+            ...     Given: Fumiko
+            ... """
+
+            >>> def normalize_key(key, keys):
+            ...     return key.lower()
+
+            >>> data = nt.loads(contents, "dict", normalize_key=normalize_key, keymap=(keymap:={}))
+
+            >>> print(get_keys(("names", "given"), keymap))
+            ('Names', 'Given')
+
+            >>> print(get_keys(("names", "given"), keymap, sep="❭"))
+            Names❭Given
+
+            >>> print(get_keys(("names", "given"), keymap, original=False))
+            ('names', 'given')
+
+            >>> keys = get_keys(("names", "surname"), keymap, strict=True)
+            Traceback (most recent call last):
+            ...
+            KeyError: ('names', 'surname')
+
+            >>> print(get_keys(("names", "surname"), keymap, strict="found"))
+            ('Names',)
+
+            >>> print(get_keys(("names", "surname"), keymap, strict="missing"))
+            ('surname',)
+
+            >>> print(get_keys(("names", "surname"), keymap, strict="all"))
+            ('Names', 'surname')
+
+    '''
+
+    # code {{{3
+    assert strict in [True, False, "missing", "error", "all", "found"], strict
+    if type(keys) is not tuple:
+        keys = tuple(keys)
+
+    to_return = ()
+    for i in range(len(keys)):
+        try:
+            loc = keymap[tuple(keys[:i+1])]
+            key = loc._get_original_key(keys[i], strict) if original else keys[i]
+            if strict != "missing":
+                to_return += key,
+        except (KeyError, IndexError):
+            if strict in [True, "error"]:
+                raise
+            if strict != "found":
+                to_return += keys[i],
+    if sep:
+        return sep.join(str(k) for k in to_return)
+    return to_return
+
+
+# get_value{{{2
+def get_value(data, keys):
+    # description {{{3
+    '''
+    Get value from keys.
+
+    Args:
+        data:
+            Your data set as returned by :meth:`load` or :meth:`loads`.
+        keys:
+            The sequence of normalized keys that identify a value in the
+            dataset.
+
+    Returns:
+        The value that corresponds to a tuple of keys from a keymap.
+
+    Examples:
+
+        .. code-block:: python
+
+            >>> import nestedtext as nt
+
+            >>> contents = """
+            ... names:
+            ...     given: Fumiko
+            ...     surname: Purvis
+            ... """
+
+            >>> data = nt.loads(contents, "dict")
+
+            >>> get_value_from_keys(data, ("names", "given"))
+            'Fumiko'
+
+    '''
+
+    # code {{{3
+    for key in keys:
+        data = data[key]
+    return data
+
+
+# get_line_numbers {{{2
+def get_line_numbers(keys, keymap, kind="value", *, strict=True, sep=None):
+    # description {{{3
+    '''
+    Get line numbers from normalized key sequence.
+
+    This function returns the line numbers of the key or value selected by
+    *keys*.  It is used when reporting an error in a value that is possibly a
+    multiline string.  If the location contained in a keymap were used the user
+    would only see the line number of the first line, which may confuse some
+    users into believing the error is actually contained in the first line.
+    Using this function gives both the starting and ending line number so the
+    user focuses on the whole string and not just the first line.  This only
+    happens for multiline keys and multiline strings.
+
+    If *sep* is given, either one line number or both the beginning and ending line
+    numbers are returned, joined with the separator. In this case the line numbers
+    start from line 1.
+
+    If *sep* is not given, the line numbers are returned as a tuple containing a pair
+    of integers that is tailored to be suitable to be arguments to the Python slice
+    function (see example). The beginning line number and 1 plus the ending line
+    number is returned as a tuple. In this case the line numbers start at 0.
+
+    If *keys* corresponds to a composite value (a dictionary or list), the
+    line on which it ends cannot be easily determined, so the value is treated
+    as if it consists of a single line.  This is considered tolerable as it is
+    expected that this function is primarily used to return the line number of
+    leaf values, which are always strings.
+
+    Args:
+        keys:
+            The sequence of normalized keys that identify a value in the
+            dataset.
+        keymap:
+            The keymap returned from :meth:`load` or :meth:`loads`.
+        kind:
+            Specify either “key” or “value” depending on which token is
+            desired.
+        strict:
+            If *strict* is true, a *KeyError* is raised if *keys* is not found.
+            Otherwise the line number that corresponds to composite value that
+            would contain *keys* if it existed.  This composite value
+            corresponds to the largest sequence of keys that does actually exist
+            in the dataset.
+        sep:
+            The separator string. If given a string is returned and *sep* is
+            inserted between two line numbers.  Otherwise a tuple is returned.
+
+    Raises:
+        KeyError:
+            If keys are not in *keymap* and *strict* is true.
+
+    Example:
+        >>> import nestedtext as nt
+
+        >>> doc = """
+        ... key:
+        ...     > this is line 1
+        ...     > this is line 2
+        ...     > this is line 3
+        ... """
+
+        >>> data = nt.loads(doc, keymap=(keymap:={}))
+        >>> keys = ("key",)
+        >>> lines = nt.get_line_numbers(keys, keymap, sep="-")
+        >>> text = doc.splitlines()
+        >>> print(
+        ...     f"Lines {lines}:",
+        ...     *text[slice(*nt.get_line_numbers(keys, keymap))],
+        ...     sep="\\n"
+        ... )
+        Lines 3-5:
+            > this is line 1
+            > this is line 2
+            > this is line 3
+
+    '''
+
+    # code {{{3
+    loc = get_location(keys, keymap)
+    if not loc:
+        if strict:
+            raise KeyError(keys)
+        else:
+            found = get_keys(keys, keymap, original=False, strict="found")
+            loc = keymap[found]
+    return loc.get_line_numbers(kind, sep)
+
+
+# get_location {{{2
+def get_location(keys, keymap):
+    # description {{{3
+    '''
+    Returns :class:`Location` information from the keys.
+    None is returned if location is unknown.
+
+    Args:
+        keys:
+            The sequence of normalized keys that identify a value in the
+            dataset.
+        keymap:
+            The keymap returned from :meth:`load` or :meth:`loads`.
+    '''
+
+    # code {{{3
+    if type(keys) is not tuple:
+        keys = tuple(keys)
+
+    try:
+        return keymap[keys]
+    except KeyError:
+        return None
+
 # vim: set sw=4 sts=4 tw=80 fo=croqj foldmethod=marker et spell:
```

### Comparing `nestedtext-3.6/nestedtext/nestedtext.pyi` & `nestedtext-3.7/nestedtext/nestedtext.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -38,18 +38,25 @@
         self,
         kind: str = ...
     ) -> tuple[Line, int]:
         ...
 
     def as_line(
         self,
-        kind: str = ...
+        kind: str = ...,
+        offset: int | (int, int) | None = ...
     ) -> str:
         ...
 
+    def get_line_numbers(
+        self,
+        kind: str = ...,
+        sep: str = ...,
+    ) -> tuple[int, int] | str:
+        ...
 def loads(
     content : str,
     top: str | Callable | Type[dict] | Type[list] | Type[str] = ...,
     *,
     source: str | Path = ...,
     on_dup: str | Callable = ...,
     # keymap: dict[tuple[str, ...], Location] = ...,
@@ -100,22 +107,47 @@
     keymap: dict[tuple[str, ...], Any] = ...,
     kind: str = ...,
     sep: str = ...
 ) -> str | tuple[int, int]:
     ...
 
 def get_original_keys(
-    keys: tuple[str, ...],
+    keys: tuple[str | int, ...],
     # keymap: dict[tuple[str, ...], Location],
-    keymap: dict[tuple[str, ...], Any] = ...,
-    strict: bool = ...
+    keymap: dict[tuple[str | int, ...], Any] = ...,
+    strict: bool | str = ...
 ) -> tuple[int]:
     ...
 
 def join_keys(
-    keys: tuple[str, ...],
+    keys: tuple[str | int, ...],
     sep: str = ...,
     # keymap: dict[tuple[str], Location] = ...,
-    keymap: dict[tuple[str, ...], Any] = ...,
-    strict: bool = ...
+    keymap: dict[tuple[str | int, ...], Any] = ...,
+    strict: bool | str = ...
 ) -> str:
     ...
+
+def get_location(
+    keys: tuple[str | int, ...],
+    keymap: dict[tuple[str | int, ...], Location],
+) -> Location:
+    ...
+
+def get_line_numbers(
+    keys: tuple[str | int, ...],
+    keymap: dict[tuple[str | int, ...], Location],
+    kind: str = ...,
+    base: int = ...,
+    strict: bool = ...,
+    sep: str = ...,
+) -> tuple[int, int] | str:
+    ...
+
+def get_keys(
+    keys: tuple[str | int, ...],
+    keymap: dict[tuple[str | int, ...], Location],
+    original: bool = ...,
+    strict: bool | string = ...,
+    sep: str = ...,
+) -> tuple[str | int, ...] | str:
+    ...
```

### Comparing `nestedtext-3.6/pyproject.toml` & `nestedtext-3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nestedtext"
-version = "3.6"
+version = "3.7"
 description = "human readable and writable data interchange format"
 readme = "README.rst"
 keywords = ["data", "serialization", "json", "yaml"]
 authors = [
     {name = "Ken Kundert"},
     {name = "Kale Kundert"},
     {email = "nestedtext@nurdletech.com"}
```

### Comparing `nestedtext-3.6/PKG-INFO` & `nestedtext-3.7/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,35 @@
-Metadata-Version: 2.1
-Name: nestedtext
-Version: 3.6
-Summary: human readable and writable data interchange format
-Keywords: data,serialization,json,yaml
-Author: Ken Kundert, Kale Kundert
-Author-email: nestedtext@nurdletech.com
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Text Processing :: Markup
-Classifier: Topic :: Utilities
-Requires-Dist: inform>=1.28
-Project-URL: changelog, https://github.com/KenKundert/nestedtext/blob/master/doc/releases.rst
-Project-URL: documentation, https://nestedtext.org
-Project-URL: homepage, https://nestedtext.org
-Project-URL: repository, https://github.com/kenkundert/nestedtext
-
 NestedText — A Human Friendly Data Format
 =========================================
 
-.. image:: https://pepy.tech/badge/nestedtext/month
-    :target: https://pepy.tech/project/nestedtext
-
-.. image:: https://img.shields.io/readthedocs/nestedtext.svg
-   :target: https://nestedtext.readthedocs.io/en/latest/?badge=latest
-
-..  image:: https://github.com/KenKundert/nestedtext/actions/workflows/build.yaml/badge.svg
-    :target: https://github.com/KenKundert/nestedtext/actions/workflows/build.yaml
-
-.. image:: https://coveralls.io/repos/github/KenKundert/nestedtext/badge.svg?branch=master
-    :target: https://coveralls.io/github/KenKundert/nestedtext?branch=master
-
-.. image:: https://img.shields.io/pypi/v/nestedtext.svg
-    :target: https://pypi.python.org/pypi/nestedtext
-
-.. image:: https://img.shields.io/pypi/pyversions/nestedtext.svg
-    :target: https://pypi.python.org/pypi/nestedtext
+|downloads| |build status| |coverage| |rtd status| |pypi version| |anaconda version| |python version|
 
 
 | Authors: Ken & Kale Kundert
-| Version: 3.6
-| Released: 2023-05-30
-| Documentation: `nestedtext.org <https://nestedtext.org>`_.
-| Please post all questions, suggestions, and bug reports to: `Github <https://github.com/KenKundert/nestedtext/issues>`_.
+| Version: 3.7
+| Released: 2024-04-27
+| Documentation: nestedtext.org_
+| Please post all questions, suggestions, and bug reports to GitHub_.
 |
 
 *NestedText* is a file format for holding structured data.  It is similar in 
-concept to `JSON <https://en.wikipedia.org/wiki/JSON>`_, except that 
-*NestedText* is designed to make it easy for people to enter, edit, or view the 
-data directly.  It organizes the data into a nested collection of name-value 
-pairs, lists, and strings.  The syntax is intended to be very simple and 
-intuitive for most people.
+concept to JSON_, except that *NestedText* is designed to make it easy for 
+people to enter, edit, or view the data directly.  It organizes the data into 
+a nested collection of name-value pairs, lists, and strings.  The syntax is 
+intended to be very simple and intuitive for most people.
 
 A unique feature of this file format is that it only supports one scalar type: 
 strings.  As such, quoting strings is unnecessary, and without quoting there is 
 no need for escaping.  While the decision to forego other types (integers, 
-reals, dates, etc.) may seem counter productive, it leads to simpler data files 
-and applications that are more robust.
+reals, Booleans, etc.) may seem counter productive, it leads to simpler data 
+files and applications that are more robust.
 
-*NestedText* is convenient for configuration files, address books, account 
-information, and the like.  Here is an example of a file that contains a few 
-addresses:
+*NestedText* is convenient for configuration files, data journals, address 
+books, account information, and the like.  Here is an example of a file that 
+contains a few addresses:
 
 .. code-block:: nestedtext
 
     # Contact information for our officers
 
     Katheryn McDaniel:
         position: president
@@ -91,55 +51,98 @@
             > Topeka, Kansas 20682
         phone: 1-470-555-0398
         email: margaret.hodge@ku.edu
         additional roles:
             - new membership task force
             - accounting task force
 
-A strength of *NestedText* is its lack of quoting and escaping, making it 
-particularly nice for holding code fragments.  Here is another example of 
-*NestedText* that shows off this feature.  It holds some `Parametrize From File 
-<https://parametrize-from-file.readthedocs.io>`_ test cases for `pytest 
-<https://docs.pytest.org>`_.  In this case a command line program is being 
-tested and its response is checked using regular expressions::
+Typical Applications
+--------------------
+
+Configuration
+"""""""""""""
+
+Configuration files are an attractive application for *NestedText*.  
+*NestedText* configuration files tend to be simple, clean and unambiguous.  
+Plus, they handle hierarchy much better than alternatives such as Ini_ and 
+TOML_.
+
+
+Structured Code
+"""""""""""""""
+
+One way to build tools to tackle difficult and complex tasks is to provide an 
+application specific language.  That can be a daunting challenge.  However, in 
+certain cases, such as specifying complex configurations, *NestedText* can help 
+make the task much easier.  *NestedText* conveys the structure of data leaving 
+the end application to interpret the data itself.  It can do so with 
+a collection of small parsers that are tailored to the specific piece of data to 
+which they are applied.  This generally results in a simpler specification since 
+each piece of data can be given in its natural format, which might otherwise 
+confuse a shared parser.  In this way, rather than building one large very 
+general language and parser, a series of much smaller and simpler parsers are 
+needed.  These smaller parsers can be as simple as splitters or partitioners, 
+value checkers, or converters for numbers in special forms (numbers with units, 
+times or dates, GPS coordinates, etc.).  Or they could be full-blown expression 
+evaluators or mini-languages.  Structured code provides a nice middle ground 
+between data and code and its use is growing in popularity.
+
+An example of structured code is provided by GitHub with its workflow 
+specification files.  They use YAML_.  Unfortunately, the syntax of the code 
+snippets held in the various fields can be confused with *YAML* syntax, which 
+leads to unnecessary errors, confusion, and complexity (see *YAML issues*).  
+JSON_ suffers from similar problems.  *NestedText* excels for these applications 
+as it holds code snippets without any need for quoting or escaping.  
+*NestedText* provides simple unambiguous rules for defining the structure of 
+your data and when these rules are followed there is no way for any syntax or 
+special characters in the values of your data to be confused with *NestedText* 
+syntax.  In fact, it is possible for *NestedText* to hold *NestedText* snippets 
+without conflict.
+
+Another example of structured code is provided by the files that contain the 
+test cases used by `Parametrize From File`_, a PyTest_ plugin.
+*Parametrize From File* simplifies the task of specifying test cases for 
+*PyTest* by separating the test cases from the test code.  Here it is being 
+applied to test a command line program.  Its response is checked using regular 
+expressions.  Each entry includes a shell command to run the program and 
+a regular expression that must match the output for the test to pass::
 
     -
         cmd: emborg version
         expected: emborg version: \d+\.\d+(\.\d+(\.?\w+\d+)?)?  \(\d\d\d\d-\d\d-\d\d\)
-        expected_type: regex
-    -
-        cmd: emborg --quiet list
-        expected: home-\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d
-        expected_type: regex
-    -
-        cmd: emborg --quiet borg list --glob-archives "home-*" --short @repo
-        expected: home-\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d
-        expected_type: regex
+        expected type: regex
     -
         cmd: emborg --quiet files -D
         expected:
             > Archive: home-\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d
             > \d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d.\d\d\d\d\d\d configs/subdir/(file|)
             > \d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d.\d\d\d\d\d\d configs/subdir/(file|)
                 # Unfortunately, we cannot check the order as they were both 
                 # created at the same time.
-        expected_type: regex
+        expected type: regex
     -
         cmd: emborg due --backup-days 1 --message "{elapsed} since last {action}"
         expected: home: (\d+(\.\d)? (seconds|minutes)) since last backup\.
-        expected_type: regex
+        expected type: regex
+
+Notice that the regular expressions are given clean, without any quoting or 
+escaping.
 
-One particularly attractive use-case for *NestedText* is command line programs 
-whose output is meant to be consumed by either people or programs.  Many 
-programs do so by supporting a ``--json`` command-line flag that indicates the 
-output should be computer readable rather than human readable.  But, with 
-*NestedText* it is not necessary to make people choose.  Just output the result 
-in *NestedText* and it can be read by people or computers.  For example, 
-consider a program that reads your address list and output particular fields on 
-demand::
+
+Composable Utilities
+""""""""""""""""""""
+
+Another attractive use-case for *NestedText* is command line programs whose 
+output is meant to be consumed by either people or other programs.  This is 
+another growing trend.  Many programs do this by supporting a ``--json`` 
+command-line flag that indicates the output should be computer readable rather 
+than human readable.  But, with *NestedText* it is not necessary to make people 
+choose.  Just output the result in *NestedText* and it can be read by people or 
+computers.  For example, consider a program that reads your address list and 
+output particular fields on demand::
 
     > address --email
     Katheryn McDaniel: KateMcD@aol.com
     Margaret Hodge: margaret.hodge@ku.edu
 
 This output could be fed directly into another program that accepts *NestedText* 
 as input::
@@ -151,10 +154,40 @@
 ------------
 
 This package contains a Python reference implementation of *NestedText* and 
 a test suite.  Implementation in many languages is required for *NestedText* to 
 catch on widely.  If you like the format, please consider contributing 
 additional implementations.
 
-Also, please consider using *NestedText* for any applications you create.  It is 
-especially suitable for configuration files.
+Also, please consider using *NestedText* for any applications you create.
+
+
+.. _json: https://www.json.org/json-en.html
+.. _yaml: https://yaml.org/
+.. _toml: https://toml.io/en/
+.. _ini: https://en.wikipedia.org/wiki/INI_file
+.. _parametrize from file: https://parametrize-from-file.readthedocs.io
+.. _pytest: https://docs.pytest.org
+.. _github: https://github.com/KenKundert/nestedtext/issues
+.. _nestedtext.org: https://nestedtext.org
+
+.. |downloads| image:: https://pepy.tech/badge/nestedtext/month
+    :target: https://pepy.tech/project/nestedtext
+
+.. |rtd status| image:: https://img.shields.io/readthedocs/nestedtext.svg
+   :target: https://nestedtext.readthedocs.io/en/latest/?badge=latest
+
+.. |build status| image:: https://github.com/KenKundert/nestedtext/actions/workflows/build.yaml/badge.svg
+    :target: https://github.com/KenKundert/nestedtext/actions/workflows/build.yaml
+
+.. |coverage| image:: https://coveralls.io/repos/github/KenKundert/nestedtext/badge.svg?branch=master
+    :target: https://coveralls.io/github/KenKundert/nestedtext?branch=master
+
+.. |pypi version| image:: https://img.shields.io/pypi/v/nestedtext.svg
+    :target: https://pypi.python.org/pypi/nestedtext
+
+.. |anaconda version| image:: https://anaconda.org/conda-forge/nestedtext/badges/version.svg
+    :target: https://anaconda.org/conda-forge/nestedtext
+
+.. |python version| image:: https://img.shields.io/pypi/pyversions/nestedtext.svg
+    :target: https://pypi.python.org/pypi/nestedtext
```

