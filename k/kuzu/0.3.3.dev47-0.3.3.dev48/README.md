# Comparing `tmp/kuzu-0.3.3.dev47.tar.gz` & `tmp/kuzu-0.3.3.dev48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.3.3.dev47.tar", last modified: Fri Apr 26 08:04:53 2024, max compression
+gzip compressed data, was "kuzu-0.3.3.dev48.tar", last modified: Sat Apr 27 08:04:51 2024, max compression
```

## Comparing `kuzu-0.3.3.dev47.tar` & `kuzu-0.3.3.dev48.tar`

### file list

```diff
@@ -1,2797 +1,2797 @@
-drwx------   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:53.600923 sdist/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-26 08:04:47.728837 sdist/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 08:04:49.184858 sdist/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-26 08:04:47.728837 sdist/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-26 08:04:49.184858 sdist/README_PYTHON_BUILD.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:53.080915 sdist/kuzu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:53.080915 sdist/kuzu-source/
--rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-04-26 08:04:50.000000 sdist/kuzu-source/.clang-format
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-26 08:04:50.000000 sdist/kuzu-source/.clang-tidy
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-26 08:04:50.000000 sdist/kuzu-source/.clang-tidy-analyzer
--rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-04-26 08:04:50.000000 sdist/kuzu-source/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-04-26 08:04:50.000000 sdist/kuzu-source/.lcovrc
--rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-04-26 08:04:50.000000 sdist/kuzu-source/CLA.md
--rw-rw-r--   0 runner    (1001) docker     (127)     8485 2024-04-26 08:04:50.000000 sdist/kuzu-source/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-04-26 08:04:50.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-26 08:04:50.000000 sdist/kuzu-source/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-04-26 08:04:50.000000 sdist/kuzu-source/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     6365 2024-04-26 08:04:50.000000 sdist/kuzu-source/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-04-26 08:04:50.000000 sdist/kuzu-source/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    26328 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
--rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
--rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/check-include-guards.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
--rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
--rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
--rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
--rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
--rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
--rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/http-server.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
--rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/pip-package/
--rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/pip-package/README.md
--rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     4441 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/pip-package/setup.py
--rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/run-clang-format.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-26 08:04:50.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/
--rw-rw-r--   0 runner    (1001) docker     (127)     2548 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/antlr4/
--rw-rw-r--   0 runner    (1001) docker     (127)    26328 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/
--rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      441 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18648 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5298 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32996 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3108 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11859 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17249 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/bind_use_database.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7684 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/read/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2996 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5622 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1740 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2202 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3088 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16864 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1410 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1677 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      926 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5174 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8729 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      585 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5982 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      576 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression/variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6470 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5779 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9670 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6621 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2689 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/data_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7841 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19820 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/c_api/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11101 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_content.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)      464 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1198 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1149 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3144 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4001 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3041 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1483 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/catalog/property.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    24631 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10592 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    35519 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5340 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/constants.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3078 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2645 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12603 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2665 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/exception/message.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/expression_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15233 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2726 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      743 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/logging_level_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/md5.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/metric.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8989 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/null_mask.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/profiler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/random_engine.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5079 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/string_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/system_message.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2720 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/task_system/task.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9755 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/type_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4772 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/blob.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/date_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1174 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    50966 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/uuid.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2799 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    34391 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/types/value/value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2904 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3350 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28649 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/common/windows_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4615 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      885 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3490 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1556 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9766 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/extension/extension.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/
--rw-rw-r--   0 runner    (1001) docker     (127)     1240 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3939 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1841 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5505 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/array/
--rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/array/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6098 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/array/array_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1328 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/array/array_value.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20031 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5405 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    33753 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/find_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12568 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/function_collection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/
--rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2749 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_agg_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_any_value_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2620 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_append_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2166 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_concat_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_contains_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2235 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_creation.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_distinct_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2192 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1184 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_position_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2490 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_prepend_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3387 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_range_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_reverse_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3355 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_slice_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9697 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_sort_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_to_string_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2240 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/list_unique_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1904 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/list/size_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/map/
--rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/map/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1095 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/map/map_creation_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/map/map_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      963 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/map/map_keys_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      955 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/map/map_values_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/path/
--rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/path/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/path/nodes_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3870 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/path/properties_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/path/rels_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1997 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/path/semantic_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/struct/
--rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/struct/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2621 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/struct/struct_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/struct/struct_pack_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2246 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1390 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2672 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/show_attached_databases.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5091 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11017 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4309 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/union/
--rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/union/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/union/union_extract_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/union/union_tag_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1873 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/union/union_value_function.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/utility/
--rw-rw-r--   0 runner    (1001) docker     (127)      183 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/utility/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3554 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/utility/coalesce.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18396 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    47564 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4887 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10069 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14671 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/
--rw-rw-r--   0 runner    (1001) docker     (127)    12711 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
--rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_database_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1901 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_export_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      713 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      877 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_import_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      787 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2666 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/bound_use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/copy/
--rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3274 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5498 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4616 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2074 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      878 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      786 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      937 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2561 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6057 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2487 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6508 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
--rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1010 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     1445 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/rewriter/
--rw-rw-r--   0 runner    (1001) docker     (127)      515 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/c_api/
--rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/c_api/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51266 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/
--rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3631 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_content.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
--rw-rw-r--   0 runner    (1001) docker     (127)     1769 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1343 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2311 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2361 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3199 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1406 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/catalog/property.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/api.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/arrow/
--rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2921 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/assert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/column_data_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9693 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/constants.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/copier_config/
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3648 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/data_chunk/
--rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1540 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1221 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      938 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
--rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/binder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
--rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/exception.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      282 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/io.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/message.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
--rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
--rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/test.h
--rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/file_system/
--rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2076 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2043 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1814 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2203 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/keyword/
--rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/logging_level_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/md5.h
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/metric.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/null_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9142 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/null_mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/profiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/random_engine.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/serializer/
--rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2228 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/static_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/string_format.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4653 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/system_message.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/task_system/
--rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/task_system/task.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/timer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11129 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/type_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/
--rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/blob.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/date_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21967 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/types.h
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/uuid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/value/
--rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/value/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21490 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/types/value/value.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1227 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/vector/
--rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13684 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/common/windows_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/
--rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/extension/
--rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/extension/catalog_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1265 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/extension/extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/extension/extension_action.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)     3538 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4106 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2918 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6996 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/array/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/array/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25289 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/blob/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/blob/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/boolean/
--rw-rw-r--   0 runner    (1001) docker     (127)    15140 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3668 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/
--rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7564 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7994 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/comparison/
--rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10062 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/date/
--rw-rw-r--   0 runner    (1001) docker     (127)     4625 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1236 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2866 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/function_collection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/hash/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/hash/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/hash/functions/md5_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      571 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/hash/functions/sha256_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6058 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/interval/
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1333 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_to_string_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1231 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3221 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2268 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/null/
--rw-rw-r--   0 runner    (1001) docker     (127)     2772 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/path/
--rw-rw-r--   0 runner    (1001) docker     (127)     6252 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      791 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10274 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/scalar_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/schema/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5537 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/struct/
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/table/
--rw-rw-r--   0 runner    (1001) docker     (127)     1702 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2912 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4127 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/table_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    22251 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/timestamp/
--rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/udf_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7936 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/union/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/union/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)     1249 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
--rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/utility/
--rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/utility/scalar_utility_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/uuid/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/uuid/functions/
--rw-rw-r--   0 runner    (1001) docker     (127)      395 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/
--rw-rw-r--   0 runner    (1001) docker     (127)      780 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/attached_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1450 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/client_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6395 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/client_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7548 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5870 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      837 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/database_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/db_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1394 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/kuzu.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1248 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3548 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/plan_printer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1992 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4968 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/query_summary.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6194 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/settings.h
--rw-rw-r--   0 runner    (1001) docker     (127)      830 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/storage_driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/main/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3621 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6889 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      936 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
--rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/copy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/database_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
--rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3025 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
--rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/parsed_data/
--rw-rw-r--   0 runner    (1001) docker     (127)      177 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2613 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/parser.h
--rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/port_db.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1521 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
--rw-rw-r--   0 runner    (1001) docker     (127)      898 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/scan_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12939 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/transformer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      330 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
--rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      920 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1107 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
--rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
--rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2791 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6065 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_simple.h
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_use_database.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/sip/
--rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
--rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16586 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/planner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/data_pos.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/execution_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)    11146 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3698 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)     4460 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4761 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3299 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
--rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1742 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)     2829 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2150 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3177 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2821 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1604 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6124 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5440 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5761 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1480 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1358 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4613 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4702 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3426 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6781 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7416 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
--rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4368 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4075 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5010 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6229 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5296 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2908 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1769 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2072 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2322 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/attach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/database_operator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      696 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/detach_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/export_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      690 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/import_db.h
--rw-rw-r--   0 runner    (1001) docker     (127)      941 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/install_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/load_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/simple.h
--rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/simple/use_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1095 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12402 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/processor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/processor_task.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16636 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1061 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1547 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)     9404 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13079 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)    15859 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3328 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/file_handle.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)    14432 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1141 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2132 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6182 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/index/in_mem_hash_index.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)     2514 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3159 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9234 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4474 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3236 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4425 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2909 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)     2297 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4969 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7895 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      774 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)     4852 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14477 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9626 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3298 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6125 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6203 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3504 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2642 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8048 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12592 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3678 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3531 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/table.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2638 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)     3663 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8162 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2356 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)     1893 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/transaction/transaction.h
--rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3747 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/
--rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20127 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/client_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11677 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2577 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/database_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/db_config.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/plan_printer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      956 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/query_summary.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/storage_driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/main/version.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/
--rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10339 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12065 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5558 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13109 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/antlr_parser/
--rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/create_macro.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/expression/
--rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4399 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1259 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/
--rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7632 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2715 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      484 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2681 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transform/transform_use_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4493 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/transformer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/visitor/
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/
--rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/join_order/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/factorization/
--rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6276 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1732 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5973 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      185 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/simple/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/operator/simple/logical_simple.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/
--rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1971 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13525 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6469 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27166 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/query_planner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/
--rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/
--rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4774 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8285 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9380 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15120 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4729 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6221 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1956 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5998 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4327 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6873 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3425 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3525 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6610 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4721 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8345 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    36724 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5470 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4848 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/call/
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2958 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/ddl/
--rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2464 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2463 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1043 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1306 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/hash_join/
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2057 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8290 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9252 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4502 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/intersect/
--rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     9664 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/macro/
--rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      727 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/
--rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14058 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9014 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7795 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/
--rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      760 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8388 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5443 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4759 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7316 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3038 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11841 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
--rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4367 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8564 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6543 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
--rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13865 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    24072 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5995 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    29865 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3449 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
--rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13988 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13452 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11285 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6592 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16464 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11697 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8457 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
--rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7361 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5067 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12987 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2479 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      825 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3865 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      625 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      651 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5110 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1378 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/attach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/detach_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/export_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/import_db.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2423 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/install_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2205 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/load_extension.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/simple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/simple/use_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2403 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/table_scan/
--rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2486 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1256 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2659 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/processor.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/processor_task.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/
--rw-rw-r--   0 runner    (1001) docker     (127)      336 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7142 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    34515 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/buffer_manager/
--rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7039 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    15692 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2145 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/compression/
--rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35327 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/file_handle.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/index/
--rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    31321 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13455 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/index/in_mem_hash_index.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/local_storage/
--rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6131 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12393 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6966 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/
--rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7957 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4352 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4017 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5914 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10057 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_structure/
--rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5262 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    23949 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9909 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/
--rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6931 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2126 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    45316 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    27639 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10968 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    23446 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16099 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9759 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10481 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9049 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8480 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    50285 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12402 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7831 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12348 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6206 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/wal/
--rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     6531 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6783 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16642 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/transaction/
--rw-rw-r--   0 runner    (1001) docker     (127)      216 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3894 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4629 2024-04-26 08:04:50.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)      489 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_cypher/
--rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    56662 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   469834 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     3272 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)    88277 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/
--rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
--rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
--rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
--rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
--rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
--rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
--rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
--rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
--rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
--rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
--rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
--rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
--rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
--rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
--rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4224 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
--rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
--rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
--rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
--rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
--rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/
--rw-rw-r--   0 runner    (1001) docker     (127)     5677 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12841 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)      652 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/README
--rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      314 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/SECURITY.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/
--rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.c
--rw-rw-r--   0 runner    (1001) docker     (127)     8011 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7965 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/context.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4666 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/context.h
--rw-rw-r--   0 runner    (1001) docker     (127)   122784 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin
--rw-rw-r--   0 runner    (1001) docker     (127)    51687 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin.br
--rw-rw-r--   0 runner    (1001) docker     (127)   472009 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1951 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.c
--rw-rw-r--   0 runner    (1001) docker     (127)    18385 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17424 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2413 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10677 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/common/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/
--rw-rw-r--   0 runner    (1001) docker     (127)     2285 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.c
--rw-rw-r--   0 runner    (1001) docker     (127)    14854 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)   103991 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/decode.c
--rw-rw-r--   0 runner    (1001) docker     (127)    11996 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.h
--rw-rw-r--   0 runner    (1001) docker     (127)    31612 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/prefix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5659 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.c
--rw-rw-r--   0 runner    (1001) docker     (127)    12546 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/
--rw-rw-r--   0 runner    (1001) docker     (127)     5673 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1301 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36639 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8181 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1685 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4109 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1137 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_encoder_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7395 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18673 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    50750 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3477 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1485 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11826 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1019 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.c
--rw-rw-r--   0 runner    (1001) docker     (127)     6892 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6645 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)    33255 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3598 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27182 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2879 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.h
--rw-rw-r--   0 runner    (1001) docker     (127)   147154 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.c
--rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.h
--rw-rw-r--   0 runner    (1001) docker     (127)    77547 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/encode.c
--rw-rw-r--   0 runner    (1001) docker     (127)    23290 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.c
--rw-rw-r--   0 runner    (1001) docker     (127)     5046 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14584 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4057 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    32951 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2194 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/find_match_length.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24481 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5097 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_composite_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11250 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_forgetful_chain_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10413 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match64_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10349 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9414 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_quickly_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7226 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_rolling_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13081 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_to_binary_tree_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1875 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1401 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5839 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.c
--rw-rw-r--   0 runner    (1001) docker     (127)      916 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5630 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4358 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26659 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4051 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7642 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock_inc.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/params.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1969 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/prefix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7592 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/quality.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6009 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/ringbuffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3040 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/state.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21117 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.h
--rw-rw-r--   0 runner    (1001) docker     (127)   469710 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict_lut.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2269 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.c
--rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/enc/write_bits.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/
--rw-rw-r--   0 runner    (1001) docker     (127)      338 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/BUILD.bazel
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/WORKSPACE.bazel
--rw-rw-r--   0 runner    (1001) docker     (127)     1837 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/decode_fuzzer.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1073 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/run_decode_fuzzer.c
--rwxrwxr-x   0 runner    (1001) docker     (127)      703 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/test_fuzzer.sh
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/
--rw-rw-r--   0 runner    (1001) docker     (127)    16886 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/decode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    19841 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/encode.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11439 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/port.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/shared_dictionary.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2615 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/types.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)    51996 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4028 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)   215208 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/brotli-comparison-study-2015-09-22.pdf
--rw-rw-r--   0 runner    (1001) docker     (127)     5130 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.1
--rw-rw-r--   0 runner    (1001) docker     (127)      244 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.svg
--rw-rw-r--   0 runner    (1001) docker     (127)     1767 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/constants.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)    17452 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/decode.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)    24109 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/encode.h.3
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/docs/types.h.3
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/
--rw-rw-r--   0 runner    (1001) docker     (127)     6077 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/shared-brotli-fetch-spec.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/
--rw-rw-r--   0 runner    (1001) docker     (127)      176 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-01-download-rfc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      882 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-02-rfc-to-bin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      875 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-03-validate-bin.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2214 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-04-generate-java-literals.py
--rwxrwxr-x   0 runner    (1001) docker     (127)      283 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/download_testdata.sh
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlicommon.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlidec.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlienc.pc.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fast_float/
--rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fast_float/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/README
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
--rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/glob/glob/
--rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/httplib/
--rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/httplib/httplib.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
--rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
--rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
--rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
--rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
--rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/
--rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26144 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
--rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/
--rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
--rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
--rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
--rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
--rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
--rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3290 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
--rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
--rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
--rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
--rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
--rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
--rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
--rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniz/
--rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
--rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniz/LICENSE
--rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
--rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/nlohmann_json/
--rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pcg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pcg/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
--rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
--rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
--rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
--rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
--rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
--rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pyparse/
--rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/compile.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/logging.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/mix.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/prog.h
--rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/re2.h
--rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/set.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
--rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/utf.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/util.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/parse.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/prog.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/re2.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/rune.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/set.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/include/serd.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
--rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/base64.c
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/base64.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/env.c
--rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/n3.c
--rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/node.c
--rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/node.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/reader.c
--rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/reader.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/stack.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/string.c
--rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/system.c
--rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/system.h
--rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/try.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/uri.c
--rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
--rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/serd/src/writer.c
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
--rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
--rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
--rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
--rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
--rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
--rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
--rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
--rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
--rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
--rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
--rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)   154181 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
--rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
--rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
--rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
--rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
--rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
--rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
--rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
--rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
--rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
--rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
--rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
--rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/taywee_args/
--rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/taywee_args/include/
--rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/
--rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/include/
--rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
--rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
--rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
--rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/LICENSE
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
--rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
--rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
--rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
--rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
--rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
--rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
--rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
--rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
--rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
--rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
--rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-04-26 08:04:50.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/
--rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/CMakeLists.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/example/
--rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
--rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
--rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/benchmark/main.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/README.md
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/jni/
--rw-rw-r--   0 runner    (1001) docker     (127)    53634 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
--rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2944 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
--rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
--rw-rw-r--   0 runner    (1001) docker     (127)     9740 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
--rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2490 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
--rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
--rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
--rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
--rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2476 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
--rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
--rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/test.java
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/third_party/
--rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/build.js
--rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4452 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/install.js
--rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/package.js
--rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/package.json
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)     4337 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     5694 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3900 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2670 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4592 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    14213 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
--rw-rw-r--   0 runner    (1001) docker     (127)     9618 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4768 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
--rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
--rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
--rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
--rw-rw-r--   0 runner    (1001) docker     (127)     4244 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     2212 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
--rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
--rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
--rw-rw-r--   0 runner    (1001) docker     (127)     8686 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
--rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
--rw-rw-r--   0 runner    (1001) docker     (127)    11965 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
--rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
--rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
--rw-rw-r--   0 runner    (1001) docker     (127)     5730 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
--rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/
--rw-rw-r--   0 runner    (1001) docker     (127)     1295 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/Makefile
--rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/README.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
--rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
--rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1942 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1266 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
--rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
--rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
--rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
--rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
--rw-rw-r--   0 runner    (1001) docker     (127)     2211 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
--rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
--rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
--rw-rw-r--   0 runner    (1001) docker     (127)     9493 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
--rw-rw-r--   0 runner    (1001) docker     (127)     3949 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7556 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    18759 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3714 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    16191 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     7703 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     4295 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/
--rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6597 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
--rw-rw-r--   0 runner    (1001) docker     (127)     9393 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)    14470 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
--rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
--rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14438 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
--rw-rw-r--   0 runner    (1001) docker     (127)    24584 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2687 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_database.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
--rw-rw-r--   0 runner    (1001) docker     (127)    20051 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
--rw-rw-r--   0 runner    (1001) docker     (127)    24852 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_df_pyarrow.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2330 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
--rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
--rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3619 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_issue.py
--rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8471 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12717 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
--rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
--rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/
--rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
--rw-rw-r--   0 runner    (1001) docker     (127)     1099 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     5748 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/build.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
--rw-rw-r--   0 runner    (1001) docker     (127)     9633 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
-lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:52.864912 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     6642 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
--rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12920 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)    11961 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     2523 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    12498 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     9355 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
--rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
--rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/rust_api/update_version.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/
--rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    27728 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/include/
--rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
--rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
--rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
--rw-rw-r--   0 runner    (1001) docker     (127)     3257 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/
--rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/conftest.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/files/
--rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
--rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4790 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4811 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
--rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-04-26 08:04:50.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:04:53.600923 sdist/kuzu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-26 08:04:53.600923 sdist/kuzu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 08:04:53.604923 sdist/kuzu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:04:53.600923 sdist/kuzu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 08:04:53.600923 sdist/kuzu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:04:53.600923 sdist/kuzu.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-26 08:04:53.080915 sdist/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 08:04:49.184858 sdist/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-26 08:04:49.184858 sdist/setup.py
+drwx------   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:51.727048 sdist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-27 08:04:44.763043 sdist/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 08:04:46.215044 sdist/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-27 08:04:44.763043 sdist/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-27 08:04:46.215044 sdist/README_PYTHON_BUILD.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:49.847047 sdist/kuzu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:49.843047 sdist/kuzu-source/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5560 2024-04-27 08:04:47.000000 sdist/kuzu-source/.clang-format
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-27 08:04:47.000000 sdist/kuzu-source/.clang-tidy
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-27 08:04:47.000000 sdist/kuzu-source/.clang-tidy-analyzer
+-rw-rw-r--   0 runner    (1001) docker     (127)     1000 2024-04-27 08:04:47.000000 sdist/kuzu-source/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)       47 2024-04-27 08:04:47.000000 sdist/kuzu-source/.lcovrc
+-rw-rw-r--   0 runner    (1001) docker     (127)     8632 2024-04-27 08:04:47.000000 sdist/kuzu-source/CLA.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     8485 2024-04-27 08:04:47.000000 sdist/kuzu-source/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      632 2024-04-27 08:04:47.000000 sdist/kuzu-source/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-27 08:04:47.000000 sdist/kuzu-source/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-04-27 08:04:47.000000 sdist/kuzu-source/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     6365 2024-04-27 08:04:47.000000 sdist/kuzu-source/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     3881 2024-04-27 08:04:47.000000 sdist/kuzu-source/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26331 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy
+-rw-rw-r--   0 runner    (1001) docker     (127)     2085 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/antlr4/generate_grammar.cmake
+-rwxrwxr-x   0 runner    (1001) docker     (127)      299 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/check-include-guards.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)       76 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/check-no-std-assert.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2837 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/collect-single-file-header.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126290 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/c/Doxyfile
+-rw-rw-r--   0 runner    (1001) docker     (127)     4738 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/collect_files.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/
+-rw-rw-r--   0 runner    (1001) docker     (127)   126295 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/cpp/Doxyfile
+-rwxrwxr-x   0 runner    (1001) docker     (127)      225 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/generate-cpp-docs/doxygen.sh
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6998 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/get-clangd-diagnostics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/http-server.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2130 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/collect-results.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1585 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/multiplatform-test-helper/notify-discord.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/
+-rw-rw-r--   0 runner    (1001) docker     (127)       37 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     3276 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/README.md
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3277 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/package_tar.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/setup.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     4441 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/pip-package/setup.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12359 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/run-clang-format.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-27 08:04:47.000000 sdist/kuzu-source/scripts/update-nightly-build-version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2548 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/antlr4/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26331 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/antlr4/Cypher.g4
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/
+-rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      441 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1323 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18648 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      518 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_export_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5298 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_file_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32996 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3380 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_import_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11859 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_projection_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4787 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1490 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17249 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_updating_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/bind_use_database.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10625 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7684 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_rdf_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1613 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/copy/bind_copy_to.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/ddl/bind_create_rdf_graph.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3178 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5622 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_load_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3009 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_match.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1740 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind/read/bind_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2202 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_boolean_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3488 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3088 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_comparison_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16864 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1410 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1677 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_null_operator_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      926 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5174 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_subquery_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1531 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bind_expression/bind_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8729 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/binder_scope.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      585 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bound_statement_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bound_statement_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/bound_statement_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5982 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/expression_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/literal_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      576 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/parameter_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression/variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6470 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression_binder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5845 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/expression_visitor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)      350 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_delete_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      707 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_insert_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1963 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_merge_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/bound_set_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9670 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/query_graph.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6621 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/query/query_graph_label_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      261 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      742 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/match_clause_pattern_label_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2547 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/rewriter/with_clause_projection_rewriter.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/default_type_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/binder/visitor/property_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4034 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2689 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/data_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1412 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7841 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4402 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19820 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/c_api/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11101 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_content.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)      464 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1198 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1149 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/catalog_entry_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/function_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2023 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/node_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3144 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/rdf_graph_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_group_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4001 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/rel_table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/scalar_macro_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_entry/table_catalog_entry.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3041 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/catalog_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1483 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/catalog/property.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      810 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/arrow/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    24631 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_array_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10592 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_converter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_null_mask_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    35519 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_row_batch.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5340 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/arrow/arrow_type.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      478 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/case_insensitive_map.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      106 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/constants.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3078 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/csv_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/rdf_reader_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1727 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/copier_config/reader_config.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)      250 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      470 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2645 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12603 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/data_chunk/data_chunk_state.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/enums/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/enums/path_semantic.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      413 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/enums/rel_direction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/enums/rel_multiplicity.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/enums/table_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      182 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/exception/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2665 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/exception/message.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3201 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/expression_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      306 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/file_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/file_system/file_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/file_system/file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15233 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/file_system/local_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2726 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/file_system/virtual_file_system.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/in_mem_overflow_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/keyword_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      743 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/logging_level_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8157 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/md5.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      995 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/metric.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8989 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/null_mask.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/profiler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/random_engine.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/serializer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/serializer/buffered_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      948 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/serializer/buffered_serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/serializer/deserializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/serializer/serializer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1355 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5079 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/string_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      884 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/system_message.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      236 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/task_system/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2720 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/task_system/progress_bar.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/task_system/task.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/task_system/task_scheduler.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9755 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/type_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4772 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/blob.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19741 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/date_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6196 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/dtime_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19061 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/int128_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1174 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/internal_id_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17620 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/interval_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/ku_list.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2364 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/ku_string.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11000 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/timestamp_t.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    50966 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4363 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/uuid.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      512 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/nested.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      354 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/recursive_rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2799 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/rel.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    34391 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/types/value/value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2904 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/vector/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3350 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/vector/auxiliary_buffer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28649 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/vector/value_vector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/common/windows_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4615 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/case_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      965 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      885 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/expression_evaluator_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3490 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/function_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1130 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/literal_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1556 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/node_rel_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9766 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/path_evaluator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/expression_evaluator/reference_evaluator.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/extension/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/extension/extension.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1240 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      227 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3939 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/collect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1841 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/count.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1044 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/aggregate/count_star.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12187 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/aggregate_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      299 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2611 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/abs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5505 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/add.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5953 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/divide.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4379 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/modulo.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8121 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/multiply.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2427 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/negate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5848 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/arithmetic/subtract.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/array/
+-rw-rw-r--   0 runner    (1001) docker     (127)      210 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/array/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6098 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/array/array_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1328 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/array/array_value.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2494 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/base_lower_upper_operation.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20031 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/built_in_function_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/cast/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5405 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/cast/cast_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11953 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/cast/cast_rdf_variant.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    33753 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/cast_from_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2442 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/cast_string_non_nested_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8637 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/comparison_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5169 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/find_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12568 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/function_collection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/
+-rw-rw-r--   0 runner    (1001) docker     (127)      711 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2749 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_agg_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_any_value_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2620 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_append_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2166 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_concat_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1580 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_contains_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2235 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_creation.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_distinct_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2192 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1184 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_position_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2490 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_prepend_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3387 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_range_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1561 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_reverse_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3355 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_slice_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9697 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_sort_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_to_string_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2240 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/list_unique_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1904 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/list/size_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/map/
+-rw-rw-r--   0 runner    (1001) docker     (127)      283 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/map/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1095 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/map/map_creation_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/map/map_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      963 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/map/map_keys_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      955 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/map/map_values_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/path/
+-rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/path/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/path/nodes_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3870 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/path/properties_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/path/rels_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1997 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/path/semantic_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      186 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/pattern/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/pattern/id_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2683 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/scalar_macro_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/struct/
+-rw-rw-r--   0 runner    (1001) docker     (127)      229 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/struct/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2621 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/struct/struct_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/struct/struct_pack_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)      218 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2246 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/current_setting.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1390 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/db_version.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2672 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/show_attached_databases.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5816 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/show_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/show_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11017 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/storage_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4309 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call/table_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/call_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/table/scan_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/union/
+-rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/union/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      628 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/union/union_extract_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/union/union_tag_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1873 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/union/union_value_function.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/utility/
+-rw-rw-r--   0 runner    (1001) docker     (127)      183 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/utility/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3554 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/utility/coalesce.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18396 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_arithmetic_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_blob_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4267 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_boolean_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    47564 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_cast_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4887 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_date_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10069 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_hash_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_node_rel_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1516 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_null_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_rdf_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14671 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_string_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_timestamp_functions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/function/vector_uuid_functions.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12711 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2756 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/binder_scope.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      605 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      862 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_database_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      891 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1901 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_export_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      713 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_extension_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      877 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_import_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2466 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      787 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      348 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2666 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      661 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_transaction_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      356 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/bound_use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1071 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/bound_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/bound_file_scan_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1014 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/copy/index_look_up_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3274 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5498 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/ddl/bound_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1468 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4616 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2074 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/expression_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      878 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      786 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/node_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/node_rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      937 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1129 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/path_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2561 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4586 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/rel_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2112 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression/variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6057 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression_binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2678 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/expression_visitor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/bound_regular_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2487 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/normalized_query_part.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1013 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/normalized_single_query.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6508 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/query_graph.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/query_graph_label_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      482 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1010 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      869 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/reading_clause/bound_unwind_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3072 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      923 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/return_with_clause/bound_with_clause.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1445 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_delete_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1520 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_insert_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5606 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1570 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      797 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_set_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/bound_updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      163 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/query/updating_clause/update_table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/rewriter/
+-rw-rw-r--   0 runner    (1001) docker     (127)      515 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/rewriter/match_clause_pattern_label_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/rewriter/with_clause_projection_rewriter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      781 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/visitor/default_type_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1211 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/binder/visitor/property_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/c_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)       86 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/c_api/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51266 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/c_api/kuzu.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4801 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3631 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_content.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1769 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/catalog_entry_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1343 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/function_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/node_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2311 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rdf_graph_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_group_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2361 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/rel_table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/scalar_macro_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3199 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_entry/table_catalog_entry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1406 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/catalog_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/catalog/property.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/api.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1542 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1943 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1449 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_nullmask_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2921 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/arrow/arrow_row_batch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/assert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/case_insensitive_map.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/column_data_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9693 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/constants.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/csv_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/rdf_reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1302 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/copier_config/reader_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3648 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/copy_constructors.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1261 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1882 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/data_chunk_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1540 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/data_chunk/sel_vector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/alter_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/clause_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/conflict_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      194 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/delete_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/explain_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1221 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/expression_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/join_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      364 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/path_semantic.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/query_rel_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/rel_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      359 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/rel_multiplicity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/scan_source_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      938 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/statement_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      164 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/subquery_type.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      431 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/enums/table_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/binder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/catalog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      286 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/exception.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      282 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/interrupt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      265 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/io.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1260 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/message.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/not_implemented.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      307 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/overflow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/runtime.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      304 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/test.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      302 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/exception/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/file_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2076 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2043 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/local_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1814 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/file_system/virtual_file_system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2203 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/in_mem_overflow_buffer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/keyword/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1576 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/keyword/rdf_keyword.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/logging_level_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3271 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/md5.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/metric.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3921 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/mpsc_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1155 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/null_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9142 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/null_mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/profiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      349 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/random_engine.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/buffered_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1716 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/buffered_serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/deserializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2467 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/serializer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      237 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/serializer/writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2228 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/static_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3858 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/string_format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4653 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      596 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/system_message.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1469 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/progress_bar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3420 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/task.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3059 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/task_system/task_scheduler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1205 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/timer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11129 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/type_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1666 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/blob.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10927 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/cast_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4563 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/date_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2446 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/dtime_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6090 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/int128_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/internal_id_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4658 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/interval_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/ku_list.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2887 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/ku_string.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4667 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/timestamp_t.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21967 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/uuid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/
+-rw-rw-r--   0 runner    (1001) docker     (127)      319 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/nested.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1670 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1145 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      635 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/recursive_rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/rel.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21490 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/types/value/value.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1227 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/vector/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3218 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/vector/auxiliary_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13684 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/vector/value_vector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/common/windows_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2419 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/case_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/expression_evaluator_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1267 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/function_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/literal_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/node_rel_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2884 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/path_evaluator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/expression_evaluator/reference_evaluator.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/extension/
+-rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/extension/catalog_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1265 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/extension/extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      193 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/extension/extension_action.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3538 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/avg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1139 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/base_count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2409 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/collect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/count.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/count_star.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4106 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/min_max.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2918 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate/sum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6996 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/aggregate_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/abs.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/add.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5133 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/arithmetic_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      957 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/divide.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1109 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/modulo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/multiply.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/negate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/subtract.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4696 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/arithmetic/vector_arithmetic_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/array/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_cosine_similarity.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      824 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_distance.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/array/functions/array_inner_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2034 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/array/vector_array_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25289 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/binary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      828 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/decode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      402 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/encode_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/functions/octet_length_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/blob/vector_blob_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15140 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/boolean_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4678 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/boolean/vector_boolean_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3668 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/built_in_function_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/
+-rw-rw-r--   0 runner    (1001) docker     (127)      674 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/cast_function_bind_data.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7564 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_from_string_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13672 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      993 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_rdf_variant.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7994 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/cast_string_non_nested_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5149 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1795 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/functions/numeric_limits.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3693 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/cast/vector_cast_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/comparison/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2928 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/comparison/comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10062 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/comparison/vector_comparison_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/const_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/date/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4625 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/date/date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1236 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/date/vector_date_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2866 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/function_collection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/functions/md5_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      571 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/functions/sha256_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6058 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/hash_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/hash/vector_hash_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/interval/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/interval/interval_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2341 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/interval/vector_interval_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3521 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/base_list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_concat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1987 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_len_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_position_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_reverse_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1333 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_sort_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      436 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_to_string_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1231 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/functions/list_unique_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3221 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/list/vector_list_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      872 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/base_map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2268 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_creation_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1515 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_keys_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/functions/map_values_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/map/vector_map_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/null/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2772 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/null/null_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/null/null_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1154 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/null/vector_null_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/path/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6252 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/path/path_function_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/path/vector_path_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      791 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/pointer_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1299 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/rdf/rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      393 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/rdf/vector_rdf_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/rewrite_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10274 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/scalar_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1403 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/scalar_macro_function.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/offset_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      642 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/vector_label_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      529 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/schema/vector_node_rel_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2242 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/array_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      669 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_lower_upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2303 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      809 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_regexp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      429 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/base_str_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/contains_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/ends_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1459 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/find_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      575 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/initcap_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      656 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/left_operation.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1738 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/levenshtein_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      444 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/lower_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/lpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      765 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/ltrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      874 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/pad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3067 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_all_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1778 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_extract_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      476 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_full_match_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_matches_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/regexp_replace_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      640 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/repeat_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/reverse_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      673 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/right_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1035 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/rpad_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      664 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/rtrim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      401 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/starts_with_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2808 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/substr_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/trim_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/functions/upper_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5537 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/string/vector_string_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/struct/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/struct/vector_struct_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/table/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1702 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/table/bind_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/table/bind_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2912 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/table/call_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/table/scan_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/table/scan_replacement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4127 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/table_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    22251 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/ternary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/timestamp/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1036 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/timestamp/timestamp_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      508 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/timestamp/vector_timestamp_functions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10907 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/udf_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7936 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/unary_function_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/union/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/union/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1249 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/union/functions/union_tag.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      519 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/union/vector_union_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/utility/
+-rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/utility/scalar_utility_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/functions/
+-rw-rw-r--   0 runner    (1001) docker     (127)      395 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/functions/gen_random_uuid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/function/uuid/vector_uuid_functions.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)      780 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/attached_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1450 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/client_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6395 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/client_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7548 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5870 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      837 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/database_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/db_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1394 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/kuzu.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1248 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/kuzu_fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3548 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/plan_printer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1992 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4968 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1015 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/query_summary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6194 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/settings.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      830 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/storage_driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      528 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/main/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/acc_hash_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/agg_key_dependency_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/correlated_subquery_unnest_solver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3621 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/filter_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_collector.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6889 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/logical_operator_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      298 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2461 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/projection_push_down_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      572 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/remove_factorization_rewriter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      936 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/remove_unnecessary_join_optimizer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/optimizer/top_k_optimizer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      895 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/kuzu_cypher_parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_listener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/antlr_parser/parser_error_strategy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      468 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      541 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/copy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1237 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/database_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1748 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/alter_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      447 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/create_table_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/ddl/drop.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      358 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      748 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/explain_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3933 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_case_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3025 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2663 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_function_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_literal_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_parameter_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1688 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_property_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_subquery_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1546 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/expression/parsed_variable_expression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      626 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/extension_statement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_data/
+-rw-rw-r--   0 runner    (1001) docker     (127)      177 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_data/attach_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_expression_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2613 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/parsed_statement_visitor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      292 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/parser.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      975 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/port_db.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      946 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/node_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1100 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/pattern_element_chain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1599 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/graph_pattern/rel_pattern.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1309 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/query_part.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/in_query_call_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1521 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/load_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1212 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/match_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/reading_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      657 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/reading_clause/unwind_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      928 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/regular_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2155 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/projection_body.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/return_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/return_with_clause/with_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1798 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/single_query.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/
+-rw-rw-r--   0 runner    (1001) docker     (127)      898 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/delete_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      601 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/insert_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1341 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/merge_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/set_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/query/updating_clause/updating_clause.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1543 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/scan_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      712 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      568 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/transaction_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12939 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/transformer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      330 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/parser/visitor/statement_read_write_analyzer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2656 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/cardinality_estimator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      801 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/cost_model.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      469 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order/join_order_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/join_order_enumerator_context.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      754 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      841 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      920 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/ddl/logical_drop_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1426 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/base_logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1107 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/extend_direction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/logical_recursive_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      200 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/extend/recursive_join_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      442 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/factorization/flatten_resolver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      950 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/factorization/sink_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2011 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_accumulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2430 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1376 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1381 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_cross_product.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1632 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_distinct.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1603 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_explain.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_flatten.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3562 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_hash_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1843 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_limit.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1147 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_mark_accmulate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      769 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_multiplcity_reducer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1224 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_node_label_filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2156 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_partitioner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1176 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1179 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_plan_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1117 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_projection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1094 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      969 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1199 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_union.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1413 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/logical_unwind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1473 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_from.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1835 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2791 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2037 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3728 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2803 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/persistent/logical_set.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_dummy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_expressions_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_index_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1089 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_internal_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/scan/logical_scan_node_property.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6065 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/schema.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      915 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      757 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      953 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_simple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/simple/logical_use_database.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/sip/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1588 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/sip/logical_semi_masker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      308 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/operator/sip/side_way_info_passing.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16586 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/planner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3416 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/planner/subplans_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1252 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/data_pos.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/execution_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2051 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/expression_mapper.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11146 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/aggregate_input.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1824 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1374 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/base_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3698 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1905 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/hash_aggregate_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2811 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1565 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/aggregate/simple_aggregate_scan.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2956 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/call/in_query_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1382 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/call/standalone_call.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1712 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/comment_on.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2858 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/cross_product.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1402 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/alter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      779 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/create_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      945 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/ddl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      777 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/ddl/drop_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      583 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/empty_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2713 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/filter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      795 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/filtering_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1255 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/flatten.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4460 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4761 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/hash_join_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3299 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/hash_join/join_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2359 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/index_lookup.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1541 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/index_scan.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3204 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1057 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/intersect/intersect_build.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1208 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/limit.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1852 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/macro/create_macro.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5181 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/mask.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      972 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/multiplicity_reducer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7982 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/key_block_merger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1868 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1742 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_data_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6358 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_key_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2060 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2533 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/order_by_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/radix_sort.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2942 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/sort_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6218 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1694 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/order_by/top_k_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5655 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/partitioner.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2829 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      983 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_rdf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2150 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3177 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_csv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2821 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/copy_to_parquet.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1604 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6124 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/delete_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1005 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/file_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      734 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5440 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/index_builder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1163 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3808 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/insert_executor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2702 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/merge.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5761 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/node_batch_insert.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/base_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1831 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/driver.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1862 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/parallel_csv_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1888 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/csv/serial_csv_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1754 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/npy/npy_reader.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1480 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/boolean_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1616 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/callback_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5214 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1962 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/decode_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1358 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/interval_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/list_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4613 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_dbp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4702 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4238 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_rle_bp_decoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/parquet_timestamp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1842 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/resizable_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1327 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/string_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/struct_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3426 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/templated_column_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6781 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/parquet/thrift_tools.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5911 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7416 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/rdf_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2388 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/rdf/triple_store.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      865 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/reader/reader_bind_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4368 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/rel_batch_insert.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1938 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6617 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/set_executor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3914 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/basic_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2248 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/boolean_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4075 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/interval_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/list_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1087 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3213 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/parquet_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3898 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/standard_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5245 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/string_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/persistent/writer/parquet/struct_column_writer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5010 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/physical_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1356 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/profile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/projection.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2317 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/all_shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3932 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/bfs_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1693 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6229 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/frontier_scanner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4590 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/path_property_probe.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5296 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/recursive_join.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1380 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/scan_frontier.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/shortest_path_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1050 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/recursive_extend/variable_length_state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2908 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/result_collector.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1769 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_node_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2072 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_multi_rel_tables.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2322 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2495 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      840 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan/scan_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3474 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/scan_node_id.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5060 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/semi_masker.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/attach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/database_operator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      696 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/detach_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/export_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      690 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/import_db.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      941 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/install_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/load_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1297 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/simple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/simple/use_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/skip.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/ftable_scan_function.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3006 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/table_scan/union_all_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1095 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1499 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/operator/unwind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      388 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/physical_plan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12402 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/plan_mapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/processor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/processor_task.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1737 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/base_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16636 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/factorized_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1187 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/flat_tuple.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1061 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/mark_hash_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1547 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/result_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1063 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/processor/result/result_set_descriptor.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)     9450 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13079 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/buffer_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      527 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/locked_queue.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2759 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/memory_manager.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1714 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/buffer_manager/vm_region.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)    15859 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/compression/compression.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1695 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/compression/sign_extend.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3328 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/file_handle.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14432 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1141 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index_header.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2132 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index_slot.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/hash_index_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6182 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/index/in_mem_hash_index.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2514 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3159 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1052 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_storage.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9234 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/local_storage/local_table.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      999 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/metadata_dah_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3254 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/node_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4474 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/nodes_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1594 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/property_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3873 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/rel_table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3236 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/rels_store_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4426 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      821 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_extension.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2909 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2297 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/db_file_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/disk_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      368 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/in_mem_page.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4969 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_structure/overflow_file.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7895 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      774 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/storage_version_info.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4852 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1626 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/chunked_node_group_collection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13745 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9626 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2508 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/dictionary_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3021 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/dictionary_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6067 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/list_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3534 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/list_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6203 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/node_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/node_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2562 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/null_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8048 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/rel_table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12551 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/rel_table_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/string_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2511 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/string_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3337 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/struct_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1968 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/struct_column_chunk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/table.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2638 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/store/table_data.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3663 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal/wal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8162 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal/wal_record.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2356 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal_replayer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/storage/wal_replayer_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1893 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      294 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction_action.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction_context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3747 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/include/transaction/transaction_manager.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/
+-rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20127 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/client_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3262 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11677 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2577 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/database_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1225 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/db_config.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13980 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/plan_printer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      956 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      578 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/query_summary.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/storage_driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      317 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/main/version.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      602 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10541 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/acc_hash_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3540 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/agg_key_dependency_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1488 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/correlated_subquery_unnest_solver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10339 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12065 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/filter_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      340 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/logical_operator_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5558 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/logical_operator_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2087 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13109 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/projection_push_down_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/remove_factorization_rewriter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1537 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/remove_unnecessary_join_optimizer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1902 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/optimizer/top_k_optimizer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/
+-rw-rw-r--   0 runner    (1001) docker     (127)      267 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/kuzu_cypher_parser.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1391 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_listener.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      827 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/antlr_parser/parser_error_strategy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      455 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/create_macro.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/expression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      346 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/expression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_case_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3281 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      785 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_function_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_property_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      491 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/expression/parsed_variable_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3506 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/parsed_expression_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4399 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/parsed_statement_visitor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1259 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/
+-rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      450 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3602 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7632 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      392 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27904 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_expression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      858 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7789 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_graph_pattern.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1272 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      833 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2587 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2253 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2715 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_reading_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1209 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2681 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_updating_clause.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transform/transform_use_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4493 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/transformer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/visitor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/visitor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/parser/visitor/statement_read_write_analyzer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/
+-rw-rw-r--   0 runner    (1001) docker     (127)      339 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5776 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/cardinality_estimator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1652 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/cost_model.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      745 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/join_order/join_order_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/join_order_enumerator_context.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1025 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      175 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/ddl/logical_ddl.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/base_logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/logical_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2914 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/extend/logical_recursive_extend.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/
+-rw-rw-r--   0 runner    (1001) docker     (127)      223 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1007 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/flatten_resolver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2591 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/factorization/sink_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1552 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2870 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      517 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      523 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      829 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1523 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      764 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7224 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      726 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1039 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1514 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6276 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2805 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      939 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_partitioner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1065 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_plan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3973 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_plan_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2197 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      980 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/logical_unwind.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1732 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2031 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1366 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2384 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/persistent/logical_set.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      328 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      347 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_index_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      643 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_internal_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/scan/logical_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5973 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/schema.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      185 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/simple/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/operator/simple/logical_simple.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      814 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1971 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      399 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13525 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      913 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      800 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      740 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2692 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4805 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      552 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      658 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      439 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      684 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1596 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2066 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6469 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      826 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/append_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8216 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_copy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27166 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_join_order.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_port_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3074 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5987 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_read.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1829 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_single_query.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8673 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_subquery.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6119 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/plan/plan_update.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5305 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/query_planner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3769 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/planner/subplans_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      272 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1486 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4774 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/create_factorized_table_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/create_result_collector.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8285 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/expression_mapper.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      702 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_acc_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1102 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9380 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1046 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15120 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_copy_from.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4729 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_cross_product.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6221 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      750 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_distinct.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_dummy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1956 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_explain.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1871 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_expressions_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6300 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      822 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      606 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_flatten.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5998 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_hash_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1217 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2425 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_index_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5186 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3182 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      933 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_label_filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_limit.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      784 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_mark_accumulate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2627 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      533 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_multiplicity_reducer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4327 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6873 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1251 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_projection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3425 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_recursive_extend.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1457 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      816 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1090 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_node.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3525 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_scan_node_property.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_semi_masker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6610 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4721 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      970 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      593 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2083 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_union.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1096 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/map_unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8345 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/map/plan_mapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    36724 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/aggregate_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1691 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      755 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/base_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5470 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/hash_aggregate_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4848 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1344 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/aggregate/simple_aggregate_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2958 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/in_query_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/call/standalone_call.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      803 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/comment_on.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1383 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/cross_product.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/
+-rw-rw-r--   0 runner    (1001) docker     (127)      256 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2464 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/alter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/create_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/ddl.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/ddl/drop_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/empty_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2463 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/filter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1043 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/filtering_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1306 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/flatten.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2057 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_build.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8290 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/hash_join_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9252 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/hash_join/join_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4502 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/index_lookup.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/index_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/intersect/
+-rw-rw-r--   0 runner    (1001) docker     (127)      208 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/intersect/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     9664 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/intersect/intersect.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1389 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/limit.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/macro/
+-rw-rw-r--   0 runner    (1001) docker     (127)      217 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/macro/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      727 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/macro/create_macro.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/multiplicity_reducer.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/
+-rw-rw-r--   0 runner    (1001) docker     (127)      410 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    16047 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/key_block_merger.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1082 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14058 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_key_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1554 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1438 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/order_by_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12968 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/radix_sort.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9014 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/sort_state.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/order_by/top_k_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7795 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/partitioner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/
+-rw-rw-r--   0 runner    (1001) docker     (127)      579 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      473 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_rdf.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      760 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8388 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_csv.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1782 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/copy_to_parquet.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/delete.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5443 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/delete_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4759 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/index_builder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      861 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7316 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/insert_executor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3038 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/merge.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11841 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/node_batch_insert.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/
+-rw-rw-r--   0 runner    (1001) docker     (127)      325 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    14378 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/base_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4367 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/driver.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8564 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/parallel_csv_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6543 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/csv/serial_csv_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13915 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      445 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      850 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/boolean_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    24072 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/interval_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5995 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/list_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    30027 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_timestamp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3928 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/string_column_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3449 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/struct_column_reader.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/
+-rw-rw-r--   0 runner    (1001) docker     (127)      254 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13988 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_reader.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13452 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2966 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/rdf/rdf_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2052 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/reader/reader_bind_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11285 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/rel_batch_insert.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      997 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6592 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/set_executor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    12826 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/basic_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1538 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/boolean_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16464 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1539 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/interval_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4734 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/list_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2633 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_rle_bp_encoder.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11697 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/parquet_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8703 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/string_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4078 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/persistent/writer/parquet/struct_column_writer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8457 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/physical_operator.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/profile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1757 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/projection.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/
+-rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      790 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7361 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/frontier_scanner.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5067 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/path_property_probe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12987 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/recursive_join.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/recursive_extend/scan_frontier.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2479 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/result_collector.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      323 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      825 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_node_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3865 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_multi_rel_tables.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      625 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      651 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan/scan_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5110 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/scan_node_id.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4582 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/semi_masker.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1378 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/attach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/detach_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4054 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/export_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/import_db.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2423 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/install_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2205 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/load_extension.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      638 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/simple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/simple/use_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2403 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/skip.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/
+-rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2486 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/ftable_scan_function.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1832 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/table_scan/union_all_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1256 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/transaction.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2659 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/operator/unwind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2709 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/processor.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1788 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/processor_task.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/
+-rw-rw-r--   0 runner    (1001) docker     (127)      336 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7142 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/base_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    34515 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/factorized_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2119 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/flat_tuple.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2304 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/mark_hash_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/result_set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1170 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/processor/result/result_set_descriptor.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      537 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/
+-rw-rw-r--   0 runner    (1001) docker     (127)      277 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7039 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/bm_file_handle.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    15692 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/buffer_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2145 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/memory_manager.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3721 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/buffer_manager/vm_region.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/compression/
+-rw-rw-r--   0 runner    (1001) docker     (127)      258 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/compression/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35327 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/compression/compression.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1880 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/file_handle.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/index/
+-rw-rw-r--   0 runner    (1001) docker     (127)      209 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/index/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    31321 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/index/hash_index.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13455 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/index/in_mem_hash_index.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      279 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6131 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12393 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_storage.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6966 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/local_storage/local_table.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/
+-rw-rw-r--   0 runner    (1001) docker     (127)      415 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1201 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/metadata_dah_info.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7957 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/node_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4352 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/nodes_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2458 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/property_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5129 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/rel_table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4017 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/rels_store_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/table_statistics.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5914 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/stats/table_statistics_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10057 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/
+-rw-rw-r--   0 runner    (1001) docker     (127)      263 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5262 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/db_file_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    23949 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/disk_array.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      557 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/in_mem_page.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9909 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_structure/overflow_file.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4286 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_utils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      737 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/storage_version_info.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/
+-rw-rw-r--   0 runner    (1001) docker     (127)      649 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6931 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/chunked_node_group.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2126 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/chunked_node_group_collection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    44319 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    27639 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3687 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/dictionary_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10644 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/dictionary_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    23851 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/list_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16099 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/list_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9759 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/node_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10288 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/node_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8500 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/null_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8480 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/rel_table.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    50483 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/rel_table_data.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11794 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/string_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7831 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/string_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12282 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/struct_column.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6206 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/struct_column_chunk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/store/table_data.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/wal/
+-rw-rw-r--   0 runner    (1001) docker     (127)      191 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/wal/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     6531 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/wal/wal.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6783 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/wal/wal_record.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16642 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/wal_replayer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1078 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/storage/wal_replayer_utils.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/transaction/
+-rw-rw-r--   0 runner    (1001) docker     (127)      216 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/transaction/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3894 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/transaction/transaction_context.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4629 2024-04-27 08:04:47.000000 sdist/kuzu-source/src/transaction/transaction_manager.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)      489 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/
+-rw-rw-r--   0 runner    (1001) docker     (127)      949 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    56662 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_lexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   469845 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3272 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_lexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    88283 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10564 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     4237 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8375 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5269 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      552 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1018 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRFileStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4326 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2623 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ANTLRInputStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1804 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2483 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BailErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1163 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1377 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BaseErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9946 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8014 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/BufferedTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      281 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1479 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4459 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4918 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1327 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2564 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenFactory.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1767 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2713 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/CommonTokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      597 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1060 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ConsoleErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    11864 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20289 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DefaultErrorStrategy.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3484 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3600 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/DiagnosticErrorListener.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2152 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Exceptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1096 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FailedPredicateException.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2767 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashMap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2676 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/FlatHashSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      559 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      783 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InputMismatchException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      350 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10251 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/IntStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      615 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1604 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/InterpreterRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6878 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7038 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Lexer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1867 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1564 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1234 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      916 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/LexerNoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2412 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3795 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ListTokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1585 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1693 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/NoViableAltException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19305 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    19393 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Parser.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    10523 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7171 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserInterpreter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3952 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5666 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ParserRuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1958 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1657 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/ProxyErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1916 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3961 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RecognitionException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4572 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5733 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Recognizer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3588 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5561 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      725 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      985 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuleContextWithAltNum.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2091 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7393 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/RuntimeMetaData.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      246 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3462 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Token.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1217 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenFactory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      264 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3839 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenSource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      284 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6098 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15023 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12507 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/TokenStreamRewriter.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5847 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4351 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedCharStream.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7467 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4241 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/UnbufferedTokenStream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2105 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Version.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1907 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6943 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/Vocabulary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      270 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      676 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/WritableToken.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5524 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/antlr4-runtime.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4193 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4845 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATN.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4158 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5513 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6500 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5185 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1252 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1302 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializationOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21573 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      835 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNDeserializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1216 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2761 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1538 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4374 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNState.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      990 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      796 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNStateType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      439 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ATNType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1214 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1104 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ActionTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      604 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3295 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AmbiguityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4211 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1900 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ArrayPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      840 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1084 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/AtomTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      729 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      649 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BasicState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      853 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/BlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      520 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2123 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ContextSensitivityInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      561 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2459 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      934 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9762 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      342 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      960 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/DecisionState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      969 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1402 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/EpsilonTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      527 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1861 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ErrorInfo.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      416 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/HashUtils.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7271 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3275 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LL1Analyzer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2950 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1666 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNConfig.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    22025 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8819 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      324 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3494 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4031 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6150 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionExecutor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerActionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1306 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1908 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerChannelAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1555 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2772 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1784 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3046 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerIndexedCustomAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1780 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1701 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerMoreAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1010 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1735 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPopModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1311 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1817 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerPushModeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      977 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1664 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerSkipAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1269 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1717 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LexerTypeAction.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      584 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1914 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LookaheadEventInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      736 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/LoopEndState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      868 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      854 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/NotSetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      484 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/OrderedATNConfigSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2789 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3665 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParseInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    53167 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    45705 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulator.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2278 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ParserATNSimulatorOptions.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1052 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      842 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PlusLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      901 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1187 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PrecedencePredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      685 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2885 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateEvalInfo.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1009 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1674 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredicateTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20987 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9173 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2360 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2738 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5386 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4033 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCache.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2602 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextMergeCacheOptions.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionContextType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5939 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    20991 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/PredictionMode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7943 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2982 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/ProfilingATNSimulator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      891 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      944 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RangeTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      746 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleStopState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1156 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1484 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/RuleTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    14979 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9030 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContext.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      451 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SemanticContextType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3246 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SerializedATNView.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      898 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1267 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SetTransition.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2870 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1834 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/SingletonPredictionContext.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      754 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarBlockStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopEntryState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      644 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      733 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/StarLoopbackState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      762 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TokensStartState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      911 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2164 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/Transition.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      778 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/TransitionType.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      680 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      839 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/atn/WildcardTransition.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2868 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3045 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFA.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1726 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      772 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFASerializer.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1490 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6068 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/DFAState.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      509 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      533 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/dfa/LexerDFASerializer.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2694 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5499 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/internal/Synchronization.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3098 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      989 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/InterpreterDataReader.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1671 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3009 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Interval.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    13209 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6478 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/IntervalSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2820 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3595 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/MurmurHash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       71 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      446 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/misc/Predicate.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/
+-rw-rw-r--   0 runner    (1001) docker     (127)      242 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      370 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Any.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      966 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3620 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Arrays.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1828 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/BitSet.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4837 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2582 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/CPPUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1195 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Casts.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4122 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Declarations.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      425 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/StringUtils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Unicode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8728 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2148 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/support/Utf8.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5650 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/AbstractParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      677 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1255 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1429 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ErrorNodeImpl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1906 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2124 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/IterativeParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      349 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4224 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      288 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1213 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1434 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeProperty.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeType.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2212 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeVisitor.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1381 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2031 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/ParseTreeWalker.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1145 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNode.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1281 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1003 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/TerminalNodeImpl.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6872 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3060 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/Trees.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1460 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/Chunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1868 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5768 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreeMatch.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1800 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4384 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePattern.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    12574 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     8715 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/ParseTreePatternMatcher.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1820 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4742 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/RuleTagToken.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      811 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3030 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TagChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1464 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TextChunk.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      959 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2786 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/pattern/TokenTagToken.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     4960 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2824 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPath.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      747 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1029 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathElement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6047 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.g4
+-rw-rw-r--   0 runner    (1001) docker     (127)     1349 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       98 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexer.tokens
+-rwxrwxr-x   0 runner    (1001) docker     (127)      506 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      635 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathLexerErrorListener.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      709 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      966 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      620 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathRuleElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      647 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      631 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1054 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      623 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathTokenElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      665 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      558 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardAnywhereElement.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      621 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)      542 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/antlr4_runtime/src/tree/xpath/XPathWildcardElement.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5677 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12841 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1633 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1084 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)      652 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/README
+-rw-rw-r--   0 runner    (1001) docker     (127)     4099 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      314 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/SECURITY.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)      621 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     8011 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/constants.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7965 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/context.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4666 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/context.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   122784 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin
+-rw-rw-r--   0 runner    (1001) docker     (127)    51687 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.bin.br
+-rw-rw-r--   0 runner    (1001) docker     (127)   472009 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1951 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    18385 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/platform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17424 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2413 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/shared_dictionary_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10677 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3209 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/transform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1723 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/common/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2285 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    14854 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/bit_reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   103991 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/decode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    11996 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/huffman.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    31612 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/prefix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5659 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    12546 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/dec/state.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5673 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1301 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36639 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3868 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_hq.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8181 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/backward_references_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1685 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4109 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/bit_cost_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1137 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_encoder_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7395 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1674 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18673 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/block_splitter_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    50750 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3477 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/brotli_bit_stream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1485 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11826 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/cluster_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1019 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     6892 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/command.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6645 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2493 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compound_dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    33255 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3598 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27182 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2879 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/compress_fragment_two_pass.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   147154 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      646 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/dictionary_hash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    77547 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/encode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    23290 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     5046 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/encoder_dict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14584 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4057 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    32951 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/entropy_encode_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6024 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/fast_log.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2194 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/find_match_length.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24481 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5097 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_composite_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11250 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_forgetful_chain_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10413 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match64_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10349 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9414 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_longest_match_quickly_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7226 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_rolling_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13081 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/hash_to_binary_tree_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1875 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1401 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/histogram_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5839 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      916 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/literal_cost.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5630 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4358 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/memory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26659 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4051 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7642 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/metablock_inc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1169 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/params.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1969 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/prefix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7592 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/quality.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6009 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/ringbuffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3040 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/state.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21117 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1275 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   469710 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/static_dict_lut.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2269 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      905 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/utf8_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/enc/write_bits.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/
+-rw-rw-r--   0 runner    (1001) docker     (127)      338 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/BUILD.bazel
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/WORKSPACE.bazel
+-rw-rw-r--   0 runner    (1001) docker     (127)     1837 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/decode_fuzzer.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1073 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/run_decode_fuzzer.c
+-rwxrwxr-x   0 runner    (1001) docker     (127)      703 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/fuzz/test_fuzzer.sh
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/
+-rw-rw-r--   0 runner    (1001) docker     (127)    16886 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/decode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    19841 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/encode.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11439 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/port.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3535 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/shared_dictionary.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2615 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/include/brotli/types.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51996 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4028 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/c/tools/brotli.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)   215208 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/brotli-comparison-study-2015-09-22.pdf
+-rw-rw-r--   0 runner    (1001) docker     (127)     5130 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.1
+-rw-rw-r--   0 runner    (1001) docker     (127)      244 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/brotli.svg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1767 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/constants.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)    17452 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/decode.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)    24109 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/encode.h.3
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/docs/types.h.3
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)     6077 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/fetch-spec/shared-brotli-fetch-spec.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/
+-rw-rw-r--   0 runner    (1001) docker     (127)      176 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      375 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-01-download-rfc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      882 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-02-rfc-to-bin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      875 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-03-validate-bin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2214 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/dictionary/step-04-generate-java-literals.py
+-rwxrwxr-x   0 runner    (1001) docker     (127)      283 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/download_testdata.sh
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlicommon.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlidec.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      300 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/brotli/scripts/libbrotlienc.pc.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/
+-rw-rw-r--   0 runner    (1001) docker     (127)       92 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    94376 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fast_float/include/fast_float.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)      150 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    10273 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)     1278 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/README
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/
+-rw-rw-r--   0 runner    (1001) docker     (127)    59414 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32124 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpacking.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23572 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/bitpackinghelpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      273 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/fastpfor/fastpfor/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/glob/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/glob/glob/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13001 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/glob/glob/glob.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/httplib/
+-rw-rw-r--   0 runner    (1001) docker     (127)   311527 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/httplib/httplib.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)      918 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11358 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26550 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15024 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/aria.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25694 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/asn1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3085 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42463 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/bignum.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2394 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/build_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13062 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/camellia.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25326 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/ccm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    38245 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/check_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51905 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/cipher.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1452 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/constant_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11057 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/des.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9867 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/entropy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7031 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/error.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    16632 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/gcm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      531 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/mbedtls_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17120 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/md.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4949 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/memory_buffer_alloc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41167 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/oid.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5270 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    35543 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/pk.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14433 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1973 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_time.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8667 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/platform_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      978 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/private_access.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    51957 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/rsa.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7854 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha1.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6640 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7084 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/include/mbedtls/sha512.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/
+-rw-rw-r--   0 runner    (1001) docker     (127)    73166 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/aes.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    36996 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/aria.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11007 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/asn1parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6762 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/base64.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    79733 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/bignum.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    56414 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/bn_mul.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36100 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/camellia.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    47452 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    49271 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4532 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/cipher_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17543 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26144 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    12167 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1638 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/constant_time_invasive.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18774 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6513 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2139 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/entropy_poll.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    34742 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/gcm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    21294 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/md.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2086 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/md_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27822 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/oid.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14294 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pem.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    17719 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pk.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    29099 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4205 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pk_wrap.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44156 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/pkparse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/platform_util.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    69416 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13253 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     8442 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/rsa_alt_helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15171 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/sha1.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16212 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/sha256.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18253 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/mbedtls/library/sha512.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1079 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       46 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)      976 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)     1879 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/
+-rw-rw-r--   0 runner    (1001) docker     (127)      320 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      406 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_constants.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   200148 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    72715 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/parquet_types.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/parquet/windows_compatibility.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9816 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3296 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7266 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-sinksource.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1837 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15040 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-internal.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     2900 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy-stubs-public.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    59102 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.cc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9748 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/snappy/snappy.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3555 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TApplicationException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1208 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TBase.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6849 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TLogging.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3185 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/TToString.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3290 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/Thrift.h
+-rw-rw-r--   0 runner    (1001) docker     (127)       65 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/config.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/
+-rwxrwxr-x   0 runner    (1001) docker     (127)     7931 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23953 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TCompactProtocol.tcc
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1140 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    21319 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocol.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     6374 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolDecorator.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3216 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1151 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TProtocolTypes.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)    18266 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/protocol/TVirtualProtocol.h
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/stdcxx.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      896 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift-config.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)      460 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/thrift_export.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4624 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/PlatformSocket.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3699 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    15004 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TBufferTransports.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     9004 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransport.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1862 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)     3335 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TTransportException.h
+-rwxrwxr-x   0 runner    (1001) docker     (127)     5167 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniparquet/src/thrift/transport/TVirtualTransport.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniz/
+-rw-rw-r--   0 runner    (1001) docker     (127)      192 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniz/CMakeLists.txt
+-rwxrwxr-x   0 runner    (1001) docker     (127)     1184 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniz/LICENSE
+-rwxrwxr-x   0 runner    (1001) docker     (127)   313123 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniz/miniz.cpp
+-rwxrwxr-x   0 runner    (1001) docker     (127)    66103 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniz/miniz.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5058 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/miniz/miniz_wrapper.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/nlohmann_json/
+-rw-rw-r--   0 runner    (1001) docker     (127)   907860 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/nlohmann_json/json.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6268 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/nlohmann_json/json_fwd.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pcg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1092 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pcg/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    20241 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pcg/pcg_extras.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    73551 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pcg/pcg_random.hpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    24875 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pcg/pcg_uint128.hpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11983 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1684 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/
+-rw-rw-r--   0 runner    (1001) docker     (127)    23979 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7069 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    65560 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8458 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      120 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2096 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 runner    (1001) docker     (127)    28251 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    52330 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5491 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17932 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    26305 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    42266 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 runner    (1001) docker     (127)    31418 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18120 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      316 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11889 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5002 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8262 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8862 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79412 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9103 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   126075 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    93433 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4185 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    15337 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    27013 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/include/pybind11/stl_bind.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2350 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)    11103 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)      817 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/JoinPaths.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     1423 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/check-style.sh
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1040 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/libsize.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1282 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      196 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (127)    13487 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     6930 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     8957 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)     8361 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 runner    (1001) docker     (127)       94 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2104 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pybind11/tools/setup_main.py.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pyparse/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4660 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/pyparse/pyparse.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1558 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (127)    12166 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/bitstate.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40923 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/compile.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    77669 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/dfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3379 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/filtered_re2.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2794 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/bitmap256.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4074 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/filtered_re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3685 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/logging.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1027 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/mix.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4596 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1051 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/pod_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4107 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/prefilter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5397 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/prefilter_tree.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20055 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/prog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    41735 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/re2.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    25053 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/regexp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2528 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12285 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/sparse_array.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7425 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/sparse_set.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6625 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/stringpiece.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      644 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/strutil.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/unicode_casefold.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1595 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/unicode_groups.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1575 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/utf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7825 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/include/walker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6308 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/mimics_pcre.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22890 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/nfa.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22239 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/onepass.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    81544 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/parse.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3448 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/perl_groups.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18698 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/prefilter.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13255 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/prefilter_tree.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    40537 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/prog.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    42418 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/re2.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28640 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/regexp.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5872 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/rune.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4636 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/set.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    20853 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/simplify.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2118 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/stringpiece.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5691 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/strutil.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9029 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/tostring.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    13413 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/unicode_casefold.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   122482 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/re2/unicode_groups.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1247 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    33294 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/include/serd.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1424 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/BSD-3-Clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      660 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/LICENSES/OBSD.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      555 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/attributes.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3172 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/base64.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/base64.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1966 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/byte_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2643 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/byte_source.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3444 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/byte_source.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6676 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/env.c
+-rw-rw-r--   0 runner    (1001) docker     (127)    46487 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/n3.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     9699 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/node.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      871 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/node.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12064 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/reader.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     4376 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/reader.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3187 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/serd_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      730 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/serd_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    10745 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/serdi.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2552 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/stack.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3507 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/string.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     3394 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/string_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1233 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/system.c
+-rw-rw-r--   0 runner    (1001) docker     (127)      650 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/system.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/try.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11749 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/uri.c
+-rw-rw-r--   0 runner    (1001) docker     (127)     2843 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/uri_utils.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    36427 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/serd/src/writer.c
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1348 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4021 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2817 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2560 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/async_logger.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/argv.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      986 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/env.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3170 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/cfg/helpers.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2050 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13194 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/common.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2004 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1165 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/backtracer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3349 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/circular_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      603 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/console_globals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4707 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1758 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/file_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4471 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/fmt_helper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1396 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1204 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1668 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      935 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/log_msg_buffer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5285 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/mpmc_blocking_q.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      930 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/null_mutex.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    17897 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3922 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1756 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/periodic_worker.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8695 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4013 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/registry.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      751 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/synchronous_factory.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4252 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3885 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/tcp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4275 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3519 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/thread_pool.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3134 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client-windows.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2237 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/udp_client.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      188 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/details/windows_include.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7380 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bin_to_hex.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/
+-rw-rw-r--   0 runner    (1001) docker     (127)     7420 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/args.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    68076 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    24896 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/color.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    21245 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   111215 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/core.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1408 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/fmt.license.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    74272 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)   154181 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/format.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      100 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/locale.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14123 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/os.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ostream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    20023 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/printf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    23218 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4880 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9001 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/bundled/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/chrono.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      559 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/compile.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1042 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/fmt.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ostr.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      551 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/ranges.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/std.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      548 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fmt/xchar.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      463 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/formatter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      305 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/fwd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6725 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13412 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/logger.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    44468 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3758 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/pattern_formatter.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4777 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/android_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4875 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3959 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ansicolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1808 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1568 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/base_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1216 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2295 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/basic_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1705 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/callback_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9452 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/daily_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2373 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dist_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3243 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/dup_filter_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     7121 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/hourly_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/kafka_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4003 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/mongo_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2049 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/msvc_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1234 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/null_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1222 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ostream_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12408 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/qt_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/ringbuffer_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4917 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3229 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/rotating_file_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      725 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      893 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1435 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1792 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_color_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4347 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2429 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/stdout_sinks.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4239 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/syslog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4872 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/systemd_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2127 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/tcp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1858 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/udp_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     8888 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/win_eventlog_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6651 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2716 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/sinks/wincolor_sink.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3118 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog-inl.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    11771 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/spdlog.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1711 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/stopwatch.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6360 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/tweakme.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      417 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/spdlog/spdlog/version.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1105 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)   152995 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/taywee_args/include/args.hxx
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/
+-rw-rw-r--   0 runner    (1001) docker     (127)      142 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     5125 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/LICENSE.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)    32757 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc.h
+-rw-rw-r--   0 runner    (1001) docker     (127)  1944550 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_data.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      888 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/include/utf8proc_wrapper.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    37876 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4483 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/utf8proc/utf8proc_wrapper.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1529 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/LICENSE
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)     8580 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/entropy_common.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2982 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/error_private.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    10089 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/fse_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    28008 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/xxhash.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2721 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/common/zstd_common.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    26469 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/fse_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7555 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/hist.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    32726 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/huf_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)   183732 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     6293 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_literals.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    19309 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_sequences.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    43614 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_compress_superblock.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25428 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_double_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    22459 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_fast.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    52956 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_lazy.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    25024 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_ldm.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    55766 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/compress/zstd_opt.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)    51287 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/huf_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     9136 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_ddict.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    83312 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    61618 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/decompress/zstd_decompress_block.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/
+-rw-rw-r--   0 runner    (1001) docker     (127)    17857 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/bitstream.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5734 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/compiler.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3893 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/debug.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2396 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/error_private.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14574 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18012 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/fse_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4717 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    14332 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/huf_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    12217 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/mem.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9897 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1779 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/xxhash_static.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3730 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_errors.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    13604 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/common/zstd_internal.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3464 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/hist.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    46030 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1262 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_literals.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2210 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_sequences.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1194 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_compress_superblock.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    18777 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_cwksp.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_double_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1171 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_fast.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2701 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_lazy.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     4010 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_ldm.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1972 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/compress/zstd_opt.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1329 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_ddict.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2081 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_block.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     6147 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    61165 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    60974 2024-04-27 08:04:47.000000 sdist/kuzu-source/third_party/zstd/include/zstd_static.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/
+-rw-rw-r--   0 runner    (1001) docker     (127)      297 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/CMakeLists.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3132 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/benchmark.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3400 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/benchmark_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/example/
+-rw-rw-r--   0 runner    (1001) docker     (127)       73 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/example/example.benchmark
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      994 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/benchmark.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      561 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_config.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      836 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/include/benchmark_runner.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2195 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/benchmark/main.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1846 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      332 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/README.md
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/jni/
+-rw-rw-r--   0 runner    (1001) docker     (127)    53634 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/jni/kuzu_java.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4861 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuConnection.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3587 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataType.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDataTypeID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2944 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuDatabase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1734 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuFlatTuple.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      495 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuInternalID.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     9740 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuNative.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      334 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuObjectRefDestroyedException.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2490 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuPreparedStatement.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5236 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQueryResult.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      853 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuQuerySummary.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4622 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValue.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1077 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueListUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2984 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueNodeUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1034 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRdfVariantUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1024 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRecursiveRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3397 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueRelUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuValueStructUtil.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      520 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/KuzuVersion.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      178 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/main/java/com/kuzudb/package-info.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11911 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ConnectionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     5025 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DataTypeTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1946 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/DatabaseTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ExtensionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/FlatTupleTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2476 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/PreparedStatementTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     4789 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/QueryResultTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      940 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestBase.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2504 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/TestHelper.java
+-rw-rw-r--   0 runner    (1001) docker     (127)    45229 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/ValueTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/src/test/java/com/kuzudb/test/VersionTest.java
+-rw-rw-r--   0 runner    (1001) docker     (127)     2271 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/test.java
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/third_party/
+-rw-rw-r--   0 runner    (1001) docker     (127)  2614186 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/java_api/third_party/junit-platform-console-standalone-1.9.3.jar
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1777 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     3043 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      397 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/build.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      615 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/clean.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4452 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/install.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     5577 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/package.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      672 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/package.json
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4337 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1625 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1635 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     5694 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/include/node_util.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/main.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3900 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2670 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2110 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4592 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    14213 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_cpp/node_util.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/
+-rw-rw-r--   0 runner    (1001) docker     (127)     9618 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4768 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      499 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/index.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      686 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/kuzu_native.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      238 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/logging_level.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     1210 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/prepared_statement.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     4244 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/src_js/query_result.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2212 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/common.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     3089 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_concurrency.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     8686 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_connection.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    19348 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_data_type.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    11965 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_database.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      266 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_extension.js
+-rw-rw-r--   0 runner    (1001) docker     (127)    10191 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_parameter.js
+-rw-rw-r--   0 runner    (1001) docker     (127)     5730 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_query_result.js
+-rw-rw-r--   0 runner    (1001) docker     (127)      384 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/nodejs_api/test/test_version.js
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1295 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1136 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (127)       23 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/README.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2381 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      203 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/requirements_dev.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_import.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      618 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/cached_import/py_cached_item.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      335 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/arrow_array.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/
+-rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_import.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      521 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_item.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3624 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/cached_import/py_cached_modules.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      430 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/numpy/numpy_type.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)      718 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_analyzer.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1290 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      931 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_column.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1942 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pandas/pandas_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1266 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_connection.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      714 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_conversion.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_database.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      676 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_object_container.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_prepared_statement.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1470 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      709 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_query_result_converter.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     1031 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/py_str_utils.h
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      383 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_bind.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     2211 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pyarrow/pyarrow_scan.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      202 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/include/pybind_include.h
+-rw-rw-r--   0 runner    (1001) docker     (127)      549 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/kuzu_binding.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/
+-rw-rw-r--   0 runner    (1001) docker     (127)     9493 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     5514 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/numpy/numpy_type.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3949 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_analyzer.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3943 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7556 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pandas/pandas_scan.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    18759 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_connection.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4462 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_conversion.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3714 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_database.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)      564 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_prepared_statement.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    16191 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     7703 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/py_query_result_converter.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_bind.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     4295 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_cpp/pyarrow/pyarrow_scan.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2111 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6597 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/connection.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     9393 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/database.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1167 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)    14470 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7586 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_feature_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4893 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_graph_store.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    13467 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/torch_geometric_result_converter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      839 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/src_py/types.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5545 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/conftest.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14438 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/ground_truth.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    24584 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_arrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2687 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_database.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12786 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_datatype.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    20051 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_df.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    24852 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_df_pyarrow.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2330 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_exception.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_extension.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1947 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_get_header.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3619 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_issue.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    10889 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_networkx.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8471 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_parameter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4511 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_prepared_statement.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1780 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_query_result.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1258 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_query_result_close.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12717 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_scan_pandas.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_timeout.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    30361 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4105 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_torch_geometric_remote_backend.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      155 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/test_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      215 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/python_api/test/type_aliases.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/
+-rw-rw-r--   0 runner    (1001) docker     (127)        7 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)    25753 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/Cargo.lock
+-rw-rw-r--   0 runner    (1001) docker     (127)     1099 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/Cargo.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5748 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/build.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      345 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_arrow.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     9633 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/include/kuzu_rs.h
+lrwxrwxrwx   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:49.627046 sdist/kuzu-source/tools/rust_api/kuzu-src -> ../..
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    13653 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/connection.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     6642 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/database.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1763 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/error.rs
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/ffi/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1123 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/ffi/arrow.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12920 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/ffi.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_arrow.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)    11961 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/kuzu_rs.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     2523 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/lib.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    12498 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/logical_type.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     9355 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/query_result.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     2629 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/rdf_variant.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)    67772 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/src/value.rs
+-rw-rw-r--   0 runner    (1001) docker     (127)     1730 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/rust_api/update_version.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/
+-rw-rw-r--   0 runner    (1001) docker     (127)      321 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    27728 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/embedded_shell.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/include/
+-rw-rw-r--   0 runner    (1001) docker     (127)      912 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/include/embedded_shell.h
+-rw-rw-r--   0 runner    (1001) docker     (127)     3116 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/include/linenoise.h
+-rw-rw-r--   0 runner    (1001) docker     (127)    79992 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/linenoise.cpp
+-rw-rw-r--   0 runner    (1001) docker     (127)     3257 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/shell_runner.cpp
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/
+-rw-rw-r--   0 runner    (1001) docker     (127)     5371 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/conftest.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/files/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3075 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/files/vPerson.csv
+-rw-rw-r--   0 runner    (1001) docker     (127)     1399 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_helper.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4790 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_basics.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4811 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_commands.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    11969 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    12995 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_control_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4297 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_edit.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4571 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_esc_search.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4904 2024-04-27 08:04:47.000000 sdist/kuzu-source/tools/shell/test/test_shell_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 08:04:51.727048 sdist/kuzu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-27 08:04:51.727048 sdist/kuzu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 08:04:51.731048 sdist/kuzu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:04:51.727048 sdist/kuzu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 08:04:51.727048 sdist/kuzu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 08:04:51.727048 sdist/kuzu.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-27 08:04:49.847047 sdist/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 08:04:46.215044 sdist/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-27 08:04:46.215044 sdist/setup.py
```

### sdist/kuzu-source/CMakeLists.txt

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.15)
 
-project(Kuzu VERSION 0.3.3.47 LANGUAGES CXX C)
+project(Kuzu VERSION 0.3.3.48 LANGUAGES CXX C)
 
 find_package(Threads REQUIRED)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
 set(CMAKE_CXX_VISIBILITY_PRESET hidden)
 set(CMAKE_C_VISIBILITY_PRESET hidden)
```

### sdist/kuzu-source/scripts/antlr4/Cypher.g4.copy

```diff
@@ -80,15 +80,15 @@
 kU_UseDatabase
     : USE SP oC_SchemaName;
 
 USE:
     ( 'U' | 'u') ( 'S' | 's') ( 'E' | 'e');
 
 kU_StandaloneCall
-    : CALL SP oC_SymbolicName SP? '=' SP? oC_Literal ;
+    : CALL SP oC_SymbolicName SP? '=' SP? oC_Expression ;
 
 CALL : ( 'C' | 'c' ) ( 'A' | 'a' ) ( 'L' | 'l' ) ( 'L' | 'l' ) ;
 
 kU_CommentOn
     : COMMENT_ SP ON SP TABLE SP oC_SchemaName SP IS SP StringLiteral ;
 
 COMMENT_ : ( 'C' | 'c' ) ( 'O' | 'o' ) ( 'M' | 'm' ) ( 'M' | 'm' ) ( 'E' | 'e' ) ( 'N' | 'n' ) ( 'T' | 't' ) ;
```

### sdist/kuzu-source/src/antlr4/Cypher.g4

```diff
@@ -80,15 +80,15 @@
 kU_UseDatabase
     : USE SP oC_SchemaName;
 
 USE:
     ( 'U' | 'u') ( 'S' | 's') ( 'E' | 'e');
 
 kU_StandaloneCall
-    : CALL SP oC_SymbolicName SP? '=' SP? oC_Literal ;
+    : CALL SP oC_SymbolicName SP? '=' SP? oC_Expression ;
 
 CALL : ( 'C' | 'c' ) ( 'A' | 'a' ) ( 'L' | 'l' ) ( 'L' | 'l' ) ;
 
 kU_CommentOn
     : COMMENT_ SP ON SP TABLE SP oC_SchemaName SP IS SP StringLiteral ;
 
 COMMENT_ : ( 'C' | 'c' ) ( 'O' | 'o' ) ( 'M' | 'm' ) ( 'M' | 'm' ) ( 'E' | 'e' ) ( 'N' | 'n' ) ( 'T' | 't' ) ;
```

### sdist/kuzu-source/src/binder/bind/bind_import_database.cpp

```diff
@@ -51,19 +51,26 @@
         auto copyFromStatement =
             ku_dynamic_cast<const Statement*, const CopyFrom*>(parsedStatement.get());
         KU_ASSERT(copyFromStatement->getSource()->type == common::ScanSourceType::FILE);
         auto filePaths = ku_dynamic_cast<parser::BaseScanSource*, parser::FileScanSource*>(
             copyFromStatement->getSource())
                              ->filePaths;
         KU_ASSERT(filePaths.size() == 1);
+        auto fileType = bindFileType(filePaths);
         auto copyFilePath = boundFilePath + "/" + filePaths[0];
-        auto csvConfig = CSVReaderConfig::construct(
-            bindParsingOptions(copyFromStatement->getParsingOptionsRef()));
-        auto csvQuery = stringFormat("COPY {} FROM \"{}\" {};", copyFromStatement->getTableName(),
-            copyFilePath, csvConfig.option.toCypher());
-        finalQueryStatements += csvQuery;
+        std::string query;
+        if (fileType == FileType::CSV) {
+            auto csvConfig = CSVReaderConfig::construct(
+                bindParsingOptions(copyFromStatement->getParsingOptionsRef()));
+            query = stringFormat("COPY {} FROM \"{}\" {};", copyFromStatement->getTableName(),
+                copyFilePath, csvConfig.option.toCypher());
+        } else {
+            query = stringFormat("COPY {} FROM \"{}\";", copyFromStatement->getTableName(),
+                copyFilePath);
+        }
+        finalQueryStatements += query;
     }
     finalQueryStatements += getQueryFromFile(fs, boundFilePath, ImportDBConstants::MACRO_NAME);
     return std::make_unique<BoundImportDatabase>(boundFilePath, finalQueryStatements);
 }
 } // namespace binder
 } // namespace kuzu
```

### sdist/kuzu-source/src/binder/bind/bind_standalone_call.cpp

```diff
@@ -1,10 +1,11 @@
 #include "binder/binder.h"
 #include "binder/bound_standalone_call.h"
 #include "binder/expression/expression_util.h"
+#include "binder/expression_visitor.h"
 #include "common/exception/binder.h"
 #include "extension/extension.h"
 #include "main/db_config.h"
 #include "parser/standalone_call.h"
 
 using namespace kuzu::common;
 
@@ -18,15 +19,19 @@
     if (option == nullptr) {
         option =
             clientContext->getExtensionOptions()->getExtensionOption(callStatement.getOptionName());
     }
     if (option == nullptr) {
         throw BinderException{"Invalid option name: " + callStatement.getOptionName() + "."};
     }
-    auto optionValue = expressionBinder.bindLiteralExpression(*callStatement.getOptionValue());
-    // TODO(Ziyi): add casting rule for option value.
-    ExpressionUtil::validateDataType(*optionValue, option->parameterType);
+    auto optionValue = expressionBinder.bindExpression(*callStatement.getOptionValue());
+    ExpressionUtil::validateExpressionType(*optionValue, ExpressionType::LITERAL);
+    optionValue =
+        expressionBinder.implicitCastIfNecessary(optionValue, LogicalType(option->parameterType));
+    if (ExpressionVisitor::needFold(*optionValue)) {
+        optionValue = expressionBinder.foldExpression(optionValue);
+    }
     return std::make_unique<BoundStandaloneCall>(option, std::move(optionValue));
 }
 
 } // namespace binder
 } // namespace kuzu
```

### sdist/kuzu-source/src/binder/bind/read/bind_in_query_call.cpp

```diff
@@ -17,36 +17,39 @@
 namespace binder {
 
 std::unique_ptr<BoundReadingClause> Binder::bindInQueryCall(const ReadingClause& readingClause) {
     auto& call = readingClause.constCast<InQueryCallClause>();
     auto expr = call.getFunctionExpression();
     auto functionExpr = expr->constPtrCast<ParsedFunctionExpression>();
     auto functionName = functionExpr->getFunctionName();
-    expression_vector params;
+    expression_vector children;
     for (auto i = 0u; i < functionExpr->getNumChildren(); i++) {
-        auto child = functionExpr->getChild(i);
-        params.push_back(expressionBinder.bindExpression(*child));
+        auto childExpr = functionExpr->getChild(i);
+        children.push_back(expressionBinder.bindExpression(*childExpr));
     }
     TableFunction tableFunction;
     std::vector<Value> inputValues;
     std::vector<LogicalType> inputTypes;
-    for (auto& param : params) {
-        ExpressionUtil::validateExpressionType(*param, ExpressionType::LITERAL);
-        auto literalExpr = param->constPtrCast<LiteralExpression>();
+    for (auto& child : children) {
+        ExpressionUtil::validateExpressionType(*child, ExpressionType::LITERAL);
+        auto literalExpr = child->constPtrCast<LiteralExpression>();
         inputTypes.push_back(literalExpr->getDataType());
         inputValues.push_back(*literalExpr->getValue());
     }
     auto catalogSet = clientContext->getCatalog()->getFunctions(clientContext->getTx());
     auto functionEntry = BuiltInFunctionsUtils::getFunctionCatalogEntry(functionName, catalogSet);
     if (functionEntry->getType() != CatalogEntryType::TABLE_FUNCTION_ENTRY) {
         throw BinderException(stringFormat("{} is not a table function.", functionName));
     }
-    auto func = BuiltInFunctionsUtils::matchFunction(functionExpr->getFunctionName(), inputTypes,
-        functionEntry);
+    auto func = BuiltInFunctionsUtils::matchFunction(functionName, inputTypes, functionEntry);
     tableFunction = *func->constPtrCast<TableFunction>();
+    for (auto i = 0u; i < children.size(); ++i) {
+        auto parameterTypeID = tableFunction.parameterTypeIDs[i];
+        ExpressionUtil::validateDataType(*children[i], parameterTypeID);
+    }
     auto bindInput = function::TableFuncBindInput();
     bindInput.inputs = std::move(inputValues);
     auto bindData = tableFunction.bindFunc(clientContext, &bindInput);
     expression_vector columns;
     for (auto i = 0u; i < bindData->columnTypes.size(); i++) {
         columns.push_back(createVariable(bindData->columnNames[i], bindData->columnTypes[i]));
     }
```

### sdist/kuzu-source/src/binder/expression_visitor.cpp

```diff
@@ -88,15 +88,16 @@
 }
 
 // isConstant requires all children to be constant.
 bool ExpressionVisitor::isConstant(const Expression& expression) {
     if (expression.expressionType == ExpressionType::AGGREGATE_FUNCTION) {
         return false; // We don't have a framework to fold aggregated constant.
     }
-    if (expression.getNumChildren() == 0) {
+    if (expression.getNumChildren() == 0 &&
+        expression.expressionType != ExpressionType::CASE_ELSE) {
         return expression.expressionType == ExpressionType::LITERAL;
     }
     for (auto& child : ExpressionChildrenCollector::collectChildren(expression)) {
         if (!isConstant(*child)) {
             return false;
         }
     }
```

### sdist/kuzu-source/src/function/table/call/show_connection.cpp

```diff
@@ -1,8 +1,9 @@
 #include "catalog/catalog.h"
+#include "catalog/catalog_entry/node_table_catalog_entry.h"
 #include "catalog/catalog_entry/rel_group_catalog_entry.h"
 #include "catalog/catalog_entry/rel_table_catalog_entry.h"
 #include "common/exception/binder.h"
 #include "function/table/bind_input.h"
 #include "function/table/call_functions.h"
 
 using namespace kuzu::catalog;
@@ -24,50 +25,63 @@
 
     inline std::unique_ptr<TableFuncBindData> copy() const override {
         return std::make_unique<ShowConnectionBindData>(context, tableEntry, columnTypes,
             columnNames, maxOffset);
     }
 };
 
-static void outputRelTableConnection(ValueVector* srcTableNameVector,
-    ValueVector* dstTableNameVector, uint64_t outputPos, ClientContext* context,
-    table_id_t tableID) {
+static void outputRelTableConnection(DataChunk& outputDataChunk, uint64_t outputPos,
+    ClientContext* context, table_id_t tableID) {
     auto catalog = context->getCatalog();
     auto tableEntry = catalog->getTableCatalogEntry(context->getTx(), tableID);
     auto relTableEntry = ku_dynamic_cast<TableCatalogEntry*, RelTableCatalogEntry*>(tableEntry);
     KU_ASSERT(tableEntry->getTableType() == TableType::REL);
+    // Get src and dst name
     auto srcTableID = relTableEntry->getSrcTableID();
     auto dstTableID = relTableEntry->getDstTableID();
-    srcTableNameVector->setValue(outputPos, catalog->getTableName(context->getTx(), srcTableID));
-    dstTableNameVector->setValue(outputPos, catalog->getTableName(context->getTx(), dstTableID));
+    auto srcTableName = catalog->getTableName(context->getTx(), srcTableID);
+    auto dstTableName = catalog->getTableName(context->getTx(), dstTableID);
+    // Get src and dst primary key
+    auto srcTableEntry = catalog->getTableCatalogEntry(context->getTx(), srcTableID);
+    auto dstTableEntry = catalog->getTableCatalogEntry(context->getTx(), dstTableID);
+    auto srcTablePrimaryKey =
+        ku_dynamic_cast<TableCatalogEntry*, NodeTableCatalogEntry*>(srcTableEntry)
+            ->getPrimaryKey()
+            ->getName();
+    auto dstTablePrimaryKey =
+        ku_dynamic_cast<TableCatalogEntry*, NodeTableCatalogEntry*>(dstTableEntry)
+            ->getPrimaryKey()
+            ->getName();
+    // Write result to dataChunk
+    outputDataChunk.getValueVector(0)->setValue(outputPos, srcTableName);
+    outputDataChunk.getValueVector(1)->setValue(outputPos, dstTableName);
+    outputDataChunk.getValueVector(2)->setValue(outputPos, srcTablePrimaryKey);
+    outputDataChunk.getValueVector(3)->setValue(outputPos, dstTablePrimaryKey);
 }
 
 static common::offset_t tableFunc(TableFuncInput& input, TableFuncOutput& output) {
     auto& dataChunk = output.dataChunk;
-    auto srcVector = dataChunk.getValueVector(0).get();
-    auto dstVector = dataChunk.getValueVector(1).get();
     auto morsel = input.sharedState->ptrCast<CallFuncSharedState>()->getMorsel();
     if (!morsel.hasMoreToOutput()) {
         return 0;
     }
     auto bindData = input.bindData->constPtrCast<ShowConnectionBindData>();
     auto tableEntry = bindData->tableEntry;
     auto numRelationsToOutput = morsel.endOffset - morsel.startOffset;
     auto vectorPos = 0u;
     switch (tableEntry->getTableType()) {
     case TableType::REL: {
-        outputRelTableConnection(srcVector, dstVector, vectorPos, bindData->context,
-            tableEntry->getTableID());
+        outputRelTableConnection(dataChunk, vectorPos, bindData->context, tableEntry->getTableID());
         vectorPos++;
     } break;
     case TableType::REL_GROUP: {
         auto relGroupEntry = ku_dynamic_cast<TableCatalogEntry*, RelGroupCatalogEntry*>(tableEntry);
         auto relTableIDs = relGroupEntry->getRelTableIDs();
         for (; vectorPos < numRelationsToOutput; vectorPos++) {
-            outputRelTableConnection(srcVector, dstVector, vectorPos, bindData->context,
+            outputRelTableConnection(dataChunk, vectorPos, bindData->context,
                 relTableIDs[morsel.startOffset + vectorPos]);
         }
     } break;
     default:
         // LCOV_EXCL_START
         KU_UNREACHABLE;
         // LCOV_EXCL_STOP
@@ -75,41 +89,41 @@
     return vectorPos;
 }
 
 static std::unique_ptr<TableFuncBindData> bindFunc(ClientContext* context,
     TableFuncBindInput* input) {
     std::vector<std::string> columnNames;
     std::vector<LogicalType> columnTypes;
-    // Special case here Due to any -> string, but lack implicit cast
-    if (input->inputs[0].getDataType()->getLogicalTypeID() != LogicalTypeID::STRING) {
-        throw BinderException{"Show connection can only bind to String!"};
-    }
     auto tableName = input->inputs[0].getValue<std::string>();
     auto catalog = context->getCatalog();
     auto tableID = catalog->getTableID(context->getTx(), tableName);
     auto tableEntry = catalog->getTableCatalogEntry(context->getTx(), tableID);
     auto tableType = tableEntry->getTableType();
     if (tableType != TableType::REL && tableType != TableType::REL_GROUP) {
         throw BinderException{"Show connection can only be called on a rel table!"};
     }
     columnNames.emplace_back("source table name");
     columnTypes.emplace_back(*LogicalType::STRING());
     columnNames.emplace_back("destination table name");
     columnTypes.emplace_back(*LogicalType::STRING());
+    columnNames.emplace_back("source table primary key");
+    columnTypes.emplace_back(*LogicalType::STRING());
+    columnNames.emplace_back("destination table primary key");
+    columnTypes.emplace_back(*LogicalType::STRING());
     common::offset_t maxOffset = 1;
     if (tableEntry->getTableType() == common::TableType::REL_GROUP) {
         auto relGroupEntry = ku_dynamic_cast<TableCatalogEntry*, RelGroupCatalogEntry*>(tableEntry);
         maxOffset = relGroupEntry->getRelTableIDs().size();
     }
     return std::make_unique<ShowConnectionBindData>(context, tableEntry, std::move(columnTypes),
         std::move(columnNames), maxOffset);
 }
 
 function_set ShowConnectionFunction::getFunctionSet() {
     function_set functionSet;
-    functionSet.push_back(std::make_unique<TableFunction>("db_version", tableFunc, bindFunc,
+    functionSet.push_back(std::make_unique<TableFunction>(name, tableFunc, bindFunc,
         initSharedState, initEmptyLocalState, std::vector<LogicalTypeID>{LogicalTypeID::STRING}));
     return functionSet;
 }
 
 } // namespace function
 } // namespace kuzu
```

### sdist/kuzu-source/src/include/storage/buffer_manager/bm_file_handle.h

```diff
@@ -171,14 +171,15 @@
     common::page_idx_t getWALPageIdxNoWALPageIdxLock(common::page_idx_t originalPageIdx);
     void setWALPageIdx(common::page_idx_t originalPageIdx, common::page_idx_t pageIdxInWAL);
     // This function assumes that the caller has already acquired the wal page idx lock.
     void setWALPageIdxNoLock(common::page_idx_t originalPageIdx, common::page_idx_t pageIdxInWAL);
 
 private:
     inline PageState* getPageState(common::page_idx_t pageIdx) {
+        std::shared_lock sLck{fhSharedMutex};
         KU_ASSERT(pageIdx < numPages && pageStates[pageIdx]);
         return pageStates[pageIdx].get();
     }
     inline common::frame_idx_t getFrameIdx(common::page_idx_t pageIdx) {
         KU_ASSERT(pageIdx < pageCapacity);
         return (frameGroupIdxes[pageIdx >> common::StorageConstants::PAGE_GROUP_SIZE_LOG2]
                    << common::StorageConstants::PAGE_GROUP_SIZE_LOG2) |
```

### sdist/kuzu-source/src/include/storage/stats/table_statistics_collection.h

```diff
@@ -77,14 +77,16 @@
         PropertyStatistics stats);
 
     static std::unique_ptr<MetadataDAHInfo> createMetadataDAHInfo(
         const common::LogicalType& dataType, BMFileHandle& metadataFH, BufferManager* bm, WAL* wal);
 
     void initTableStatisticsForWriteTrx();
 
+    void setToUpdated() { isUpdated = true; }
+
 protected:
     virtual std::unique_ptr<TableStatistics> constructTableStatistic(
         catalog::TableCatalogEntry* tableEntry) = 0;
 
     virtual std::string getTableStatisticsFilePath(const std::string& directory,
         common::FileVersionType dbFileType, common::VirtualFileSystem* fs) = 0;
 
@@ -97,15 +99,14 @@
     void readFromFile(common::FileVersionType dbFileType, common::VirtualFileSystem* fs);
 
     void saveToFile(const std::string& directory, common::FileVersionType dbFileType,
         transaction::TransactionType transactionType, common::VirtualFileSystem* fs);
 
     void initTableStatisticsForWriteTrxNoLock();
 
-    void setToUpdated() { isUpdated = true; }
     void resetToNotUpdated() { isUpdated = false; }
 
 protected:
     BMFileHandle* metadataFH;
     BufferManager* bufferManager;
     WAL* wal;
     bool isUpdated;
```

### sdist/kuzu-source/src/include/storage/store/column.h

```diff
@@ -34,48 +34,47 @@
     friend class StringColumn;
     friend class ListLocalColumn;
     friend class StructColumn;
     friend class ListColumn;
     friend class RelTableData;
 
 public:
-    struct ReadState {
-        explicit ReadState() = default;
-        ReadState(ColumnChunkMetadata metadata, uint64_t numValuesPerPage)
+    struct ChunkState {
+        explicit ChunkState() = default;
+        ChunkState(ColumnChunkMetadata metadata, uint64_t numValuesPerPage)
             : metadata{std::move(metadata)}, numValuesPerPage{numValuesPerPage} {}
 
         ColumnChunkMetadata metadata;
         uint64_t numValuesPerPage = UINT64_MAX;
         common::node_group_idx_t nodeGroupIdx = common::INVALID_NODE_GROUP_IDX;
-        std::unique_ptr<ReadState> nullState = nullptr;
+        std::unique_ptr<ChunkState> nullState = nullptr;
         // Used for struct/list/string columns.
-        std::vector<ReadState> childrenStates;
+        std::vector<ChunkState> childrenStates;
     };
 
     Column(std::string name, common::LogicalType dataType, const MetadataDAHInfo& metaDAHeaderInfo,
         BMFileHandle* dataFH, BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal,
         transaction::Transaction* transaction, RWPropertyStats propertyStatistics,
         bool enableCompression, bool requireNullColumn = true);
     virtual ~Column();
 
     // Expose for feature store
     virtual void batchLookup(transaction::Transaction* transaction,
         const common::offset_t* nodeOffsets, size_t size, uint8_t* result);
 
-    virtual void initReadState(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, common::offset_t startOffsetInChunk,
-        ReadState& columnReadState);
+    virtual void initChunkState(transaction::Transaction* transaction,
+        common::node_group_idx_t nodeGroupIdx, ChunkState& state);
 
-    virtual void scan(transaction::Transaction* transaction, ReadState& readState,
+    virtual void scan(transaction::Transaction* transaction, ChunkState& state,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector);
-    virtual void lookup(transaction::Transaction* transaction, ReadState& readState,
+    virtual void lookup(transaction::Transaction* transaction, ChunkState& state,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector);
 
     // Scan from [startOffsetInGroup, endOffsetInGroup).
-    virtual void scan(transaction::Transaction* transaction, ReadState& readState,
+    virtual void scan(transaction::Transaction* transaction, ChunkState& state,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup,
         common::ValueVector* resultVector, uint64_t offsetInVector);
     // Scan from [startOffsetInGroup, endOffsetInGroup).
     virtual void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET);
 
@@ -110,65 +109,58 @@
         transaction::TransactionType transaction) const {
         return metadataDA->get(nodeGroupIdx, transaction);
     }
     inline InMemDiskArray<ColumnChunkMetadata>* getMetadataDA() const { return metadataDA.get(); }
 
     inline std::string getName() const { return name; }
 
-    virtual void scan(transaction::Transaction* transaction, const ReadState& state,
+    virtual void scan(transaction::Transaction* transaction, const ChunkState& state,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup, uint8_t* result);
 
     // Write a single value from the vectorToWriteFrom.
-    virtual void write(common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk,
+    virtual void write(ChunkState& state, common::offset_t offsetInChunk,
         common::ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom);
     // Batch write to a set of sequential pages.
-    virtual void write(common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk,
-        ColumnChunk* data, common::offset_t dataOffset, common::length_t numValues);
+    virtual void write(ChunkState& state, common::offset_t offsetInChunk, ColumnChunk* data,
+        common::offset_t dataOffset, common::length_t numValues);
 
     // Append values to the end of the node group, resizing it if necessary
-    common::offset_t appendValues(common::node_group_idx_t nodeGroupIdx, const uint8_t* data,
+    common::offset_t appendValues(ChunkState& state, const uint8_t* data,
         const common::NullMask* nullChunkData, common::offset_t numValues);
 
-    ReadState getReadState(transaction::TransactionType transactionType,
-        common::node_group_idx_t nodeGroupIdx) const;
-
     virtual std::unique_ptr<ColumnChunk> getEmptyChunkForCommit(uint64_t capacity);
     static void applyLocalChunkToColumnChunk(const ChunkCollection& localChunks,
         ColumnChunk* columnChunk, const offset_to_row_idx_t& info);
 
 protected:
-    virtual void scanInternal(transaction::Transaction* transaction, ReadState& readState,
+    virtual void scanInternal(transaction::Transaction* transaction, ChunkState& state,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector);
     void scanUnfiltered(transaction::Transaction* transaction, PageCursor& pageCursor,
         uint64_t numValuesToScan, common::ValueVector* resultVector,
         const ColumnChunkMetadata& chunkMeta, uint64_t startPosInVector = 0);
     void scanFiltered(transaction::Transaction* transaction, PageCursor& pageCursor,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector,
         const ColumnChunkMetadata& chunkMeta);
-    virtual void lookupInternal(transaction::Transaction* transaction, ReadState& readState,
+    virtual void lookupInternal(transaction::Transaction* transaction, ChunkState& state,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector);
-    virtual void lookupValue(transaction::Transaction* transaction, ReadState& readState,
+    virtual void lookupValue(transaction::Transaction* transaction, ChunkState& state,
         common::offset_t nodeOffset, common::ValueVector* resultVector, uint32_t posInVector);
 
     void readFromPage(transaction::Transaction* transaction, common::page_idx_t pageIdx,
         const std::function<void(uint8_t*)>& func);
 
-    virtual void writeValue(const ColumnChunkMetadata& chunkMeta,
-        common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk,
+    virtual void writeValue(ChunkState& state, common::offset_t offsetInChunk,
         common::ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom);
-    virtual void writeValues(ReadState& state, common::offset_t offsetInChunk, const uint8_t* data,
+    virtual void writeValues(ChunkState& state, common::offset_t offsetInChunk, const uint8_t* data,
         const common::NullMask* nullChunkData, common::offset_t dataOffset = 0,
         common::offset_t numValues = 1);
 
     // Produces a page cursor for the offset relative to the given node group
     PageCursor getPageCursorForOffsetInGroup(common::offset_t offsetInChunk,
-        const ReadState& state);
-    // Produces a page cursor for the absolute node offset
-    PageCursor getPageCursorForOffset(transaction::TransactionType transactionType,
-        common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk);
+        const ChunkState& state);
     void updatePageWithCursor(PageCursor cursor,
         const std::function<void(uint8_t*, common::offset_t)>& writeOp);
 
     inline common::offset_t getMaxOffset(const std::vector<common::offset_t>& offsets) {
         common::offset_t maxOffset = 0u;
         for (auto offset : offsets) {
             maxOffset = std::max(maxOffset, offset);
@@ -181,40 +173,42 @@
 private:
     bool isInsertionsOutOfPagesCapacity(const ColumnChunkMetadata& metadata,
         const offset_to_row_idx_t& insertInfo);
     bool isMaxOffsetOutOfPagesCapacity(const ColumnChunkMetadata& metadata,
         common::offset_t maxOffset);
     bool checkUpdateInPlace(const ColumnChunkMetadata& metadata, const ChunkCollection& localChunks,
         const offset_to_row_idx_t& writeInfo);
-    virtual bool canCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunks,
+
+    virtual bool canCommitInPlace(const ChunkState& state, const ChunkCollection& localInsertChunks,
         const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
         const offset_to_row_idx_t& updateInfo);
-    virtual bool canCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
-        ColumnChunk* chunk, common::offset_t srcOffset);
-    virtual void commitLocalChunkInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunks,
-        const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
-        const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo);
+    virtual bool canCommitInPlace(const ChunkState& state,
+        const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
+        common::offset_t srcOffset);
+
+    virtual void commitLocalChunkInPlace(transaction::Transaction* transaction, ChunkState& state,
+        const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
+        const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
+        const offset_set_t& deleteInfo);
     virtual void commitLocalChunkOutOfPlace(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, bool isNewNodeGroup,
         const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
         const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
         const offset_set_t& deleteInfo);
-    virtual void commitColumnChunkInPlace(common::node_group_idx_t nodeGroupIdx,
+
+    virtual void commitColumnChunkInPlace(ChunkState& state,
         const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
         common::offset_t srcOffset);
     virtual void commitColumnChunkOutOfPlace(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, bool isNewNodeGroup,
         const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
         common::offset_t srcOffset);
 
-    void applyLocalChunkToColumn(common::node_group_idx_t nodeGroupIdx,
-        const ChunkCollection& localChunks, const offset_to_row_idx_t& info);
+    void applyLocalChunkToColumn(ChunkState& state, const ChunkCollection& localChunks,
+        const offset_to_row_idx_t& info);
 
     // check if val is in range [start, end)
     static inline bool isInRange(uint64_t val, uint64_t start, uint64_t end) {
         return val >= start && val < end;
     }
 
 protected:
@@ -241,31 +235,31 @@
 
 class InternalIDColumn : public Column {
 public:
     InternalIDColumn(std::string name, const MetadataDAHInfo& metaDAHeaderInfo,
         BMFileHandle* dataFH, BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal,
         transaction::Transaction* transaction, RWPropertyStats stats, bool enableCompression);
 
-    inline void scan(transaction::Transaction* transaction, ReadState& readState,
+    inline void scan(transaction::Transaction* transaction, ChunkState& state,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override {
-        Column::scan(transaction, readState, nodeIDVector, resultVector);
+        Column::scan(transaction, state, nodeIDVector, resultVector);
         populateCommonTableID(resultVector);
     }
 
-    inline void scan(transaction::Transaction* transaction, ReadState& readState,
+    inline void scan(transaction::Transaction* transaction, ChunkState& state,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup,
         common::ValueVector* resultVector, uint64_t offsetInVector) override {
-        Column::scan(transaction, readState, startOffsetInGroup, endOffsetInGroup, resultVector,
+        Column::scan(transaction, state, startOffsetInGroup, endOffsetInGroup, resultVector,
             offsetInVector);
         populateCommonTableID(resultVector);
     }
 
-    inline void lookup(transaction::Transaction* transaction, ReadState& readState,
+    inline void lookup(transaction::Transaction* transaction, ChunkState& state,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override {
-        Column::lookup(transaction, readState, nodeIDVector, resultVector);
+        Column::lookup(transaction, state, nodeIDVector, resultVector);
         populateCommonTableID(resultVector);
     }
 
     // TODO(Guodong): This function should be removed through rewritting INTERNAL_ID as STRUCT.
     inline void setCommonTableID(common::table_id_t tableID) { commonTableID = tableID; }
 
 private:
```

### sdist/kuzu-source/src/include/storage/store/dictionary_column.h

```diff
@@ -11,57 +11,52 @@
     static constexpr common::vector_idx_t DATA_COLUMN_CHILD_READ_STATE_IDX = 0;
     static constexpr common::vector_idx_t OFFSET_COLUMN_CHILD_READ_STATE_IDX = 1;
 
     DictionaryColumn(const std::string& name, const MetadataDAHInfo& metaDAHeaderInfo,
         BMFileHandle* dataFH, BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal,
         transaction::Transaction* transaction, RWPropertyStats stats, bool enableCompression);
 
-    void initReadState(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
-        common::offset_t startOffsetInChunk, Column::ReadState& columnReadState);
+    void initChunkState(transaction::Transaction* transaction,
+        common::node_group_idx_t nodeGroupIdx, Column::ChunkState& columnReadState);
 
     void append(common::node_group_idx_t nodeGroupIdx, const DictionaryChunk& dictChunk);
+
     void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         DictionaryChunk& dictChunk);
     // Offsets to scan should be a sorted list of pairs mapping the index of the entry in the string
     // dictionary (as read from the index column) to the output index in the result vector to store
     // the string.
-    void scan(transaction::Transaction* transaction, const Column::ReadState& offsetState,
-        const Column::ReadState& dataState,
+    void scan(transaction::Transaction* transaction, const Column::ChunkState& offsetState,
+        const Column::ChunkState& dataState,
         std::vector<std::pair<DictionaryChunk::string_index_t, uint64_t>>& offsetsToScan,
         common::ValueVector* resultVector, const ColumnChunkMetadata& indexMeta);
 
-    DictionaryChunk::string_index_t append(common::node_group_idx_t nodeGroupIdx,
-        std::string_view val);
+    DictionaryChunk::string_index_t append(Column::ChunkState& state, std::string_view val);
 
-    bool canCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, uint64_t numNewStrings,
+    bool canCommitInPlace(const Column::ChunkState& state, uint64_t numNewStrings,
         uint64_t totalStringLengthToAdd);
 
-    uint64_t getNumValuesInOffsets(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx);
-
     void prepareCommit();
     void checkpointInMemory();
     void rollbackInMemory();
 
     inline Column* getDataColumn() const { return dataColumn.get(); }
     inline Column* getOffsetColumn() const { return offsetColumn.get(); }
 
 private:
-    void scanOffsets(transaction::Transaction* transaction, const Column::ReadState& state,
+    void scanOffsets(transaction::Transaction* transaction, const Column::ChunkState& state,
         DictionaryChunk::string_offset_t* offsets, uint64_t index, uint64_t numValues,
         uint64_t dataSize);
     void scanValueToVector(transaction::Transaction* transaction,
-        const Column::ReadState& dataState, uint64_t startOffset, uint64_t endOffset,
+        const Column::ChunkState& dataState, uint64_t startOffset, uint64_t endOffset,
         common::ValueVector* resultVector, uint64_t offsetInVector);
 
-    bool canDataCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, uint64_t totalStringLengthToAdd);
-    bool canOffsetCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, uint64_t numNewStrings,
+    bool canDataCommitInPlace(const Column::ChunkState& dataState, uint64_t totalStringLengthToAdd);
+    bool canOffsetCommitInPlace(const Column::ChunkState& offsetState,
+        const Column::ChunkState& dataState, uint64_t numNewStrings,
         uint64_t totalStringLengthToAdd);
 
 private:
     // The offset column stores the offsets for each index, and the data column stores the data in
     // order. Values are never removed from the dictionary during in-place updates, only appended to
     // the end.
     std::unique_ptr<Column> dataColumn;
```

### sdist/kuzu-source/src/include/storage/store/list_column.h

```diff
@@ -49,72 +49,70 @@
 
 public:
     ListColumn(std::string name, common::LogicalType dataType,
         const MetadataDAHInfo& metaDAHeaderInfo, BMFileHandle* dataFH, BMFileHandle* metadataFH,
         BufferManager* bufferManager, WAL* wal, transaction::Transaction* transaction,
         RWPropertyStats propertyStatistics, bool enableCompression);
 
-    void initReadState(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
-        common::offset_t startOffsetInChunk, ReadState& columnReadState) override;
-    void scan(transaction::Transaction* transaction, ReadState& readState,
+    void initChunkState(transaction::Transaction* transaction,
+        common::node_group_idx_t nodeGroupIdx, ChunkState& columnReadState) override;
+
+    void scan(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup,
         common::ValueVector* resultVector, uint64_t offsetInVector = 0) override;
-
     void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET) override;
 
     inline Column* getDataColumn() { return dataColumn.get(); }
 
 protected:
-    void scanInternal(transaction::Transaction* transaction, ReadState& readState,
+    void scanInternal(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override;
 
-    void lookupValue(transaction::Transaction* transaction, ReadState& readState,
+    void lookupValue(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t nodeOffset, common::ValueVector* resultVector,
         uint32_t posInVector) override;
 
     void append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) override;
 
 private:
-    void scanUnfiltered(transaction::Transaction* transaction, ReadState& readState,
+    void scanUnfiltered(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* resultVector, const ListOffsetSizeInfo& listOffsetInfoInStorage);
-    void scanFiltered(transaction::Transaction* transaction, ReadState& readState,
+    void scanFiltered(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* offsetVector, const ListOffsetSizeInfo& listOffsetInfoInStorage);
 
     void prepareCommit() override;
     void checkpointInMemory() override;
     void rollbackInMemory() override;
 
-    common::offset_t readOffset(transaction::Transaction* transaction, const ReadState& readState,
+    common::offset_t readOffset(transaction::Transaction* transaction, const ChunkState& readState,
         common::offset_t offsetInNodeGroup);
-    common::list_size_t readSize(transaction::Transaction* transaction, const ReadState& readState,
+    common::list_size_t readSize(transaction::Transaction* transaction, const ChunkState& readState,
         common::offset_t offsetInNodeGroup);
 
     ListOffsetSizeInfo getListOffsetSizeInfo(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, common::offset_t startOffsetInNodeGroup,
         common::offset_t endOffsetInNodeGroup);
 
     void prepareCommitForChunk(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunks,
         const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
         const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo) override;
     void prepareCommitForChunk(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
         ColumnChunk* chunk, common::offset_t startSrcOffset) override;
 
-    void prepareCommitForOffsetChunk(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
-        ColumnChunk* chunk, common::offset_t startSrcOffset);
-
+    void prepareCommitForOffsetChunk(transaction::Transaction* transaction, ChunkState& offsetState,
+        const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
+        common::offset_t startSrcOffset);
     void commitOffsetColumnChunkOutOfPlace(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
         ColumnChunk* chunk, common::offset_t startSrcOffset);
-
-    void commitOffsetColumnChunkInPlace(common::node_group_idx_t nodeGroupIdx,
+    void commitOffsetColumnChunkInPlace(ChunkState& offsetChunk,
         const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
         common::offset_t srcOffset);
 
 private:
     std::unique_ptr<Column> sizeColumn;
     std::unique_ptr<Column> dataColumn;
 };
```

### sdist/kuzu-source/src/include/storage/store/node_table_data.h

```diff
@@ -10,15 +10,15 @@
 class LocalNodeNG;
 struct NodeDataReadState : public TableDataReadState {
     NodeDataReadState() : TableDataReadState{} {}
     DELETE_COPY_DEFAULT_MOVE(NodeDataReadState);
 
     common::node_group_idx_t nodeGroupIdx = common::INVALID_NODE_GROUP_IDX;
     bool readFromPersistent = false;
-    std::vector<Column::ReadState> columnReadStates;
+    std::vector<Column::ChunkState> columnReadStates;
 
     // Should be moved into LocalNodeReadState.
     LocalNodeNG* localNodeGroup = nullptr;
 };
 
 class LocalTableData;
 class NodeTableData final : public TableData {
@@ -53,16 +53,15 @@
         common::node_group_idx_t nodeGroupIdx) const {
         KU_ASSERT(nodeGroupIdx < getNumNodeGroups(transaction));
         return columns[0]->getMetadata(nodeGroupIdx, transaction->getType()).numValues;
     }
 
 private:
     void initializeColumnReadStates(transaction::Transaction* transaction,
-        common::offset_t startNodeOffset, kuzu::storage::NodeDataReadState& readState,
-        common::node_group_idx_t nodeGroupIdx);
+        NodeDataReadState& readState, common::node_group_idx_t nodeGroupIdx);
     void initializeLocalNodeReadState(transaction::Transaction* transaction,
         NodeDataReadState& readState, common::node_group_idx_t nodeGroupIdx);
 
     void scan(transaction::Transaction* transaction, TableDataReadState& readState,
         const common::ValueVector& nodeIDVector,
         const std::vector<common::ValueVector*>& outputVectors) override;
     void lookup(transaction::Transaction* transaction, TableDataReadState& readState,
```

### sdist/kuzu-source/src/include/storage/store/null_column.h

```diff
@@ -16,38 +16,37 @@
     // without the possibility of memory errors from reading/writing off the end of a page.
     static_assert(PageUtils::getNumElementsInAPage(1, false /*requireNullColumn*/) % 8 == 0);
 
     NullColumn(std::string name, page_idx_t metaDAHPageIdx, BMFileHandle* dataFH,
         BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal, Transaction* transaction,
         RWPropertyStats propertyStatistics, bool enableCompression);
 
-    void scan(Transaction* transaction, ReadState& readState, ValueVector* nodeIDVector,
+    void scan(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
         ValueVector* resultVector) override;
-    void scan(transaction::Transaction* transaction, ReadState& readState,
+    void scan(transaction::Transaction* transaction, ChunkState& readState,
         offset_t startOffsetInGroup, offset_t endOffsetInGroup, ValueVector* resultVector,
         uint64_t offsetInVector) override;
     void scan(transaction::Transaction* transaction, node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET) override;
 
-    void lookup(Transaction* transaction, ReadState& readState, ValueVector* nodeIDVector,
+    void lookup(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
         ValueVector* resultVector) override;
 
     void append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) override;
 
-    bool isNull(transaction::Transaction* transaction, node_group_idx_t nodeGroupIdx,
-        offset_t offsetInChunk);
-    void setNull(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk, uint64_t value = true);
-
-    void write(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk,
-        ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) override;
-    void write(common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk,
-        ColumnChunk* data, common::offset_t dataOffset, common::length_t numValues) override;
+    bool isNull(Transaction* transaction, const ChunkState& state, offset_t offsetInChunk);
+    void setNull(ChunkState& state, offset_t offsetInChunk, uint64_t value = true);
 
-    void commitLocalChunkInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+    void write(ChunkState& state, offset_t offsetInChunk, ValueVector* vectorToWriteFrom,
+        uint32_t posInVectorToWriteFrom) override;
+    void write(ChunkState& state, common::offset_t offsetInChunk, ColumnChunk* data,
+        common::offset_t dataOffset, common::length_t numValues) override;
+
+    void commitLocalChunkInPlace(Transaction* transaction, ChunkState& state,
         const ChunkCollection& localInsertChunk, const offset_to_row_idx_t& insertInfo,
         const ChunkCollection& localUpdateChunk, const offset_to_row_idx_t& updateInfo,
         const offset_set_t& deleteInfo) override;
 
 private:
     std::unique_ptr<ColumnChunk> getEmptyChunkForCommit(uint64_t capacity) override {
         return ColumnChunkFactory::createNullColumnChunk(enableCompression, capacity);
```

### sdist/kuzu-source/src/include/storage/store/rel_table_data.h

```diff
@@ -13,15 +13,15 @@
     common::offset_t startNodeOffset;
     common::offset_t numNodes;
     common::offset_t currentNodeOffset;
     common::offset_t posInCurrentCSR;
     std::vector<common::list_entry_t> csrListEntries;
     // Temp auxiliary data structure to scan the offset of each CSR node in the offset column chunk.
     ChunkedCSRHeader csrHeaderChunks = ChunkedCSRHeader(false /*enableCompression*/);
-    std::vector<Column::ReadState> columnStates;
+    std::vector<Column::ChunkState> columnStates;
 
     bool readFromPersistentStorage;
     // Following fields are used for local storage.
     bool readFromLocalStorage;
     LocalRelNG* localNodeGroup;
 
     explicit RelDataReadState();
@@ -178,16 +178,15 @@
     }
 
 private:
     static common::offset_t getMaxNumNodesInRegion(const ChunkedCSRHeader& header,
         const PackedCSRRegion& region, const LocalRelNG* localNG);
 
     void initializeColumnReadStates(transaction::Transaction* transaction,
-        common::offset_t startNodeOffset, RelDataReadState& readState,
-        common::node_group_idx_t nodeGroupIdx);
+        RelDataReadState& readState, common::node_group_idx_t nodeGroupIdx);
 
     std::vector<PackedCSRRegion> findRegions(const ChunkedCSRHeader& headerChunks,
         LocalState& localState);
     common::length_t getNewRegionSize(const ChunkedCSRHeader& header,
         const std::vector<int64_t>& sizeChangesPerSegment, PackedCSRRegion& region);
     bool isWithinDensityBound(const ChunkedCSRHeader& headerChunks,
         const std::vector<int64_t>& sizeChangesPerSegment, PackedCSRRegion& region);
```

### sdist/kuzu-source/src/include/storage/store/string_column.h

```diff
@@ -8,67 +8,60 @@
 class StringColumn final : public Column {
 public:
     StringColumn(std::string name, common::LogicalType dataType,
         const MetadataDAHInfo& metaDAHeaderInfo, BMFileHandle* dataFH, BMFileHandle* metadataFH,
         BufferManager* bufferManager, WAL* wal, transaction::Transaction* transaction,
         RWPropertyStats propertyStatistics, bool enableCompression);
 
-    void initReadState(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
-        common::offset_t startOffsetInChunk, ReadState& columnReadState) override;
+    void initChunkState(transaction::Transaction* transaction,
+        common::node_group_idx_t nodeGroupIdx, ChunkState& columnReadState) override;
 
-    void scan(transaction::Transaction* transaction, ReadState& readState,
+    void scan(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup,
         common::ValueVector* resultVector, uint64_t offsetInVector = 0) override;
     void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET) override;
 
     void append(ColumnChunk* columnChunk, common::node_group_idx_t nodeGroupIdx) override;
 
-    void writeValue(const ColumnChunkMetadata& chunkMeta, common::node_group_idx_t nodeGroupIdx,
-        common::offset_t offsetInChunk, common::ValueVector* vectorToWriteFrom,
-        uint32_t posInVectorToWriteFrom) override;
+    void writeValue(ChunkState& state, common::offset_t offsetInChunk,
+        common::ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) override;
 
-    void write(common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk,
-        ColumnChunk* data, common::offset_t dataOffset, common::length_t numValues) override;
+    void write(ChunkState& state, common::offset_t offsetInChunk, ColumnChunk* data,
+        common::offset_t dataOffset, common::length_t numValues) override;
 
     void prepareCommit() override;
     void checkpointInMemory() override;
     void rollbackInMemory() override;
 
     inline const DictionaryColumn& getDictionary() const { return dictionary; }
 
 protected:
-    void scanInternal(transaction::Transaction* transaction, ReadState& readState,
+    void scanInternal(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override;
-    void scanUnfiltered(transaction::Transaction* transaction, ReadState& readState,
+    void scanUnfiltered(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t startOffsetInChunk, common::offset_t numValuesToRead,
         common::ValueVector* resultVector, common::sel_t startPosInVector = 0);
-    void scanFiltered(transaction::Transaction* transaction, ReadState& readState,
+    void scanFiltered(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t startOffsetInChunk, common::ValueVector* nodeIDVector,
         common::ValueVector* resultVector);
 
-    void lookupInternal(transaction::Transaction* transaction, ReadState& readState,
+    void lookupInternal(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override;
 
 private:
-    bool canCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunk,
+    bool canCommitInPlace(const ChunkState& state, const ChunkCollection& localInsertChunk,
         const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunk,
         const offset_to_row_idx_t& updateInfo) override;
-    bool canCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
+    bool canCommitInPlace(const ChunkState& state, const std::vector<common::offset_t>& dstOffsets,
         ColumnChunk* chunk, common::offset_t srcOffset) override;
 
-    bool canIndexCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, uint64_t numStrings, common::offset_t maxOffset);
-
-    bool checkUpdateInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const ChunkCollection& localChunk,
-        const offset_to_row_idx_t& writeInfo);
+    bool canIndexCommitInPlace(const Column::ChunkState& dataState, uint64_t numStrings,
+        common::offset_t maxOffset);
 
 private:
     // Main column stores indices of values in the dictionary
     DictionaryColumn dictionary;
 };
 
 } // namespace storage
```

### sdist/kuzu-source/src/include/storage/store/struct_column.h

```diff
@@ -8,58 +8,56 @@
 class StructColumn final : public Column {
 public:
     StructColumn(std::string name, common::LogicalType dataType,
         const MetadataDAHInfo& metaDAHeaderInfo, BMFileHandle* dataFH, BMFileHandle* metadataFH,
         BufferManager* bufferManager, WAL* wal, transaction::Transaction* transaction,
         RWPropertyStats propertyStatistics, bool enableCompression);
 
-    void initReadState(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
-        common::offset_t startOffsetInChunk, ReadState& columnReadState) override;
+    void initChunkState(transaction::Transaction* transaction,
+        common::node_group_idx_t nodeGroupIdx, ChunkState& columnReadState) override;
     void scan(transaction::Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
         ColumnChunk* columnChunk, common::offset_t startOffset = 0,
         common::offset_t endOffset = common::INVALID_OFFSET) override;
-    void scan(transaction::Transaction* transaction, ReadState& readState,
+    void scan(transaction::Transaction* transaction, ChunkState& readState,
         common::offset_t startOffsetInGroup, common::offset_t endOffsetInGroup,
         common::ValueVector* resultVector, uint64_t offsetInVector) override;
 
     void append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) override;
 
     void checkpointInMemory() override;
     void rollbackInMemory() override;
     void prepareCommit() override;
 
     inline Column* getChild(common::vector_idx_t childIdx) {
         KU_ASSERT(childIdx < childColumns.size());
         return childColumns[childIdx].get();
     }
-    void write(common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk,
+    void write(ChunkState& state, common::offset_t offsetInChunk,
         common::ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) override;
-    void write(common::node_group_idx_t nodeGroupIdx, common::offset_t offsetInChunk,
-        ColumnChunk* data, common::offset_t dataOffset, common::length_t numValues) override;
+    void write(ChunkState& state, common::offset_t offsetInChunk, ColumnChunk* data,
+        common::offset_t dataOffset, common::length_t numValues) override;
 
     void prepareCommitForChunk(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunk,
         const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunk,
         const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo) override;
     void prepareCommitForChunk(transaction::Transaction* transaction,
         common::node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
         ColumnChunk* chunk, common::offset_t startSrcOffset) override;
 
 protected:
-    void scanInternal(transaction::Transaction* transaction, ReadState& readState,
+    void scanInternal(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override;
-    void lookupInternal(transaction::Transaction* transaction, ReadState& readState,
+    void lookupInternal(transaction::Transaction* transaction, ChunkState& readState,
         common::ValueVector* nodeIDVector, common::ValueVector* resultVector) override;
 
-    bool canCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunk,
+    bool canCommitInPlace(const ChunkState& state, const ChunkCollection& localInsertChunk,
         const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunk,
         const offset_to_row_idx_t& updateInfo) override;
-    bool canCommitInPlace(transaction::Transaction* transaction,
-        common::node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
+    bool canCommitInPlace(const ChunkState& state, const std::vector<common::offset_t>& dstOffsets,
         ColumnChunk* chunk, common::offset_t dataOffset) override;
 
 private:
     static ChunkCollection getStructChildChunkCollection(const ChunkCollection& chunkCollection,
         common::vector_idx_t childIdx);
 
 private:
```

### sdist/kuzu-source/src/main/storage_driver.cpp

```diff
@@ -67,16 +67,16 @@
     if (dataType.getPhysicalType() == PhysicalTypeID::LIST ||
         dataType.getPhysicalType() == PhysicalTypeID::ARRAY) {
         auto resultVector = ValueVector(dataType);
         for (auto i = 0u; i < size; ++i) {
             auto nodeOffset = offsets[i];
             auto [nodeGroupIdx, offsetInChunk] =
                 StorageUtils::getNodeGroupIdxAndOffsetInChunk(nodeOffset);
-            Column::ReadState readState;
-            column->initReadState(transaction, nodeGroupIdx, offsetInChunk, readState);
+            Column::ChunkState readState;
+            column->initChunkState(transaction, nodeGroupIdx, readState);
             column->scan(transaction, readState, offsetInChunk, offsetInChunk + 1, &resultVector,
                 i);
         }
         auto dataVector = ListVector::getDataVector(&resultVector);
         auto dataVectorSize = ListVector::getDataVectorSize(&resultVector);
         auto dataChildTypeSize = LogicalTypeUtils::getRowLayoutSize(dataVector->dataType);
         memcpy(result, dataVector->getData(), dataVectorSize * dataChildTypeSize);
```

### sdist/kuzu-source/src/parser/transform/transform_standalone_call.cpp

```diff
@@ -3,13 +3,13 @@
 
 namespace kuzu {
 namespace parser {
 
 std::unique_ptr<Statement> Transformer::transformStandaloneCall(
     CypherParser::KU_StandaloneCallContext& ctx) {
     auto optionName = transformSymbolicName(*ctx.oC_SymbolicName());
-    auto parameter = transformLiteral(*ctx.oC_Literal());
+    auto parameter = transformExpression(*ctx.oC_Expression());
     return std::make_unique<StandaloneCall>(std::move(optionName), std::move(parameter));
 }
 
 } // namespace parser
 } // namespace kuzu
```

### sdist/kuzu-source/src/processor/map/map_standalone_call.cpp

```diff
@@ -6,17 +6,17 @@
 using namespace kuzu::planner;
 
 namespace kuzu {
 namespace processor {
 
 std::unique_ptr<PhysicalOperator> PlanMapper::mapStandaloneCall(
     planner::LogicalOperator* logicalOperator) {
-    auto logicalStandaloneCall = reinterpret_cast<LogicalStandaloneCall*>(logicalOperator);
+    auto logicalStandaloneCall = logicalOperator->constPtrCast<LogicalStandaloneCall>();
     auto optionValue =
-        reinterpret_cast<binder::LiteralExpression*>(logicalStandaloneCall->getOptionValue().get());
+        logicalStandaloneCall->getOptionValue()->constPtrCast<binder::LiteralExpression>();
     auto standaloneCallInfo = std::make_unique<StandaloneCallInfo>(
         logicalStandaloneCall->getOption(), *optionValue->getValue());
     return std::make_unique<StandaloneCall>(std::move(standaloneCallInfo),
         PhysicalOperatorType::STANDALONE_CALL, getOperatorID(),
         logicalStandaloneCall->getExpressionsForPrinting());
 }
```

### sdist/kuzu-source/src/processor/operator/persistent/reader/npy/npy_reader.cpp

```diff
@@ -292,14 +292,15 @@
         columnTypes.push_back(tmpColumnTypes[0]);
     }
 }
 
 static std::unique_ptr<function::TableFuncBindData> bindFunc(main::ClientContext* /*context*/,
     function::TableFuncBindInput* input) {
     auto scanInput = reinterpret_cast<function::ScanTableFuncBindInput*>(input);
+    KU_ASSERT(scanInput->config.options.empty());
     std::vector<std::string> detectedColumnNames;
     std::vector<common::LogicalType> detectedColumnTypes;
     bindColumns(scanInput->config, detectedColumnNames, detectedColumnTypes);
     std::vector<std::string> resultColumnNames;
     std::vector<common::LogicalType> resultColumnTypes;
     ReaderBindUtils::resolveColumns(scanInput->expectedColumnNames, detectedColumnNames,
         resultColumnNames, scanInput->expectedColumnTypes, detectedColumnTypes, resultColumnTypes);
```

### sdist/kuzu-source/src/processor/operator/persistent/reader/parquet/parquet_reader.cpp

```diff
@@ -1,11 +1,12 @@
 #include "processor/operator/persistent/reader/parquet/parquet_reader.h"
 
 #include <fcntl.h>
 
+#include "common/exception/binder.h"
 #include "common/exception/copy.h"
 #include "common/file_system/virtual_file_system.h"
 #include "common/string_format.h"
 #include "function/table/bind_data.h"
 #include "processor/operator/persistent/reader/parquet/list_column_reader.h"
 #include "processor/operator/persistent/reader/parquet/struct_column_reader.h"
 #include "processor/operator/persistent/reader/parquet/thrift_tools.h"
@@ -648,14 +649,17 @@
     }
 }
 
 static std::unique_ptr<function::TableFuncBindData> bindFunc(main::ClientContext* /*context*/,
     function::TableFuncBindInput* input) {
     auto scanInput =
         ku_dynamic_cast<function::TableFuncBindInput*, function::ScanTableFuncBindInput*>(input);
+    if (!scanInput->config.options.empty()) {
+        throw BinderException{"Copy from Parquet cannot have options."};
+    }
     std::vector<std::string> detectedColumnNames;
     std::vector<common::LogicalType> detectedColumnTypes;
     bindColumns(scanInput, detectedColumnNames, detectedColumnTypes);
     std::vector<std::string> resultColumnNames;
     std::vector<common::LogicalType> resultColumnTypes;
     ReaderBindUtils::resolveColumns(scanInput->expectedColumnNames, detectedColumnNames,
         resultColumnNames, scanInput->expectedColumnTypes, detectedColumnTypes, resultColumnTypes);
```

### sdist/kuzu-source/src/storage/stats/property_statistics.cpp

```diff
@@ -41,16 +41,18 @@
 
 void RWPropertyStats::setHasNull(const transaction::Transaction& transaction) {
     // TODO(Guodong): INVALID_PROPERTY_ID is used here because we have a column, i.e., nbrIDColumn,
     // not exposed as property in table schema, but still have nullColumn. Should be fixed once we
     // properly align properties and chunks.
     if (propertyID != common::INVALID_PROPERTY_ID) {
         KU_ASSERT(tablesStatistics);
-        auto propStats =
+        auto& propStats =
             tablesStatistics->getPropertyStatisticsForTable(transaction, tableID, propertyID);
-        propStats.setHasNull();
-        tablesStatistics->setPropertyStatisticsForTable(tableID, propertyID, propStats);
+        if (!propStats.mayHaveNull()) {
+            propStats.setHasNull();
+            tablesStatistics->setToUpdated();
+        }
     }
 }
 
 } // namespace storage
 } // namespace kuzu
```

### sdist/kuzu-source/src/storage/store/column.cpp

```diff
@@ -97,74 +97,71 @@
     SerialColumn(std::string name, const MetadataDAHInfo& metaDAHeaderInfo, BMFileHandle* dataFH,
         BMFileHandle* metadataFH, BufferManager* bufferManager, WAL* wal, Transaction* transaction)
         : Column{name, *LogicalType::SERIAL(), metaDAHeaderInfo, dataFH, metadataFH,
               // Serials can't be null, so they don't need PropertyStatistics
               bufferManager, wal, transaction, RWPropertyStats::empty(),
               false /* enableCompression */, false /*requireNullColumn*/} {}
 
-    void scan(Transaction*, ReadState&, ValueVector* nodeIDVector,
+    void scan(Transaction*, ChunkState&, ValueVector* nodeIDVector,
         ValueVector* resultVector) override {
         // Serial column cannot contain null values.
         for (auto i = 0ul; i < nodeIDVector->state->selVector->selectedSize; i++) {
             auto pos = nodeIDVector->state->selVector->selectedPositions[i];
             auto offset = nodeIDVector->readNodeOffset(pos);
             resultVector->setNull(pos, false);
             resultVector->setValue<offset_t>(pos, offset);
         }
     }
 
-    void lookup(Transaction*, ReadState&, ValueVector* nodeIDVector,
+    void lookup(Transaction*, ChunkState&, ValueVector* nodeIDVector,
         ValueVector* resultVector) override {
         // Serial column cannot contain null values.
         for (auto i = 0ul; i < nodeIDVector->state->selVector->selectedSize; i++) {
             auto pos = nodeIDVector->state->selVector->selectedPositions[i];
             auto offset = nodeIDVector->readNodeOffset(pos);
             resultVector->setNull(pos, false);
             resultVector->setValue<offset_t>(pos, offset);
         }
     }
 
-    bool canCommitInPlace(Transaction*, node_group_idx_t, const ChunkCollection&,
-        const offset_to_row_idx_t&, const ChunkCollection&,
-        const offset_to_row_idx_t& updateInfo) override {
+    bool canCommitInPlace(const ChunkState&, const ChunkCollection&, const offset_to_row_idx_t&,
+        const ChunkCollection&, const offset_to_row_idx_t& updateInfo) override {
         (void)updateInfo; // Avoid unused parameter warnings during release build.
         KU_ASSERT(updateInfo.empty());
         return true;
     }
 
-    bool canCommitInPlace(transaction::Transaction* /*transaction*/,
-        common::node_group_idx_t /*nodeGroupIdx*/,
-        const std::vector<common::offset_t>& /*dstOffset*/, ColumnChunk* /*chunk*/,
-        common::offset_t /*startOffset*/) override {
+    bool canCommitInPlace(const ChunkState&, const std::vector<common::offset_t>&, ColumnChunk*,
+        common::offset_t) override {
         // Note: only updates to rel table can trigger this code path. SERIAL is not supported in
         // rel table yet.
         KU_UNREACHABLE;
     }
 
-    void commitLocalChunkInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-        const ChunkCollection&, const offset_to_row_idx_t& insertInfo, const ChunkCollection&,
+    void commitLocalChunkInPlace(Transaction*, ChunkState& state, const ChunkCollection&,
+        const offset_to_row_idx_t& insertInfo, const ChunkCollection&,
         const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo) override {
         // Avoid unused parameter warnings during release build.
         (void)updateInfo;
         (void)deleteInfo;
         KU_ASSERT(updateInfo.empty() && deleteInfo.empty());
-        auto chunkMeta = metadataDA->get(nodeGroupIdx, transaction->getType());
-        auto numValues = chunkMeta.numValues;
+        auto numValues = state.metadata.numValues;
         for (auto& [offsetInChunk, _] : insertInfo) {
             if (offsetInChunk >= numValues) {
                 numValues = offsetInChunk + 1;
             }
         }
-        if (numValues > chunkMeta.numValues) {
-            chunkMeta.numValues = numValues;
-            metadataDA->update(nodeGroupIdx, chunkMeta);
+        if (numValues > state.metadata.numValues) {
+            state.metadata.numValues = numValues;
+            // TODO: Avoid updating metadataDA.
+            metadataDA->update(state.nodeGroupIdx, state.metadata);
         }
     }
 
-    void commitLocalChunkOutOfPlace(Transaction* /*transaction*/, node_group_idx_t nodeGroupIdx,
+    void commitLocalChunkOutOfPlace(Transaction*, node_group_idx_t nodeGroupIdx,
         bool isNewNodeGroup, const ChunkCollection&, const offset_to_row_idx_t& insertInfo,
         const ChunkCollection&, const offset_to_row_idx_t& updateInfo,
         const offset_set_t& deleteInfo) override {
         // Avoid unused parameter warnings during release build.
         (void)isNewNodeGroup;
         (void)updateInfo;
         (void)deleteInfo;
@@ -176,17 +173,16 @@
         }
         ColumnChunkMetadata chunkMeta;
         chunkMeta.numValues = numValues;
         metadataDA->resize(nodeGroupIdx + 1);
         metadataDA->update(nodeGroupIdx, chunkMeta);
     }
 
-    void commitColumnChunkInPlace(common::node_group_idx_t /*nodeGroupIdx*/,
-        const std::vector<common::offset_t>& /*dstOffset*/, ColumnChunk* /*chunk*/,
-        common::offset_t /*srcOffsetInChunk*/) override {
+    void commitColumnChunkInPlace(ChunkState&, const std::vector<common::offset_t>&, ColumnChunk*,
+        common::offset_t) override {
         // Note: only updates to rel table can trigger this code path. SERIAL is not supported in
         // rel table yet.
         KU_UNREACHABLE;
     }
 
     void commitColumnChunkOutOfPlace(Transaction* /*transaction*/,
         common::node_group_idx_t /*nodeGroupIdx*/, bool /*isNewNodeGroup*/,
@@ -255,54 +251,55 @@
 // NOTE: This function should only be called on node tables.
 void Column::batchLookup(Transaction* transaction, const offset_t* nodeOffsets, size_t size,
     uint8_t* result) {
     for (auto i = 0u; i < size; ++i) {
         auto nodeOffset = nodeOffsets[i];
         auto [nodeGroupIdx, offsetInChunk] =
             StorageUtils::getNodeGroupIdxAndOffsetInChunk(nodeOffset);
-        auto cursor = getPageCursorForOffset(transaction->getType(), nodeGroupIdx, offsetInChunk);
+        ChunkState state;
+        initChunkState(transaction, nodeGroupIdx, state);
+        auto cursor = getPageCursorForOffsetInGroup(offsetInChunk, state);
         auto chunkMeta = metadataDA->get(nodeGroupIdx, transaction->getType());
         KU_ASSERT(isPageIdxValid(cursor.pageIdx, chunkMeta));
         readFromPage(transaction, cursor.pageIdx, [&](uint8_t* frame) -> void {
             batchLookupFunc(frame, cursor, result, i, 1, chunkMeta.compMeta);
         });
     }
 }
 
-void Column::initReadState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    common::offset_t startOffsetInChunk, ReadState& readState) {
+void Column::initChunkState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+    ChunkState& readState) {
     if (nullColumn) {
         if (!readState.nullState) {
-            readState.nullState = std::make_unique<ReadState>();
+            readState.nullState = std::make_unique<ChunkState>();
         }
-        nullColumn->initReadState(transaction, nodeGroupIdx, startOffsetInChunk,
-            *readState.nullState);
+        nullColumn->initChunkState(transaction, nodeGroupIdx, *readState.nullState);
     }
     KU_ASSERT(nodeGroupIdx < metadataDA->getNumElements(transaction->getType()));
     if (nodeGroupIdx != readState.nodeGroupIdx) {
         // Only update metadata and numValuesPerPage if we're reading a different node group.
         // This is an optimization to reduce accesses to metadataDA, which can lead to contention
         // due to lock acquiring in DiskArray.
         readState.nodeGroupIdx = nodeGroupIdx;
         readState.metadata = metadataDA->get(nodeGroupIdx, transaction->getType());
         readState.numValuesPerPage =
             readState.metadata.compMeta.numValues(BufferPoolConstants::PAGE_4KB_SIZE, dataType);
     }
 }
 
-void Column::scan(Transaction* transaction, ReadState& readState, ValueVector* nodeIDVector,
+void Column::scan(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
     ValueVector* resultVector) {
     if (nullColumn) {
         KU_ASSERT(readState.nullState);
         nullColumn->scan(transaction, *readState.nullState, nodeIDVector, resultVector);
     }
     scanInternal(transaction, readState, nodeIDVector, resultVector);
 }
 
-void Column::scan(Transaction* transaction, ReadState& readState, offset_t startOffsetInGroup,
+void Column::scan(Transaction* transaction, ChunkState& readState, offset_t startOffsetInGroup,
     offset_t endOffsetInGroup, ValueVector* resultVector, uint64_t offsetInVector) {
     if (nullColumn) {
         KU_ASSERT(readState.nullState);
         nullColumn->scan(transaction, *readState.nullState, startOffsetInGroup, endOffsetInGroup,
             resultVector, offsetInVector);
     }
     auto pageCursor = getPageCursorForOffsetInGroup(startOffsetInGroup, readState);
@@ -350,15 +347,15 @@
             cursor.nextPage();
         }
         KU_ASSERT(numValuesScanned == numValuesToScan);
         columnChunk->setNumValues(numValuesScanned);
     }
 }
 
-void Column::scan(Transaction* transaction, const ReadState& state, offset_t startOffsetInGroup,
+void Column::scan(Transaction* transaction, const ChunkState& state, offset_t startOffsetInGroup,
     offset_t endOffsetInGroup, uint8_t* result) {
     auto cursor = getPageCursorForOffsetInGroup(startOffsetInGroup, state);
     auto numValuesToScan = endOffsetInGroup - startOffsetInGroup;
     uint64_t numValuesScanned = 0;
     while (numValuesScanned < numValuesToScan) {
         uint64_t numValuesToScanInPage =
             std::min((uint64_t)state.numValuesPerPage - cursor.elemPosInPage,
@@ -368,16 +365,16 @@
                 state.metadata.compMeta);
         });
         numValuesScanned += numValuesToScanInPage;
         cursor.nextPage();
     }
 }
 
-void Column::scanInternal(Transaction* transaction, ReadState& readState, ValueVector* nodeIDVector,
-    ValueVector* resultVector) {
+void Column::scanInternal(Transaction* transaction, ChunkState& readState,
+    ValueVector* nodeIDVector, ValueVector* resultVector) {
     auto [nodeGroupIdx, startOffsetInChunk] =
         StorageUtils::getNodeGroupIdxAndOffsetInChunk(nodeIDVector->readNodeOffset(0));
     KU_ASSERT(nodeGroupIdx == readState.nodeGroupIdx);
     auto cursor = getPageCursorForOffsetInGroup(startOffsetInChunk, readState);
     if (nodeIDVector->state->selVector->isUnfiltered()) {
         scanUnfiltered(transaction, cursor, nodeIDVector->state->selVector->selectedSize,
             resultVector, readState.metadata);
@@ -431,36 +428,36 @@
             posInSelVector < nodeIDVector->state->selVector->selectedSize &&
             nodeIDVector->state->selVector->selectedPositions[posInSelVector] < numValuesScanned) {
             posInSelVector++;
         }
     }
 }
 
-void Column::lookup(Transaction* transaction, ReadState& readState, ValueVector* nodeIDVector,
+void Column::lookup(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
     ValueVector* resultVector) {
     if (nullColumn) {
         KU_ASSERT(readState.nullState);
         nullColumn->lookup(transaction, *readState.nullState, nodeIDVector, resultVector);
     }
     lookupInternal(transaction, readState, nodeIDVector, resultVector);
 }
 
-void Column::lookupInternal(transaction::Transaction* transaction, ReadState& readState,
+void Column::lookupInternal(transaction::Transaction* transaction, ChunkState& readState,
     ValueVector* nodeIDVector, ValueVector* resultVector) {
     for (auto i = 0ul; i < nodeIDVector->state->selVector->selectedSize; i++) {
         auto pos = nodeIDVector->state->selVector->selectedPositions[i];
         if (nodeIDVector->isNull(pos)) {
             continue;
         }
         auto nodeOffset = nodeIDVector->readNodeOffset(pos);
         lookupValue(transaction, readState, nodeOffset, resultVector, pos);
     }
 }
 
-void Column::lookupValue(transaction::Transaction* transaction, ReadState& readState,
+void Column::lookupValue(transaction::Transaction* transaction, ChunkState& readState,
     offset_t nodeOffset, ValueVector* resultVector, uint32_t posInVector) {
     auto [nodeGroupIdx, offsetInChunk] = StorageUtils::getNodeGroupIdxAndOffsetInChunk(nodeOffset);
     auto cursor = getPageCursorForOffsetInGroup(offsetInChunk, readState);
     KU_ASSERT(isPageIdxValid(cursor.pageIdx, readState.metadata));
     readFromPage(transaction, cursor.pageIdx, [&](uint8_t* frame) -> void {
         readToVectorFunc(frame, cursor, resultVector, posInVector, 1 /* numValuesToRead */,
             readState.metadata.compMeta);
@@ -507,57 +504,49 @@
     metadataDA->update(nodeGroupIdx, metadata);
     if (nullColumn) {
         // Null column chunk.
         nullColumn->append(columnChunk->getNullChunk(), nodeGroupIdx);
     }
 }
 
-void Column::write(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk,
-    ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) {
+void Column::write(ChunkState& state, offset_t offsetInChunk, ValueVector* vectorToWriteFrom,
+    uint32_t posInVectorToWriteFrom) {
     bool isNull = vectorToWriteFrom->isNull(posInVectorToWriteFrom);
-    auto chunkMeta = metadataDA->get(nodeGroupIdx, TransactionType::WRITE);
     if (!isNull) {
-        writeValue(chunkMeta, nodeGroupIdx, offsetInChunk, vectorToWriteFrom,
-            posInVectorToWriteFrom);
+        writeValue(state, offsetInChunk, vectorToWriteFrom, posInVectorToWriteFrom);
     }
-    if (offsetInChunk >= chunkMeta.numValues) {
-        chunkMeta.numValues = offsetInChunk + 1;
-        KU_ASSERT(sanityCheckForWrites(chunkMeta, dataType));
-        metadataDA->update(nodeGroupIdx, chunkMeta);
+    if (offsetInChunk >= state.metadata.numValues) {
+        state.metadata.numValues = offsetInChunk + 1;
     }
 }
 
-void Column::writeValue(const ColumnChunkMetadata& chunkMeta, node_group_idx_t nodeGroupIdx,
-    offset_t offsetInChunk, ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) {
-    updatePageWithCursor(
-        getPageCursorForOffset(TransactionType::WRITE, nodeGroupIdx, offsetInChunk),
+void Column::writeValue(ChunkState& state, offset_t offsetInChunk, ValueVector* vectorToWriteFrom,
+    uint32_t posInVectorToWriteFrom) {
+    updatePageWithCursor(getPageCursorForOffsetInGroup(offsetInChunk, state),
         [&](auto frame, auto posInPage) {
             writeFromVectorFunc(frame, posInPage, vectorToWriteFrom, posInVectorToWriteFrom,
-                chunkMeta.compMeta);
+                state.metadata.compMeta);
         });
 }
 
-void Column::write(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk, ColumnChunk* data,
+void Column::write(ChunkState& state, offset_t offsetInChunk, ColumnChunk* data,
     offset_t dataOffset, length_t numValues) {
-    auto state = getReadState(TransactionType::WRITE, nodeGroupIdx);
     NullMask nullMask{std::span<uint64_t>()};
     NullMask* nullMaskPtr = nullptr;
     if (data->getNullChunk()) {
         nullMask = data->getNullChunk()->getNullMask();
         nullMaskPtr = &nullMask;
     }
     writeValues(state, offsetInChunk, data->getData(), nullMaskPtr, dataOffset, numValues);
     if (offsetInChunk + numValues > state.metadata.numValues) {
         state.metadata.numValues = offsetInChunk + numValues;
-        KU_ASSERT(sanityCheckForWrites(state.metadata, dataType));
-        metadataDA->update(nodeGroupIdx, state.metadata);
     }
 }
 
-void Column::writeValues(ReadState& state, common::offset_t dstOffset, const uint8_t* data,
+void Column::writeValues(ChunkState& state, common::offset_t dstOffset, const uint8_t* data,
     const common::NullMask* nullChunkData, common::offset_t srcOffset, common::offset_t numValues) {
     auto numValuesWritten = 0u;
     auto cursor = getPageCursorForOffsetInGroup(dstOffset, state);
     while (numValuesWritten < numValues) {
         auto numValuesToWriteInPage =
             std::min(numValues - numValuesWritten, state.numValuesPerPage - cursor.elemPosInPage);
         updatePageWithCursor(cursor, [&](auto frame, auto offsetInPage) {
@@ -566,28 +555,29 @@
         });
 
         numValuesWritten += numValuesToWriteInPage;
         cursor.nextPage();
     }
 }
 
-offset_t Column::appendValues(node_group_idx_t nodeGroupIdx, const uint8_t* data,
+// Apend to the end of the chunk.
+offset_t Column::appendValues(ChunkState& state, const uint8_t* data,
     const common::NullMask* nullChunkData, offset_t numValues) {
-    auto state = getReadState(TransactionType::WRITE, nodeGroupIdx);
     auto startOffset = state.metadata.numValues;
     auto numPages = dataFH->getNumPages();
+    // TODO: writeValues should return new pages appended if any.
     writeValues(state, state.metadata.numValues, data, nullChunkData, 0 /*dataOffset*/, numValues);
     auto newNumPages = dataFH->getNumPages();
     state.metadata.numValues += numValues;
     state.metadata.numPages += (newNumPages - numPages);
-    metadataDA->update(nodeGroupIdx, state.metadata);
+    metadataDA->update(state.nodeGroupIdx, state.metadata);
     return startOffset;
 }
 
-PageCursor Column::getPageCursorForOffsetInGroup(offset_t offsetInChunk, const ReadState& state) {
+PageCursor Column::getPageCursorForOffsetInGroup(offset_t offsetInChunk, const ChunkState& state) {
     auto pageCursor = PageUtils::getPageCursorForPos(offsetInChunk, state.numValuesPerPage);
     pageCursor.pageIdx += state.metadata.pageIdx;
     return pageCursor;
 }
 
 void Column::updatePageWithCursor(PageCursor cursor,
     const std::function<void(uint8_t*, offset_t)>& writeOp) {
@@ -599,61 +589,60 @@
         DBFileUtils::insertNewPage(*dataFH, dbFileID, *bufferManager, *wal);
         insertingNewPage = true;
     }
     DBFileUtils::updatePage(*dataFH, dbFileID, cursor.pageIdx, insertingNewPage, *bufferManager,
         *wal, [&](auto frame) { writeOp(frame, cursor.elemPosInPage); });
 }
 
-Column::ReadState Column::getReadState(TransactionType transactionType,
-    node_group_idx_t nodeGroupIdx) const {
-    auto metadata = metadataDA->get(nodeGroupIdx, transactionType);
-    return {metadata, metadata.compMeta.numValues(BufferPoolConstants::PAGE_4KB_SIZE, dataType)};
-}
-
 void Column::prepareCommit() {
     metadataDA->prepareCommit();
     if (nullColumn) {
         nullColumn->prepareCommit();
     }
 }
 
-void Column::prepareCommitForChunk(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+void Column::prepareCommitForChunk(Transaction* transaction, common::node_group_idx_t nodeGroupIdx,
     const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
     const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
     const offset_set_t& deleteInfo) {
     auto currentNumNodeGroups = metadataDA->getNumElements(transaction->getType());
     auto isNewNodeGroup = nodeGroupIdx >= currentNumNodeGroups;
     if (isNewNodeGroup) {
         // If this is a new node group, updateInfo should be empty. We should perform out-of-place
         // commit with a new column chunk.
         commitLocalChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, localInsertChunks,
             insertInfo, localUpdateChunks, updateInfo, deleteInfo);
     } else {
         bool didInPlaceCommit = false;
+        ChunkState state;
+        initChunkState(transaction, nodeGroupIdx, state);
         // If this is not a new node group, we should first check if we can perform in-place commit.
-        if (canCommitInPlace(transaction, nodeGroupIdx, localInsertChunks, insertInfo,
-                localUpdateChunks, updateInfo)) {
-            commitLocalChunkInPlace(transaction, nodeGroupIdx, localInsertChunks, insertInfo,
+        if (canCommitInPlace(state, localInsertChunks, insertInfo, localUpdateChunks, updateInfo)) {
+            commitLocalChunkInPlace(transaction, state, localInsertChunks, insertInfo,
                 localUpdateChunks, updateInfo, deleteInfo);
             didInPlaceCommit = true;
+            KU_ASSERT(sanityCheckForWrites(state.metadata, dataType));
+            metadataDA->update(nodeGroupIdx, state.metadata);
         } else {
-            commitLocalChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, localInsertChunks,
-                insertInfo, localUpdateChunks, updateInfo, deleteInfo);
+            commitLocalChunkOutOfPlace(transaction, state.nodeGroupIdx, isNewNodeGroup,
+                localInsertChunks, insertInfo, localUpdateChunks, updateInfo, deleteInfo);
         }
         // TODO(Guodong/Ben): The logic here on NullColumn is confusing as out-of-place commits and
         // in-place commits handle it differently. See if we can unify them.
         if (nullColumn) {
             // Uses functions written for the null chunk which only access the localColumnChunk's
             // null information
-            if (nullColumn->canCommitInPlace(transaction, nodeGroupIdx,
+            KU_ASSERT(state.nullState);
+            if (nullColumn->canCommitInPlace(*state.nullState,
                     getNullChunkCollection(localInsertChunks), insertInfo,
                     getNullChunkCollection(localUpdateChunks), updateInfo)) {
-                nullColumn->commitLocalChunkInPlace(transaction, nodeGroupIdx,
+                nullColumn->commitLocalChunkInPlace(transaction, *state.nullState,
                     getNullChunkCollection(localInsertChunks), insertInfo,
                     getNullChunkCollection(localUpdateChunks), updateInfo, deleteInfo);
+                nullColumn->metadataDA->update(nodeGroupIdx, state.nullState->metadata);
             } else if (didInPlaceCommit) {
                 // Out-of-place commits also commit the null chunk out of place,
                 // so we only need to do a separate out of place commit for the null chunk if the
                 // main chunk did an in-place commit.
                 nullColumn->commitLocalChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup,
                     getNullChunkCollection(localInsertChunks), insertInfo,
                     getNullChunkCollection(localUpdateChunks), updateInfo, deleteInfo);
@@ -662,33 +651,40 @@
     }
 }
 
 void Column::prepareCommitForChunk(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk, offset_t startSrcOffset) {
     metadataDA->prepareCommit();
     auto currentNumNodeGroups = metadataDA->getNumElements(transaction->getType());
+    // TODO: Move newNodeGroup out to the table data level.
     auto isNewNodeGroup = nodeGroupIdx >= currentNumNodeGroups;
     if (isNewNodeGroup) {
         commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets, chunk,
             startSrcOffset);
     } else {
         bool didInPlaceCommit = false;
         // If this is not a new node group, we should first check if we can perform in-place commit.
-        if (canCommitInPlace(transaction, nodeGroupIdx, dstOffsets, chunk, startSrcOffset)) {
-            commitColumnChunkInPlace(nodeGroupIdx, dstOffsets, chunk, startSrcOffset);
+        ChunkState state;
+        initChunkState(transaction, nodeGroupIdx, state);
+        if (canCommitInPlace(state, dstOffsets, chunk, startSrcOffset)) {
+            commitColumnChunkInPlace(state, dstOffsets, chunk, startSrcOffset);
             didInPlaceCommit = true;
+            KU_ASSERT(sanityCheckForWrites(state.metadata, dataType));
+            metadataDA->update(nodeGroupIdx, state.metadata);
         } else {
             commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets,
                 chunk, startSrcOffset);
         }
         if (nullColumn) {
-            if (nullColumn->canCommitInPlace(transaction, nodeGroupIdx, dstOffsets,
-                    chunk->getNullChunk(), startSrcOffset)) {
-                nullColumn->commitColumnChunkInPlace(nodeGroupIdx, dstOffsets,
+            KU_ASSERT(state.nullState);
+            if (nullColumn->canCommitInPlace(*state.nullState, dstOffsets, chunk->getNullChunk(),
+                    startSrcOffset)) {
+                nullColumn->commitColumnChunkInPlace(*state.nullState, dstOffsets,
                     chunk->getNullChunk(), startSrcOffset);
+                nullColumn->metadataDA->update(nodeGroupIdx, state.nullState->metadata);
             } else if (didInPlaceCommit) {
                 nullColumn->commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup,
                     dstOffsets, chunk->getNullChunk(), startSrcOffset);
             }
         }
     }
 }
@@ -734,54 +730,52 @@
                 offsetInLocalChunk, dataType.getPhysicalType())) {
             return false;
         }
     }
     return true;
 }
 
-bool Column::canCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
-    const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo) {
-    auto metadata = getMetadata(nodeGroupIdx, transaction->getType());
-    if (isInsertionsOutOfPagesCapacity(metadata, insertInfo)) {
+bool Column::canCommitInPlace(const ChunkState& state, const ChunkCollection& localInsertChunks,
+    const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
+    const offset_to_row_idx_t& updateInfo) {
+    if (isInsertionsOutOfPagesCapacity(state.metadata, insertInfo)) {
         return false;
     }
-    if (metadata.compMeta.canAlwaysUpdateInPlace()) {
+    if (state.metadata.compMeta.canAlwaysUpdateInPlace()) {
         return true;
     }
-    return checkUpdateInPlace(metadata, localInsertChunks, insertInfo) &&
-           checkUpdateInPlace(metadata, localUpdateChunks, updateInfo);
+    return checkUpdateInPlace(state.metadata, localInsertChunks, insertInfo) &&
+           checkUpdateInPlace(state.metadata, localUpdateChunks, updateInfo);
 }
 
-bool Column::canCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+bool Column::canCommitInPlace(const ChunkState& state,
     const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk,
     common::offset_t srcOffset) {
     auto maxDstOffset = getMaxOffset(dstOffsets);
-    auto metadata = getMetadata(nodeGroupIdx, transaction->getType());
-    if (isMaxOffsetOutOfPagesCapacity(metadata, maxDstOffset)) {
+    if (isMaxOffsetOutOfPagesCapacity(state.metadata, maxDstOffset)) {
         return false;
     }
-    if (metadata.compMeta.canAlwaysUpdateInPlace()) {
+    if (state.metadata.compMeta.canAlwaysUpdateInPlace()) {
         return true;
     }
     for (auto i = 0u; i < dstOffsets.size(); i++) {
-        if (!metadata.compMeta.canUpdateInPlace(chunk->getData(), srcOffset + i,
+        if (!state.metadata.compMeta.canUpdateInPlace(chunk->getData(), srcOffset + i,
                 dataType.getPhysicalType())) {
             return false;
         }
     }
     return true;
 }
 
-void Column::commitLocalChunkInPlace(Transaction* /*transaction*/, node_group_idx_t nodeGroupIdx,
+void Column::commitLocalChunkInPlace(Transaction*, ChunkState& state,
     const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
     const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
-    const offset_set_t& /*deleteInfo*/) {
-    applyLocalChunkToColumn(nodeGroupIdx, localUpdateChunks, updateInfo);
-    applyLocalChunkToColumn(nodeGroupIdx, localInsertChunks, insertInfo);
+    const offset_set_t&) {
+    applyLocalChunkToColumn(state, localUpdateChunks, updateInfo);
+    applyLocalChunkToColumn(state, localInsertChunks, insertInfo);
 }
 
 std::unique_ptr<ColumnChunk> Column::getEmptyChunkForCommit(uint64_t capacity) {
     return ColumnChunkFactory::createColumnChunk(*dataType.copy(), enableCompression, capacity);
 }
 
 void Column::commitLocalChunkOutOfPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
@@ -808,18 +802,19 @@
         }
     }
     columnChunk->finalize();
     KU_ASSERT(columnChunk->sanityCheck());
     append(columnChunk.get(), nodeGroupIdx);
 }
 
-void Column::commitColumnChunkInPlace(node_group_idx_t nodeGroupIdx,
-    const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk, offset_t srcOffset) {
+void Column::commitColumnChunkInPlace(ChunkState& state, const std::vector<offset_t>& dstOffsets,
+    ColumnChunk* chunk, offset_t srcOffset) {
+    // TODO: Should always sort dstOffsets, and group writes to the same page.
     for (auto i = 0u; i < dstOffsets.size(); i++) {
-        write(nodeGroupIdx, dstOffsets[i], chunk, srcOffset + i, 1 /* numValues */);
+        write(state, dstOffsets[i], chunk, srcOffset + i, 1 /* numValues */);
     }
 }
 
 void Column::commitColumnChunkOutOfPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     bool isNewNodeGroup, const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk,
     offset_t srcOffset) {
     if (isNewNodeGroup) {
@@ -846,28 +841,25 @@
         auto [chunkIdx, offsetInLocalChunk] =
             LocalChunkedGroupCollection::getChunkIdxAndOffsetInChunk(rowIdx);
         columnChunk->write(localChunks[chunkIdx], offsetInLocalChunk, offsetInDstChunk,
             1 /* numValues */);
     }
 }
 
-void Column::applyLocalChunkToColumn(node_group_idx_t nodeGroupIdx,
-    const ChunkCollection& localChunks, const offset_to_row_idx_t& updateInfo) {
+void Column::applyLocalChunkToColumn(ChunkState& state, const ChunkCollection& localChunks,
+    const offset_to_row_idx_t& updateInfo) {
     for (auto& [offsetInDstChunk, rowIdx] : updateInfo) {
         auto [chunkIdx, offsetInLocalChunk] =
             LocalChunkedGroupCollection::getChunkIdxAndOffsetInChunk(rowIdx);
         if (!localChunks[chunkIdx]->getNullChunk()->isNull(offsetInLocalChunk)) {
-            write(nodeGroupIdx, offsetInDstChunk, localChunks[chunkIdx], offsetInLocalChunk,
+            write(state, offsetInDstChunk, localChunks[chunkIdx], offsetInLocalChunk,
                 1 /*numValues*/);
         } else {
-            auto chunkMeta = metadataDA->get(nodeGroupIdx, TransactionType::WRITE);
-            if (offsetInDstChunk >= chunkMeta.numValues) {
-                chunkMeta.numValues = offsetInDstChunk + 1;
-                KU_ASSERT(sanityCheckForWrites(chunkMeta, dataType));
-                metadataDA->update(nodeGroupIdx, chunkMeta);
+            if (offsetInDstChunk >= state.metadata.numValues) {
+                state.metadata.numValues = offsetInDstChunk + 1;
             }
         }
     }
 }
 
 void Column::checkpointInMemory() {
     metadataDA->checkpointInMemoryIfNecessary();
@@ -904,20 +896,14 @@
         } else {
             columnChunk->setNumValues(chunkMeta.numValues);
             append(columnChunk.get(), i);
         }
     }
 }
 
-PageCursor Column::getPageCursorForOffset(TransactionType transactionType,
-    node_group_idx_t nodeGroupIdx, offset_t offsetInChunk) {
-    auto state = getReadState(transactionType, nodeGroupIdx);
-    return getPageCursorForOffsetInGroup(offsetInChunk, state);
-}
-
 ChunkCollection Column::getNullChunkCollection(const ChunkCollection& chunkCollection) {
     ChunkCollection nullChunkCollection;
     for (const auto& chunk : chunkCollection) {
         nullChunkCollection.push_back(chunk->getNullChunk());
     }
     return nullChunkCollection;
 }
```

### sdist/kuzu-source/src/storage/store/dictionary_column.cpp

```diff
@@ -20,21 +20,21 @@
         stats, false /*enableCompression*/, false /*requireNullColumn*/);
     auto offsetColName = StorageUtils::getColumnName(name, StorageUtils::ColumnType::OFFSET, "");
     offsetColumn = std::make_unique<Column>(offsetColName, *LogicalType::UINT64(),
         *metaDAHeaderInfo.childrenInfos[1], dataFH, metadataFH, bufferManager, wal, transaction,
         stats, enableCompression, false /*requireNullColumn*/);
 }
 
-void DictionaryColumn::initReadState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    offset_t startOffsetInChunk, Column::ReadState& readState) {
+void DictionaryColumn::initChunkState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+    Column::ChunkState& readState) {
     // We put states for data and offset columns into childrenStates.
     readState.childrenStates.resize(2);
-    dataColumn->initReadState(transaction, nodeGroupIdx, startOffsetInChunk,
+    dataColumn->initChunkState(transaction, nodeGroupIdx,
         readState.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX]);
-    offsetColumn->initReadState(transaction, nodeGroupIdx, startOffsetInChunk,
+    offsetColumn->initChunkState(transaction, nodeGroupIdx,
         readState.childrenStates[OFFSET_COLUMN_CHILD_READ_STATE_IDX]);
 }
 
 void DictionaryColumn::append(node_group_idx_t nodeGroupIdx, const DictionaryChunk& dictChunk) {
     KU_ASSERT(dictChunk.sanityCheck());
     dataColumn->append(dictChunk.getStringDataChunk(), nodeGroupIdx);
     offsetColumn->append(dictChunk.getOffsetChunk(), nodeGroupIdx);
@@ -55,16 +55,16 @@
     // Make sure that the chunk is large enough
     if (offsetMetadata.numValues > offsetChunk->getCapacity()) {
         offsetChunk->resize(std::bit_ceil(offsetMetadata.numValues));
     }
     offsetColumn->scan(transaction, nodeGroupIdx, offsetChunk);
 }
 
-void DictionaryColumn::scan(Transaction* transaction, const Column::ReadState& offsetState,
-    const Column::ReadState& dataState,
+void DictionaryColumn::scan(Transaction* transaction, const Column::ChunkState& offsetState,
+    const Column::ChunkState& dataState,
     std::vector<std::pair<string_index_t, uint64_t>>& offsetsToScan, ValueVector* resultVector,
     const ColumnChunkMetadata& indexMeta) {
     string_index_t firstOffsetToScan, lastOffsetToScan;
     auto comp = [](auto pair1, auto pair2) { return pair1.first < pair2.first; };
     auto duplicationFactor = (double)offsetState.metadata.numValues / indexMeta.numValues;
     if (duplicationFactor <= 0.5) {
         // If at least 50% of strings are duplicated, sort the offsets so we can re-use scanned
@@ -103,19 +103,20 @@
                offsetsToScan[pos + 1].first == offsetsToScan[pos].first) {
             pos++;
             resultVector->setValue<ku_string_t>(offsetsToScan[pos].second, scannedString);
         }
     }
 }
 
-string_index_t DictionaryColumn::append(node_group_idx_t nodeGroupIdx, std::string_view val) {
-    auto startOffset = dataColumn->appendValues(nodeGroupIdx,
-        reinterpret_cast<const uint8_t*>(val.data()), nullptr /*nullChunkData*/, val.size());
-    return offsetColumn->appendValues(nodeGroupIdx, reinterpret_cast<const uint8_t*>(&startOffset),
-        nullptr /*nullChunkData*/, 1 /*numValues*/);
+string_index_t DictionaryColumn::append(Column::ChunkState& state, std::string_view val) {
+    auto startOffset =
+        dataColumn->appendValues(state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX],
+            reinterpret_cast<const uint8_t*>(val.data()), nullptr /*nullChunkData*/, val.size());
+    return offsetColumn->appendValues(state.childrenStates[OFFSET_COLUMN_CHILD_READ_STATE_IDX],
+        reinterpret_cast<const uint8_t*>(&startOffset), nullptr /*nullChunkData*/, 1 /*numValues*/);
 }
 
 void DictionaryColumn::prepareCommit() {
     dataColumn->prepareCommit();
     offsetColumn->prepareCommit();
 }
 
@@ -125,74 +126,74 @@
 }
 
 void DictionaryColumn::rollbackInMemory() {
     dataColumn->rollbackInMemory();
     offsetColumn->rollbackInMemory();
 }
 
-void DictionaryColumn::scanOffsets(Transaction* transaction, const Column::ReadState& state,
+void DictionaryColumn::scanOffsets(Transaction* transaction, const Column::ChunkState& state,
     DictionaryChunk::string_offset_t* offsets, uint64_t index, uint64_t numValues,
     uint64_t dataSize) {
     // We either need to read the next value, or store the maximum string offset at the end.
     // Otherwise we won't know what the length of the last string is.
     if (index + numValues < state.metadata.numValues) {
         offsetColumn->scan(transaction, state, index, index + numValues + 1, (uint8_t*)offsets);
     } else {
         offsetColumn->scan(transaction, state, index, index + numValues, (uint8_t*)offsets);
         offsets[numValues] = dataSize;
     }
 }
 
 void DictionaryColumn::scanValueToVector(Transaction* transaction,
-    const Column::ReadState& dataState, uint64_t startOffset, uint64_t endOffset,
+    const Column::ChunkState& dataState, uint64_t startOffset, uint64_t endOffset,
     ValueVector* resultVector, uint64_t offsetInVector) {
     KU_ASSERT(endOffset >= startOffset);
     // Add string to vector first and read directly into the vector
     auto& kuString =
         StringVector::reserveString(resultVector, offsetInVector, endOffset - startOffset);
     dataColumn->scan(transaction, dataState, startOffset, endOffset, (uint8_t*)kuString.getData());
     // Update prefix to match the scanned string data
     if (!ku_string_t::isShortString(kuString.len)) {
         memcpy(kuString.prefix, kuString.getData(), ku_string_t::PREFIX_LENGTH);
     }
 }
 
-bool DictionaryColumn::canCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    uint64_t numNewStrings, uint64_t totalStringLengthToAdd) {
-    if (!canDataCommitInPlace(transaction, nodeGroupIdx, totalStringLengthToAdd)) {
+bool DictionaryColumn::canCommitInPlace(const Column::ChunkState& state, uint64_t numNewStrings,
+    uint64_t totalStringLengthToAdd) {
+    if (!canDataCommitInPlace(state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX],
+            totalStringLengthToAdd)) {
         return false;
     }
-    if (!canOffsetCommitInPlace(transaction, nodeGroupIdx, numNewStrings, totalStringLengthToAdd)) {
+    if (!canOffsetCommitInPlace(state.childrenStates[OFFSET_COLUMN_CHILD_READ_STATE_IDX],
+            state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX], numNewStrings,
+            totalStringLengthToAdd)) {
         return false;
     }
     return true;
 }
 
-bool DictionaryColumn::canDataCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+bool DictionaryColumn::canDataCommitInPlace(const Column::ChunkState& dataState,
     uint64_t totalStringLengthToAdd) {
     // Make sure there is sufficient space in the data chunk (not currently compressed)
-    auto dataColumnMetadata = dataColumn->getMetadata(nodeGroupIdx, transaction->getType());
-    auto totalStringDataAfterUpdate = dataColumnMetadata.numValues + totalStringLengthToAdd;
+    auto totalStringDataAfterUpdate = dataState.metadata.numValues + totalStringLengthToAdd;
     if (totalStringDataAfterUpdate >
-        dataColumnMetadata.numPages * BufferPoolConstants::PAGE_4KB_SIZE) {
+        dataState.metadata.numPages * BufferPoolConstants::PAGE_4KB_SIZE) {
         // Data cannot be updated in place
         return false;
     }
     return true;
 }
 
-bool DictionaryColumn::canOffsetCommitInPlace(Transaction* transaction,
-    node_group_idx_t nodeGroupIdx, uint64_t numNewStrings, uint64_t totalStringLengthToAdd) {
-    auto offsetColumnMetadata = offsetColumn->getMetadata(nodeGroupIdx, transaction->getType());
-    auto dataColumnMetadata = dataColumn->getMetadata(nodeGroupIdx, transaction->getType());
-    auto totalStringOffsetsAfterUpdate = dataColumnMetadata.numValues + totalStringLengthToAdd;
-    auto offsetCapacity = offsetColumnMetadata.compMeta.numValues(
+bool DictionaryColumn::canOffsetCommitInPlace(const Column::ChunkState& offsetState,
+    const Column::ChunkState& dataState, uint64_t numNewStrings, uint64_t totalStringLengthToAdd) {
+    auto totalStringOffsetsAfterUpdate = dataState.metadata.numValues + totalStringLengthToAdd;
+    auto offsetCapacity = offsetState.metadata.compMeta.numValues(
                               BufferPoolConstants::PAGE_4KB_SIZE, dataColumn->getDataType()) *
-                          offsetColumnMetadata.numPages;
-    auto numStringsAfterUpdate = offsetColumnMetadata.numValues + numNewStrings;
+                          offsetState.metadata.numPages;
+    auto numStringsAfterUpdate = offsetState.metadata.numValues + numNewStrings;
     if (numStringsAfterUpdate > offsetCapacity) {
         // Offsets cannot be updated in place
         return false;
     }
     // Indices are limited to 32 bits but in theory could be larger than that since the offset
     // column can grow beyond the node group size.
     //
@@ -200,25 +201,20 @@
     // which are all updated in-place many times (which may fit if the first string is large
     // enough that 2^n minus the first string's size is large enough to fit the other strings,
     // for some n.
     // 32 bits should give plenty of space for updates.
     if (numStringsAfterUpdate > std::numeric_limits<string_index_t>::max()) [[unlikely]] {
         return false;
     }
-    if (offsetColumnMetadata.compMeta.canAlwaysUpdateInPlace()) {
+    if (offsetState.metadata.compMeta.canAlwaysUpdateInPlace()) {
         return true;
     }
-    if (!offsetColumnMetadata.compMeta.canUpdateInPlace(
+    if (!offsetState.metadata.compMeta.canUpdateInPlace(
             (const uint8_t*)&totalStringOffsetsAfterUpdate, 0,
             offsetColumn->getDataType().getPhysicalType())) {
         return false;
     }
     return true;
 }
 
-uint64_t DictionaryColumn::getNumValuesInOffsets(Transaction* transaction,
-    node_group_idx_t nodeGroupIdx) {
-    return offsetColumn->getMetadata(nodeGroupIdx, transaction->getType()).numValues;
-}
-
 } // namespace storage
 } // namespace kuzu
```

### sdist/kuzu-source/src/storage/store/list_column.cpp

```diff
@@ -58,26 +58,26 @@
         *metaDAHeaderInfo.childrenInfos[0], dataFH, metadataFH, bufferManager, wal, transaction,
         propertyStatistics, enableCompression);
     dataColumn = ColumnFactory::createColumn(dataColName,
         *ListType::getChildType(&this->dataType)->copy(), *metaDAHeaderInfo.childrenInfos[1],
         dataFH, metadataFH, bufferManager, wal, transaction, propertyStatistics, enableCompression);
 }
 
-void ListColumn::initReadState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    offset_t startOffsetInChunk, ReadState& readState) {
-    Column::initReadState(transaction, nodeGroupIdx, startOffsetInChunk, readState);
+void ListColumn::initChunkState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+    ChunkState& readState) {
+    Column::initChunkState(transaction, nodeGroupIdx, readState);
     // We put states for size and data column into childrenStates.
     readState.childrenStates.resize(2);
-    sizeColumn->initReadState(transaction, nodeGroupIdx, startOffsetInChunk,
+    sizeColumn->initChunkState(transaction, nodeGroupIdx,
         readState.childrenStates[SIZE_COLUMN_CHILD_READ_STATE_IDX]);
-    dataColumn->initReadState(transaction, nodeGroupIdx, startOffsetInChunk,
+    dataColumn->initChunkState(transaction, nodeGroupIdx,
         readState.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX]);
 }
 
-void ListColumn::scan(Transaction* transaction, ReadState& readState, offset_t startOffsetInGroup,
+void ListColumn::scan(Transaction* transaction, ChunkState& readState, offset_t startOffsetInGroup,
     offset_t endOffsetInGroup, ValueVector* resultVector, uint64_t offsetInVector) {
     nullColumn->scan(transaction, *readState.nullState, startOffsetInGroup, endOffsetInGroup,
         resultVector, offsetInVector);
     auto listOffsetInfoInStorage = getListOffsetSizeInfo(transaction, readState.nodeGroupIdx,
         startOffsetInGroup, endOffsetInGroup);
     offset_t listOffsetInVector =
         offsetInVector == 0 ? 0 :
@@ -163,30 +163,30 @@
                     tmpDataColumnChunk->dataColumnChunk->getNumValues());
             }
             listColumnChunk->resetOffset();
         }
     }
 }
 
-void ListColumn::scanInternal(Transaction* transaction, ReadState& readState,
+void ListColumn::scanInternal(Transaction* transaction, ChunkState& readState,
     ValueVector* nodeIDVector, ValueVector* resultVector) {
     resultVector->resetAuxiliaryBuffer();
     KU_ASSERT(resultVector->state);
     auto [nodeGroupIdx, startOffsetInChunk] =
         StorageUtils::getNodeGroupIdxAndOffsetInChunk(nodeIDVector->readNodeOffset(0));
     auto listOffsetSizeInfo = getListOffsetSizeInfo(transaction, readState.nodeGroupIdx,
         startOffsetInChunk, startOffsetInChunk + nodeIDVector->state->getOriginalSize());
     if (resultVector->state->selVector->isUnfiltered()) {
         scanUnfiltered(transaction, readState, resultVector, listOffsetSizeInfo);
     } else {
         scanFiltered(transaction, readState, resultVector, listOffsetSizeInfo);
     }
 }
 
-void ListColumn::lookupValue(Transaction* transaction, ReadState& readState, offset_t nodeOffset,
+void ListColumn::lookupValue(Transaction* transaction, ChunkState& readState, offset_t nodeOffset,
     ValueVector* resultVector, uint32_t posInVector) {
     auto nodeGroupIdx = StorageUtils::getNodeGroupIdx(nodeOffset);
     KU_ASSERT(readState.nodeGroupIdx == nodeGroupIdx);
     auto nodeOffsetInGroup = nodeOffset - StorageUtils::getStartOffsetOfNodeGroup(nodeGroupIdx);
     auto listEndOffset = readOffset(transaction, readState, nodeOffsetInGroup);
     auto size = readSize(transaction, readState.childrenStates[SIZE_COLUMN_CHILD_READ_STATE_IDX],
         nodeOffsetInGroup);
@@ -205,15 +205,15 @@
     Column::append(listColumnChunk, nodeGroupIdx);
     auto sizeColumnChunk = listColumnChunk->getSizeColumnChunk();
     sizeColumn->append(sizeColumnChunk, nodeGroupIdx);
     auto dataColumnChunk = listColumnChunk->getDataColumnChunk();
     dataColumn->append(dataColumnChunk, nodeGroupIdx);
 }
 
-void ListColumn::scanUnfiltered(Transaction* transaction, ReadState& readState,
+void ListColumn::scanUnfiltered(Transaction* transaction, ChunkState& readState,
     ValueVector* resultVector, const ListOffsetSizeInfo& listOffsetInfoInStorage) {
     auto numValuesToScan = resultVector->state->selVector->selectedSize;
     numValuesToScan = std::min(numValuesToScan, listOffsetInfoInStorage.numTotal);
     offset_t offsetInVector = 0;
     for (auto i = 0u; i < numValuesToScan; i++) {
         auto listLen = listOffsetInfoInStorage.getListSize(i);
         resultVector->setValue(i, list_entry_t{offsetInVector, listLen});
@@ -238,15 +238,15 @@
                 startListOffsetInStorage, startListOffsetInStorage + appendSize, dataVector,
                 offsetInVector);
             offsetInVector += appendSize;
         }
     }
 }
 
-void ListColumn::scanFiltered(Transaction* transaction, ReadState& readState,
+void ListColumn::scanFiltered(Transaction* transaction, ChunkState& readState,
     ValueVector* resultVector, const ListOffsetSizeInfo& listOffsetSizeInfo) {
     offset_t listOffset = 0;
     for (auto i = 0u; i < resultVector->state->selVector->selectedSize; i++) {
         auto pos = resultVector->state->selVector->selectedPositions[i];
         auto listSize = listOffsetSizeInfo.getListSize(pos);
         resultVector->setValue(pos, list_entry_t{(offset_t)listOffset, listSize});
         listOffset += listSize;
@@ -279,26 +279,26 @@
 
 void ListColumn::rollbackInMemory() {
     Column::rollbackInMemory();
     sizeColumn->rollbackInMemory();
     dataColumn->rollbackInMemory();
 }
 
-offset_t ListColumn::readOffset(Transaction* transaction, const ReadState& readState,
+offset_t ListColumn::readOffset(Transaction* transaction, const ChunkState& readState,
     offset_t offsetInNodeGroup) {
     auto pageCursor = getPageCursorForOffsetInGroup(offsetInNodeGroup, readState);
     offset_t value;
     readFromPage(transaction, pageCursor.pageIdx, [&](uint8_t* frame) -> void {
         readToPageFunc(frame, pageCursor, (uint8_t*)&value, 0 /* posInVector */,
             1 /* numValuesToRead */, readState.metadata.compMeta);
     });
     return value;
 }
 
-list_size_t ListColumn::readSize(Transaction* transaction, const ReadState& readState,
+list_size_t ListColumn::readSize(Transaction* transaction, const ChunkState& readState,
     offset_t offsetInNodeGroup) {
     auto pageCursor = getPageCursorForOffsetInGroup(offsetInNodeGroup, readState);
     offset_t value;
     readFromPage(transaction, pageCursor.pageIdx, [&](uint8_t* frame) -> void {
         readToPageFunc(frame, pageCursor, (uint8_t*)&value, 0 /* posInVector */,
             1 /* numValuesToRead */, readState.metadata.compMeta);
     });
@@ -343,15 +343,16 @@
         for (auto& [offsetInDstChunk, rowIdx] : insertInfo) {
             auto [chunkIdx, offsetInLocalChunk] =
                 LocalChunkedGroupCollection::getChunkIdxAndOffsetInChunk(rowIdx);
             auto localInsertChunk = localInsertChunks[chunkIdx];
             dstOffsets.push_back(offsetInDstChunk);
             columnChunk->append(localInsertChunk, offsetInLocalChunk, 1);
         }
-        prepareCommitForChunk(transaction, nodeGroupIdx, dstOffsets, columnChunk.get(), 0);
+        prepareCommitForChunk(transaction, nodeGroupIdx, dstOffsets, columnChunk.get(),
+            0 /*startSrcOffset*/);
     }
 }
 
 void ListColumn::prepareCommitForChunk(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk, offset_t startSrcOffset) {
     auto currentNumNodeGroups = metadataDA->getNumElements(transaction->getType());
     auto isNewNodeGroup = nodeGroupIdx >= currentNumNodeGroups;
@@ -360,72 +361,80 @@
             startSrcOffset);
         return;
     }
     // we first check if we can in place commit data column chunk
     // if we can not in place commit data column chunk, we will out place commit offset/size/data
     // column chunk otherwise, we commit data column chunk in place and separately commit
     // offset/size column chunk
+    ChunkState state;
+    initChunkState(transaction, nodeGroupIdx, state);
     auto listChunk = ku_dynamic_cast<ColumnChunk*, ListColumnChunk*>(chunk);
-    auto dataColumnSize = dataColumn->getMetadata(nodeGroupIdx, transaction->getType()).numValues;
+    auto dataColumnSize = state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX].metadata.numValues;
     auto dataColumnChunk = listChunk->getDataColumnChunk();
     auto numListsToAppend = std::min(chunk->getNumValues(), (uint64_t)dstOffsets.size());
     auto dataSize = 0u;
     auto startListOffset = listChunk->getListStartOffset(startSrcOffset);
     std::vector<common::offset_t> dstOffsetsInDataColumn;
     for (auto i = 0u; i < numListsToAppend; i++) {
         for (auto j = 0u; j < listChunk->getListSize(startSrcOffset + i); j++) {
             dstOffsetsInDataColumn.push_back(dataColumnSize + dataSize++);
         }
     }
-    bool dataColumnCanCommitInPlace = dataColumn->canCommitInPlace(transaction, nodeGroupIdx,
-        dstOffsetsInDataColumn, dataColumnChunk, startListOffset);
+    bool dataColumnCanCommitInPlace =
+        dataColumn->canCommitInPlace(state.childrenStates[DATA_COLUMN_CHILD_READ_STATE_IDX],
+            dstOffsetsInDataColumn, dataColumnChunk, startListOffset);
     if (!dataColumnCanCommitInPlace) {
-        commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets, chunk,
-            startSrcOffset);
+        commitColumnChunkOutOfPlace(transaction, state.nodeGroupIdx, isNewNodeGroup, dstOffsets,
+            chunk, startSrcOffset);
     } else {
+        // TODO: Shouldn't here be in place commit?
         dataColumn->commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup,
             dstOffsetsInDataColumn, dataColumnChunk, startListOffset);
         sizeColumn->prepareCommitForChunk(transaction, nodeGroupIdx, dstOffsets,
             listChunk->getSizeColumnChunk(), startSrcOffset);
         for (auto i = 0u; i < numListsToAppend; i++) {
             auto listEndOffset = listChunk->getListEndOffset(startSrcOffset + i);
             chunk->setValue<offset_t>(dataColumnSize + listEndOffset, startSrcOffset + i);
         }
-        prepareCommitForOffsetChunk(transaction, nodeGroupIdx, dstOffsets, chunk, startSrcOffset);
+        prepareCommitForOffsetChunk(transaction, state, dstOffsets, chunk, startSrcOffset);
     }
 }
 
-void ListColumn::prepareCommitForOffsetChunk(Transaction* transaction,
-    node_group_idx_t nodeGroupIdx, const std::vector<common::offset_t>& dstOffsets,
-    ColumnChunk* chunk, offset_t startSrcOffset) {
+void ListColumn::prepareCommitForOffsetChunk(Transaction* transaction, ChunkState& offsetState,
+    const std::vector<common::offset_t>& dstOffsets, ColumnChunk* chunk, offset_t startSrcOffset) {
     metadataDA->prepareCommit();
     bool didInPlaceCommit = false;
-    if (canCommitInPlace(transaction, nodeGroupIdx, dstOffsets, chunk, startSrcOffset)) {
-        commitOffsetColumnChunkInPlace(nodeGroupIdx, dstOffsets, chunk, startSrcOffset);
+    if (canCommitInPlace(offsetState, dstOffsets, chunk, startSrcOffset)) {
+        commitOffsetColumnChunkInPlace(offsetState, dstOffsets, chunk, startSrcOffset);
         didInPlaceCommit = true;
+        metadataDA->update(offsetState.nodeGroupIdx, offsetState.metadata);
     } else {
-        commitOffsetColumnChunkOutOfPlace(transaction, nodeGroupIdx, dstOffsets, chunk,
+        commitOffsetColumnChunkOutOfPlace(transaction, offsetState.nodeGroupIdx, dstOffsets, chunk,
             startSrcOffset);
     }
     if (nullColumn) {
-        if (nullColumn->canCommitInPlace(transaction, nodeGroupIdx, dstOffsets,
-                chunk->getNullChunk(), startSrcOffset)) {
-            nullColumn->commitColumnChunkInPlace(nodeGroupIdx, dstOffsets, chunk->getNullChunk(),
-                startSrcOffset);
-        } else if (didInPlaceCommit) {
-            nullColumn->commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, false, dstOffsets,
+        KU_ASSERT(offsetState.nullState);
+        if (nullColumn->canCommitInPlace(*offsetState.nullState, dstOffsets, chunk->getNullChunk(),
+                startSrcOffset)) {
+            nullColumn->commitColumnChunkInPlace(*offsetState.nullState, dstOffsets,
                 chunk->getNullChunk(), startSrcOffset);
+            nullColumn->metadataDA->update(offsetState.nodeGroupIdx,
+                offsetState.nullState->metadata);
+        } else if (didInPlaceCommit) {
+            nullColumn->commitColumnChunkOutOfPlace(transaction, offsetState.nodeGroupIdx, false,
+                dstOffsets, chunk->getNullChunk(), startSrcOffset);
         }
     }
 }
 
-void ListColumn::commitOffsetColumnChunkInPlace(node_group_idx_t nodeGroupIdx,
+void ListColumn::commitOffsetColumnChunkInPlace(ChunkState& offsetState,
     const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk, offset_t srcOffset) {
+    // TODO: Should sort and write per page.
     for (auto i = 0u; i < dstOffsets.size(); i++) {
-        Column::write(nodeGroupIdx, dstOffsets[i], chunk, srcOffset + i, 1 /* numValues */);
+        Column::write(offsetState, dstOffsets[i], chunk, srcOffset + i, 1 /* numValues */);
     }
 }
 
 void ListColumn::commitOffsetColumnChunkOutOfPlace(Transaction* transaction,
     node_group_idx_t nodeGroupIdx, const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk,
     offset_t startSrcOffset) {
     auto listChunk = ku_dynamic_cast<ColumnChunk*, ListColumnChunk*>(chunk);
```

### sdist/kuzu-source/src/storage/store/node_table_data.cpp

```diff
@@ -63,32 +63,29 @@
     }
     dataReadState.readFromPersistent = nodeGroupIdx < numExistingNodeGroups;
     // Sanity check on that we should always be able to readFromPersistent if the transaction is
     // read only.
     KU_ASSERT((dataReadState.readFromPersistent && transaction->isReadOnly()) ||
               transaction->isWriteTransaction());
     if (dataReadState.readFromPersistent) {
-        initializeColumnReadStates(transaction, startNodeOffset, dataReadState, nodeGroupIdx);
+        initializeColumnReadStates(transaction, dataReadState, nodeGroupIdx);
     }
     if (transaction->isWriteTransaction()) {
         initializeLocalNodeReadState(transaction, dataReadState, nodeGroupIdx);
     }
     dataReadState.nodeGroupIdx = nodeGroupIdx;
 }
 
-void NodeTableData::initializeColumnReadStates(Transaction* transaction, offset_t startNodeOffset,
+void NodeTableData::initializeColumnReadStates(Transaction* transaction,
     NodeDataReadState& readState, node_group_idx_t nodeGroupIdx) {
-    auto startOffsetInChunk =
-        startNodeOffset - StorageUtils::getStartOffsetOfNodeGroup(nodeGroupIdx);
     auto& dataReadState = ku_dynamic_cast<TableDataReadState&, NodeDataReadState&>(readState);
     for (auto i = 0u; i < readState.columnIDs.size(); i++) {
         if (readState.columnIDs[i] != INVALID_COLUMN_ID) {
             getColumn(readState.columnIDs[i])
-                ->initReadState(transaction, nodeGroupIdx, startOffsetInChunk,
-                    dataReadState.columnReadStates[i]);
+                ->initChunkState(transaction, nodeGroupIdx, dataReadState.columnReadStates[i]);
         }
     }
     if (nodeGroupIdx != dataReadState.nodeGroupIdx) {
         KU_ASSERT(sanityCheckOnColumnNumValues(dataReadState));
     }
 }
```

### sdist/kuzu-source/src/storage/store/null_column.cpp

```diff
@@ -41,24 +41,24 @@
           false /*requireNullColumn*/} {
     readToVectorFunc = NullColumnFunc::readValuesFromPageToVector;
     writeFromVectorFunc = NullColumnFunc::writeValueToPageFromVector;
     // Should never be used
     batchLookupFunc = nullptr;
 }
 
-void NullColumn::scan(Transaction* transaction, ReadState& readState, ValueVector* nodeIDVector,
+void NullColumn::scan(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
     ValueVector* resultVector) {
     if (propertyStatistics.mayHaveNull(*transaction)) {
         scanInternal(transaction, readState, nodeIDVector, resultVector);
     } else {
         resultVector->setAllNonNull();
     }
 }
 
-void NullColumn::scan(transaction::Transaction* transaction, ReadState& readState,
+void NullColumn::scan(transaction::Transaction* transaction, ChunkState& readState,
     offset_t startOffsetInGroup, offset_t endOffsetInGroup, ValueVector* resultVector,
     uint64_t offsetInVector) {
     if (propertyStatistics.mayHaveNull(*transaction)) {
         Column::scan(transaction, readState, startOffsetInGroup, endOffsetInGroup, resultVector,
             offsetInVector);
     } else {
         resultVector->setNullRange(offsetInVector, endOffsetInGroup - startOffsetInGroup,
@@ -80,15 +80,15 @@
                                  0 :
                                  std::min(endOffset, chunkMetadata.numValues) - startOffset;
             columnChunk->setNumValues(numValues);
         }
     }
 }
 
-void NullColumn::lookup(Transaction* transaction, ReadState& readState, ValueVector* nodeIDVector,
+void NullColumn::lookup(Transaction* transaction, ChunkState& readState, ValueVector* nodeIDVector,
     ValueVector* resultVector) {
     if (propertyStatistics.mayHaveNull(*transaction)) {
         lookupInternal(transaction, readState, nodeIDVector, resultVector);
     } else {
         for (auto i = 0ul; i < nodeIDVector->state->selVector->selectedSize; i++) {
             auto pos = nodeIDVector->state->selVector->selectedPositions[i];
             resultVector->setNull(pos, false);
@@ -103,92 +103,84 @@
     metadataDA->resize(nodeGroupIdx + 1);
     metadataDA->update(nodeGroupIdx, metadata);
     if (static_cast<NullColumnChunk*>(columnChunk)->mayHaveNull()) {
         propertyStatistics.setHasNull(DUMMY_WRITE_TRANSACTION);
     }
 }
 
-bool NullColumn::isNull(transaction::Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    offset_t offsetInChunk) {
-    auto state = getReadState(transaction->getType(), nodeGroupIdx);
+bool NullColumn::isNull(Transaction* transaction, const ChunkState& state, offset_t offsetInChunk) {
     uint64_t result = false;
     if (offsetInChunk >= state.metadata.numValues) {
         return true;
     }
     // Must be aligned to an 8-byte chunk for NullMask read to not overflow
     Column::scan(transaction, state, offsetInChunk, offsetInChunk + 1,
         reinterpret_cast<uint8_t*>(&result));
     return result;
 }
 
-void NullColumn::setNull(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk, uint64_t value) {
+void NullColumn::setNull(ChunkState& state, offset_t offsetInChunk, uint64_t value) {
     propertyStatistics.setHasNull(DUMMY_WRITE_TRANSACTION);
     // Must be aligned to an 8-byte chunk for NullMask read to not overflow
-    auto state = getReadState(TransactionType::WRITE, nodeGroupIdx);
     writeValues(state, offsetInChunk, reinterpret_cast<const uint8_t*>(&value),
         nullptr /*nullChunkData=*/);
     if (offsetInChunk >= state.metadata.numValues) {
         state.metadata.numValues = offsetInChunk + 1;
-        metadataDA->update(nodeGroupIdx, state.metadata);
     }
 }
 
-void NullColumn::write(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk,
-    ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) {
-    auto chunkMeta = metadataDA->get(nodeGroupIdx, TransactionType::WRITE);
-    writeValue(chunkMeta, nodeGroupIdx, offsetInChunk, vectorToWriteFrom, posInVectorToWriteFrom);
+void NullColumn::write(ChunkState& state, offset_t offsetInChunk, ValueVector* vectorToWriteFrom,
+    uint32_t posInVectorToWriteFrom) {
+    writeValue(state, offsetInChunk, vectorToWriteFrom, posInVectorToWriteFrom);
     if (vectorToWriteFrom->isNull(posInVectorToWriteFrom)) {
         propertyStatistics.setHasNull(DUMMY_WRITE_TRANSACTION);
     }
-    if (offsetInChunk >= chunkMeta.numValues) {
-        chunkMeta.numValues = offsetInChunk + 1;
-        metadataDA->update(nodeGroupIdx, chunkMeta);
+    if (offsetInChunk >= state.metadata.numValues) {
+        state.metadata.numValues = offsetInChunk + 1;
     }
 }
 
-void NullColumn::write(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk, ColumnChunk* data,
+void NullColumn::write(ChunkState& state, offset_t offsetInChunk, ColumnChunk* data,
     offset_t dataOffset, length_t numValues) {
-    auto state = getReadState(TransactionType::WRITE, nodeGroupIdx);
     writeValues(state, offsetInChunk, data->getData(), nullptr /*nullChunkData=*/, dataOffset,
         numValues);
     auto nullChunk = ku_dynamic_cast<ColumnChunk*, NullColumnChunk*>(data);
     for (auto i = 0u; i < numValues; i++) {
         if (nullChunk->isNull(dataOffset + i)) {
             propertyStatistics.setHasNull(DUMMY_WRITE_TRANSACTION);
         }
     }
     if (offsetInChunk + numValues > state.metadata.numValues) {
         state.metadata.numValues = offsetInChunk + numValues;
-        metadataDA->update(nodeGroupIdx, state.metadata);
     }
 }
 
-void NullColumn::commitLocalChunkInPlace(Transaction* /*transaction*/,
-    node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunks,
-    const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
-    const offset_to_row_idx_t& updateInfo, const offset_set_t& deleteInfo) {
+void NullColumn::commitLocalChunkInPlace(Transaction* /*transaction*/, ChunkState& state,
+    const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
+    const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo,
+    const offset_set_t& deleteInfo) {
     for (auto& [offsetInChunk, rowIdx] : updateInfo) {
         auto [chunkIdx, offsetInLocalChunk] =
             LocalChunkedGroupCollection::getChunkIdxAndOffsetInChunk(rowIdx);
         auto localChunk = localUpdateChunks[chunkIdx];
         KU_ASSERT(localChunk->getDataType().getPhysicalType() == PhysicalTypeID::BOOL &&
                   !localChunk->getNullChunk());
-        write(nodeGroupIdx, offsetInChunk, localChunk, offsetInLocalChunk, 1 /*numValues*/);
+        write(state, offsetInChunk, localChunk, offsetInLocalChunk, 1 /*numValues*/);
     }
     for (auto& [offsetInChunk, rowIdx] : insertInfo) {
         auto [chunkIdx, offsetInLocalChunk] =
             LocalChunkedGroupCollection::getChunkIdxAndOffsetInChunk(rowIdx);
         auto localChunk = localInsertChunks[chunkIdx];
         KU_ASSERT(localChunk->getDataType().getPhysicalType() == PhysicalTypeID::BOOL &&
                   !localChunk->getNullChunk());
-        write(nodeGroupIdx, offsetInChunk, localChunk, offsetInLocalChunk, 1 /*numValues*/);
+        write(state, offsetInChunk, localChunk, offsetInLocalChunk, 1 /*numValues*/);
     }
     // Set nulls based on deleteInfo. Note that this code path actually only gets executed when
     // the column is a regular format one. This is not a good design, should be unified with csr
     // one in the future.
     for (auto offsetInChunk : deleteInfo) {
-        setNull(nodeGroupIdx, offsetInChunk);
+        setNull(state, offsetInChunk);
     }
 }
 
 } // namespace storage
 } // namespace kuzu
```

### sdist/kuzu-source/src/storage/store/rel_table_data.cpp

```diff
@@ -167,63 +167,59 @@
     ku_dynamic_cast<Column*, InternalIDColumn*>(columns[NBR_ID_COLUMN_ID].get())
         ->setCommonTableID(nbrTableID);
     ku_dynamic_cast<Column*, InternalIDColumn*>(columns[REL_ID_COLUMN_ID].get())
         ->setCommonTableID(tableID);
     packedCSRInfo = PackedCSRInfo();
 }
 
-// TODO: Two optimizations:
-//       1. avoid scan the whole group of the csr header. just scan the vector.
-//       2. cache column chunk metadata.
+// TODO: avoid scan the whole group of the csr header. just scan the vector.
 void RelTableData::initializeReadState(Transaction* transaction, std::vector<column_id_t> columnIDs,
     const ValueVector& inNodeIDVector, RelDataReadState& readState) {
     readState.direction = direction;
     readState.columnIDs.clear();
     readState.columnIDs.push_back(NBR_ID_COLUMN_ID);
     readState.columnIDs.insert(readState.columnIDs.end(), columnIDs.begin(), columnIDs.end());
     // Reset to read from persistent storage.
     readState.readFromLocalStorage = false;
     auto nodeOffset =
         inNodeIDVector.readNodeOffset(inNodeIDVector.state->selVector->selectedPositions[0]);
-    auto nodeGroupIdx = StorageUtils::getNodeGroupIdx(nodeOffset);
-    auto startNodeOffset = StorageUtils::getStartOffsetOfNodeGroup(nodeGroupIdx);
     // Reset to read from beginning for the csr of the new node offset.
     readState.posInCurrentCSR = 0;
     if (readState.isOutOfRange(nodeOffset)) {
         // Scan csr offsets and populate csr list entries for the new node group.
-        readState.startNodeOffset = startNodeOffset;
+        auto nodeGroupIdx = StorageUtils::getNodeGroupIdx(nodeOffset);
+        readState.startNodeOffset = StorageUtils::getStartOffsetOfNodeGroup(nodeGroupIdx);
         csrHeaderColumns.scan(transaction, nodeGroupIdx, readState.csrHeaderChunks);
         KU_ASSERT(readState.csrHeaderChunks.offset->getNumValues() ==
                   readState.csrHeaderChunks.length->getNumValues());
         readState.numNodes = readState.csrHeaderChunks.offset->getNumValues();
         readState.populateCSRListEntries();
         readState.readFromPersistentStorage =
             nodeGroupIdx < columns[REL_ID_COLUMN_ID]->getNumNodeGroups(transaction);
         if (readState.readFromPersistentStorage) {
-            initializeColumnReadStates(transaction, startNodeOffset, readState, nodeGroupIdx);
+            initializeColumnReadStates(transaction, readState, nodeGroupIdx);
         }
         if (transaction->isWriteTransaction()) {
             readState.localNodeGroup = getLocalNodeGroup(transaction, nodeGroupIdx);
         }
     }
     if (nodeOffset != readState.currentNodeOffset) {
         readState.currentNodeOffset = nodeOffset;
     }
 }
 
-void RelTableData::initializeColumnReadStates(Transaction* transaction, offset_t startNodeOffset,
-    RelDataReadState& readState, node_group_idx_t nodeGroupIdx) {
+void RelTableData::initializeColumnReadStates(Transaction* transaction, RelDataReadState& readState,
+    node_group_idx_t nodeGroupIdx) {
     readState.columnStates.resize(readState.columnIDs.size());
     for (auto i = 0u; i < readState.columnIDs.size(); i++) {
         auto columnID = readState.columnIDs[i];
         if (columnID == INVALID_COLUMN_ID) {
             continue;
         }
-        getColumn(columnID)->initReadState(transaction, nodeGroupIdx, startNodeOffset,
-            readState.columnStates[i]);
+        getColumn(columnID)->initChunkState(transaction, nodeGroupIdx, readState.columnStates[i]);
     }
 }
 
 void RelTableData::scan(Transaction* transaction, TableDataReadState& readState,
     const ValueVector& inNodeIDVector, const std::vector<ValueVector*>& outputVectors) {
     auto& relReadState = ku_dynamic_cast<TableDataReadState&, RelDataReadState&>(readState);
     if (relReadState.readFromLocalStorage) {
@@ -292,15 +288,16 @@
 }
 
 bool RelTableData::checkIfNodeHasRels(Transaction* transaction, offset_t nodeOffset) const {
     auto [nodeGroupIdx, offsetInChunk] = StorageUtils::getNodeGroupIdxAndOffsetInChunk(nodeOffset);
     if (nodeGroupIdx >= csrHeaderColumns.length->getNumNodeGroups(transaction)) {
         return false;
     }
-    auto readState = csrHeaderColumns.length->getReadState(transaction->getType(), nodeGroupIdx);
+    Column::ChunkState readState;
+    csrHeaderColumns.length->initChunkState(transaction, nodeGroupIdx, readState);
     if (offsetInChunk >= readState.metadata.numValues) {
         return false;
     }
     length_t length;
     csrHeaderColumns.length->scan(transaction, readState, offsetInChunk, offsetInChunk + 1,
         reinterpret_cast<uint8_t*>(&length));
     return length > 0;
@@ -810,14 +807,15 @@
         dstOffsets[i] = slides[i].second;
     }
     column->prepareCommitForChunk(transaction, nodeGroupIdx, dstOffsets, chunk.get(), 0);
 }
 
 // TODO(Guodong): Optimize the sliding by moving the suffix/prefix depending on shifting
 //                left/right.
+// TODO: applySliding should work for all columns. so no redundant computation of slidings.
 void RelTableData::applySliding(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     LocalState& localState, const PersistentState& persistentState, Column* column) {
     if (!localState.needSliding) {
         return;
     }
     auto [leftBoundary, rightBoundary] = localState.region.getNodeOffsetBoundaries();
     std::vector<std::pair<offset_t, offset_t>> slides;
@@ -929,22 +927,28 @@
     commitCSRHeaderChunk(transaction, isNewNodeGroup, nodeGroupIdx, csrHeaderColumns.length.get(),
         newHeader.length.get(), localState, dstOffsets);
 }
 
 void RelTableData::commitCSRHeaderChunk(Transaction* transaction, bool isNewNodeGroup,
     node_group_idx_t nodeGroupIdx, Column* column, ColumnChunk* chunk, LocalState& localState,
     const std::vector<common::offset_t>& dstOffsets) {
-    if (!isNewNodeGroup && column->canCommitInPlace(transaction, nodeGroupIdx, dstOffsets, chunk,
-                               localState.region.leftBoundary)) {
-        column->write(nodeGroupIdx, dstOffsets[0], chunk, localState.region.leftBoundary,
-            dstOffsets.size());
-    } else {
-        column->commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets,
-            chunk, localState.region.leftBoundary);
+    if (!isNewNodeGroup) {
+        Column::ChunkState state;
+        column->initChunkState(transaction, nodeGroupIdx, state);
+        if (column->canCommitInPlace(state, dstOffsets, chunk, localState.region.leftBoundary)) {
+            // TODO: We're assuming dstOffsets are consecutive here. Always true? if so, bad
+            // interface then.
+            column->write(state, dstOffsets[0], chunk, localState.region.leftBoundary,
+                dstOffsets.size());
+            column->getMetadataDA()->update(nodeGroupIdx, state.metadata);
+            return;
+        }
     }
+    column->commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets,
+        chunk, localState.region.leftBoundary);
 }
 
 void RelTableData::distributeOffsets(const ChunkedCSRHeader& header, LocalState& localState,
     offset_t leftBoundary, offset_t rightBoundary) {
     if (localState.region.level > packedCSRInfo.calibratorTreeHeight) {
         // Need to resize the capacity and reset regionToDistribute to the top level one.
         localState.region =
```

### sdist/kuzu-source/src/storage/store/string_column.cpp

```diff
@@ -21,22 +21,23 @@
     BufferManager* bufferManager, WAL* wal, transaction::Transaction* transaction,
     RWPropertyStats stats, bool enableCompression)
     : Column{name, std::move(dataType), metaDAHeaderInfo, dataFH, metadataFH, bufferManager, wal,
           transaction, stats, enableCompression, true /* requireNullColumn */},
       dictionary{name, metaDAHeaderInfo, dataFH, metadataFH, bufferManager, wal, transaction, stats,
           enableCompression} {}
 
-void StringColumn::initReadState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    offset_t startOffsetInChunk, ReadState& readState) {
-    Column::initReadState(transaction, nodeGroupIdx, startOffsetInChunk, readState);
-    dictionary.initReadState(transaction, nodeGroupIdx, startOffsetInChunk, readState);
+void StringColumn::initChunkState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+    ChunkState& readState) {
+    Column::initChunkState(transaction, nodeGroupIdx, readState);
+    dictionary.initChunkState(transaction, nodeGroupIdx, readState);
 }
 
-void StringColumn::scan(Transaction* transaction, ReadState& readState, offset_t startOffsetInGroup,
-    offset_t endOffsetInGroup, ValueVector* resultVector, uint64_t offsetInVector) {
+void StringColumn::scan(Transaction* transaction, ChunkState& readState,
+    offset_t startOffsetInGroup, offset_t endOffsetInGroup, ValueVector* resultVector,
+    uint64_t offsetInVector) {
     nullColumn->scan(transaction, *readState.nullState, startOffsetInGroup, endOffsetInGroup,
         resultVector, offsetInVector);
     scanUnfiltered(transaction, readState, startOffsetInGroup,
         endOffsetInGroup - startOffsetInGroup, resultVector, offsetInVector);
 }
 
 void StringColumn::scan(Transaction* transaction, node_group_idx_t nodeGroupIdx,
@@ -51,69 +52,64 @@
 
 void StringColumn::append(ColumnChunk* columnChunk, node_group_idx_t nodeGroupIdx) {
     Column::append(columnChunk, nodeGroupIdx);
     auto stringColumnChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(columnChunk);
     dictionary.append(nodeGroupIdx, stringColumnChunk->getDictionaryChunk());
 }
 
-void StringColumn::writeValue(const ColumnChunkMetadata& chunkMeta, node_group_idx_t nodeGroupIdx,
-    offset_t offsetInChunk, ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) {
+void StringColumn::writeValue(ChunkState& state, offset_t offsetInChunk,
+    ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) {
     auto& kuStr = vectorToWriteFrom->getValue<ku_string_t>(posInVectorToWriteFrom);
-    auto index = dictionary.append(nodeGroupIdx, kuStr.getAsStringView());
-    NullMask nullMask(1);
-    nullMask.setNull(0, vectorToWriteFrom->isNull(posInVectorToWriteFrom));
+    auto index = dictionary.append(state, kuStr.getAsStringView());
     // Write index to main column
-    auto state = ReadState{chunkMeta,
-        chunkMeta.compMeta.numValues(BufferPoolConstants::PAGE_4KB_SIZE, dataType)};
     // This function should only be called when the string is non-null, so we don't need to pass
     // null data
+    KU_ASSERT(!vectorToWriteFrom->isNull(posInVectorToWriteFrom));
     Column::writeValues(state, offsetInChunk, (uint8_t*)&index, nullptr /*nullChunkData*/);
 }
 
-void StringColumn::write(node_group_idx_t nodeGroupIdx, offset_t dstOffset, ColumnChunk* data,
+void StringColumn::write(ChunkState& state, offset_t dstOffset, ColumnChunk* data,
     offset_t srcOffset, length_t numValues) {
-    auto state = getReadState(TransactionType::WRITE, nodeGroupIdx);
     numValues = std::min(numValues, data->getNumValues() - srcOffset);
     auto strChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(data);
     std::vector<string_index_t> indices;
     indices.resize(numValues);
     for (auto i = 0u; i < numValues; i++) {
         if (strChunk->getNullChunk()->isNull(i + srcOffset)) {
             indices[i] = 0;
             continue;
         }
         auto strVal = strChunk->getValue<std::string_view>(i + srcOffset);
-        indices[i] = dictionary.append(nodeGroupIdx, strVal);
+        indices[i] = dictionary.append(state, strVal);
     }
     NullMask nullMask(numValues);
     nullMask.copyFromNullBits(data->getNullChunk()->getNullMask().getData(), srcOffset,
         0 /*dstOffset=*/, numValues);
     // Write index to main column
     Column::writeValues(state, dstOffset, reinterpret_cast<const uint8_t*>(&indices[0]), &nullMask,
         0 /*srcOffset*/, numValues);
     if (dstOffset + numValues > state.metadata.numValues) {
         state.metadata.numValues = dstOffset + numValues;
-        metadataDA->update(nodeGroupIdx, state.metadata);
     }
 }
 
-void StringColumn::scanInternal(Transaction* transaction, ReadState& readState,
+void StringColumn::scanInternal(Transaction* transaction, ChunkState& readState,
     ValueVector* nodeIDVector, ValueVector* resultVector) {
     KU_ASSERT(resultVector->dataType.getPhysicalType() == PhysicalTypeID::STRING);
     auto [nodeGroupIdx, startOffsetInChunk] =
         StorageUtils::getNodeGroupIdxAndOffsetInChunk(nodeIDVector->readNodeOffset(0));
     if (nodeIDVector->state->selVector->isUnfiltered()) {
         scanUnfiltered(transaction, readState, startOffsetInChunk,
             nodeIDVector->state->selVector->selectedSize, resultVector);
     } else {
         scanFiltered(transaction, readState, startOffsetInChunk, nodeIDVector, resultVector);
     }
 }
 
-void StringColumn::scanUnfiltered(transaction::Transaction* transaction, ReadState& readState,
+void StringColumn::scanUnfiltered(transaction::Transaction* transaction, ChunkState& readState,
     offset_t startOffsetInChunk, offset_t numValuesToRead, ValueVector* resultVector,
     sel_t startPosInVector) {
     // TODO: Replace indices with ValueVector to avoid maintaining `scan` interface from uint8_t*.
     auto indices = std::make_unique<string_index_t[]>(numValuesToRead);
     Column::scan(transaction, readState, startOffsetInChunk, startOffsetInChunk + numValuesToRead,
         (uint8_t*)indices.get());
 
@@ -129,15 +125,15 @@
     }
     dictionary.scan(transaction,
         readState.childrenStates[DictionaryColumn::OFFSET_COLUMN_CHILD_READ_STATE_IDX],
         readState.childrenStates[DictionaryColumn::DATA_COLUMN_CHILD_READ_STATE_IDX], offsetsToScan,
         resultVector, readState.metadata);
 }
 
-void StringColumn::scanFiltered(transaction::Transaction* transaction, ReadState& readState,
+void StringColumn::scanFiltered(transaction::Transaction* transaction, ChunkState& readState,
     common::offset_t startOffsetInChunk, ValueVector* nodeIDVector, ValueVector* resultVector) {
     std::vector<std::pair<string_index_t, uint64_t>> offsetsToScan;
     for (auto i = 0u; i < nodeIDVector->state->selVector->selectedSize; i++) {
         auto pos = nodeIDVector->state->selVector->selectedPositions[i];
         if (!resultVector->isNull(pos)) {
             // TODO(bmwinger): optimize index scans by grouping them when adjacent
             auto offsetInGroup = startOffsetInChunk + pos;
@@ -153,15 +149,15 @@
     }
     dictionary.scan(transaction,
         readState.childrenStates[DictionaryColumn::OFFSET_COLUMN_CHILD_READ_STATE_IDX],
         readState.childrenStates[DictionaryColumn::DATA_COLUMN_CHILD_READ_STATE_IDX], offsetsToScan,
         resultVector, readState.metadata);
 }
 
-void StringColumn::lookupInternal(Transaction* transaction, ReadState& readState,
+void StringColumn::lookupInternal(Transaction* transaction, ChunkState& readState,
     ValueVector* nodeIDVector, ValueVector* resultVector) {
     KU_ASSERT(dataType.getPhysicalType() == PhysicalTypeID::STRING);
     std::vector<std::pair<string_index_t, uint64_t>> offsetsToScan;
     for (auto i = 0u; i < nodeIDVector->state->selVector->selectedSize; i++) {
         auto pos = nodeIDVector->state->selVector->selectedPositions[i];
         if (!nodeIDVector->isNull(pos)) {
             auto offsetInGroup = nodeIDVector->readNodeOffset(pos) -
@@ -178,18 +174,17 @@
     }
     dictionary.scan(transaction,
         readState.childrenStates[DictionaryColumn::OFFSET_COLUMN_CHILD_READ_STATE_IDX],
         readState.childrenStates[DictionaryColumn::DATA_COLUMN_CHILD_READ_STATE_IDX], offsetsToScan,
         resultVector, readState.metadata);
 }
 
-bool StringColumn::canCommitInPlace(transaction::Transaction* transaction,
-    node_group_idx_t nodeGroupIdx, const ChunkCollection& localInsertChunks,
-    const offset_to_row_idx_t& insertInfo, const ChunkCollection& localUpdateChunks,
-    const offset_to_row_idx_t& updateInfo) {
+bool StringColumn::canCommitInPlace(const ChunkState& state,
+    const ChunkCollection& localInsertChunks, const offset_to_row_idx_t& insertInfo,
+    const ChunkCollection& localUpdateChunks, const offset_to_row_idx_t& updateInfo) {
     auto strLenToAdd = 0u;
     for (auto& [_, rowIdx] : updateInfo) {
         auto [chunkIdx, offsetInLocalChunk] =
             LocalChunkedGroupCollection::getChunkIdxAndOffsetInChunk(rowIdx);
         auto localUpdateChunk =
             ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(localUpdateChunks[chunkIdx]);
         strLenToAdd += localUpdateChunk->getStringLength(offsetInLocalChunk);
@@ -202,53 +197,54 @@
         auto [chunkIdx, offsetInLocalChunk] =
             LocalChunkedGroupCollection::getChunkIdxAndOffsetInChunk(rowIdx);
         auto localInsertChunk =
             ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(localInsertChunks[chunkIdx]);
         strLenToAdd += localInsertChunk->getStringLength(offsetInLocalChunk);
     }
     auto numStrings = insertInfo.size() + updateInfo.size();
-    if (!dictionary.canCommitInPlace(transaction, nodeGroupIdx, numStrings, strLenToAdd)) {
+    if (!dictionary.canCommitInPlace(state, numStrings, strLenToAdd)) {
         return false;
     }
-    return canIndexCommitInPlace(transaction, nodeGroupIdx, numStrings, maxOffset);
+    return canIndexCommitInPlace(state, numStrings, maxOffset);
 }
 
-bool StringColumn::canCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+bool StringColumn::canCommitInPlace(const ChunkState& state,
     const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk, offset_t srcOffset) {
     auto strLenToAdd = 0u;
     auto strChunk = ku_dynamic_cast<ColumnChunk*, StringColumnChunk*>(chunk);
     auto length = std::min((uint64_t)dstOffsets.size(), strChunk->getNumValues());
     for (auto i = 0u; i < length; i++) {
         if (strChunk->getNullChunk()->isNull(i)) {
             continue;
         }
         strLenToAdd += strChunk->getStringLength(i + srcOffset);
     }
     auto numStrings = dstOffsets.size();
-    if (!dictionary.canCommitInPlace(transaction, nodeGroupIdx, numStrings, strLenToAdd)) {
+    if (!dictionary.canCommitInPlace(state, numStrings, strLenToAdd)) {
         return false;
     }
     auto maxDstOffset = getMaxOffset(dstOffsets);
-    return canIndexCommitInPlace(transaction, nodeGroupIdx, numStrings, maxDstOffset);
+    return canIndexCommitInPlace(state, numStrings, maxDstOffset);
 }
 
-bool StringColumn::canIndexCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    uint64_t numStrings, offset_t maxOffset) {
-    auto metadata = getMetadata(nodeGroupIdx, transaction->getType());
-    if (isMaxOffsetOutOfPagesCapacity(metadata, maxOffset)) {
+bool StringColumn::canIndexCommitInPlace(const ChunkState& state, uint64_t numStrings,
+    offset_t maxOffset) {
+    if (isMaxOffsetOutOfPagesCapacity(state.metadata, maxOffset)) {
         return false;
     }
-    if (metadata.compMeta.canAlwaysUpdateInPlace()) {
+    if (state.metadata.compMeta.canAlwaysUpdateInPlace()) {
         return true;
     }
     auto totalStringsAfterUpdate =
-        dictionary.getNumValuesInOffsets(transaction, nodeGroupIdx) + numStrings;
+        state.childrenStates[DictionaryColumn::OFFSET_COLUMN_CHILD_READ_STATE_IDX]
+            .metadata.numValues +
+        numStrings;
     // Check if the index column can store the largest new index in-place
-    if (!metadata.compMeta.canUpdateInPlace((const uint8_t*)&totalStringsAfterUpdate, 0 /*pos*/,
-            PhysicalTypeID::UINT32)) {
+    if (!state.metadata.compMeta.canUpdateInPlace((const uint8_t*)&totalStringsAfterUpdate,
+            0 /*pos*/, PhysicalTypeID::UINT32)) {
         return false;
     }
     return true;
 }
 
 void StringColumn::prepareCommit() {
     Column::prepareCommit();
```

### sdist/kuzu-source/src/storage/store/struct_column.cpp

```diff
@@ -46,73 +46,75 @@
     auto structColumnChunk = ku_dynamic_cast<ColumnChunk*, StructColumnChunk*>(columnChunk);
     for (auto i = 0u; i < childColumns.size(); i++) {
         childColumns[i]->scan(transaction, nodeGroupIdx, structColumnChunk->getChild(i),
             startOffset, endOffset);
     }
 }
 
-void StructColumn::initReadState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
-    offset_t startOffsetInChunk, ReadState& readState) {
-    Column::initReadState(transaction, nodeGroupIdx, startOffsetInChunk, readState);
+void StructColumn::initChunkState(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+    ChunkState& readState) {
+    Column::initChunkState(transaction, nodeGroupIdx, readState);
     readState.childrenStates.resize(childColumns.size());
     for (auto i = 0u; i < childColumns.size(); i++) {
-        childColumns[i]->initReadState(transaction, nodeGroupIdx, startOffsetInChunk,
-            readState.childrenStates[i]);
+        childColumns[i]->initChunkState(transaction, nodeGroupIdx, readState.childrenStates[i]);
     }
 }
 
-void StructColumn::scan(Transaction* transaction, ReadState& readState, offset_t startOffsetInGroup,
-    offset_t endOffsetInGroup, ValueVector* resultVector, uint64_t offsetInVector) {
+void StructColumn::scan(Transaction* transaction, ChunkState& readState,
+    offset_t startOffsetInGroup, offset_t endOffsetInGroup, ValueVector* resultVector,
+    uint64_t offsetInVector) {
     nullColumn->scan(transaction, *readState.nullState, startOffsetInGroup, endOffsetInGroup,
         resultVector, offsetInVector);
     for (auto i = 0u; i < childColumns.size(); i++) {
         auto fieldVector = StructVector::getFieldVector(resultVector, i).get();
         childColumns[i]->scan(transaction, readState.childrenStates[i], startOffsetInGroup,
             endOffsetInGroup, fieldVector, offsetInVector);
     }
 }
 
-void StructColumn::scanInternal(Transaction* transaction, ReadState& readState,
+void StructColumn::scanInternal(Transaction* transaction, ChunkState& readState,
     ValueVector* nodeIDVector, ValueVector* resultVector) {
     for (auto i = 0u; i < childColumns.size(); i++) {
         auto fieldVector = StructVector::getFieldVector(resultVector, i).get();
         childColumns[i]->scan(transaction, readState.childrenStates[i], nodeIDVector, fieldVector);
     }
 }
 
-void StructColumn::lookupInternal(Transaction* transaction, ReadState& readState,
+void StructColumn::lookupInternal(Transaction* transaction, ChunkState& readState,
     ValueVector* nodeIDVector, ValueVector* resultVector) {
     for (auto i = 0u; i < childColumns.size(); i++) {
         auto fieldVector = StructVector::getFieldVector(resultVector, i).get();
         childColumns[i]->lookup(transaction, readState.childrenStates[i], nodeIDVector,
             fieldVector);
     }
 }
 
-void StructColumn::write(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk,
-    ValueVector* vectorToWriteFrom, uint32_t posInVectorToWriteFrom) {
+void StructColumn::write(ChunkState& state, offset_t offsetInChunk, ValueVector* vectorToWriteFrom,
+    uint32_t posInVectorToWriteFrom) {
     KU_ASSERT(vectorToWriteFrom->dataType.getPhysicalType() == PhysicalTypeID::STRUCT);
     if (vectorToWriteFrom->isNull(posInVectorToWriteFrom)) {
         return;
     }
     KU_ASSERT(childColumns.size() == StructVector::getFieldVectors(vectorToWriteFrom).size());
     for (auto i = 0u; i < childColumns.size(); i++) {
         auto fieldVector = StructVector::getFieldVector(vectorToWriteFrom, i).get();
-        childColumns[i]->write(nodeGroupIdx, offsetInChunk, fieldVector, posInVectorToWriteFrom);
+        childColumns[i]->write(state.childrenStates[i], offsetInChunk, fieldVector,
+            posInVectorToWriteFrom);
     }
 }
 
-void StructColumn::write(node_group_idx_t nodeGroupIdx, offset_t offsetInChunk, ColumnChunk* data,
+void StructColumn::write(ChunkState& state, offset_t offsetInChunk, ColumnChunk* data,
     offset_t dataOffset, length_t numValues) {
     KU_ASSERT(data->getDataType().getPhysicalType() == PhysicalTypeID::STRUCT);
-    nullColumn->write(nodeGroupIdx, offsetInChunk, data->getNullChunk(), dataOffset, numValues);
+    nullColumn->write(*state.nullState, offsetInChunk, data->getNullChunk(), dataOffset, numValues);
     auto structData = ku_dynamic_cast<ColumnChunk*, StructColumnChunk*>(data);
     for (auto i = 0u; i < childColumns.size(); i++) {
         auto childData = structData->getChild(i);
-        childColumns[i]->write(nodeGroupIdx, offsetInChunk, childData, dataOffset, numValues);
+        childColumns[i]->write(state.childrenStates[i], offsetInChunk, childData, dataOffset,
+            numValues);
     }
 }
 
 void StructColumn::append(ColumnChunk* columnChunk, uint64_t nodeGroupIdx) {
     Column::append(columnChunk, nodeGroupIdx);
     KU_ASSERT(columnChunk->getDataType().getPhysicalType() == PhysicalTypeID::STRUCT);
     auto structColumnChunk = static_cast<StructColumnChunk*>(columnChunk);
@@ -138,28 +140,28 @@
 void StructColumn::prepareCommit() {
     Column::prepareCommit();
     for (const auto& childColumn : childColumns) {
         childColumn->prepareCommit();
     }
 }
 
-bool StructColumn::canCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+bool StructColumn::canCommitInPlace(const ChunkState& state,
     const ChunkCollection& localInsertChunk, const offset_to_row_idx_t& insertInfo,
     const ChunkCollection& localUpdateChunk, const offset_to_row_idx_t& updateInfo) {
     // STRUCT column doesn't have actual data stored in buffer. Only need to check the null column.
     // Children columns are committed separately.
-    return nullColumn->canCommitInPlace(transaction, nodeGroupIdx,
-        getNullChunkCollection(localInsertChunk), insertInfo,
-        getNullChunkCollection(localUpdateChunk), updateInfo);
+    KU_ASSERT(state.nullState);
+    return nullColumn->canCommitInPlace(*state.nullState, getNullChunkCollection(localInsertChunk),
+        insertInfo, getNullChunkCollection(localUpdateChunk), updateInfo);
 }
 
-bool StructColumn::canCommitInPlace(Transaction* transaction, node_group_idx_t nodeGroupIdx,
+bool StructColumn::canCommitInPlace(const ChunkState& state,
     const std::vector<offset_t>& dstOffsets, ColumnChunk* chunk, offset_t srcOffset) {
-    return nullColumn->canCommitInPlace(transaction, nodeGroupIdx, dstOffsets,
-        chunk->getNullChunk(), srcOffset);
+    return nullColumn->canCommitInPlace(*state.nullState, dstOffsets, chunk->getNullChunk(),
+        srcOffset);
 }
 
 void StructColumn::prepareCommitForChunk(Transaction* transaction, node_group_idx_t nodeGroupIdx,
     const ChunkCollection& localInsertChunk, const offset_to_row_idx_t& insertInfo,
     const ChunkCollection& localUpdateChunk, const offset_to_row_idx_t& updateInfo,
     const offset_set_t& deleteInfo) {
     auto currentNumNodeGroups = metadataDA->getNumElements(transaction->getType());
@@ -168,30 +170,30 @@
         // If this is a new node group, updateInfo should be empty. We should perform out-of-place
         // commit with a new column chunk.
         commitLocalChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, localInsertChunk,
             insertInfo, localUpdateChunk, updateInfo, deleteInfo);
     } else {
         // STRUCT column doesn't have actual data stored in buffer. Only need to update the null
         // column.
-        if (canCommitInPlace(transaction, nodeGroupIdx, localInsertChunk, insertInfo,
-                localUpdateChunk, updateInfo)) {
-            nullColumn->commitLocalChunkInPlace(transaction, nodeGroupIdx,
+        ChunkState state;
+        initChunkState(transaction, nodeGroupIdx, state);
+        if (canCommitInPlace(state, localInsertChunk, insertInfo, localUpdateChunk, updateInfo)) {
+            KU_ASSERT(state.nullState);
+            nullColumn->commitLocalChunkInPlace(transaction, *state.nullState,
                 getNullChunkCollection(localInsertChunk), insertInfo,
                 getNullChunkCollection(localUpdateChunk), updateInfo, deleteInfo);
+            nullColumn->metadataDA->update(state.nodeGroupIdx, state.nullState->metadata);
         } else {
-            nullColumn->commitLocalChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup,
+            nullColumn->commitLocalChunkOutOfPlace(transaction, state.nodeGroupIdx, isNewNodeGroup,
                 getNullChunkCollection(localInsertChunk), insertInfo,
                 getNullChunkCollection(localUpdateChunk), updateInfo, deleteInfo);
         }
-        auto chunkMeta = metadataDA->get(nodeGroupIdx, transaction->getType());
-        if (nullColumn->getMetadata(nodeGroupIdx, transaction->getType()).numValues !=
-            chunkMeta.numValues) {
-            chunkMeta.numValues =
-                nullColumn->getMetadata(nodeGroupIdx, transaction->getType()).numValues;
-            metadataDA->update(nodeGroupIdx, chunkMeta);
+        if (state.metadata.numValues != state.nullState->metadata.numValues) {
+            state.metadata.numValues = state.nullState->metadata.numValues;
+            metadataDA->update(state.nodeGroupIdx, state.metadata);
         }
         // Update each child column separately
         for (auto i = 0u; i < childColumns.size(); i++) {
             const auto& childColumn = childColumns[i];
             childColumn->prepareCommitForChunk(transaction, nodeGroupIdx,
                 getStructChildChunkCollection(localInsertChunk, i), insertInfo,
                 getStructChildChunkCollection(localUpdateChunk, i), updateInfo, deleteInfo);
@@ -208,27 +210,27 @@
         // If this is a new node group, updateInfo should be empty. We should perform out-of-place
         // commit with a new column chunk.
         commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup, dstOffsets, chunk,
             srcOffset);
     } else {
         // STRUCT column doesn't have actual data stored in buffer. Only need to update the null
         // column.
-        if (canCommitInPlace(transaction, nodeGroupIdx, dstOffsets, chunk, srcOffset)) {
-            nullColumn->commitColumnChunkInPlace(nodeGroupIdx, dstOffsets, chunk->getNullChunk(),
-                srcOffset);
+        ChunkState state;
+        initChunkState(transaction, nodeGroupIdx, state);
+        if (canCommitInPlace(state, dstOffsets, chunk, srcOffset)) {
+            nullColumn->commitColumnChunkInPlace(*state.nullState, dstOffsets,
+                chunk->getNullChunk(), srcOffset);
+            nullColumn->metadataDA->update(state.nodeGroupIdx, state.nullState->metadata);
         } else {
-            nullColumn->commitColumnChunkOutOfPlace(transaction, nodeGroupIdx, isNewNodeGroup,
+            nullColumn->commitColumnChunkOutOfPlace(transaction, state.nodeGroupIdx, isNewNodeGroup,
                 dstOffsets, chunk->getNullChunk(), srcOffset);
         }
-        auto chunkMeta = metadataDA->get(nodeGroupIdx, transaction->getType());
-        if (nullColumn->getMetadata(nodeGroupIdx, transaction->getType()).numValues !=
-            chunkMeta.numValues) {
-            chunkMeta.numValues =
-                nullColumn->getMetadata(nodeGroupIdx, transaction->getType()).numValues;
-            metadataDA->update(nodeGroupIdx, chunkMeta);
+        if (state.metadata.numValues != state.nullState->metadata.numValues) {
+            state.metadata.numValues = state.nullState->metadata.numValues;
+            metadataDA->update(state.nodeGroupIdx, state.metadata);
         }
         // Update each child column separately
         for (auto i = 0u; i < childColumns.size(); i++) {
             const auto& childColumn = childColumns[i];
             auto childChunk = ku_dynamic_cast<ColumnChunk*, StructColumnChunk*>(chunk)->getChild(i);
             childColumn->prepareCommitForChunk(transaction, nodeGroupIdx, dstOffsets, childChunk,
                 srcOffset);
```

### sdist/kuzu-source/third_party/antlr4_cypher/cypher_parser.cpp

```diff
@@ -447,15 +447,15 @@
   	506,5,136,0,0,505,507,5,150,0,0,506,505,1,0,0,0,506,507,1,0,0,0,507,508,
   	1,0,0,0,508,510,5,4,0,0,509,496,1,0,0,0,509,510,1,0,0,0,510,21,1,0,0,
   	0,511,512,5,96,0,0,512,513,5,150,0,0,513,514,3,284,142,0,514,23,1,0,0,
   	0,515,516,5,48,0,0,516,517,5,150,0,0,517,518,3,284,142,0,518,25,1,0,0,
   	0,519,520,5,49,0,0,520,521,5,150,0,0,521,523,3,286,143,0,522,524,5,150,
   	0,0,523,522,1,0,0,0,523,524,1,0,0,0,524,525,1,0,0,0,525,527,5,6,0,0,526,
   	528,5,150,0,0,527,526,1,0,0,0,527,528,1,0,0,0,528,529,1,0,0,0,529,530,
-  	3,238,119,0,530,27,1,0,0,0,531,532,5,50,0,0,532,533,5,150,0,0,533,534,
+  	3,190,95,0,530,27,1,0,0,0,531,532,5,50,0,0,532,533,5,150,0,0,533,534,
   	5,94,0,0,534,535,5,150,0,0,535,536,5,60,0,0,536,537,5,150,0,0,537,538,
   	3,284,142,0,538,539,5,150,0,0,539,540,5,125,0,0,540,541,5,150,0,0,541,
   	542,5,136,0,0,542,29,1,0,0,0,543,544,5,92,0,0,544,545,5,150,0,0,545,546,
   	5,51,0,0,546,547,5,150,0,0,547,549,3,254,127,0,548,550,5,150,0,0,549,
   	548,1,0,0,0,549,550,1,0,0,0,550,551,1,0,0,0,551,553,5,2,0,0,552,554,5,
   	150,0,0,553,552,1,0,0,0,553,554,1,0,0,0,554,556,1,0,0,0,555,557,3,32,
   	16,0,556,555,1,0,0,0,556,557,1,0,0,0,557,559,1,0,0,0,558,560,5,150,0,
@@ -2608,16 +2608,16 @@
   return getToken(CypherParser::SP, i);
 }
 
 CypherParser::OC_SymbolicNameContext* CypherParser::KU_StandaloneCallContext::oC_SymbolicName() {
   return getRuleContext<CypherParser::OC_SymbolicNameContext>(0);
 }
 
-CypherParser::OC_LiteralContext* CypherParser::KU_StandaloneCallContext::oC_Literal() {
-  return getRuleContext<CypherParser::OC_LiteralContext>(0);
+CypherParser::OC_ExpressionContext* CypherParser::KU_StandaloneCallContext::oC_Expression() {
+  return getRuleContext<CypherParser::OC_ExpressionContext>(0);
 }
 
 
 size_t CypherParser::KU_StandaloneCallContext::getRuleIndex() const {
   return CypherParser::RuleKU_StandaloneCall;
 }
 
@@ -2657,15 +2657,15 @@
 
     _la = _input->LA(1);
     if (_la == CypherParser::SP) {
       setState(526);
       match(CypherParser::SP);
     }
     setState(529);
-    oC_Literal();
+    oC_Expression();
    
   }
   catch (RecognitionException &e) {
     _errHandler->reportError(this, e);
     _localctx->exception = std::current_exception();
     _errHandler->recover(this, _localctx->exception);
   }
```

### sdist/kuzu-source/third_party/antlr4_cypher/include/cypher_parser.h

```diff
@@ -484,15 +484,15 @@
   public:
     KU_StandaloneCallContext(antlr4::ParserRuleContext *parent, size_t invokingState);
     virtual size_t getRuleIndex() const override;
     antlr4::tree::TerminalNode *CALL();
     std::vector<antlr4::tree::TerminalNode *> SP();
     antlr4::tree::TerminalNode* SP(size_t i);
     OC_SymbolicNameContext *oC_SymbolicName();
-    OC_LiteralContext *oC_Literal();
+    OC_ExpressionContext *oC_Expression();
 
    
   };
 
   KU_StandaloneCallContext* kU_StandaloneCall();
 
   class  KU_CommentOnContext : public antlr4::ParserRuleContext {
```

### sdist/kuzu.egg-info/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuzu
-Version: 0.3.3.dev47
+Version: 0.3.3.dev48
 Summary: An in-process property graph database management system built for query speed and scalability.
 Home-page: https://github.com/kuzudb/kuzu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kuzu Version: 0.3.3.dev47 Summary: An in-process
+Metadata-Version: 2.1 Name: kuzu Version: 0.3.3.dev48 Summary: An in-process
 property graph database management system built for query speed and
 scalability. Home-page: https://github.com/kuzudb/kuzu License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE
                     [https://kuzudb.com/img/kuzu-logo.png]
 
   _[_G_i_t_h_u_b_ _A_c_t_i_o_n_s_ _B_a_d_g_e_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_k_u_z_u_d_b_/_k_u_z_u_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
               _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_N_1_A_T_6_H_7_9_L_M_]_[_d_i_s_c_o_r_d_]_[_t_w_i_t_t_e_r_]
```

### sdist/pyproject.toml

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "kuzu"
 description = "Highly scalable, extremely fast, easy-to-use embeddable graph database"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["graph", "database"]
-version = "0.3.3.dev47"
+version = "0.3.3.dev48"
 
 [project.urls]
 Homepage = "https://kuzudb.com/"
 Documentation = "https://docs.kuzudb.com/"
 Repository = "https://github.com/kuzudb/kuzu"
 Changelog = "https://github.com/kuzudb/kuzu/releases"
```

