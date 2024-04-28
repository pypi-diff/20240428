# Comparing `tmp/pdbstore-1.0.0.tar.gz` & `tmp/pdbstore-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbstore-1.0.0.tar", last modified: Sun Mar 24 16:00:56 2024, max compression
+gzip compressed data, was "pdbstore-1.1.0.tar", last modified: Sun Apr 28 17:56:34 2024, max compression
```

## Comparing `pdbstore-1.0.0.tar` & `pdbstore-1.1.0.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.811067 pdbstore-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      201 2024-03-24 16:00:52.000000 pdbstore-1.0.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     3653 2024-03-24 16:00:52.000000 pdbstore-1.0.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1077 2024-03-24 16:00:52.000000 pdbstore-1.0.0/COPYING
--rw-r--r--   0 root         (0) root         (0)      275 2024-03-24 16:00:52.000000 pdbstore-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4091 2024-03-24 16:00:56.811067 pdbstore-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2787 2024-03-24 16:00:52.000000 pdbstore-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.779067 pdbstore-1.0.0/docs/
--rw-r--r--   0 root         (0) root         (0)     7066 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     6724 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.783067 pdbstore-1.0.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.783067 pdbstore-1.0.0/docs/source/_static/
--rw-r--r--   0 root         (0) root         (0)      174 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/_static/rtd_literal_block.css
--rw-r--r--   0 root         (0) root         (0)      465 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/_static/rtd_theme_overrides.css
--rw-r--r--   0 root         (0) root         (0)      939 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/_static/terminal_output.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.783067 pdbstore-1.0.0/docs/source/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.783067 pdbstore-1.0.0/docs/source/api/cli/
--rw-r--r--   0 root         (0) root         (0)      115 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/cli/class.rst
--rw-r--r--   0 root         (0) root         (0)      616 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/cli/command.rst
--rw-r--r--   0 root         (0) root         (0)     2729 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/cli/decorators.rst
--rw-r--r--   0 root         (0) root         (0)      100 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/cli/functions.rst
--rw-r--r--   0 root         (0) root         (0)      297 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/cli.rst
--rw-r--r--   0 root         (0) root         (0)      159 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/config.rst
--rw-r--r--   0 root         (0) root         (0)      156 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/const.rst
--rw-r--r--   0 root         (0) root         (0)      171 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/exceptions.rst
--rw-r--r--   0 root         (0) root         (0)      132 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.787067 pdbstore-1.0.0/docs/source/api/io/
--rw-r--r--   0 root         (0) root         (0)      116 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/io/file.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/io/functions.rst
--rw-r--r--   0 root         (0) root         (0)      124 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/io/pdbfile.rst
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/io.rst
--rw-r--r--   0 root         (0) root         (0)      149 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/report.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.787067 pdbstore-1.0.0/docs/source/api/store/
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store/entry.rst
--rw-r--r--   0 root         (0) root         (0)      127 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store/history.rst
--rw-r--r--   0 root         (0) root         (0)      121 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store/store.rst
--rw-r--r--   0 root         (0) root         (0)      127 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store/summary.rst
--rw-r--r--   0 root         (0) root         (0)      139 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store/transaction.rst
--rw-r--r--   0 root         (0) root         (0)      152 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store/transaction_type.rst
--rw-r--r--   0 root         (0) root         (0)      142 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store/transactions.rst
--rw-r--r--   0 root         (0) root         (0)      540 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/api/store.rst
--rw-r--r--   0 root         (0) root         (0)       36 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/changelog.md
--rw-r--r--   0 root         (0) root         (0)     1088 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/cli-commands.rst
--rw-r--r--   0 root         (0) root         (0)     3227 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/cli-usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.787067 pdbstore-1.0.0/docs/source/commands/
--rw-r--r--   0 root         (0) root         (0)     3446 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/add.rst
--rw-r--r--   0 root         (0) root         (0)     2394 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/clean.rst
--rw-r--r--   0 root         (0) root         (0)     2388 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/del.rst
--rw-r--r--   0 root         (0) root         (0)     2417 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/fetch.rst
--rw-r--r--   0 root         (0) root         (0)     2774 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/promote.rst
--rw-r--r--   0 root         (0) root         (0)     1982 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/query.rst
--rw-r--r--   0 root         (0) root         (0)     5434 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/report.rst
--rw-r--r--   0 root         (0) root         (0)     2189 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/commands/unused.rst
--rw-r--r--   0 root         (0) root         (0)     9047 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)       35 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      309 2024-03-24 16:00:52.000000 pdbstore-1.0.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.791067 pdbstore-1.0.0/pdbstore/
--rw-r--r--   0 root         (0) root         (0)      482 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/__main__.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-03-24 16:00:53.000000 pdbstore-1.0.0/pdbstore/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.795067 pdbstore-1.0.0/pdbstore/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2428 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/args.py
--rw-r--r--   0 root         (0) root         (0)     1300 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/boolean_action.py
--rw-r--r--   0 root         (0) root         (0)     9688 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)    13151 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.795067 pdbstore-1.0.0/pdbstore/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6135 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/add.py
--rw-r--r--   0 root         (0) root         (0)     3256 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/clean.py
--rw-r--r--   0 root         (0) root         (0)     3206 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/del.py
--rw-r--r--   0 root         (0) root         (0)     7127 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/fetch.py
--rw-r--r--   0 root         (0) root         (0)     3604 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/promote.py
--rw-r--r--   0 root         (0) root         (0)     6717 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/query.py
--rw-r--r--   0 root         (0) root         (0)     5203 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/report.py
--rw-r--r--   0 root         (0) root         (0)     7342 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/commands/unused.py
--rw-r--r--   0 root         (0) root         (0)      510 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/exit_codes.py
--rw-r--r--   0 root         (0) root         (0)     1196 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/formatters.py
--rw-r--r--   0 root         (0) root         (0)      686 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/once_argument.py
--rw-r--r--   0 root         (0) root         (0)      316 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/cli/smart_formatter.py
--rw-r--r--   0 root         (0) root         (0)     7497 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/config.py
--rw-r--r--   0 root         (0) root         (0)     3435 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/const.py
--rw-r--r--   0 root         (0) root         (0)     6634 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.795067 pdbstore-1.0.0/pdbstore/io/
--rw-r--r--   0 root         (0) root         (0)      638 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3631 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/io/cab.py
--rw-r--r--   0 root         (0) root         (0)     1706 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/io/colors.py
--rw-r--r--   0 root         (0) root         (0)     9906 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/io/file.py
--rw-r--r--   0 root         (0) root         (0)    11369 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/io/output.py
--rw-r--r--   0 root         (0) root         (0)     8468 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/io/pdbfile.py
--rw-r--r--   0 root         (0) root         (0)     5658 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/io/portablepdbfile.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/py.typed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.799067 pdbstore-1.0.0/pdbstore/report/
--rw-r--r--   0 root         (0) root         (0)      240 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1520 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/report/base.py
--rw-r--r--   0 root         (0) root         (0)     2582 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/report/file.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/report/generator.py
--rw-r--r--   0 root         (0) root         (0)     3417 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/report/product.py
--rw-r--r--   0 root         (0) root         (0)     4489 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/report/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.799067 pdbstore-1.0.0/pdbstore/store/
--rw-r--r--   0 root         (0) root         (0)      509 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10651 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/entry.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/history.py
--rw-r--r--   0 root         (0) root         (0)    17804 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/store.py
--rw-r--r--   0 root         (0) root         (0)     7389 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/summary.py
--rw-r--r--   0 root         (0) root         (0)    15762 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/transaction.py
--rw-r--r--   0 root         (0) root         (0)      524 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/transaction_type.py
--rw-r--r--   0 root         (0) root         (0)     8621 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/store/transactions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.799067 pdbstore-1.0.0/pdbstore/templates/
--rw-r--r--   0 root         (0) root         (0)      109 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/README.md
--rw-r--r--   0 root         (0) root         (0)     2527 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.799067 pdbstore-1.0.0/pdbstore/templates/html/
--rw-r--r--   0 root         (0) root         (0)     3899 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/html/files.tmpl
--rw-r--r--   0 root         (0) root         (0)     3839 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/html/products.tmpl
--rw-r--r--   0 root         (0) root         (0)    11106 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/html/transactions.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.803067 pdbstore-1.0.0/pdbstore/templates/json/
--rw-r--r--   0 root         (0) root         (0)      831 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/json/files.tmpl
--rw-r--r--   0 root         (0) root         (0)      649 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/json/products.tmpl
--rw-r--r--   0 root         (0) root         (0)      767 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/json/transactions.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.803067 pdbstore-1.0.0/pdbstore/templates/markdown/
--rw-r--r--   0 root         (0) root         (0)      563 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/markdown/files.tmpl
--rw-r--r--   0 root         (0) root         (0)      527 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/markdown/products.tmpl
--rw-r--r--   0 root         (0) root         (0)      792 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/markdown/transactions.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.803067 pdbstore-1.0.0/pdbstore/templates/text/
--rw-r--r--   0 root         (0) root         (0)      661 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/text/files.tmpl
--rw-r--r--   0 root         (0) root         (0)      578 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/text/products.tmpl
--rw-r--r--   0 root         (0) root         (0)     1077 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/templates/text/transactions.tmpl
--rw-r--r--   0 root         (0) root         (0)      842 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/typing.py
--rw-r--r--   0 root         (0) root         (0)     4304 2024-03-24 16:00:52.000000 pdbstore-1.0.0/pdbstore/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.811067 pdbstore-1.0.0/pdbstore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4091 2024-03-24 16:00:56.000000 pdbstore-1.0.0/pdbstore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4422 2024-03-24 16:00:56.000000 pdbstore-1.0.0/pdbstore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-24 16:00:56.000000 pdbstore-1.0.0/pdbstore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-24 16:00:56.000000 pdbstore-1.0.0/pdbstore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-24 16:00:56.000000 pdbstore-1.0.0/pdbstore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-24 16:00:56.000000 pdbstore-1.0.0/pdbstore.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4196 2024-03-24 16:00:53.000000 pdbstore-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-24 16:00:52.000000 pdbstore-1.0.0/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      171 2024-03-24 16:00:52.000000 pdbstore-1.0.0/requirements-doc.txt
--rw-r--r--   0 root         (0) root         (0)      170 2024-03-24 16:00:52.000000 pdbstore-1.0.0/requirements-lint.txt
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-24 16:00:52.000000 pdbstore-1.0.0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-03-24 16:00:52.000000 pdbstore-1.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-24 16:00:56.811067 pdbstore-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      213 2024-03-24 16:00:52.000000 pdbstore-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.803067 pdbstore-1.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.803067 pdbstore-1.0.0/tests/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_add.py
--rw-r--r--   0 root         (0) root         (0)     3018 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_clean.py
--rw-r--r--   0 root         (0) root         (0)     4328 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4165 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     4476 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_fetch.py
--rw-r--r--   0 root         (0) root         (0)     8190 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_promote.py
--rw-r--r--   0 root         (0) root         (0)     4121 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_query.py
--rw-r--r--   0 root         (0) root         (0)     3514 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_report.py
--rw-r--r--   0 root         (0) root         (0)     5088 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/cli/test_unused.py
--rw-r--r--   0 root         (0) root         (0)     3146 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.775067 pdbstore-1.0.0/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.803067 pdbstore-1.0.0/tests/data/history/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/data/history/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.807067 pdbstore-1.0.0/tests/data/invalid/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/data/invalid/bad.exe
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.807067 pdbstore-1.0.0/tests/data/native/
--rw-r--r--   0 root         (0) root         (0)     6656 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/data/native/dummyapp.exe
--rw-r--r--   0 root         (0) root         (0)    30208 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/data/native/dummyapp.pdb
--rw-r--r--   0 root         (0) root         (0)     4096 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/data/native/dummylib.dll
--rw-r--r--   0 root         (0) root         (0)    13824 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/data/native/dummylib.pdb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.807067 pdbstore-1.0.0/tests/data/portable/
--rw-r--r--   0 root         (0) root         (0)    10260 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/data/portable/dummylib.pdb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.807067 pdbstore-1.0.0/tests/smoke/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/smoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1642 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/smoke/test_dist.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 16:00:56.811067 pdbstore-1.0.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8937 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_cab.py
--rw-r--r--   0 root         (0) root         (0)     2045 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_command.py
--rw-r--r--   0 root         (0) root         (0)     8239 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_config.py
--rw-r--r--   0 root         (0) root         (0)     3300 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_file.py
--rw-r--r--   0 root         (0) root         (0)     3628 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_formatters.py
--rw-r--r--   0 root         (0) root         (0)     2602 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_hash.py
--rw-r--r--   0 root         (0) root         (0)     1793 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_io_colors.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_native_pdb.py
--rw-r--r--   0 root         (0) root         (0)    13981 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_output.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_portable_pdb.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_report.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_setup.py
--rw-r--r--   0 root         (0) root         (0)     7973 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_store.py
--rw-r--r--   0 root         (0) root         (0)     6705 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_transaction.py
--rw-r--r--   0 root         (0) root         (0)     6729 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_transaction_entry.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tests/unit/test_util.py
--rw-r--r--   0 root         (0) root         (0)     3984 2024-03-24 16:00:52.000000 pdbstore-1.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.056468 pdbstore-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-04-28 17:56:29.000000 pdbstore-1.1.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     4398 2024-04-28 17:56:29.000000 pdbstore-1.1.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-28 17:56:29.000000 pdbstore-1.1.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-28 17:56:29.000000 pdbstore-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4091 2024-04-28 17:56:34.056468 pdbstore-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2787 2024-04-28 17:56:29.000000 pdbstore-1.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.024468 pdbstore-1.1.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     7066 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6724 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.028468 pdbstore-1.1.0/docs/source/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.028468 pdbstore-1.1.0/docs/source/_static/
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/_static/rtd_literal_block.css
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/_static/rtd_theme_overrides.css
+-rw-r--r--   0 root         (0) root         (0)      939 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/_static/terminal_output.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.028468 pdbstore-1.1.0/docs/source/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.032468 pdbstore-1.1.0/docs/source/api/cli/
+-rw-r--r--   0 root         (0) root         (0)      115 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/cli/class.rst
+-rw-r--r--   0 root         (0) root         (0)      616 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/cli/command.rst
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/cli/decorators.rst
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/cli/functions.rst
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/cli.rst
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/config.rst
+-rw-r--r--   0 root         (0) root         (0)      156 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/const.rst
+-rw-r--r--   0 root         (0) root         (0)      171 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/exceptions.rst
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.032468 pdbstore-1.1.0/docs/source/api/io/
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/io/file.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/io/functions.rst
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/io/pdbfile.rst
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/io.rst
+-rw-r--r--   0 root         (0) root         (0)      149 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/report.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.032468 pdbstore-1.1.0/docs/source/api/store/
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store/entry.rst
+-rw-r--r--   0 root         (0) root         (0)      127 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store/history.rst
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store/store.rst
+-rw-r--r--   0 root         (0) root         (0)      127 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store/summary.rst
+-rw-r--r--   0 root         (0) root         (0)      139 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store/transaction.rst
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store/transaction_type.rst
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store/transactions.rst
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/api/store.rst
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/changelog.md
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/cli-commands.rst
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/cli-usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.032468 pdbstore-1.1.0/docs/source/commands/
+-rw-r--r--   0 root         (0) root         (0)     3446 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/add.rst
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/clean.rst
+-rw-r--r--   0 root         (0) root         (0)     2388 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/del.rst
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/fetch.rst
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/promote.rst
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/query.rst
+-rw-r--r--   0 root         (0) root         (0)     5434 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/report.rst
+-rw-r--r--   0 root         (0) root         (0)     2189 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/commands/unused.rst
+-rw-r--r--   0 root         (0) root         (0)     9047 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      309 2024-04-28 17:56:29.000000 pdbstore-1.1.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.036468 pdbstore-1.1.0/pdbstore/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-04-28 17:56:30.000000 pdbstore-1.1.0/pdbstore/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.040468 pdbstore-1.1.0/pdbstore/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/boolean_action.py
+-rw-r--r--   0 root         (0) root         (0)     9688 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)    13151 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.040468 pdbstore-1.1.0/pdbstore/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6135 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/add.py
+-rw-r--r--   0 root         (0) root         (0)     3256 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/clean.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/del.py
+-rw-r--r--   0 root         (0) root         (0)     7091 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/promote.py
+-rw-r--r--   0 root         (0) root         (0)     6677 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/query.py
+-rw-r--r--   0 root         (0) root         (0)     5203 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/report.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/commands/unused.py
+-rw-r--r--   0 root         (0) root         (0)      510 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/exit_codes.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      686 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/once_argument.py
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/cli/smart_formatter.py
+-rw-r--r--   0 root         (0) root         (0)     7497 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/config.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/const.py
+-rw-r--r--   0 root         (0) root         (0)     6634 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.044468 pdbstore-1.1.0/pdbstore/io/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/io/cab.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/io/colors.py
+-rw-r--r--   0 root         (0) root         (0)     9906 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/io/file.py
+-rw-r--r--   0 root         (0) root         (0)    11369 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/io/output.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/io/pdbfile.py
+-rw-r--r--   0 root         (0) root         (0)     5658 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/io/portablepdbfile.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/py.typed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.044468 pdbstore-1.1.0/pdbstore/report/
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/report/base.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/report/file.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/report/generator.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/report/product.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/report/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.044468 pdbstore-1.1.0/pdbstore/store/
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10651 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/entry.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/history.py
+-rw-r--r--   0 root         (0) root         (0)    17804 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/store.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/summary.py
+-rw-r--r--   0 root         (0) root         (0)    15763 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/transaction.py
+-rw-r--r--   0 root         (0) root         (0)      524 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/transaction_type.py
+-rw-r--r--   0 root         (0) root         (0)     8621 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/store/transactions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.044468 pdbstore-1.1.0/pdbstore/templates/
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/README.md
+-rw-r--r--   0 root         (0) root         (0)     2527 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.048468 pdbstore-1.1.0/pdbstore/templates/html/
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/html/files.tmpl
+-rw-r--r--   0 root         (0) root         (0)     3839 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/html/products.tmpl
+-rw-r--r--   0 root         (0) root         (0)    11106 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/html/transactions.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.048468 pdbstore-1.1.0/pdbstore/templates/json/
+-rw-r--r--   0 root         (0) root         (0)      831 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/json/files.tmpl
+-rw-r--r--   0 root         (0) root         (0)      649 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/json/products.tmpl
+-rw-r--r--   0 root         (0) root         (0)      767 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/json/transactions.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.048468 pdbstore-1.1.0/pdbstore/templates/markdown/
+-rw-r--r--   0 root         (0) root         (0)      563 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/markdown/files.tmpl
+-rw-r--r--   0 root         (0) root         (0)      527 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/markdown/products.tmpl
+-rw-r--r--   0 root         (0) root         (0)      792 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/markdown/transactions.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.048468 pdbstore-1.1.0/pdbstore/templates/text/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/text/files.tmpl
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/text/products.tmpl
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/templates/text/transactions.tmpl
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/typing.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2024-04-28 17:56:29.000000 pdbstore-1.1.0/pdbstore/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.056468 pdbstore-1.1.0/pdbstore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4091 2024-04-28 17:56:34.000000 pdbstore-1.1.0/pdbstore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4422 2024-04-28 17:56:34.000000 pdbstore-1.1.0/pdbstore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 17:56:34.000000 pdbstore-1.1.0/pdbstore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-28 17:56:34.000000 pdbstore-1.1.0/pdbstore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-28 17:56:34.000000 pdbstore-1.1.0/pdbstore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-28 17:56:34.000000 pdbstore-1.1.0/pdbstore.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4521 2024-04-28 17:56:30.000000 pdbstore-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-28 17:56:29.000000 pdbstore-1.1.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2024-04-28 17:56:29.000000 pdbstore-1.1.0/requirements-doc.txt
+-rw-r--r--   0 root         (0) root         (0)      169 2024-04-28 17:56:29.000000 pdbstore-1.1.0/requirements-lint.txt
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-28 17:56:29.000000 pdbstore-1.1.0/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-28 17:56:29.000000 pdbstore-1.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 17:56:34.056468 pdbstore-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      213 2024-04-28 17:56:29.000000 pdbstore-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.048468 pdbstore-1.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.052468 pdbstore-1.1.0/tests/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_add.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_clean.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     4476 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_fetch.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_promote.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_query.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_report.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/cli/test_unused.py
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.024468 pdbstore-1.1.0/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.052468 pdbstore-1.1.0/tests/data/history/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/data/history/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.052468 pdbstore-1.1.0/tests/data/invalid/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/data/invalid/bad.exe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.052468 pdbstore-1.1.0/tests/data/native/
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/data/native/dummyapp.exe
+-rw-r--r--   0 root         (0) root         (0)    30208 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/data/native/dummyapp.pdb
+-rw-r--r--   0 root         (0) root         (0)     4096 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/data/native/dummylib.dll
+-rw-r--r--   0 root         (0) root         (0)    13824 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/data/native/dummylib.pdb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.052468 pdbstore-1.1.0/tests/data/portable/
+-rw-r--r--   0 root         (0) root         (0)    10260 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/data/portable/dummylib.pdb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.052468 pdbstore-1.1.0/tests/smoke/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/smoke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/smoke/test_dist.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 17:56:34.056468 pdbstore-1.1.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8937 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_cab.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_command.py
+-rw-r--r--   0 root         (0) root         (0)     8239 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_file.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_formatters.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_hash.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_io_colors.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_native_pdb.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_output.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_portable_pdb.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_report.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_setup.py
+-rw-r--r--   0 root         (0) root         (0)     7973 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_store.py
+-rw-r--r--   0 root         (0) root         (0)     6705 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     6729 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_transaction_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tests/unit/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-04-28 17:56:29.000000 pdbstore-1.1.0/tox.ini
```

### Comparing `pdbstore-1.0.0/CHANGELOG.md` & `pdbstore-1.1.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,42 @@
 # CHANGELOG
 
+## v1.0.0 (2024-03-24)
+
+### Breaking
+
+* feat(command): add --days option to unused command (#21)
+
+BREAKING CHANGE: DATE positional argument has been converted into an option ([`19424ea`](https://github.com/crabisoft/pdbstore/commit/19424eaff569e9c3cf004bc7678ee7bcd6d3ca75))
+
+### Chore
+
+* chore: update release worklow ([`cbe8de9`](https://github.com/crabisoft/pdbstore/commit/cbe8de9f357f972c9ccc58ea50f97fd7827a9d7e))
+
+### Documentation
+
+* docs: improve documentation (#23) ([`f7b2ba5`](https://github.com/crabisoft/pdbstore/commit/f7b2ba52dc60699f37b77c7baa9afadc4e67a3dc))
+
+### Feature
+
+* feat(command): display total file size for unused command (#22) ([`3d414cb`](https://github.com/crabisoft/pdbstore/commit/3d414cbfa192fa8c0e619a1aea5795e40f7f8074))
+
 ## v0.3.0 (2024-03-23)
 
 ### Feature
 
 * feat(command): add --dry-run option for del command (#18) ([`99f038a`](https://github.com/crabisoft/pdbstore/commit/99f038a7c404182d8b44d2b33b3971ecdbdc3e09))
 
 * feat(command): add --delete option for unused command (#17) ([`c83851f`](https://github.com/crabisoft/pdbstore/commit/c83851fbe3335343757b445f96552773722c30f6))
 
 ### Fix
 
-* fix(transaction): no transaction created if file already exists from store (#19) ([`1754d19`](https://github.com/crabisoft/pdbstore/commit/1754d19153c99006d5d1b61cf55679f319c0934d))
+* fix(transaction): no transaction created if file already exists from … (#19) ([`1754d19`](https://github.com/crabisoft/pdbstore/commit/1754d19153c99006d5d1b61cf55679f319c0934d))
 
-### Documentation
+### Unknown
 
 * doc: refactor documentation (#20) ([`c600537`](https://github.com/crabisoft/pdbstore/commit/c600537d6c9b348ecf0004d11a0920cb94979d7d))
 
 ## v0.2.0 (2024-03-17)
 
 ### Chore
 
@@ -30,15 +50,15 @@
 
 * feat: commit files in parallel (#12) ([`88b5084`](https://github.com/crabisoft/pdbstore/commit/88b5084674a3f477ef8993f87d0bac490edb8a49))
 
 ### Test
 
 * test: add dedicated compression test when supported (#14) ([`3b6dfda`](https://github.com/crabisoft/pdbstore/commit/3b6dfdab3eb58d35735d0149d480cc9488548ff6))
 
-### Documentation
+### Unknown
 
 * doc: add promote command (#16) ([`c0e5328`](https://github.com/crabisoft/pdbstore/commit/c0e5328e1f725bc7eeac4fc98f802effd51f7bc0))
 
 ## v0.1.2 (2024-03-03)
 
 ### Fix
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pdbstore-1.0.0/COPYING` & `pdbstore-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/PKG-INFO` & `pdbstore-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbstore
-Version: 1.0.0
+Version: 1.1.0
 Summary: manage PDB and PE files through a local symbols store
 Author-email: Jacques Raphanel <jrp@crabisoft.fr>
 License: MIT
 Project-URL: changelog, https://github.com/crabisoft/pdbstore/blob/main/CHANGELOG.md
 Project-URL: documentation, https://pdbstore.readthedocs.io
 Project-URL: homepage, https://github.com/crabisoft/pdbstore
 Project-URL: issues, https://github.com/crabisoft/pdbstore/issues
```

### Comparing `pdbstore-1.0.0/README.rst` & `pdbstore-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/Makefile` & `pdbstore-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/make.bat` & `pdbstore-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/_static/terminal_output.css` & `pdbstore-1.1.0/docs/source/_static/terminal_output.css`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/api/cli/command.rst` & `pdbstore-1.1.0/docs/source/api/cli/command.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/api/cli/decorators.rst` & `pdbstore-1.1.0/docs/source/api/cli/decorators.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/api/store.rst` & `pdbstore-1.1.0/docs/source/api/store.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/cli-commands.rst` & `pdbstore-1.1.0/docs/source/cli-commands.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/cli-usage.rst` & `pdbstore-1.1.0/docs/source/cli-usage.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/add.rst` & `pdbstore-1.1.0/docs/source/commands/add.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/clean.rst` & `pdbstore-1.1.0/docs/source/commands/clean.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/del.rst` & `pdbstore-1.1.0/docs/source/commands/del.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/fetch.rst` & `pdbstore-1.1.0/docs/source/commands/fetch.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/promote.rst` & `pdbstore-1.1.0/docs/source/commands/promote.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/query.rst` & `pdbstore-1.1.0/docs/source/commands/query.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/report.rst` & `pdbstore-1.1.0/docs/source/commands/report.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/commands/unused.rst` & `pdbstore-1.1.0/docs/source/commands/unused.rst`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/docs/source/conf.py` & `pdbstore-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/args.py` & `pdbstore-1.1.0/pdbstore/cli/args.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/boolean_action.py` & `pdbstore-1.1.0/pdbstore/cli/boolean_action.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/cli.py` & `pdbstore-1.1.0/pdbstore/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/command.py` & `pdbstore-1.1.0/pdbstore/cli/command.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/add.py` & `pdbstore-1.1.0/pdbstore/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/clean.py` & `pdbstore-1.1.0/pdbstore/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/del.py` & `pdbstore-1.1.0/pdbstore/cli/commands/del.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/fetch.py` & `pdbstore-1.1.0/pdbstore/cli/commands/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,15 @@
             for queryd in cur.files:
                 symbol_path = queryd.get("path", "")
                 file_path = queryd.get("input", "")
                 if not file_path:
                     file_path = symbol_path
                     symbol_path = None
                 file_len = len(symbol_path or file_path)
-                if (file_len + 2) > input_len:
-                    input_len = file_len + 2
+                input_len = max(input_len, file_len + 2)
 
     cli_out_write(f"{'Input File':<{input_len}s}{'Compressed':^10s} Symbol File")
     for cur in summary.iterator():
         for queryd in cur.files:
             symbol_path = queryd.get("path", "")
             file_path = queryd.get("input", "")
             if not file_path:
```

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/promote.py` & `pdbstore-1.1.0/pdbstore/cli/commands/promote.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/query.py` & `pdbstore-1.1.0/pdbstore/cli/commands/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
                     if (
                         OpStatus.from_str(queryd.get("status", OpStatus.SKIPPED))
                         == OpStatus.SUCCESS
                     ):
                         file_len = len(input_path)
                     else:
                         file_len = len(file_path)
-                    if (file_len + 2) > input_len:
-                        input_len = file_len + 2
+                    input_len = max(input_len, file_len + 2)
 
     cli_out_write(f"{'Input File':<{input_len}s}{'Compressed':^10s} Symbol File")
     for cur in summary.iterator():
         for queryd in cur.files:
             file_path = queryd.get("path", "")
             input_path = queryd.get("input", "")
             status: OpStatus = OpStatus.from_str(queryd.get("status", OpStatus.SKIPPED))
```

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/report.py` & `pdbstore-1.1.0/pdbstore/cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/commands/unused.py` & `pdbstore-1.1.0/pdbstore/cli/commands/unused.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/formatters.py` & `pdbstore-1.1.0/pdbstore/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/cli/once_argument.py` & `pdbstore-1.1.0/pdbstore/cli/once_argument.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/config.py` & `pdbstore-1.1.0/pdbstore/config.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/const.py` & `pdbstore-1.1.0/pdbstore/const.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/exceptions.py` & `pdbstore-1.1.0/pdbstore/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/io/__init__.py` & `pdbstore-1.1.0/pdbstore/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/io/cab.py` & `pdbstore-1.1.0/pdbstore/io/cab.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/io/colors.py` & `pdbstore-1.1.0/pdbstore/io/colors.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/io/file.py` & `pdbstore-1.1.0/pdbstore/io/file.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/io/output.py` & `pdbstore-1.1.0/pdbstore/io/output.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/io/pdbfile.py` & `pdbstore-1.1.0/pdbstore/io/pdbfile.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/io/portablepdbfile.py` & `pdbstore-1.1.0/pdbstore/io/portablepdbfile.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/report/base.py` & `pdbstore-1.1.0/pdbstore/report/base.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/report/file.py` & `pdbstore-1.1.0/pdbstore/report/file.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/report/generator.py` & `pdbstore-1.1.0/pdbstore/report/generator.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/report/product.py` & `pdbstore-1.1.0/pdbstore/report/product.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/report/transaction.py` & `pdbstore-1.1.0/pdbstore/report/transaction.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/store/entry.py` & `pdbstore-1.1.0/pdbstore/store/entry.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/store/history.py` & `pdbstore-1.1.0/pdbstore/store/history.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/store/store.py` & `pdbstore-1.1.0/pdbstore/store/store.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/store/summary.py` & `pdbstore-1.1.0/pdbstore/store/summary.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/store/transaction.py` & `pdbstore-1.1.0/pdbstore/store/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Manage a single transaction.
 """
+
 import concurrent.futures as cf
 import os
 import re
 import shutil
 from datetime import datetime
 from pathlib import Path
```

### Comparing `pdbstore-1.0.0/pdbstore/store/transaction_type.py` & `pdbstore-1.1.0/pdbstore/store/transaction_type.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/store/transactions.py` & `pdbstore-1.1.0/pdbstore/store/transactions.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/__init__.py` & `pdbstore-1.1.0/pdbstore/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/html/files.tmpl` & `pdbstore-1.1.0/pdbstore/templates/html/files.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/html/products.tmpl` & `pdbstore-1.1.0/pdbstore/templates/html/products.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/html/transactions.tmpl` & `pdbstore-1.1.0/pdbstore/templates/html/transactions.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/json/files.tmpl` & `pdbstore-1.1.0/pdbstore/templates/json/files.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/json/products.tmpl` & `pdbstore-1.1.0/pdbstore/templates/json/products.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/json/transactions.tmpl` & `pdbstore-1.1.0/pdbstore/templates/json/transactions.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/markdown/files.tmpl` & `pdbstore-1.1.0/pdbstore/templates/markdown/files.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/markdown/products.tmpl` & `pdbstore-1.1.0/pdbstore/templates/markdown/products.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/markdown/transactions.tmpl` & `pdbstore-1.1.0/pdbstore/templates/markdown/transactions.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/text/files.tmpl` & `pdbstore-1.1.0/pdbstore/templates/text/files.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/text/products.tmpl` & `pdbstore-1.1.0/pdbstore/templates/text/products.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/templates/text/transactions.tmpl` & `pdbstore-1.1.0/pdbstore/templates/text/transactions.tmpl`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/typing.py` & `pdbstore-1.1.0/pdbstore/typing.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore/util.py` & `pdbstore-1.1.0/pdbstore/util.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pdbstore.egg-info/PKG-INFO` & `pdbstore-1.1.0/pdbstore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbstore
-Version: 1.0.0
+Version: 1.1.0
 Summary: manage PDB and PE files through a local symbols store
 Author-email: Jacques Raphanel <jrp@crabisoft.fr>
 License: MIT
 Project-URL: changelog, https://github.com/crabisoft/pdbstore/blob/main/CHANGELOG.md
 Project-URL: documentation, https://pdbstore.readthedocs.io
 Project-URL: homepage, https://github.com/crabisoft/pdbstore
 Project-URL: issues, https://github.com/crabisoft/pdbstore/issues
```

### Comparing `pdbstore-1.0.0/pdbstore.egg-info/SOURCES.txt` & `pdbstore-1.1.0/pdbstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/pyproject.toml` & `pdbstore-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pdbstore"
-version = "1.0.0"
+version = "1.1.0"
 description="manage PDB and PE files through a local symbols store"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -36,14 +36,23 @@
 homepage = "https://github.com/crabisoft/pdbstore"
 issues = "https://github.com/crabisoft/pdbstore/issues"
 repository = "http://github.com/crabisoft/pdbstore.git"
 
 [tool.black]
 line-length = 100
 
+[flake8]
+exclude = [".git",".venv",".tox","dist","docs","*egg,build"]
+max-line-length = 100
+# We ignore the following because we use black to handle code-formatting
+# E203: Whitespace before ':'
+# E501: Line too long
+# W503: Line break occurred before a binary operator
+ignore = ["E203","E501","W503"]
+
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 order_by_type = false
 
 [tool.mypy]
 files = "."
@@ -122,14 +131,15 @@
 max-line-length = 100
 max-return = 10
 jobs = 0  # Use auto-detected number of multiple processes to speed up Pylint.
 disable = [
     "missing-module-docstring",
     "too-many-branches",
     "too-many-statements",
+    "duplicate-code",
 ]
 max-args=15 # Maximum number of arguments for function / method.
 max-attributes=20   # Maximum number of attributes for a class (see R0902).
 max-local=25    # Maximum number of local variables
 max-bool-expr=8 # Maximum number of boolean expressions in an if statement (see R0916).
 max-public-methods = 25 # Maximum number of public methods for a class (see R0904).
```

### Comparing `pdbstore-1.0.0/tests/cli/test_add.py` & `pdbstore-1.1.0/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_clean.py` & `pdbstore-1.1.0/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_cli.py` & `pdbstore-1.1.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_delete.py` & `pdbstore-1.1.0/tests/cli/test_delete.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_fetch.py` & `pdbstore-1.1.0/tests/cli/test_fetch.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_promote.py` & `pdbstore-1.1.0/tests/cli/test_promote.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_query.py` & `pdbstore-1.1.0/tests/cli/test_query.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_report.py` & `pdbstore-1.1.0/tests/cli/test_report.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/cli/test_unused.py` & `pdbstore-1.1.0/tests/cli/test_unused.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/conftest.py` & `pdbstore-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/data/native/dummyapp.exe` & `pdbstore-1.1.0/tests/data/native/dummyapp.exe`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/data/native/dummyapp.pdb` & `pdbstore-1.1.0/tests/data/native/dummyapp.pdb`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/data/native/dummylib.dll` & `pdbstore-1.1.0/tests/data/native/dummylib.dll`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/data/native/dummylib.pdb` & `pdbstore-1.1.0/tests/data/native/dummylib.pdb`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/data/portable/dummylib.pdb` & `pdbstore-1.1.0/tests/data/portable/dummylib.pdb`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/smoke/test_dist.py` & `pdbstore-1.1.0/tests/smoke/test_dist.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_cab.py` & `pdbstore-1.1.0/tests/unit/test_cab.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_command.py` & `pdbstore-1.1.0/tests/unit/test_command.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_config.py` & `pdbstore-1.1.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_file.py` & `pdbstore-1.1.0/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_formatters.py` & `pdbstore-1.1.0/tests/unit/test_formatters.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_hash.py` & `pdbstore-1.1.0/tests/unit/test_hash.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_io_colors.py` & `pdbstore-1.1.0/tests/unit/test_io_colors.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_native_pdb.py` & `pdbstore-1.1.0/tests/unit/test_native_pdb.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_output.py` & `pdbstore-1.1.0/tests/unit/test_output.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_portable_pdb.py` & `pdbstore-1.1.0/tests/unit/test_portable_pdb.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_report.py` & `pdbstore-1.1.0/tests/unit/test_report.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_store.py` & `pdbstore-1.1.0/tests/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_transaction.py` & `pdbstore-1.1.0/tests/unit/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_transaction_entry.py` & `pdbstore-1.1.0/tests/unit/test_transaction_entry.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tests/unit/test_util.py` & `pdbstore-1.1.0/tests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `pdbstore-1.0.0/tox.ini` & `pdbstore-1.1.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tox]
 minversion = 1.6
 skipsdist = True
 skip_missing_interpreters = True
-envlist = py311,py310,py39,py38,syntax,cover,twine-check,cz
+envlist = py313,py312,py311,py310,py39,py38,syntax,cover,twine-check,cz
 
 [testenv]
 passenv =
   PY_COLORS
   NO_COLOR
   FORCE_COLOR
   PWD
@@ -23,15 +23,15 @@
   pytest tests/unit tests/smoke {posargs}
 
 [testenv:black]
 basepython = python3
 envdir={toxworkdir}/black
 deps = -r{toxinidir}/requirements-lint.txt
 commands =
-  black {posargs} --line-length 88 {toxinidir}/pdbstore/ {toxinidir}/tests/ {toxinidir}/installer/
+  black {posargs} {toxinidir}/pdbstore/ {toxinidir}/tests/ {toxinidir}/installer/
 
 [testenv:isort]
 basepython = python3
 envdir={toxworkdir}/isort
 deps = -r{toxinidir}/requirements-lint.txt
 commands =
   isort {posargs} {toxinidir}/pdbstore/ {toxinidir}/tests/ {toxinidir}/installer/
@@ -58,15 +58,15 @@
   pylint {posargs} {toxinidir}/pdbstore/ {toxinidir}/tests/ {toxinidir}/installer/
 
 [testenv:cz]
 basepython = python3
 envdir={toxworkdir}/cz
 deps = -r{toxinidir}/requirements-lint.txt
 commands =
-  cz check --rev-range f3cb6c0..HEAD
+  cz check --rev-range b508ef5..HEAD
 
 [testenv:twine-check]
 basepython = python3
 deps = -r{toxinidir}/requirements.txt
        twine
        build
 commands =
```

