# Comparing `tmp/jupyter-duckdb-0.9.2.5.tar.gz` & `tmp/jupyter-duckdb-0.9.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-duckdb-0.9.2.5.tar", last modified: Tue Jan 23 15:33:23 2024, max compression
+gzip compressed data, was "jupyter-duckdb-0.9.2.6.tar", last modified: Mon Jan 29 12:38:06 2024, max compression
```

## Comparing `jupyter-duckdb-0.9.2.5.tar` & `jupyter-duckdb-0.9.2.6.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.609109 jupyter-duckdb-0.9.2.5/
--rw-r--r--   0 root         (0) root         (0)     7746 2024-01-23 15:33:23.609109 jupyter-duckdb-0.9.2.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     7121 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-23 15:33:23.609109 jupyter-duckdb-0.9.2.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1520 2024-01-22 16:56:16.000000 jupyter-duckdb-0.9.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.593108 jupyter-duckdb-0.9.2.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.593108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      165 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.597108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/Column.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/Connection.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/Constraint.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/DatabaseError.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/ForeignKey.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/Table.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.597108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/error/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/error/EmptyResultError.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/error/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.593108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.597108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/duckdb/
--rw-rw-rw-   0 root         (0) root         (0)     6086 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/duckdb/Connection.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/duckdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.597108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/postgres/
--rw-rw-rw-   0 root         (0) root         (0)     8738 2024-01-23 15:16:01.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/postgres/Connection.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/postgres/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-01-23 15:16:01.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/postgres/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.597108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/sqlite/
--rw-rw-rw-   0 root         (0) root         (0)     6822 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/sqlite/Connection.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/sqlite/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      127 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/kernel.json
--rwxrwxrwx   0 root         (0) root         (0)    18666 2024-01-23 15:16:01.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/kernel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.597108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/
--rwxrwxrwx   0 root         (0) root         (0)     2346 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/MagicCommand.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/MagicCommandCallback.py
--rwxrwxrwx   0 root         (0) root         (0)       49 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/MagicCommandException.py
--rwxrwxrwx   0 root         (0) root         (0)     2743 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/MagicCommandHandler.py
--rwxrwxrwx   0 root         (0) root         (0)      204 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.597108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/DCParser.py
--rw-rw-rw-   0 root         (0) root         (0)     1137 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/LogicParser.py
--rw-rw-rw-   0 root         (0) root         (0)     2891 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/RAParser.py
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.601108 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/DCOperand.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/LogicElement.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/LogicOperand.py
--rw-rw-rw-   0 root         (0) root         (0)     1028 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/LogicOperator.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RABinaryOperator.py
--rw-rw-rw-   0 root         (0) root         (0)     1468 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RAElement.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RAOperand.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RAOperator.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RAUnaryOperator.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.605109 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Add.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/And.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/ArrowLeft.py
--rw-rw-rw-   0 root         (0) root         (0)    16649 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/ConditionalSet.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Cross.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Difference.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Divide.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Equal.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/GreaterThan.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/GreaterThanEqual.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Intersection.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Join.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/LessThan.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/LessThanEqual.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Minus.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Multiply.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Or.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Unequal.py
--rw-rw-rw-   0 root         (0) root         (0)      739 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Union.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.605109 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Not.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Projection.py
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Rename.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Selection.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.605109 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/tokenizer/
--rw-rw-rw-   0 root         (0) root         (0)     1800 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/tokenizer/Token.py
--rw-rw-rw-   0 root         (0) root         (0)     5081 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/tokenizer/Tokenizer.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/tokenizer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.605109 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/util/
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/util/RenamableColumn.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/util/RenamableColumnList.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-23 15:33:13.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.605109 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/util/
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/util/ResultSetComparator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-23 15:33:13.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/util/formatting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.609109 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/visualization/
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/visualization/Drawer.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/visualization/RATreeDrawer.py
--rw-rw-rw-   0 root         (0) root         (0)     2955 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/visualization/SchemaDrawer.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/src/duckdb_kernel/visualization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.609109 jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7746 2024-01-23 15:33:23.000000 jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3886 2024-01-23 15:33:23.000000 jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-23 15:33:23.000000 jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-01-23 15:33:23.000000 jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-01-23 15:33:23.000000 jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 15:33:23.609109 jupyter-duckdb-0.9.2.5/test/
--rw-rw-rw-   0 root         (0) root         (0)     8482 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/test/test_dc.py
--rw-rw-rw-   0 root         (0) root         (0)    22790 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/test/test_ra.py
--rw-rw-rw-   0 root         (0) root         (0)     3859 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.5/test/test_result_comparison.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.426815 jupyter-duckdb-0.9.2.6/
+-rw-r--r--   0 root         (0) root         (0)     7762 2024-01-29 12:38:06.426815 jupyter-duckdb-0.9.2.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     7137 2024-01-29 08:28:33.000000 jupyter-duckdb-0.9.2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-29 12:38:06.426815 jupyter-duckdb-0.9.2.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1520 2024-01-22 16:56:16.000000 jupyter-duckdb-0.9.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.394815 jupyter-duckdb-0.9.2.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.398815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      165 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.398815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/Connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/Constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/DatabaseError.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/ForeignKey.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/Table.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.398815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/error/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/error/EmptyResultError.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/error/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.394815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.402815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/duckdb/
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/duckdb/Connection.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/duckdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.402815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/postgres/
+-rw-rw-rw-   0 root         (0) root         (0)     8738 2024-01-23 15:16:01.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/postgres/Connection.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/postgres/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-01-23 15:16:01.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/postgres/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.402815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/sqlite/
+-rw-rw-rw-   0 root         (0) root         (0)     6822 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/sqlite/Connection.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/sqlite/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      127 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/kernel.json
+-rwxrwxrwx   0 root         (0) root         (0)    18666 2024-01-23 15:16:01.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/kernel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.402815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/
+-rwxrwxrwx   0 root         (0) root         (0)     2346 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/MagicCommand.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/MagicCommandCallback.py
+-rwxrwxrwx   0 root         (0) root         (0)       49 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/MagicCommandException.py
+-rwxrwxrwx   0 root         (0) root         (0)     2743 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/MagicCommandHandler.py
+-rwxrwxrwx   0 root         (0) root         (0)      204 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.406815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/DCParser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/LogicParser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/RAParser.py
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.410815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/DCOperand.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/LogicElement.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/LogicOperand.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/LogicOperator.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RABinaryOperator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RAElement.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RAOperand.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RAOperator.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RAUnaryOperator.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.414815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Add.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/And.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/ArrowLeft.py
+-rw-rw-rw-   0 root         (0) root         (0)    16649 2024-01-22 10:36:06.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/ConditionalSet.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Cross.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2024-01-29 08:26:38.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Difference.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Divide.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2024-01-29 08:26:38.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Division.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Equal.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/GreaterThan.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/GreaterThanEqual.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Intersection.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Join.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/LessThan.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/LessThanEqual.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Minus.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Multiply.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Or.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Unequal.py
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Union.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2024-01-29 08:26:38.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.418815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Not.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Projection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Rename.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Selection.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.418815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/tokenizer/
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/tokenizer/Token.py
+-rw-rw-rw-   0 root         (0) root         (0)     5081 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/tokenizer/Tokenizer.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/tokenizer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.418815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/util/
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/util/RenamableColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3015 2024-01-29 08:26:38.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/util/RenamableColumnList.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:37:53.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.422815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/util/
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/util/ResultSetComparator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:37:53.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/util/formatting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.422815 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/visualization/Drawer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/visualization/RATreeDrawer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2955 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/visualization/SchemaDrawer.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/src/duckdb_kernel/visualization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.426815 jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7762 2024-01-29 12:38:06.000000 jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3939 2024-01-29 12:38:06.000000 jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-29 12:38:06.000000 jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-01-29 12:38:06.000000 jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-01-29 12:38:06.000000 jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 12:38:06.426815 jupyter-duckdb-0.9.2.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)     8482 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/test/test_dc.py
+-rw-rw-rw-   0 root         (0) root         (0)    27284 2024-01-29 08:26:38.000000 jupyter-duckdb-0.9.2.6/test/test_ra.py
+-rw-rw-rw-   0 root         (0) root         (0)     3859 2024-01-19 16:56:08.000000 jupyter-duckdb-0.9.2.6/test/test_result_comparison.py
```

### Comparing `jupyter-duckdb-0.9.2.5/PKG-INFO` & `jupyter-duckdb-0.9.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-duckdb
-Version: 0.9.2.5
+Version: 0.9.2.6
 Summary: a basic wrapper kernel for DuckDB
 Home-page: https://github.com/erictroebs/jupyter-duckdb
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Project-URL: Bug Tracker, https://github.com/erictroebs/jupyter-duckdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -243,14 +243,15 @@
 - Selection `σ`
 - Rename `β`
 - Union `∪`
 - Intersection `∩`
 - Difference `\`
 - Natural Join `⋈`
 - Cross Product `×`
+- Division `÷`
 
 The Dockerfile also installs the Jupyter Lab plugin
 [jupyter-ra-extension](https://pypi.org/project/jupyter-ra-extension/). It adds
 the symbols mentioned above and some other supported symbols to the toolbar for
 insertion on click.
 
 ### Domain Calculus
```

### Comparing `jupyter-duckdb-0.9.2.5/README.md` & `jupyter-duckdb-0.9.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
 - Selection `σ`
 - Rename `β`
 - Union `∪`
 - Intersection `∩`
 - Difference `\`
 - Natural Join `⋈`
 - Cross Product `×`
+- Division `÷`
 
 The Dockerfile also installs the Jupyter Lab plugin
 [jupyter-ra-extension](https://pypi.org/project/jupyter-ra-extension/). It adds
 the symbols mentioned above and some other supported symbols to the toolbar for
 insertion on click.
 
 ### Domain Calculus
```

### Comparing `jupyter-duckdb-0.9.2.5/setup.py` & `jupyter-duckdb-0.9.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/Column.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/Column.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/Connection.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/Connection.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/Table.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/Table.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/duckdb/Connection.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/duckdb/Connection.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/postgres/Connection.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/postgres/Connection.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/db/implementation/sqlite/Connection.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/db/implementation/sqlite/Connection.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/kernel.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/MagicCommand.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/MagicCommand.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/MagicCommandCallback.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/MagicCommandCallback.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/magics/MagicCommandHandler.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/magics/MagicCommandHandler.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/DCParser.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/DCParser.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/LogicParser.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/LogicParser.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/RAParser.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/RAParser.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/DCOperand.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/DCOperand.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/LogicOperand.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/LogicOperand.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/LogicOperator.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/LogicOperator.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RABinaryOperator.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RABinaryOperator.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RAElement.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RAElement.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RAOperand.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RAOperand.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/RAUnaryOperator.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/RAUnaryOperator.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/__init__.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/ConditionalSet.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/ConditionalSet.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Cross.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Cross.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Difference.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,11 @@
     def to_sql(self, tables: Dict[str, Table]) -> Tuple[str, RenamableColumnList]:
         # execute subqueries
         lq, lcols = self.left.to_sql(tables)
         rq, rcols = self.right.to_sql(tables)
 
         # check number of columns
         if len(lcols) != len(rcols):
-            raise AssertionError(f'difference can only be applied to relations with the same number of columns')
+            raise AssertionError('difference can only be applied to relations with the same number of columns')
 
         # create sql
         return f'{lq} EXCEPT {rq}', lcols
```

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Intersection.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Intersection.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Join.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Join.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/Union.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/Union.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/binary/__init__.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/binary/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .Union import Union
 
 from .Add import Add
 from .And import And
 from .ArrowLeft import ArrowLeft
 from .ConditionalSet import ConditionalSet
 from .Divide import Divide
+from .Division import Division
 from .Equal import Equal
 from .GreaterThan import GreaterThan
 from .GreaterThanEqual import GreaterThanEqual
 from .LessThan import LessThan
 from .LessThanEqual import LessThanEqual
 from .Minus import Minus
 from .Multiply import Multiply
@@ -29,11 +30,12 @@
 ], key=lambda x: x.order, reverse=True)
 
 RA_BINARY_OPERATORS = [
     Difference,
     Union,
     Intersection,
     Join,
-    Cross
+    Cross,
+    Division
 ]
 
 DC_SET = ConditionalSet
```

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Not.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Not.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Projection.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Projection.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Rename.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Rename.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/elements/unary/Selection.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/elements/unary/Selection.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/tokenizer/Token.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/tokenizer/Token.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/tokenizer/Tokenizer.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/tokenizer/Tokenizer.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/util/RenamableColumn.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/util/RenamableColumn.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/parser/util/RenamableColumnList.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/parser/util/RenamableColumnList.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,14 +57,26 @@
             if col.full_name in cols:
                 raise AssertionError(f'column {col.full_name} present in both relations')
 
             cols[col.full_name] = col
 
         return RenamableColumnList(cols.values())
 
+    def difference(self, other: 'RenamableColumnList') -> 'RenamableColumnList':
+        cols: Dict[str, RenamableColumn] = {}
+
+        for col in self:
+            cols[col.name] = col
+
+        for col in other:
+            if col.name in cols:
+                del cols[col.name]
+
+        return RenamableColumnList(cols.values())
+
     def intersect(self, other: 'RenamableColumnList') \
             -> Tuple[List[Tuple[RenamableColumn, RenamableColumn]], 'RenamableColumnList']:
         self_cols: Dict[str, RenamableColumn] = {col.name: col for col in self}
         other_cols: Dict[str, RenamableColumn] = {col.name: col for col in other}
 
         intersection: List[Tuple[RenamableColumn, RenamableColumn]] = []
         for name in tuple(self_cols.keys()):
```

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/util/ResultSetComparator.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/util/ResultSetComparator.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/util/formatting.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/util/formatting.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/visualization/RATreeDrawer.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/visualization/RATreeDrawer.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/duckdb_kernel/visualization/SchemaDrawer.py` & `jupyter-duckdb-0.9.2.6/src/duckdb_kernel/visualization/SchemaDrawer.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/PKG-INFO` & `jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-duckdb
-Version: 0.9.2.5
+Version: 0.9.2.6
 Summary: a basic wrapper kernel for DuckDB
 Home-page: https://github.com/erictroebs/jupyter-duckdb
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Project-URL: Bug Tracker, https://github.com/erictroebs/jupyter-duckdb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -243,14 +243,15 @@
 - Selection `σ`
 - Rename `β`
 - Union `∪`
 - Intersection `∩`
 - Difference `\`
 - Natural Join `⋈`
 - Cross Product `×`
+- Division `÷`
 
 The Dockerfile also installs the Jupyter Lab plugin
 [jupyter-ra-extension](https://pypi.org/project/jupyter-ra-extension/). It adds
 the symbols mentioned above and some other supported symbols to the toolbar for
 insertion on click.
 
 ### Domain Calculus
```

### Comparing `jupyter-duckdb-0.9.2.5/src/jupyter_duckdb.egg-info/SOURCES.txt` & `jupyter-duckdb-0.9.2.6/src/jupyter_duckdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/duckdb_kernel/parser/elements/binary/Add.py
 src/duckdb_kernel/parser/elements/binary/And.py
 src/duckdb_kernel/parser/elements/binary/ArrowLeft.py
 src/duckdb_kernel/parser/elements/binary/ConditionalSet.py
 src/duckdb_kernel/parser/elements/binary/Cross.py
 src/duckdb_kernel/parser/elements/binary/Difference.py
 src/duckdb_kernel/parser/elements/binary/Divide.py
+src/duckdb_kernel/parser/elements/binary/Division.py
 src/duckdb_kernel/parser/elements/binary/Equal.py
 src/duckdb_kernel/parser/elements/binary/GreaterThan.py
 src/duckdb_kernel/parser/elements/binary/GreaterThanEqual.py
 src/duckdb_kernel/parser/elements/binary/Intersection.py
 src/duckdb_kernel/parser/elements/binary/Join.py
 src/duckdb_kernel/parser/elements/binary/LessThan.py
 src/duckdb_kernel/parser/elements/binary/LessThanEqual.py
```

### Comparing `jupyter-duckdb-0.9.2.5/test/test_dc.py` & `jupyter-duckdb-0.9.2.6/test/test_dc.py`

 * *Files identical despite different names*

### Comparing `jupyter-duckdb-0.9.2.5/test/test_ra.py` & `jupyter-duckdb-0.9.2.6/test/test_ra.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from duckdb_kernel.parser import RAParser
 from duckdb_kernel.parser.elements import RAOperand, LogicElement
 from . import Connection
 
 
 def test_case_insensitivity():
     for query in (
-        'users',
-        'Users',
-        'USERS',
-        'userS'
+            'users',
+            'Users',
+            'USERS',
+            'userS'
     ):
         root = RAParser.parse_query(query)
 
         # root is an RAOperand
         assert isinstance(root, RAOperand)
 
         # Root's name is the relation name in whatever case
@@ -68,14 +68,35 @@
         with Connection() as con:
             assert con.execute_ra(root) == [
                 (1, 'Alice'),
                 (3, 'Charlie')
             ]
 
 
+def test_binary_operator_division():
+    for query in (
+            r'π [show_id, season_number, episode_number] (episodes) ÷ π [ episode_number ] (σ [ show_id = 1 AND season_number = 1 ] (episodes))',
+            r'π [show_id, season_number, episode_number] (episodes) : π [ episode_number ] (σ [ show_id = 1 AND season_number = 1 ] (episodes))',
+    ):
+        root = RAParser.parse_query(query)
+
+        assert isinstance(root, BinaryOperators.Division)
+        assert isinstance(root.left, UnaryOperators.Projection)
+        assert isinstance(root.left.target, RAOperand) and root.left.target.name == 'episodes'
+        assert isinstance(root.right, UnaryOperators.Projection)
+        assert isinstance(root.right.target, UnaryOperators.Selection)
+        assert isinstance(root.right.target.target, RAOperand) and root.right.target.target.name == 'episodes'
+
+        with Connection() as con:
+            assert con.execute_ra(root) == [
+                (1, 1),
+                (1, 2)
+            ]
+
+
 def test_binary_operator_intersection():
     for query in (
             r'users ∩ banned_users',
             r'users cap banned_users'
     ):
         root = RAParser.parse_query(query)
 
@@ -321,14 +342,23 @@
     assert isinstance(root, BinaryOperators.Difference)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Cross)
 
     root = RAParser.parse_query(r'a x b \ c')
     assert isinstance(root, BinaryOperators.Difference)
     assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Cross)
 
+    # difference <-> division
+    root = RAParser.parse_query(r'a \ b ÷ c')
+    assert isinstance(root, BinaryOperators.Difference)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Division)
+
+    root = RAParser.parse_query(r'a ÷ b \ c')
+    assert isinstance(root, BinaryOperators.Difference)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Division)
+
     # union <-> intersection
     root = RAParser.parse_query(r'a ∪ b ∩ c')
     assert isinstance(root, BinaryOperators.Union)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Intersection)
 
     root = RAParser.parse_query(r'a ∩ b ∪ c')
     assert isinstance(root, BinaryOperators.Union)
@@ -348,14 +378,23 @@
     assert isinstance(root, BinaryOperators.Union)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Cross)
 
     root = RAParser.parse_query(r'a x b ∪ c')
     assert isinstance(root, BinaryOperators.Union)
     assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Cross)
 
+    # union <-> division
+    root = RAParser.parse_query(r'a ∪ b ÷ c')
+    assert isinstance(root, BinaryOperators.Union)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Division)
+
+    root = RAParser.parse_query(r'a ÷ b ∪ c')
+    assert isinstance(root, BinaryOperators.Union)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Division)
+
     # intersection <-> join
     root = RAParser.parse_query(r'a ∩ b ⋈ c')
     assert isinstance(root, BinaryOperators.Intersection)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Join)
 
     root = RAParser.parse_query(r'a ⋈ b ∩ c')
     assert isinstance(root, BinaryOperators.Intersection)
@@ -366,23 +405,50 @@
     assert isinstance(root, BinaryOperators.Intersection)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Cross)
 
     root = RAParser.parse_query(r'a x b ∩ c')
     assert isinstance(root, BinaryOperators.Intersection)
     assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Cross)
 
+    # intersection <-> division
+    root = RAParser.parse_query(r'a ∩ b ÷ c')
+    assert isinstance(root, BinaryOperators.Intersection)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Division)
+
+    root = RAParser.parse_query(r'a ÷ b ∩ c')
+    assert isinstance(root, BinaryOperators.Intersection)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Division)
+
     # join <-> cross
     root = RAParser.parse_query(r'a ⋈ b x c')
     assert isinstance(root, BinaryOperators.Join)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Cross)
 
     root = RAParser.parse_query(r'a x b ⋈ c')
     assert isinstance(root, BinaryOperators.Join)
     assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Cross)
 
+    # join <-> division
+    root = RAParser.parse_query(r'a ⋈ b ÷ c')
+    assert isinstance(root, BinaryOperators.Join)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Division)
+
+    root = RAParser.parse_query(r'a ÷ b ⋈ c')
+    assert isinstance(root, BinaryOperators.Join)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Division)
+
+    # cross <-> division
+    root = RAParser.parse_query(r'a x b ÷ c')
+    assert isinstance(root, BinaryOperators.Cross)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, BinaryOperators.Division)
+
+    root = RAParser.parse_query(r'a ÷ b x c')
+    assert isinstance(root, BinaryOperators.Cross)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, BinaryOperators.Division)
+
 
 def test_mixed_evaluation_order():
     # difference <-> projection
     root = RAParser.parse_query(r'a \ π [ id ] b')
     assert isinstance(root, BinaryOperators.Difference)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, UnaryOperators.Projection)
 
@@ -512,14 +578,41 @@
     assert isinstance(root, BinaryOperators.Cross)
     assert isinstance(root.left, RAOperand) and isinstance(root.right, UnaryOperators.Selection)
 
     root = RAParser.parse_query(r'σ [ id > 1 ] a x b')
     assert isinstance(root, BinaryOperators.Cross)
     assert isinstance(root.right, RAOperand) and isinstance(root.left, UnaryOperators.Selection)
 
+    # division <-> projection
+    root = RAParser.parse_query(r'a ÷ π [ id ] b')
+    assert isinstance(root, BinaryOperators.Division)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, UnaryOperators.Projection)
+
+    root = RAParser.parse_query(r'π [ id ] a ÷ b')
+    assert isinstance(root, BinaryOperators.Division)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, UnaryOperators.Projection)
+
+    # division <-> rename
+    root = RAParser.parse_query(r'a ÷ β [ id2 ← id ] b')
+    assert isinstance(root, BinaryOperators.Division)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, UnaryOperators.Rename)
+
+    root = RAParser.parse_query(r'β [ id2 ← id ] a ÷ b')
+    assert isinstance(root, BinaryOperators.Division)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, UnaryOperators.Rename)
+
+    # division <-> selection
+    root = RAParser.parse_query(r'a ÷ σ [ id > 1 ] b')
+    assert isinstance(root, BinaryOperators.Division)
+    assert isinstance(root.left, RAOperand) and isinstance(root.right, UnaryOperators.Selection)
+
+    root = RAParser.parse_query(r'σ [ id > 1 ] a ÷ b')
+    assert isinstance(root, BinaryOperators.Division)
+    assert isinstance(root.right, RAOperand) and isinstance(root.left, UnaryOperators.Selection)
+
 
 def test_special_queries():
     with Connection() as con:
         # Consecutive operators triggered a recursion error in a previous
         # version, leading to an infinite loop / stack overflow.
         with pytest.raises(AssertionError, match='right operand missing after x'):
             RAParser.parse_query(r'''
```

### Comparing `jupyter-duckdb-0.9.2.5/test/test_result_comparison.py` & `jupyter-duckdb-0.9.2.6/test/test_result_comparison.py`

 * *Files identical despite different names*

