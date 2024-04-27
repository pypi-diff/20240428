# Comparing `tmp/basic_data_structure-0.0.2.tar.gz` & `tmp/basic_data_structure-0.0.3.tar.gz`

## Comparing `basic_data_structure-0.0.2.tar` & `basic_data_structure-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/src/basic_data_structure/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/src/basic_data_structure/lists/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/src/basic_data_structure/lists/linked_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/src/basic_data_structure/trees/__init__.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/src/basic_data_structure/trees/binary_tree.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/LICENSE
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/README.md
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 basic_data_structure-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/lists/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/lists/linked_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/trees/__init__.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/src/basic_data_structure/trees/binary_tree.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/README.md
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 basic_data_structure-0.0.3/PKG-INFO
```

### Comparing `basic_data_structure-0.0.2/.github/workflows/pylint.yml` & `basic_data_structure-0.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `basic_data_structure-0.0.2/src/basic_data_structure/trees/binary_tree.py` & `basic_data_structure-0.0.3/src/basic_data_structure/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `basic_data_structure-0.0.2/LICENSE` & `basic_data_structure-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `basic_data_structure-0.0.2/README.md` & `basic_data_structure-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,53 +2,67 @@
 
 Implementation of basic sata structures in Python
 
 Including:
 1. Linked lists
 2. Binary trees
 
-Example for linked list:
+## Example for linked list
+
 ```python
 from basic_data_structure import ListNode
 
 
 def generate_list(size: int) -> ListNode | None:
+    """Generate linked list of N nodes.
+
+    0 → 1 → 2 → 3 → ... → N
+    """
     assert size >= 0
     dummy = ListNode(None)
     pointer = dummy
     for i in range(size):
         pointer.next = ListNode(i)
         pointer = pointer.next
     return dummy.next
 
 
 def print_list(head: ListNode | None) -> None:
-    print('[', end=' ')
     while head:
-        print(head.value, end=' ')
+        print(head.value, end=' → ' if head.next else '\n')
         head = head.next
-    print(']')
 
 
 def main() -> None:
     print_list(head=generate_list(5))
 
 
 if __name__ == '__main__':
     main()
 ```
 
-Example with binary tree:
+## Example for binary tree
+
 ```python
 from typing import Generator
 
 from basic_data_structure import TreeNode
 
 
 def generate_tree() -> TreeNode:
+    """Generate binary tree.
+
+                 8
+          ┌──────┴───────┐
+          4              12
+      ┌───┴───┐       ┌───┴───┐
+      2       6       10      14
+    ┌─┴─┐   ┌─┴─┐   ┌─┴─┐   ┌─┴─┐
+    1   3   5   7   9   11  13  15
+    """
     return TreeNode(
         8,
         left=TreeNode(
             4,
             left=TreeNode(
                 2,
                 left=TreeNode(1),
@@ -72,15 +86,15 @@
                 left=TreeNode(13),
                 right=TreeNode(15),
             ),
         ),
     )
 
 
-def dfs(root: TreeNode | None) -> Generator[str, None, None]:
+def dfs(root: TreeNode | None) -> Generator[int, None, None]:
     """Depth-first search."""
     if root:
         if root.left:
             yield from dfs(root.left)
 
         yield root.value
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `basic_data_structure-0.0.2/pyproject.toml` & `basic_data_structure-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "basic_data_structure"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mikhail Shagov", email="mishaga@me.com" },
 ]
 description = "Implementation of basic sata structures in Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/mishaga/struct"
-Issues = "https://github.com/mishaga/struct/issues"
+Homepage = "https://github.com/mishaga/basic_data_structure"
+Issues = "https://github.com/mishaga/basic_data_structure/issues"
 
 
 [tool.flake8]
 format = "wemake"
 max-complexity = "10"
 import-order-style = "pycharm"
 min-coverage-percents = "80"
```

### Comparing `basic_data_structure-0.0.2/PKG-INFO` & `basic_data_structure-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: basic_data_structure
-Version: 0.0.2
+Version: 0.0.3
 Summary: Implementation of basic sata structures in Python
-Project-URL: Homepage, https://github.com/mishaga/struct
-Project-URL: Issues, https://github.com/mishaga/struct/issues
+Project-URL: Homepage, https://github.com/mishaga/basic_data_structure
+Project-URL: Issues, https://github.com/mishaga/basic_data_structure/issues
 Author-email: Mikhail Shagov <mishaga@me.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -16,53 +16,67 @@
 
 Implementation of basic sata structures in Python
 
 Including:
 1. Linked lists
 2. Binary trees
 
-Example for linked list:
+## Example for linked list
+
 ```python
 from basic_data_structure import ListNode
 
 
 def generate_list(size: int) -> ListNode | None:
+    """Generate linked list of N nodes.
+
+    0 → 1 → 2 → 3 → ... → N
+    """
     assert size >= 0
     dummy = ListNode(None)
     pointer = dummy
     for i in range(size):
         pointer.next = ListNode(i)
         pointer = pointer.next
     return dummy.next
 
 
 def print_list(head: ListNode | None) -> None:
-    print('[', end=' ')
     while head:
-        print(head.value, end=' ')
+        print(head.value, end=' → ' if head.next else '\n')
         head = head.next
-    print(']')
 
 
 def main() -> None:
     print_list(head=generate_list(5))
 
 
 if __name__ == '__main__':
     main()
 ```
 
-Example with binary tree:
+## Example for binary tree
+
 ```python
 from typing import Generator
 
 from basic_data_structure import TreeNode
 
 
 def generate_tree() -> TreeNode:
+    """Generate binary tree.
+
+                 8
+          ┌──────┴───────┐
+          4              12
+      ┌───┴───┐       ┌───┴───┐
+      2       6       10      14
+    ┌─┴─┐   ┌─┴─┐   ┌─┴─┐   ┌─┴─┐
+    1   3   5   7   9   11  13  15
+    """
     return TreeNode(
         8,
         left=TreeNode(
             4,
             left=TreeNode(
                 2,
                 left=TreeNode(1),
@@ -86,15 +100,15 @@
                 left=TreeNode(13),
                 right=TreeNode(15),
             ),
         ),
     )
 
 
-def dfs(root: TreeNode | None) -> Generator[str, None, None]:
+def dfs(root: TreeNode | None) -> Generator[int, None, None]:
     """Depth-first search."""
     if root:
         if root.left:
             yield from dfs(root.left)
 
         yield root.value
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

