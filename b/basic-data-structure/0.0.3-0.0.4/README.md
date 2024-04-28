# Comparing `tmp/basic_data_structure-0.0.3.tar.gz` & `tmp/basic_data_structure-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "basic_data_structure-0.0.4.tar", max compression
```

## Comparing `basic_data_structure-0.0.3.tar` & `basic_data_structure-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/lists/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/lists/linked_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/trees/__init__.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/trees/binary_tree.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/LICENSE
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/README.md
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-28 08:59:59.054530 basic_data_structure-0.0.4/LICENSE
+-rw-r--r--   0        0        0      200 2024-04-28 12:46:15.312904 basic_data_structure-0.0.4/README.md
+-rw-r--r--   0        0        0      171 2024-04-28 12:26:39.411611 basic_data_structure-0.0.4/basic_data_structure/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-28 12:08:02.577734 basic_data_structure-0.0.4/basic_data_structure/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055304 basic_data_structure-0.0.4/basic_data_structure/lists/__init__.py
+-rw-r--r--   0        0        0      462 2024-04-28 12:07:08.784934 basic_data_structure-0.0.4/basic_data_structure/lists/linked_list.py
+-rw-r--r--   0        0        0        0 2024-04-28 10:54:44.865814 basic_data_structure-0.0.4/basic_data_structure/stack/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-28 12:23:43.893829 basic_data_structure-0.0.4/basic_data_structure/stack/stack.py
+-rw-r--r--   0        0        0        0 2024-04-28 08:59:59.055652 basic_data_structure-0.0.4/basic_data_structure/trees/__init__.py
+-rw-r--r--   0        0        0      611 2024-04-28 11:41:56.300001 basic_data_structure-0.0.4/basic_data_structure/trees/binary_tree.py
+-rw-r--r--   0        0        0     1546 2024-04-28 11:00:27.880165 basic_data_structure-0.0.4/examples/binary_tree.py
+-rw-r--r--   0        0        0      614 2024-04-28 11:00:27.880508 basic_data_structure-0.0.4/examples/linked_list.py
+-rw-r--r--   0        0        0      669 2024-04-28 12:09:03.807986 basic_data_structure-0.0.4/examples/stack.py
+-rw-r--r--   0        0        0     3052 2024-04-28 13:03:00.823024 basic_data_structure-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1009 1970-01-01 00:00:00.000000 basic_data_structure-0.0.4/PKG-INFO
```

### Comparing `basic_data_structure-0.0.3/src/basic_data_structure/trees/binary_tree.py` & `basic_data_structure-0.0.4/basic_data_structure/trees/binary_tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Any, Self
+from typing import Any, Optional
 
 
 class TreeNode:
     """A node of a binary tree."""
 
     def __init__(
         self,
         value: Any,  # noqa: WPS110 Found wrong variable name
-        left: Self | None = None,
-        right: Self | None = None,
+        left: Optional['TreeNode'] = None,
+        right: Optional['TreeNode'] = None,
     ) -> None:
         """Init a tree node.
 
         Parameters:
             value: a value of the node
             left: (optional) left child of the node
             right: (optional) right child of the node
```

### Comparing `basic_data_structure-0.0.3/LICENSE` & `basic_data_structure-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_data_structure-0.0.3/README.md` & `basic_data_structure-0.0.4/examples/binary_tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,7 @@
-# Basic Data Structure
-
-Implementation of basic sata structures in Python
-
-Including:
-1. Linked lists
-2. Binary trees
-
-## Example for linked list
-
-```python
-from basic_data_structure import ListNode
-
-
-def generate_list(size: int) -> ListNode | None:
-    """Generate linked list of N nodes.
-
-    0 → 1 → 2 → 3 → ... → N
-    """
-    assert size >= 0
-    dummy = ListNode(None)
-    pointer = dummy
-    for i in range(size):
-        pointer.next = ListNode(i)
-        pointer = pointer.next
-    return dummy.next
-
-
-def print_list(head: ListNode | None) -> None:
-    while head:
-        print(head.value, end=' → ' if head.next else '\n')
-        head = head.next
-
-
-def main() -> None:
-    print_list(head=generate_list(5))
-
-
-if __name__ == '__main__':
-    main()
-```
-
-## Example for binary tree
-
-```python
 from typing import Generator
 
 from basic_data_structure import TreeNode
 
 
 def generate_tree() -> TreeNode:
     """Generate binary tree.
@@ -106,8 +61,7 @@
     print('Depth-first search (DFS)')
     for data in dfs(root=generate_tree()):
         print(data, end=' ')
 
 
 if __name__ == '__main__':
     main()
-```
```

### Comparing `basic_data_structure-0.0.3/pyproject.toml` & `basic_data_structure-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-[project]
-name = "basic_data_structure"
-version = "0.0.3"
-authors = [
-  { name="Mikhail Shagov", email="mishaga@me.com" },
-]
+
+[tool.poetry]
+name = "basic-data-structure"
+version = "0.0.4"
 description = "Implementation of basic sata structures in Python"
+authors = ["Mikhail Shagov <mishaga@me.com>"]
 readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
+license = "MIT"
+homepage = "https://github.com/mishaga/basic_data_structure"
+repository = "https://github.com/mishaga/basic_data_structure"
+keywords = ["data structure", "data structures"]
+include = ["examples", "tests"]
+
+[tool.poetry.urls]
+"Issues" = "https://github.com/mishaga/basic_data_structure/issues"
+
+[tool.poetry.dependencies]
+python = "^3.9"
 
-[project.urls]
-Homepage = "https://github.com/mishaga/basic_data_structure"
-Issues = "https://github.com/mishaga/basic_data_structure/issues"
+[tool.poetry.group.dev.dependencies]
+wemake-python-styleguide = "^0.19.2"
+flake8-pyproject = "^1.2.3"
 
 
 [tool.flake8]
 format = "wemake"
 max-complexity = "10"
 import-order-style = "pycharm"
 min-coverage-percents = "80"
@@ -35,15 +39,15 @@
     "magic_method",
     "property_method",
     "static_method",
     "class_method",
     "method",
     "private_method",
 ]
-ignore = ["D100", "D104"]
+ignore = ["D100", "D104", "WPS112"]
 per-file-ignores = [
     "*/__init__.py: F401, WPS300, WPS412",
 ]
 # B001   – Do not use bare except
 # B008   – Do not perform function calls in argument defaults
 # D100   – Missing docstring in public module
 # D104   – Missing docstring in public package
@@ -53,14 +57,15 @@
 # DAR401 – Missing exception in Raises section
 # E722   – Do not use bare except
 # F401   – Imported but unused
 # E711   – comparison to None
 # N805   – first argument of a method should be named 'self'
 # S101   – Use of assert detected
 # WPS110 – Found wrong variable name
+# WPS112 – Found private name pattern
 # WPS115 – Found upper-case constant in a class
 # WPS201 – Found module with too many imports
 # WPS202 – Found too many module members
 # WPS204 – Found overused expression
 # WPS210 – Found too many local variables
 # WPS213 – Found too many expressions
 # WPS214 – Found too many methods
```

