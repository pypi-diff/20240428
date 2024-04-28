# Comparing `tmp/myst_parser-3.0.0.tar.gz` & `tmp/myst_parser-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myst_parser-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "myst_parser-3.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `myst_parser-3.0.0.tar` & `myst_parser-3.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1746 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/ISSUE_TEMPLATE/1-bug-report.yml
--rw-r--r--   0        0        0      834 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/ISSUE_TEMPLATE/2-feature-request.yml
--rw-r--r--   0        0        0      692 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/ISSUE_TEMPLATE/3-documentation.yml
--rw-r--r--   0        0        0      185 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      598 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/dependabot.yml
--rwxr-xr-x   0        0        0     1696 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/workflows/docutils_setup.py
--rw-r--r--   0        0        0     2219 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/workflows/test-formats.yml
--rw-r--r--   0        0        0     4590 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1860 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.gitignore
--rw-r--r--   0        0        0      896 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      234 2024-04-23 14:36:03.258124 myst_parser-3.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    43261 2024-04-23 14:36:03.258124 myst_parser-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2024-04-23 14:36:03.258124 myst_parser-3.0.0/LICENSE
--rw-r--r--   0        0        0     2703 2024-04-23 14:36:03.258124 myst_parser-3.0.0/README.md
--rw-r--r--   0        0        0      162 2024-04-23 14:36:03.258124 myst_parser-3.0.0/codecov.yml
--rw-r--r--   0        0        0       71 2024-04-23 14:36:03.262124 myst_parser-3.0.0/example-include.md
--rw-r--r--   0        0        0      479 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/__init__.py
--rw-r--r--   0        0        0      389 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/_compat.py
--rw-r--r--   0        0        0    13904 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/_docs.py
--rw-r--r--   0        0        0     1373 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/cli.py
--rw-r--r--   0        0        0       84 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/config/__init__.py
--rw-r--r--   0        0        0     5182 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/config/dc_validators.py
--rw-r--r--   0        0        0    19244 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/config/main.py
--rw-r--r--   0        0        0      246 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/docutils_.py
--rw-r--r--   0        0        0    16017 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/inventory.py
--rw-r--r--   0        0        0      302 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/mdit_to_docutils/__init__.py
--rw-r--r--   0        0        0    80773 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/mdit_to_docutils/base.py
--rw-r--r--   0        0        0     4451 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py
--rw-r--r--   0        0        0     9459 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/mdit_to_docutils/sphinx_.py
--rw-r--r--   0        0        0     5706 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/mdit_to_docutils/transforms.py
--rw-r--r--   0        0        0    22398 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/mocking.py
--rw-r--r--   0        0        0       60 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/parsers/__init__.py
--rw-r--r--   0        0        0    10854 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/parsers/directives.py
--rw-r--r--   0        0        0    16285 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/parsers/docutils_.py
--rw-r--r--   0        0        0     4744 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/parsers/mdit.py
--rw-r--r--   0        0        0    20982 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/parsers/options.py
--rw-r--r--   0        0        0    13703 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/parsers/parse_html.py
--rw-r--r--   0        0        0     2456 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/parsers/sphinx_.py
--rw-r--r--   0        0        0       26 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/py.typed
--rw-r--r--   0        0        0      257 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/sphinx_.py
--rw-r--r--   0        0        0       40 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/sphinx_ext/__init__.py
--rw-r--r--   0        0        0     4310 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/sphinx_ext/directives.py
--rw-r--r--   0        0        0     3384 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/sphinx_ext/main.py
--rw-r--r--   0        0        0     4745 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/sphinx_ext/mathjax.py
--rw-r--r--   0        0        0    15298 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/sphinx_ext/myst_refs.py
--rw-r--r--   0        0        0     4306 2024-04-23 14:36:03.262124 myst_parser-3.0.0/myst_parser/warnings_.py
--rw-r--r--   0        0        0     4023 2024-04-23 14:36:03.262124 myst_parser-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1390 2024-04-23 14:36:03.270124 myst_parser-3.0.0/tox.ini
--rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 myst_parser-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1746 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/ISSUE_TEMPLATE/1-bug-report.yml
+-rw-r--r--   0        0        0      834 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/ISSUE_TEMPLATE/2-feature-request.yml
+-rw-r--r--   0        0        0      692 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/ISSUE_TEMPLATE/3-documentation.yml
+-rw-r--r--   0        0        0      185 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      598 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     1696 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/workflows/docutils_setup.py
+-rw-r--r--   0        0        0     2219 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/workflows/test-formats.yml
+-rw-r--r--   0        0        0     4590 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1860 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.gitignore
+-rw-r--r--   0        0        0      896 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      234 2024-04-28 20:22:36.609521 myst_parser-3.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0    43607 2024-04-28 20:22:36.609521 myst_parser-3.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2024-04-28 20:22:36.609521 myst_parser-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2703 2024-04-28 20:22:36.609521 myst_parser-3.0.1/README.md
+-rw-r--r--   0        0        0      162 2024-04-28 20:22:36.609521 myst_parser-3.0.1/codecov.yml
+-rw-r--r--   0        0        0       71 2024-04-28 20:22:36.613521 myst_parser-3.0.1/example-include.md
+-rw-r--r--   0        0        0      479 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/_compat.py
+-rw-r--r--   0        0        0    13904 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/_docs.py
+-rw-r--r--   0        0        0     1373 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/cli.py
+-rw-r--r--   0        0        0       84 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/config/__init__.py
+-rw-r--r--   0        0        0     5182 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/config/dc_validators.py
+-rw-r--r--   0        0        0    19244 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/config/main.py
+-rw-r--r--   0        0        0      246 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/docutils_.py
+-rw-r--r--   0        0        0    16017 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/inventory.py
+-rw-r--r--   0        0        0      302 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/mdit_to_docutils/__init__.py
+-rw-r--r--   0        0        0    80773 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/mdit_to_docutils/base.py
+-rw-r--r--   0        0        0     4451 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/mdit_to_docutils/html_to_nodes.py
+-rw-r--r--   0        0        0     9459 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/mdit_to_docutils/sphinx_.py
+-rw-r--r--   0        0        0     5706 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/mdit_to_docutils/transforms.py
+-rw-r--r--   0        0        0    22398 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/mocking.py
+-rw-r--r--   0        0        0       60 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/parsers/__init__.py
+-rw-r--r--   0        0        0    10879 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/parsers/directives.py
+-rw-r--r--   0        0        0    16285 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/parsers/docutils_.py
+-rw-r--r--   0        0        0     4744 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/parsers/mdit.py
+-rw-r--r--   0        0        0    21058 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/parsers/options.py
+-rw-r--r--   0        0        0    13703 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/parsers/parse_html.py
+-rw-r--r--   0        0        0     2456 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/parsers/sphinx_.py
+-rw-r--r--   0        0        0       26 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/py.typed
+-rw-r--r--   0        0        0      257 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/sphinx_.py
+-rw-r--r--   0        0        0       40 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/sphinx_ext/__init__.py
+-rw-r--r--   0        0        0     4310 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/sphinx_ext/directives.py
+-rw-r--r--   0        0        0     3384 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/sphinx_ext/main.py
+-rw-r--r--   0        0        0     4745 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/sphinx_ext/mathjax.py
+-rw-r--r--   0        0        0    15298 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/sphinx_ext/myst_refs.py
+-rw-r--r--   0        0        0     4306 2024-04-28 20:22:36.613521 myst_parser-3.0.1/myst_parser/warnings_.py
+-rw-r--r--   0        0        0     4023 2024-04-28 20:22:36.613521 myst_parser-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1390 2024-04-28 20:22:36.625521 myst_parser-3.0.1/tox.ini
+-rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 myst_parser-3.0.1/PKG-INFO
```

### Comparing `myst_parser-3.0.0/.github/ISSUE_TEMPLATE/1-bug-report.yml` & `myst_parser-3.0.1/.github/ISSUE_TEMPLATE/1-bug-report.yml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.github/ISSUE_TEMPLATE/2-feature-request.yml` & `myst_parser-3.0.1/.github/ISSUE_TEMPLATE/2-feature-request.yml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.github/ISSUE_TEMPLATE/3-documentation.yml` & `myst_parser-3.0.1/.github/ISSUE_TEMPLATE/3-documentation.yml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.github/dependabot.yml` & `myst_parser-3.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.github/workflows/docutils_setup.py` & `myst_parser-3.0.1/.github/workflows/docutils_setup.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.github/workflows/test-formats.yml` & `myst_parser-3.0.1/.github/workflows/test-formats.yml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.github/workflows/tests.yml` & `myst_parser-3.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.gitignore` & `myst_parser-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/.pre-commit-config.yaml` & `myst_parser-3.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/CHANGELOG.md` & `myst_parser-3.0.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## 3.0.1 - 2024-04-28
+
+### 🐛 Bug Fixes
+
+- Account for the final directive option having an empty value, by <gh-user:chrisjsewell> in <gh-pr:924>
+- Re-allow indented directive option blocks, by <gh-user:chrisjsewell> in <gh-pr:925>
+
+**Full Changelog**: [v3.0.1...v3.0.0](https://github.com/executablebooks/MyST-Parser/compare/v3.0.1...v3.0.0)
+
 ## 3.0.0 - 2024-04-23
 
 ### Upgraded dependencies
 
 - ⬆️ Add support for Python 3.12 by <gh-user:hugovk> in <gh-pr:848>
 - ⬆️ Update docutils requirement from >=0.16,<0.21 to >=0.18,<0.22 by <gh-user:chrisjsewell> in <gh-pr:916>
```

### Comparing `myst_parser-3.0.0/LICENSE` & `myst_parser-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/README.md` & `myst_parser-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/_docs.py` & `myst_parser-3.0.1/myst_parser/_docs.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/cli.py` & `myst_parser-3.0.1/myst_parser/cli.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/config/dc_validators.py` & `myst_parser-3.0.1/myst_parser/config/dc_validators.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/config/main.py` & `myst_parser-3.0.1/myst_parser/config/main.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/inventory.py` & `myst_parser-3.0.1/myst_parser/inventory.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/mdit_to_docutils/base.py` & `myst_parser-3.0.1/myst_parser/mdit_to_docutils/base.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py` & `myst_parser-3.0.1/myst_parser/mdit_to_docutils/html_to_nodes.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/mdit_to_docutils/sphinx_.py` & `myst_parser-3.0.1/myst_parser/mdit_to_docutils/sphinx_.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/mdit_to_docutils/transforms.py` & `myst_parser-3.0.1/myst_parser/mdit_to_docutils/transforms.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/mocking.py` & `myst_parser-3.0.1/myst_parser/mocking.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/parsers/directives.py` & `myst_parser-3.0.1/myst_parser/parsers/directives.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 from docutils.parsers.rst import Directive
 from docutils.parsers.rst.directives import flag
 from docutils.parsers.rst.directives.misc import TestDirective
 from docutils.parsers.rst.states import MarkupError
 
 from myst_parser.warnings_ import MystWarnings
 
-from .options import TokenizeError
-from .options import to_items as options_to_items
+from .options import TokenizeError, options_to_items
 
 
 @dataclass
 class ParseWarnings:
     msg: str
     lineno: int | None = None
     type: MystWarnings = MystWarnings.DIRECTIVE_PARSING
@@ -172,42 +171,42 @@
     line: int | None,
     additional_options: dict[str, str] | None = None,
 ) -> _DirectiveOptions:
     """Parse (and validate) the directive option section.
 
     :returns: (content, options, validation_errors)
     """
-    yaml_block: None | str = None
+    options_block: None | str = None
     if content.startswith("---"):
         line = None if line is None else line + 1
         content = "\n".join(content.splitlines()[1:])
         match = re.search(r"^-{3,}", content, re.MULTILINE)
         if match:
-            yaml_block = content[: match.start()]
+            options_block = content[: match.start()]
             content = content[match.end() + 1 :]  # TODO advance line number
         else:
-            yaml_block = content
+            options_block = content
             content = ""
-        yaml_block = dedent(yaml_block)
-    elif content.startswith(":"):
+        options_block = dedent(options_block)
+    elif content.lstrip().startswith(":"):
         content_lines = content.splitlines()
         yaml_lines = []
         while content_lines:
-            if not content_lines[0].startswith(":"):
+            if not content_lines[0].lstrip().startswith(":"):
                 break
-            yaml_lines.append(content_lines.pop(0)[1:])
-        yaml_block = "\n".join(yaml_lines)
+            yaml_lines.append(content_lines.pop(0).lstrip()[1:])
+        options_block = "\n".join(yaml_lines)
         content = "\n".join(content_lines)
 
-    has_options_block = yaml_block is not None
+    has_options_block = options_block is not None
 
     if as_yaml:
         yaml_errors: list[ParseWarnings] = []
         try:
-            yaml_options = yaml.safe_load(yaml_block or "") or {}
+            yaml_options = yaml.safe_load(options_block or "") or {}
         except (yaml.parser.ParserError, yaml.scanner.ScannerError):
             yaml_options = {}
             yaml_errors.append(
                 ParseWarnings(
                     "Invalid options format (bad YAML)",
                     line,
                     MystWarnings.DIRECTIVE_OPTION,
@@ -223,17 +222,17 @@
                 )
             )
         return _DirectiveOptions(content, yaml_options, yaml_errors, has_options_block)
 
     validation_errors: list[ParseWarnings] = []
 
     options: dict[str, str] = {}
-    if yaml_block is not None:
+    if options_block is not None:
         try:
-            _options, state = options_to_items(yaml_block)
+            _options, state = options_to_items(options_block)
             options = dict(_options)
         except TokenizeError as err:
             return _DirectiveOptions(
                 content,
                 options,
                 [
                     ParseWarnings(
```

### Comparing `myst_parser-3.0.0/myst_parser/parsers/docutils_.py` & `myst_parser-3.0.1/myst_parser/parsers/docutils_.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/parsers/mdit.py` & `myst_parser-3.0.1/myst_parser/parsers/mdit.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/parsers/options.py` & `myst_parser-3.0.1/myst_parser/parsers/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
 
 @dataclass
 class State:
     has_comments: bool = False
 
 
-def to_items(
+def options_to_items(
     text: str, line_offset: int = 0, column_offset: int = 0
 ) -> tuple[list[tuple[str, str]], State]:
     """Parse a directive option block into (key, value) tuples.
 
     :param text: The directive option text.
     :param line_offset: The line offset to apply to the error positions.
     :param column_offset: The column offset to apply to the error positions.
@@ -207,14 +207,16 @@
                     yield key_token, None
                 key_token = token
             elif isinstance(token, ValueToken):
                 if key_token is None:
                     raise TokenizeError("expected key before value", token.start)
                 yield key_token, token
                 key_token = None
+        if key_token is not None:
+            yield key_token, None
     except TokenizeError as exc:
         if line_offset or column_offset:
             raise exc.clone(line_offset, column_offset) from exc
         raise
 
 
 def _tokenize(text: str, state: State) -> Iterable[Token]:
```

### Comparing `myst_parser-3.0.0/myst_parser/parsers/parse_html.py` & `myst_parser-3.0.1/myst_parser/parsers/parse_html.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/parsers/sphinx_.py` & `myst_parser-3.0.1/myst_parser/parsers/sphinx_.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/sphinx_ext/directives.py` & `myst_parser-3.0.1/myst_parser/sphinx_ext/directives.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/sphinx_ext/main.py` & `myst_parser-3.0.1/myst_parser/sphinx_ext/main.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/sphinx_ext/mathjax.py` & `myst_parser-3.0.1/myst_parser/sphinx_ext/mathjax.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/sphinx_ext/myst_refs.py` & `myst_parser-3.0.1/myst_parser/sphinx_ext/myst_refs.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/myst_parser/warnings_.py` & `myst_parser-3.0.1/myst_parser/warnings_.py`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/pyproject.toml` & `myst_parser-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/tox.ini` & `myst_parser-3.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `myst_parser-3.0.0/PKG-INFO` & `myst_parser-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myst-parser
-Version: 3.0.0
+Version: 3.0.1
 Summary: An extended [CommonMark](https://spec.commonmark.org/) compliant parser,
 Keywords: markdown,lexer,parser,development,docutils,sphinx
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
```

