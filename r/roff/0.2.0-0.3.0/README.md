# Comparing `tmp/roff-0.2.0.tar.gz` & `tmp/roff-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roff-0.2.0.tar", last modified: Tue Apr 23 11:36:40 2024, max compression
+gzip compressed data, was "roff-0.3.0.tar", last modified: Sun Apr 28 12:35:14 2024, max compression
```

## Comparing `roff-0.2.0.tar` & `roff-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.850998 roff-0.2.0/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-23 10:39:23.000000 roff-0.2.0/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     2759 2024-04-23 11:36:40.850998 roff-0.2.0/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1510 2024-04-23 10:39:23.000000 roff-0.2.0/README.md
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.846997 roff-0.2.0/docs/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1354 2024-04-23 11:36:29.000000 roff-0.2.0/docs/roff.1
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-23 10:39:23.000000 roff-0.2.0/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-23 11:36:40.850998 roff-0.2.0/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1940 2024-04-23 10:39:23.000000 roff-0.2.0/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.846997 roff-0.2.0/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.846997 roff-0.2.0/src/roff/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.850998 roff-0.2.0/src/roff/__cli__/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       78 2024-04-23 10:39:23.000000 roff-0.2.0/src/roff/__cli__/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      513 2024-04-23 10:39:23.000000 roff-0.2.0/src/roff/__cli__/convert.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      950 2024-04-23 10:56:38.000000 roff-0.2.0/src/roff/__cli__/template.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-04-23 11:36:18.000000 roff-0.2.0/src/roff/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1457 2024-04-23 10:54:12.000000 roff-0.2.0/src/roff/__main__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     6732 2024-04-23 11:33:32.000000 roff-0.2.0/src/roff/convert.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-23 11:36:40.850998 roff-0.2.0/src/roff.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     2759 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      395 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/entry_points.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       15 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-04-23 11:36:40.000000 roff-0.2.0/src/roff.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-28 12:35:14.629850 roff-0.3.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-21 09:37:21.000000 roff-0.3.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-28 12:35:14.629850 roff-0.3.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1673 2024-04-28 12:23:56.000000 roff-0.3.0/README.md
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-28 12:35:14.625850 roff-0.3.0/docs/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1645 2024-04-28 12:31:29.000000 roff-0.3.0/docs/roff.1
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2857 2024-04-28 12:31:35.000000 roff-0.3.0/docs/roff.5
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-21 09:38:29.000000 roff-0.3.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-28 12:35:14.629850 roff-0.3.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2155 2024-04-25 15:15:31.000000 roff-0.3.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-28 12:35:14.621850 roff-0.3.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-28 12:35:14.625850 roff-0.3.0/src/roff/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-28 12:35:14.629850 roff-0.3.0/src/roff/__cli__/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      104 2024-04-23 17:04:15.000000 roff-0.3.0/src/roff/__cli__/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      446 2024-04-25 15:15:31.000000 roff-0.3.0/src/roff/__cli__/convert.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1036 2024-04-27 11:45:13.000000 roff-0.3.0/src/roff/__cli__/template.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      713 2024-04-23 17:04:15.000000 roff-0.3.0/src/roff/__cli__/util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-04-28 12:35:09.000000 roff-0.3.0/src/roff/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1601 2024-04-23 20:27:06.000000 roff-0.3.0/src/roff/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2641 2024-04-25 15:15:31.000000 roff-0.3.0/src/roff/_images.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2303 2024-04-27 11:04:01.000000 roff-0.3.0/src/roff/_markdown.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      213 2024-04-26 19:43:17.000000 roff-0.3.0/src/roff/_util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)    10801 2024-04-28 12:31:05.000000 roff-0.3.0/src/roff/convert.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-28 12:35:14.629850 roff-0.3.0/src/roff.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-28 12:35:14.000000 roff-0.3.0/src/roff.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      492 2024-04-28 12:35:14.000000 roff-0.3.0/src/roff.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-28 12:35:14.000000 roff-0.3.0/src/roff.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-04-28 12:35:14.000000 roff-0.3.0/src/roff.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       94 2024-04-28 12:35:14.000000 roff-0.3.0/src/roff.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-04-28 12:35:14.000000 roff-0.3.0/src/roff.egg-info/top_level.txt
```

### Comparing `roff-0.2.0/LICENSE` & `roff-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roff-0.2.0/setup.py` & `roff-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 import sys; sys.path.append('./src')  # noqa
 import setuptools
 from roff import __author__, __version__, __description__, __license__
 
 
 install_requires = ['markdown-it-py']
 
-all_requires = []
+images_requires = ['pillow']
+images_svg_requires = [*images_requires, 'cairosvg']
+all_requires = [images_requires, images_svg_requires]
 
 extras_require = {
-    # 'all': all_requires,
+    'images': all_requires,
+    'images-svg': all_requires,
+    'all': all_requires,
 }
 
 setuptools.setup(
     name="roff",
     version=__version__,
     description=__description__,
     long_description=open("README.md", "r", encoding="utf-8").read(),
@@ -55,9 +59,10 @@
     entry_points={
         "console_scripts": [
             "roff = roff.__main__:main"
         ]
     },
     data_files=[
         ("man/man1", ["docs/roff.1"]),
+        ("man/man5", ["docs/roff.5"]),
     ],
 )
```

### Comparing `roff-0.2.0/src/roff/__cli__/template.py` & `roff-0.3.0/src/roff/__cli__/template.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,28 +22,46 @@
 
     with open(dest, 'w') as f:
         f.write(fr"""{command}({manpage_area}) -- @DESCRIPTION
 =============================================
 
 ## SYNOPSIS
 
-- `{command} [-h]`
+- $`{command} [-h]`
 
 ## DESCRIPTION
 
 
 ## OPTIONS
 
 <!--
 ### `{command} <SUBCOMMAND>`
 -->
 
 * `-h`, `--help`:
 show the help message and exits
 
+## CONFIGURATION
+
+
+## ENVIRONMENT
+
+
+## FILES
+
+
+## VERSIONS
+
+
+## NOTES
+
+
+## EXAMPLE
+
+
 ## BUGS
 
 
 ## AUTHOR
 
 
 ## SEE ALSO
```

### Comparing `roff-0.2.0/src/roff/__init__.py` & `roff-0.3.0/src/roff/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 __copyright__ = "Copyright 2024, utility-toolbox"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "python-based cli to convert markdown to the roff (man-pages) format"
-__version_info__ = (0, 2, 0)
+__version_info__ = (0, 3, 0)
 __version__ = '.'.join(str(_) for _ in __version_info__)
```

### Comparing `roff-0.2.0/src/roff/__main__.py` & `roff-0.3.0/src/roff/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import argparse as ap
 from . import __version__, __cli__
 
 
 parser = ap.ArgumentParser(prog='roff', formatter_class=ap.ArgumentDefaultsHelpFormatter, description=__doc__)
 parser.set_defaults(__cmd__=parser.print_help)
 parser.add_argument('-v', '--version', action='version', version='{}'.format(__version__))
+parser.add_argument('--list-areas', action=__cli__.util.ActionListManpageAreas,
+                    help="Lists the manpage-areas")
 subparsers = parser.add_subparsers()
 
 
 convert_parser = subparsers.add_parser('convert',
-                                       help="Converts markdown to roff")
+                                       help="Converts markdown files to roff files")
 convert_parser.set_defaults(__cmd__=__cli__.convert.__cmd__)
 convert_parser.add_argument('source',
                             help="Markdown file that should be parsed")
 convert_parser.add_argument('dest', nargs=ap.OPTIONAL,
                             help="Manpage file that should be generated")
```

### Comparing `roff-0.2.0/src/roff/convert.py` & `roff-0.3.0/src/roff/convert.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,43 +4,58 @@
 """
 import os
 import io
 import re
 import textwrap
 import warnings
 import typing as t
+from pathlib import Path
 import markdown_it.tree
 from . import __version__
+from ._util import *
+from ._images import render_image
+from ._markdown import markdown_plugin_command
 
 
 __all__ = ['convert', 'Converter']
 
 
-def convert(source: str) -> str:
+def convert(fp: t.Union[str, os.PathLike]) -> str:
     r"""
     converts markdown to roff
 
-    :param source: markdown file content
+    :param fp: markdown file to convert
     :return: roff file content
     """
-    return Converter(source).getvalue()
+    return Converter(fp).getvalue()
 
 
 class Converter:
     _stream: io.StringIO
     _had_head: bool
+    _fp: Path
+    _root: Path
     manpage_area: int
 
-    def __init__(self, source: str) -> None:
+    width: int = int(os.getenv('ROFF_WIDTH', 80))
+    ascii: bool = os.getenv('ROFF_ASCII', "no").lower() in {"yes", "true", "1"}
+
+    def __init__(self, fp: t.Union[str, os.PathLike]) -> None:
         self._stream = io.StringIO()
         self._had_head = False
+        self._fp = Path(fp).absolute()
+        self._root = self._fp.parent
 
-        self.manpage_area = 1  # default. should be overwritten
+        self.manpage_area = 1  # default. should be overwritten while parsing
 
         parser = markdown_it.MarkdownIt()
+        parser.use(markdown_plugin_command)
+
+        with open(self._fp, 'r') as file:
+            source = file.read()
 
         tokens = parser.parse(src=source)
         root_node = markdown_it.tree.SyntaxTreeNode(tokens=tokens, create_root=True)
 
         self._add_head()
         # print(root_node.pretty(show_text=True))
         self._parse_children(children=root_node.children)
@@ -63,113 +78,178 @@
     def _parse_node(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         if not self._had_head and node.tag != 'h1':
             raise SyntaxError("First element in the document should be the header")
         parser = getattr(self, f"_parse_{node.tag}", None)
         if parser is None:
             warnings.warn(f"Unsupported node tag '{node.tag}' of type '{node.type}'", RuntimeWarning)
             return
-        parser(node=node)
+        parser(node)
 
-    def _parse_inline(self, node: markdown_it.tree.SyntaxTreeNode) -> str:
+    def _render_inline(self, node: markdown_it.tree.SyntaxTreeNode) -> str:
         chunks = []
 
         for child in node.children:
             if child.type == 'text':
                 chunks.append(escape(child.content))
             elif child.type == 'code_inline':
-                chunks.append(f'\\fB{child.content}\\fP')
+                chunks.append(f'\\fI{child.content}\\fP')
             elif child.type == 'strong':
-                chunks.append(f'\\fB{self._parse_inline(node=child)}\\fP')
+                chunks.append(f'\\fB{self._render_inline(node=child)}\\fP')
             elif child.type == 'em':
-                chunks.append(f'\\fI{self._parse_inline(node=child)}\\fR')
+                chunks.append(f'\\fI{self._render_inline(node=child)}\\fP')
             elif child.type == 'softbreak':
-                chunks.append('\n.br\n')
+                chunks.append(' ')
             elif child.type == 'hardbreak':
-                chunks.append('\n.br\n.br\n')
+                chunks.append('\n.br\n')
             elif child.type == 'link':
                 href = child.attrGet('href')
-                text = self._parse_inline(node=child)
+                text = self._render_inline(node=child)
                 if href == text:
                     chunks.append(escape(text))
                 else:
                     chunks.append(f'\n.UR {href}\n{escape(text)}\n.UE')
-            # elif child.type == 'image':
-            #     pass  # todo: `pip install roff[image]` with Pillow
+            elif child.type == 'image':
+                href = child.attrGet('src')
+                hyperref_re = re.compile(r'^\w+://')  # checks for http://, https://, data://, file://
+                if hyperref_re.match(href) is None:  # relative path to a file
+                    href = f'file://{self._root.joinpath(href).absolute()}'  # make it absolute to our root directory
+                braille = render_image(url=href, max_dimensions=(self.width, self.width * 3))
+                content = textwrap.indent(braille, '.br\n')  # ensure line-wraps
+                chunks.append(f'.sp\n{content}\n.sp\n')
+            elif child.type == 'command_inline':  # custom through plugin
+                chunks.append(self._render_inline_command(command=child.content))
             else:
                 warnings.warn(f"Unsupported inline node tag '{child.tag}' of type '{child.type}'", RuntimeWarning)
 
         return ''.join(chunks)
 
+    @staticmethod
+    def _render_inline_command(command: str) -> str:
+        command = command.strip()
+
+        def repl(match: re.Match) -> str:
+            head = match.group('head')
+            if head is not None:
+                return f'\\fB{escape(head)}\\fP'
+            argkey = match.group('argkey')
+            if argkey:
+                argvalue = match.group('argvalue')
+                if argvalue:
+                    return f'[\\fB{escape(argkey)}\\fP \\fI{escape(argvalue)}\\fP]'
+                else:
+                    return f'[\\fB{escape(argkey)}\\fP]'
+            argument = match.group()
+            if argument.startswith("-"):
+                return f'\\fB{escape(argument)}\\fP'
+            else:
+                return f'\\fI{escape(argument)}\\fP'
+
+        return re.sub(r'^(?P<head>\w+)|\[(?P<argkey>--?\w+)(?: (?P<argvalue>\w+))?]|(-{0,2}\w+)', repl, command)
+
     def _parse_h1(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         from datetime import date
 
         if self._had_head:
             raise SyntaxError("Duplicate Head detected")
         self._had_head = True
 
         head_re = re.compile(r'^(?P<command>\w+)\\?\((?P<manpage_area>\d)\\?\) \\?-\\?- (?P<description>.+)$')
-        content = self._parse_inline(node=node.children[0])
+        content = self._render_inline(node=node.children[0])
         match = head_re.search(content)
         if match is None:
             raise SyntaxError("Unsupported format of head. (expected 'command(1) -- description')")
 
         command = match.group('command')
         self.manpage_area = area = match.group('manpage_area')
 
         # Congratulations. This part is not documented.
         # You are probably here to hide this advertisement. Because I'm generous I'll make it easy for you
         ad_url = "" if os.getenv('ROFF_NO_ADD') == 'yes' else "github.com/utility-toolbox/roff"
         self._stream.write(f'.TH "{command.upper()}" "{area}" "{date.today():%d %B %Y}" "{ad_url}"\n')
         self._stream.write(f'.SH "NAME"\n')
-        self._stream.write(f'\\fB{command}\\fP \\- {match.group("description")}\n')
+        self._stream.write(f'\\fB{command}\\fP {"-" if self.ascii else "•"} {match.group("description")}\n')
 
     def _parse_h2(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
-        self._stream.write(f'.SH "{self._parse_inline(node=node.children[0])}"\n')
+        self._stream.write(f'.SH "{self._render_inline(node=node.children[0])}"\n')
 
     def _parse_h3(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
-        self._stream.write(f'.SS "{self._parse_inline(node=node.children[0])}"\n')
+        self._stream.write(f'.SS "{self._render_inline(node=node.children[0])}"\n')
 
     def _parse_h4(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
-        self._stream.write(f'.sp\n{self._parse_inline(node=node.children[0])}\n.br\n')
+        self._stream.write(f'.sp\n{self._render_inline(node=node.children[0])}\n.sp\n')
+
+    # maybe not the best solution
+    _parse_h5 = _parse_h4
+    _parse_h6 = _parse_h4
 
     def _parse_p(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
-        content = self._parse_inline(node=node.children[0])
-        if not content.strip():
-            return
-        content = re.sub(r'\n{2,}', '\n.\n', content)
+        content = self._render_inline(node=node.children[0])
+        content = re.sub(r'\n{2,}', '\n.sp\n', content)
+        # if node.level > 0:  # destroys the structure
+        #     self._stream.write('.P\n')
         self._stream.write(f'{content}\n')
 
+    def _check_inline_text_list(self, node: markdown_it.tree.SyntaxTreeNode) -> bool:
+        r""" Better do not touch this function. It's a mess. But at least it works """
+        assert node.tag in {'ul', 'ol'}
+        return all((
+            (len(li.children)  # any children
+             and li.children[0].type == 'paragraph'  # first is paragraph
+             and len(li.children[0].children) == 1  # with one child
+             and li.children[0].children[0].type == 'inline'  # which is inline
+             and '\n' not in self._render_inline(node=li.children[0].children[0]))  # and not over multiple lines
+            for li in node.children
+        ))
+
     def _parse_ul(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         r""" unordered list """
-        self._stream.write('.br\n')
-        for child in node.children:
-            self._stream.write(f'*\n.RS 2\n')
-            self._parse_children(children=child.children)
-            self._stream.write(f'.RE\n')
-        self._stream.write('.br\n')
+        deep = node.level > 0
+        self._stream.write('.br\n' if deep else '.sp\n')
+        bullet = '*' if self.ascii else '•'
+        if self._check_inline_text_list(node=node):
+            for list_item in node.children:
+                head, *body = list_item.children
+                self._stream.write(f'{bullet} {self._render_inline(head.children[0])}\n.br\n')
+                if body:
+                    self._stream.write('.RS 2\n')
+                    self._parse_children(children=body)
+                    self._stream.write('.RE\n')
+        else:
+            for list_item in node.children:
+                self._stream.write(f'{bullet}\n.RS 2\n')
+                self._parse_children(children=list_item.children)
+                self._stream.write(f'.RE\n')
+        self._stream.write('.br\n' if deep else '.sp\n')
 
     def _parse_ol(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         r""" ordered list """
-        self._stream.write('.br\n')
-        for i, child in enumerate(node.children):
-            self._stream.write(f'{i+1}.\n.RS 2\n')
-            self._parse_children(children=child.children)
-            self._stream.write(f'.RE\n')
-        self._stream.write('.br\n')
+        deep = node.level > 0
+        self._stream.write('.br\n' if deep else '.sp\n')
+        if self._check_inline_text_list(node=node):
+            for i, list_item in enumerate(node.children):
+                head, *body = list_item.children
+                self._stream.write(f'{i+1}. {self._render_inline(head.children[0])}\n.br\n')
+                if body:
+                    self._stream.write('.RS 2\n')
+                    self._parse_children(children=body)
+                    self._stream.write('.RE\n')
+        else:
+            for i, list_item in enumerate(node.children):
+                self._stream.write(f'{i+1}.\n.RS 2\n')
+                self._parse_children(children=list_item.children)
+                self._stream.write(f'.RE\n')
+        self._stream.write('.br\n' if deep else '.sp\n')
 
     def _parse_blockquote(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         self._stream.write(f'.sp\n.RS 2\n')
         self._parse_children(children=node.children)
         self._stream.write(f'.RE\n.sp\n')
 
     def _parse_code(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         content = re.sub(r'\n{2,}', '\n.sp\n', node.content.expandtabs(4).strip())
         content = textwrap.dedent(content)  # left-align
         content = textwrap.indent(content, prefix='.br\n')  # ensures newlines
-        self._stream.write(f'.sp\n.RS 2\n\\fI\n{content}\n\\fR\n.RE\n.sp\n')
-
+        self._stream.write(f'.sp\n.RS 2\n.EX\n\\fI\n{content}\n\\fP\n.EE\n.RE\n.sp\n')
 
-def escape(text: str, *, _escapes: str = '"\'.\\') -> str:
-    return text.translate(str.maketrans({
-        c: f"\\{c}"
-        for c in _escapes
-    }))
+    def _parse_hr(self, _node: markdown_it.tree.SyntaxTreeNode) -> None:
+        character = "-" if self.ascii else "━"
+        self._stream.write(f".sp\n{character * self.width}\n.sp\n")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

