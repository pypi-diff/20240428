# Comparing `tmp/combustache-1.1.0.tar.gz` & `tmp/combustache-1.2.0.tar.gz`

## Comparing `combustache-1.1.0.tar` & `combustache-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 combustache-1.1.0/.gitmodules
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 combustache-1.1.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 combustache-1.1.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/__init__.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/__version__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/ctx.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/exceptions.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/main.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/util.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/nodes/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/nodes/comment.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/nodes/delimiter.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/nodes/interpolation.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/nodes/node.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/nodes/partial.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 combustache-1.1.0/src/combustache/nodes/section.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 combustache-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 combustache-1.1.0/tests/custom/conftest.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 combustache-1.1.0/tests/custom/indexing.yml
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 combustache-1.1.0/tests/custom/test_bad_template.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 combustache-1.1.0/tests/custom/test_cli.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 combustache-1.1.0/tests/custom/test_misc.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 combustache-1.1.0/tests/custom/test_opts.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 combustache-1.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 combustache-1.1.0/LICENSE
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 combustache-1.1.0/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 combustache-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 combustache-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 combustache-1.2.0/.gitmodules
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 combustache-1.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 combustache-1.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/__init__.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/__version__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/ctx.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/exceptions.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/main.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/util.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/comment.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/delimiter.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/interpolation.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/node.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/partial.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 combustache-1.2.0/src/combustache/nodes/section.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/conftest.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/indexing.yml
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_bad_template.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_misc.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 combustache-1.2.0/tests/custom/test_opts.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 combustache-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 combustache-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 combustache-1.2.0/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 combustache-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 combustache-1.2.0/PKG-INFO
```

### Comparing `combustache-1.1.0/.github/workflows/ci.yaml` & `combustache-1.2.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/.github/workflows/publish.yaml` & `combustache-1.2.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/src/combustache/__init__.py` & `combustache-1.2.0/src/combustache/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
-Mustache v1.4 implementation with lambdas.
+Cached Mustache v1.4 implementation with lambdas.
 
 Usable both in code and as CLI.
 To render a mustache template use `combustache.render`.
-Processed templates are cached; to clear cache use `combustache.cache_clear`.
+To clear cache use `combustache.cache_clear`.
+To load templates/partials from a directory use `combustache.load_templates`.
+To work with template objects directly use `combustache.Template`.
 
 Typical usage in code: ::
 
     >>> import combustache
     >>> template = 'Hello my name is {{>fancy_name}}!'
     >>> partials = {'fancy_name': '-> {{name}} <-'}
     >>> data = {'name': 'Anahit'}
@@ -23,19 +25,21 @@
 
 from combustache.exceptions import (
     CombustacheError,
     DelimiterError,
     MissingClosingTagError,
     StrayClosingTagError,
 )
-from combustache.main import cache_clear, render
-from combustache.util import load_partials
+from combustache.main import Template, cache_clear, render
+from combustache.util import load_partials, load_templates
 
 __all__ = [
     'render',
     'cache_clear',
+    'Template',
     'CombustacheError',
     'DelimiterError',
     'MissingClosingTagError',
     'StrayClosingTagError',
     'load_partials',
+    'load_templates',
 ]
```

### Comparing `combustache-1.1.0/src/combustache/__main__.py` & `combustache-1.2.0/src/combustache/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import json
 from pathlib import Path
 from typing import Sequence
 
 from combustache.__version__ import __version__
 from combustache.main import render
-from combustache.util import find_partial_files, paths_to_partials
+from combustache.util import find_template_files, paths_to_templates
 
 
 def cli(argv: Sequence[str] | None = None):
     parser = argparse.ArgumentParser(
         prog='combustache',
         description='an explosive mustache v1.4 implementation with lambdas',
     )
@@ -91,17 +91,17 @@
 
     data = json.load(args.data)
 
     if args.partial is None:
         args.partial = []
 
     if args.partial_dir:
-        partial_files = find_partial_files(args.partial_dir, args.partial_ext)
+        partial_files = find_template_files(args.partial_dir, args.partial_ext)
         args.partial.extend(partial_files)
-    partials = paths_to_partials(args.partial, args.partial_ext)
+    partials = paths_to_templates(args.partial, args.partial_ext)
 
     left_delimiter = args.left_delimiter
     right_delimiter = args.right_delimiter
 
     output = render(template, data, partials, left_delimiter, right_delimiter)
     args.output.write(output)
```

### Comparing `combustache-1.1.0/src/combustache/nodes/delimiter.py` & `combustache-1.2.0/src/combustache/nodes/delimiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 class Delimiter(Node):
     left = '='
     right = '='
     ignorable = True
 
     def __init__(
         self,
-        content: str,
+        contents: str,
         tag_start: int,
         tag_end: int,
         template: str,
         template_start: int,
         template_end: int,
         left_delimiter: str,
         right_delimiter: str,
     ) -> None:
         super().__init__(
-            content,
+            contents,
             tag_start,
             tag_end,
             template,
             template_start,
             template_end,
             left_delimiter,
             right_delimiter,
         )
-        split = self.content.split()
+        split = self.contents.split()
         if len(split) != 2:
             row, col = find_position(self.template, self.start)
             raise DelimiterError(
                 'Impossible delimiter tag found: '
                 f'{self.tag_string} at {row}:{col}'
             )
         self.left_delimiter = split[0]
```

### Comparing `combustache-1.1.0/src/combustache/nodes/interpolation.py` & `combustache-1.2.0/src/combustache/nodes/interpolation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Callable
 
 import combustache.main
 from combustache.ctx import MISSING, Ctx
 from combustache.nodes.node import Node
-from combustache.util import LAMBDA, Opts, is_callable
+from combustache.util import LAMBDA, Opts
 
 
 class Interpolation(Node):
     standalonable = False
 
     def get_string(
         self,
@@ -18,22 +18,25 @@
         return escape(stringify(data))
 
     def handle(self, ctx: Ctx, partials: dict[str, str], opts: Opts) -> str:
         stringify = opts['stringify']
         escape = opts['escape']
         missing_data = opts['missing_data']
 
-        data = ctx.get(self.content)
+        data = ctx.get(self.contents)
         if data is MISSING:
             return missing_data()
 
-        if is_callable(data):
+        if callable(data):
+            # if the callable is a lambda function we should render its result
+            # in the current context
             if data.__name__ == LAMBDA:
                 template = str(data())
                 data = combustache.main._render(template, ctx, partials, opts)
+            # otherwise we should just get the result
             else:
                 data = data()
 
         string = self.get_string(data, stringify, escape)
         return string
```

### Comparing `combustache-1.1.0/src/combustache/nodes/node.py` & `combustache-1.2.0/src/combustache/nodes/node.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,54 +6,59 @@
     left = ''
     right = ''
     ignorable = False
     standalonable = True
 
     def __init__(
         self,
-        content: str,
+        contents: str,
         tag_start: int,
         tag_end: int,
         template: str,
         template_start: int,
         template_end: int,
         left_delimiter: str,
         right_delimiter: str,
     ) -> None:
-        self.content = content
+        self.contents = contents
         self.template = template
         self.template_start = template_start
         self.template_end = template_end
         self.left_delimiter = left_delimiter
         self.right_delimiter = right_delimiter
-        self.inside: list[Node | str] = []
 
         # we +1 to line_start and line_end to get 'hello\n' instad of '\nhello'
         # and we get a nice side effect for end of getting 0 if we dont find \n
         # (i.e. we hit end of string) because str.find returns -1 in that case
         # so we can 'or len(template)' our value to get the end of the template
         line_start = template.rfind('\n', 0, tag_start) + 1
         line_end = template.find('\n', tag_end) + 1 or len(template)
 
+        # string between the last linebreak and node start
         self.before = template[line_start:tag_start]
+        # string between node end and the next linebreak
         self.after = template[tag_end:line_end]
+        # these are used to check if the tag is standalone
 
         self.is_standalone = is_whitespace(self.before) and is_whitespace(
             self.after
         )
         if self.standalonable and self.is_standalone:
             self.start = line_start
             self.end = line_end
         else:
             self.start = tag_start
             self.end = tag_end
+        # parse_end shows the parser from where it should continue parsing
+        # tags like Section and Inverted find their closing tag and set
+        # parse_end to the end of their closing tag
         self.parse_end = self.end
 
     @property
     def tag_string(self) -> str:
         return (
             f'{self.left_delimiter}{self.left} '
-            f'{self.content} {self.right}{self.right_delimiter}'
+            f'{self.contents} {self.right}{self.right_delimiter}'
         )
 
     def handle(self, ctx: Ctx, partials: dict[str, str], opts: Opts) -> str:
         raise NotImplementedError
```

### Comparing `combustache-1.1.0/src/combustache/nodes/partial.py` & `combustache-1.2.0/src/combustache/nodes/partial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class Partial(Node):
     left = '>'
 
     def handle(self, ctx: Ctx, partials: dict[str, str], opts: Opts) -> str:
         missing_data = opts['missing_data']
 
-        partial_template = partials.get(self.content)
+        partial_template = partials.get(self.contents)
 
         if partial_template is None:
             return missing_data()
 
         if self.is_standalone:
             partial_template = '\n'.join(
                 bool(line) * self.before + line
```

### Comparing `combustache-1.1.0/src/combustache/nodes/section.py` & `combustache-1.2.0/src/combustache/nodes/section.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import combustache.main
 from combustache.ctx import MISSING, Ctx
 from combustache.exceptions import MissingClosingTagError, StrayClosingTagError
 from combustache.nodes.node import Node
-from combustache.util import LAMBDA, Opts, find_position, is_callable
+from combustache.util import LAMBDA, Opts, find_position
 
 
 class Section(Node):
     left = '#'
 
     def __init__(
         self,
-        content: str,
+        contents: str,
         tag_start: int,
         tag_end: int,
         template: str,
         template_start: int,
         template_end: int,
         left_delimiter: str,
         right_delimiter: str,
     ) -> None:
         super().__init__(
-            content,
+            contents,
             tag_start,
             tag_end,
             template,
             template_start,
             template_end,
             left_delimiter,
             right_delimiter,
@@ -41,95 +41,93 @@
             )
             if node_info is None:
                 row, col = find_position(self.template, self.start)
                 raise MissingClosingTagError(
                     f'No closing tag found: {self.tag_string} at {row}:{col}'
                 )
 
-            node_type, content, start, end = node_info
-            if content == self.content:
-                if node_type is self.__class__:
+            NodeType, contents, start, end = node_info
+            if contents == self.contents:
+                if NodeType is self.__class__:
                     depth += 1
-                elif node_type is Closing:
+                elif NodeType is Closing:
                     if depth == 0:
                         break
                     depth -= 1
 
             search_start = end
 
-        # not creating ClosingTag because it raises the stray tag error
+        # not creating a ClosingTag because it raises the stray tag error
         closing_tag = Node(
-            content,
+            contents,
             start,
             end,
             self.template,
             self.template_start,
             self.template_end,
             self.left_delimiter,
             self.right_delimiter,
         )
 
         self.inside_start = self.end
         self.inside_end = closing_tag.start
         self.parse_end = closing_tag.end
-        self.inside = combustache.main.parse(
+        self.inside = combustache.main.Template(
             self.template,
-            self.inside_start,
-            self.inside_end,
             self.left_delimiter,
             self.right_delimiter,
+            self.inside_start,
+            self.inside_end,
         )
 
     def should_be_rendered(self, item):
         return item and item is not MISSING
 
     def handle(self, ctx: Ctx, partials: dict[str, str], opts: Opts) -> str:
         missing_data = opts['missing_data']
 
-        data = ctx.get(self.content)
+        data = ctx.get(self.contents)
 
         if not self.should_be_rendered(data):
             if data is MISSING:
                 return missing_data()
             return ''
 
-        if is_callable(data):
+        if callable(data):
             unprocessed = self.template[self.inside_start : self.inside_end]
+            # if the callable is a lambda we should call it with the string
+            # between the tag and its closing tag and render the result
+            # in the current context
             if data.__name__ == LAMBDA:
                 template = str(data(unprocessed))
                 return combustache.main._render(
                     template,
                     ctx,
                     partials,
                     opts,
                     self.left_delimiter,
                     self.right_delimiter,
                 )
             else:
+                # otherwise we should get the result with the string passed in
                 try:
                     data = data(unprocessed)
+                # or just called
                 except TypeError:
                     data = data()
 
         # if data is not a list we put it into one
         # so we can process it easily
         if not isinstance(data, list) or not data:
             data = [data]
 
         handled = []
         for item in data:
             ctx.append(item)
-            handled.extend(
-                [
-                    node.handle(ctx, partials, opts)
-                    if isinstance(node, Node)
-                    else node
-                    for node in self.inside
-                ]
-            )
+            handled.append(self.inside._render(ctx, partials, opts))
             ctx.pop()
         return ''.join(handled)
 
 
 class Inverted(Section):
     left = '^'
 
@@ -137,13 +135,16 @@
         return not item or item is MISSING
 
 
 class Closing(Node):
     left = '/'
     ignorable = True
 
+    # Section and Inverted find their closing tags themselves
+    # so if the parser tries to create a Closing tag that means that the tag
+    # was not opened to be closed
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         row, col = find_position(self.template, self.start)
         raise StrayClosingTagError(
             f'Stray closing tag found: {self.tag_string} at {row}:{col}'
         )
```

### Comparing `combustache-1.1.0/tests/conftest.py` & `combustache-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/tests/custom/conftest.py` & `combustache-1.2.0/tests/custom/conftest.py`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/tests/custom/indexing.yml` & `combustache-1.2.0/tests/custom/indexing.yml`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/tests/custom/test_bad_template.py` & `combustache-1.2.0/tests/custom/test_bad_template.py`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/tests/custom/test_cli.py` & `combustache-1.2.0/tests/custom/test_cli.py`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/tests/custom/test_opts.py` & `combustache-1.2.0/tests/custom/test_opts.py`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/.gitignore` & `combustache-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/LICENSE` & `combustache-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/README.md` & `combustache-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # combustache
 
 [![CI](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml/badge.svg)](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml)
 
-Mustache v1.4 implementation with lambdas.
+Cached Mustache v1.4 implementation with lambdas.
 
 Usable both in code and as CLI.
 To render a mustache template use `combustache.render`.
-Processed templates are cached; to clear cache use `combustache.cache_clear`.
-To load partials from a directory use `combustache.load_partials`.
+To clear cache use `combustache.cache_clear`.
+To load templates/partials from a directory use `combustache.load_templates`.
+To work with template objects directly use `combustache.Template`.
 
 ## Installation
 
 From [PyPI](https://pypi.org/project/combustache/):
 
 ```sh
 pip install combustache
@@ -24,15 +25,15 @@
 ```
 
 ## Usage as CLI
 
 `combustache ...` or `python -m combustache ...`
 
 ```console
-$ hashime -h
+$ combustache -h
 usage: combustache [-h] [-v] [-s] [-d DATA] [-o OUTPUT] [-p PARTIAL]
                    [--partial-dir PARTIAL_DIR] [--partial-ext PARTIAL_EXT]
                    [--left-delimiter LEFT_DELIMITER] [--right-delimiter RIGHT_DELIMITER]
                    template
 
 an explosive mustache v1.4 implementation with lambdas
```

### Comparing `combustache-1.1.0/pyproject.toml` & `combustache-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `combustache-1.1.0/PKG-INFO` & `combustache-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: combustache
-Version: 1.1.0
+Version: 1.2.0
 Summary: Mustache v1.4 implementation with lambdas.
 Project-URL: Homepage, https://github.com/sakhezech/combustache
 License: MIT License
         
         Copyright (c) 2023 Sakhezech
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,20 +31,21 @@
 Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # combustache
 
 [![CI](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml/badge.svg)](https://github.com/sakhezech/combustache/actions/workflows/ci.yaml)
 
-Mustache v1.4 implementation with lambdas.
+Cached Mustache v1.4 implementation with lambdas.
 
 Usable both in code and as CLI.
 To render a mustache template use `combustache.render`.
-Processed templates are cached; to clear cache use `combustache.cache_clear`.
-To load partials from a directory use `combustache.load_partials`.
+To clear cache use `combustache.cache_clear`.
+To load templates/partials from a directory use `combustache.load_templates`.
+To work with template objects directly use `combustache.Template`.
 
 ## Installation
 
 From [PyPI](https://pypi.org/project/combustache/):
 
 ```sh
 pip install combustache
@@ -57,15 +58,15 @@
 ```
 
 ## Usage as CLI
 
 `combustache ...` or `python -m combustache ...`
 
 ```console
-$ hashime -h
+$ combustache -h
 usage: combustache [-h] [-v] [-s] [-d DATA] [-o OUTPUT] [-p PARTIAL]
                    [--partial-dir PARTIAL_DIR] [--partial-ext PARTIAL_EXT]
                    [--left-delimiter LEFT_DELIMITER] [--right-delimiter RIGHT_DELIMITER]
                    template
 
 an explosive mustache v1.4 implementation with lambdas
```

