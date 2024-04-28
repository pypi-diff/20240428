# Comparing `tmp/mau-3.1.0.tar.gz` & `tmp/mau-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mau-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mau-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mau-3.1.0.tar` & `mau-4.0.0.tar`

### file list

```diff
@@ -1,127 +1,151 @@
--rw-r--r--   0        0        0      528 2022-10-26 07:17:29.495806 mau-3.1.0/.gitignore
--rw-r--r--   0        0        0     6099 2023-11-13 17:11:02.058605 mau-3.1.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1084 2023-08-14 07:33:57.840796 mau-3.1.0/LICENSE
--rw-r--r--   0        0        0     2161 2023-08-14 07:41:01.637557 mau-3.1.0/README.md
--rw-r--r--   0        0        0     9226 2023-11-12 18:00:34.095200 mau-3.1.0/e2e_tests/output/test_blocks.yaml
--rw-r--r--   0        0        0     5805 2023-11-12 18:00:34.227201 mau-3.1.0/e2e_tests/output/test_directives.yaml
--rw-r--r--   0        0        0     7878 2023-11-12 18:00:34.351202 mau-3.1.0/e2e_tests/output/test_footnotes.yaml
--rw-r--r--   0        0        0     5403 2023-11-12 18:00:34.483203 mau-3.1.0/e2e_tests/output/test_inline_nodes.yaml
--rw-r--r--   0        0        0    10326 2023-11-12 18:00:34.619203 mau-3.1.0/e2e_tests/output/test_page_nodes.yaml
--rw-r--r--   0        0        0     4520 2023-11-12 18:00:34.735204 mau-3.1.0/e2e_tests/output/test_references.yaml
--rw-r--r--   0        0        0     4415 2023-11-13 17:11:02.058605 mau-3.1.0/e2e_tests/output/test_source_blocks.yaml
--rw-r--r--   0        0        0     3675 2023-11-12 18:00:34.963206 mau-3.1.0/e2e_tests/output/test_toc.yaml
--rw-r--r--   0        0        0     2534 2023-11-12 18:00:35.079206 mau-3.1.0/e2e_tests/output/test_variables.yaml
--rw-r--r--   0        0        0     9226 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_blocks.yaml
--rw-r--r--   0        0        0     5805 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_directives.yaml
--rw-r--r--   0        0        0     7878 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_footnotes.yaml
--rw-r--r--   0        0        0     5403 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_inline_nodes.yaml
--rw-r--r--   0        0        0    10326 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_page_nodes.yaml
--rw-r--r--   0        0        0     4520 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_references.yaml
--rw-r--r--   0        0        0     4415 2023-11-13 17:11:02.058605 mau-3.1.0/e2e_tests/parser/test_source_blocks.yaml
--rw-r--r--   0        0        0     3675 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_toc.yaml
--rw-r--r--   0        0        0     2534 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/parser/test_variables.yaml
--rwxr-xr-x   0        0        0      584 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/run_tests.sh
--rw-r--r--   0        0        0     9226 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_blocks
--rw-r--r--   0        0        0     1678 2023-08-29 06:19:18.363744 mau-3.1.0/e2e_tests/source/test_blocks.mau
--rw-r--r--   0        0        0       91 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_directives.mau
--rw-r--r--   0        0        0      679 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_footnotes.mau
--rw-r--r--   0        0        0      818 2023-08-28 10:16:38.416059 mau-3.1.0/e2e_tests/source/test_inline_nodes.mau
--rw-r--r--   0        0        0     1182 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_page_nodes.mau
--rw-r--r--   0        0        0      363 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_references.mau
--rw-r--r--   0        0        0     4135 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_source_blocks
--rw-r--r--   0        0        0      879 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_source_blocks.mau
--rw-r--r--   0        0        0      328 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_toc.mau
--rw-r--r--   0        0        0      652 2023-08-14 07:33:57.840796 mau-3.1.0/e2e_tests/source/test_variables.mau
--rw-r--r--   0        0        0     3815 2023-11-13 17:11:02.058605 mau-3.1.0/mau/__init__.py
--rw-r--r--   0        0        0     1177 2023-11-13 17:11:02.058605 mau-3.1.0/mau/errors.py
--rw-r--r--   0        0        0      142 2023-08-14 07:33:57.840796 mau-3.1.0/mau/helpers.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.840796 mau-3.1.0/mau/lexers/__init__.py
--rw-r--r--   0        0        0      914 2023-08-28 13:30:41.168675 mau-3.1.0/mau/lexers/arguments_lexer.py
--rw-r--r--   0        0        0     6054 2023-11-13 17:11:02.058605 mau-3.1.0/mau/lexers/base_lexer.py
--rw-r--r--   0        0        0     7848 2023-08-29 12:56:01.747050 mau-3.1.0/mau/lexers/main_lexer.py
--rw-r--r--   0        0        0      530 2023-08-14 07:33:57.840796 mau-3.1.0/mau/lexers/preprocess_variables_lexer.py
--rw-r--r--   0        0        0      914 2023-08-28 13:30:38.944653 mau-3.1.0/mau/lexers/text_lexer.py
--rw-r--r--   0        0        0     4829 2023-11-13 17:11:02.058605 mau-3.1.0/mau/main.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.840796 mau-3.1.0/mau/nodes/__init__.py
--rw-r--r--   0        0        0      582 2023-08-14 07:33:57.840796 mau-3.1.0/mau/nodes/arguments.py
--rw-r--r--   0        0        0     1391 2023-08-14 07:33:57.840796 mau-3.1.0/mau/nodes/footnotes.py
--rw-r--r--   0        0        0     3753 2023-11-13 17:11:02.058605 mau-3.1.0/mau/nodes/inline.py
--rw-r--r--   0        0        0     1005 2023-08-14 07:33:57.840796 mau-3.1.0/mau/nodes/nodes.py
--rw-r--r--   0        0        0     6936 2023-08-17 07:03:39.012518 mau-3.1.0/mau/nodes/page.py
--rw-r--r--   0        0        0     2115 2023-08-14 07:33:57.840796 mau-3.1.0/mau/nodes/references.py
--rw-r--r--   0        0        0     2764 2023-08-14 07:33:57.840796 mau-3.1.0/mau/nodes/source.py
--rw-r--r--   0        0        0     1271 2023-08-14 07:33:57.840796 mau-3.1.0/mau/nodes/toc.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.840796 mau-3.1.0/mau/parsers/__init__.py
--rw-r--r--   0        0        0     1122 2023-08-14 07:33:57.840796 mau-3.1.0/mau/parsers/arguments.py
--rw-r--r--   0        0        0     3485 2023-08-14 07:33:57.840796 mau-3.1.0/mau/parsers/arguments_parser.py
--rw-r--r--   0        0        0    11647 2023-11-13 17:11:02.058605 mau-3.1.0/mau/parsers/base_parser.py
--rw-r--r--   0        0        0     1394 2023-08-14 07:33:57.840796 mau-3.1.0/mau/parsers/environment.py
--rw-r--r--   0        0        0    38353 2023-11-13 17:11:02.058605 mau-3.1.0/mau/parsers/main_parser.py
--rw-r--r--   0        0        0     2164 2023-08-14 07:33:57.844796 mau-3.1.0/mau/parsers/preprocess_variables_parser.py
--rw-r--r--   0        0        0     9920 2023-08-17 08:29:57.551726 mau-3.1.0/mau/parsers/text_parser.py
--rw-r--r--   0        0        0     1249 2023-08-14 07:33:57.844796 mau-3.1.0/mau/parsers/toc.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/mau/text_buffer/__init__.py
--rw-r--r--   0        0        0     1169 2023-11-13 17:11:02.058605 mau-3.1.0/mau/text_buffer/context.py
--rw-r--r--   0        0        0     5331 2023-08-15 07:24:48.600651 mau-3.1.0/mau/text_buffer/text_buffer.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/mau/tokens/__init__.py
--rw-r--r--   0        0        0     1230 2023-08-14 07:33:57.844796 mau-3.1.0/mau/tokens/tokens.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/mau/visitors/__init__.py
--rw-r--r--   0        0        0    15396 2023-11-13 17:11:02.062605 mau-3.1.0/mau/visitors/base_visitor.py
--rw-r--r--   0        0        0     6934 2023-08-17 11:25:05.252752 mau-3.1.0/mau/visitors/jinja_visitor.py
--rw-r--r--   0        0        0      152 2023-08-14 07:33:57.844796 mau-3.1.0/noxfile.py
--rw-r--r--   0        0        0     2040 2023-11-13 17:11:02.062605 mau-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-08-14 07:33:57.844796 mau-3.1.0/requirements.txt
--rw-r--r--   0        0        0       15 2023-08-14 07:33:57.844796 mau-3.1.0/requirements/development.txt
--rw-r--r--   0        0        0        2 2023-08-14 07:33:57.844796 mau-3.1.0/requirements/production.txt
--rw-r--r--   0        0        0       11 2023-08-14 07:33:57.844796 mau-3.1.0/requirements/testing.txt
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1120 2023-08-14 07:33:57.844796 mau-3.1.0/tests/helpers.py
--rw-r--r--   0        0        0        0 2023-08-14 07:30:31.547551 mau-3.1.0/tests/lexers/__init__.py
--rw-r--r--   0        0        0      483 2023-08-14 07:33:57.844796 mau-3.1.0/tests/lexers/data_file_lexer.txt
--rw-r--r--   0        0        0     4996 2023-11-13 17:11:02.062605 mau-3.1.0/tests/lexers/test_arguments_lexer.py
--rw-r--r--   0        0        0     5768 2023-11-13 17:11:02.062605 mau-3.1.0/tests/lexers/test_base_lexer.py
--rw-r--r--   0        0        0    20837 2023-11-13 17:11:02.062605 mau-3.1.0/tests/lexers/test_main_lexer.py
--rw-r--r--   0        0        0     5084 2023-11-13 17:11:02.062605 mau-3.1.0/tests/lexers/test_preprocess_variables_lexer.py
--rw-r--r--   0        0        0     6321 2023-11-13 17:11:02.062605 mau-3.1.0/tests/lexers/test_text_lexer.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/__init__.py
--rw-r--r--   0        0        0      566 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/test_arguments.py
--rw-r--r--   0        0        0     2637 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/test_footnotes.py
--rw-r--r--   0        0        0     3124 2023-11-13 17:11:02.062605 mau-3.1.0/tests/nodes/test_inline.py
--rw-r--r--   0        0        0      940 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/test_nodes.py
--rw-r--r--   0        0        0     6136 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/test_page.py
--rw-r--r--   0        0        0     3978 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/test_references.py
--rw-r--r--   0        0        0     1511 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/test_source.py
--rw-r--r--   0        0        0      949 2023-08-14 07:33:57.844796 mau-3.1.0/tests/nodes/test_toc.py
--rw-r--r--   0        0        0        0 2023-08-14 07:30:31.551551 mau-3.1.0/tests/parsers/__init__.py
--rw-r--r--   0        0        0        0 2023-08-14 07:30:31.551551 mau-3.1.0/tests/parsers/main_parser/__init__.py
--rw-r--r--   0        0        0    15591 2023-11-13 17:11:02.062605 mau-3.1.0/tests/parsers/main_parser/test_block_attributes.py
--rw-r--r--   0        0        0     4982 2023-11-13 17:11:02.062605 mau-3.1.0/tests/parsers/main_parser/test_block_basic.py
--rw-r--r--   0        0        0     4095 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_block_engine.py
--rw-r--r--   0        0        0     2656 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_block_footnote.py
--rw-r--r--   0        0        0     2407 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_block_other.py
--rw-r--r--   0        0        0     7909 2023-11-13 17:11:02.062605 mau-3.1.0/tests/parsers/main_parser/test_block_source.py
--rw-r--r--   0        0        0     4909 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_headers.py
--rw-r--r--   0        0        0     2760 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_include_content.py
--rw-r--r--   0        0        0     4930 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_lists.py
--rw-r--r--   0        0        0     6675 2023-11-13 17:11:02.062605 mau-3.1.0/tests/parsers/main_parser/test_main_parser.py
--rw-r--r--   0        0        0     9964 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_references.py
--rw-r--r--   0        0        0     3710 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/main_parser/test_variables.py
--rw-r--r--   0        0        0    10159 2023-11-13 17:11:02.062605 mau-3.1.0/tests/parsers/test_arguments_parser.py
--rw-r--r--   0        0        0    12120 2023-11-13 17:11:02.062605 mau-3.1.0/tests/parsers/test_base_parser.py
--rw-r--r--   0        0        0     2433 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/test_environment.py
--rw-r--r--   0        0        0     3474 2023-11-13 17:11:02.062605 mau-3.1.0/tests/parsers/test_preprocess_variables_parser.py
--rw-r--r--   0        0        0    14196 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/test_text_parser.py
--rw-r--r--   0        0        0     2520 2023-08-14 07:33:57.844796 mau-3.1.0/tests/parsers/test_toc.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/tests/text_buffer/__init__.py
--rw-r--r--   0        0        0      386 2023-08-14 07:33:57.844796 mau-3.1.0/tests/text_buffer/test_context.py
--rw-r--r--   0        0        0     4786 2023-08-14 07:33:57.844796 mau-3.1.0/tests/text_buffer/test_text_buffer.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/tests/tokens/__init__.py
--rw-r--r--   0        0        0     2192 2023-08-14 07:33:57.844796 mau-3.1.0/tests/tokens/test_tokens.py
--rw-r--r--   0        0        0        0 2023-08-14 07:30:31.551551 mau-3.1.0/tests/visitors/__init__.py
--rw-r--r--   0        0        0        0 2023-08-14 07:33:57.844796 mau-3.1.0/tests/visitors/base_visitor/__init__.py
--rw-r--r--   0        0        0     8779 2023-11-13 17:11:02.062605 mau-3.1.0/tests/visitors/base_visitor/test_inline_nodes.py
--rw-r--r--   0        0        0    24850 2023-08-14 07:33:57.844796 mau-3.1.0/tests/visitors/base_visitor/test_page_nodes.py
--rw-r--r--   0        0        0       66 2023-11-13 17:11:02.062605 mau-3.1.0/tests/visitors/jinja_visitor/conftest.py
--rw-r--r--   0        0        0     7258 2023-11-13 17:11:02.062605 mau-3.1.0/tests/visitors/jinja_visitor/test_inline_nodes.py
--rw-r--r--   0        0        0    18490 2023-11-13 17:11:02.062605 mau-3.1.0/tests/visitors/jinja_visitor/test_page_nodes.py
--rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 mau-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      528 2022-10-26 07:17:29.495806 mau-4.0.0/.gitignore
+-rw-r--r--   0        0        0     8985 2024-04-28 20:04:41.973523 mau-4.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1084 2023-08-14 07:33:57.840796 mau-4.0.0/LICENSE
+-rw-r--r--   0        0        0     1477 2024-04-28 20:06:54.954456 mau-4.0.0/README.md
+-rw-r--r--   0        0        0     2203 2024-04-28 20:04:41.973523 mau-4.0.0/mau/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.973523 mau-4.0.0/mau/environment/__init__.py
+-rw-r--r--   0        0        0     2721 2024-04-28 20:04:41.973523 mau-4.0.0/mau/environment/environment.py
+-rw-r--r--   0        0        0     1190 2024-04-28 20:04:41.973523 mau-4.0.0/mau/errors.py
+-rw-r--r--   0        0        0      142 2024-03-29 22:28:59.350920 mau-4.0.0/mau/helpers.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.0/mau/lexers/__init__.py
+-rw-r--r--   0        0        0      914 2024-03-29 22:28:59.346920 mau-4.0.0/mau/lexers/arguments_lexer.py
+-rw-r--r--   0        0        0     6172 2024-04-28 20:04:41.973523 mau-4.0.0/mau/lexers/base_lexer.py
+-rw-r--r--   0        0        0     8613 2024-04-28 20:04:41.973523 mau-4.0.0/mau/lexers/main_lexer.py
+-rw-r--r--   0        0        0      530 2024-03-29 22:28:59.346920 mau-4.0.0/mau/lexers/preprocess_variables_lexer.py
+-rw-r--r--   0        0        0      919 2024-04-28 20:04:41.973523 mau-4.0.0/mau/lexers/text_lexer.py
+-rw-r--r--   0        0        0     5594 2024-04-28 20:04:41.973523 mau-4.0.0/mau/main.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.0/mau/nodes/__init__.py
+-rw-r--r--   0        0        0      936 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/arguments.py
+-rw-r--r--   0        0        0     2468 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/block.py
+-rw-r--r--   0        0        0     2047 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/content.py
+-rw-r--r--   0        0        0     1731 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/footnotes.py
+-rw-r--r--   0        0        0      842 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/header.py
+-rw-r--r--   0        0        0      989 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/inline.py
+-rw-r--r--   0        0        0     1508 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/lists.py
+-rw-r--r--   0        0        0     3770 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/macros.py
+-rw-r--r--   0        0        0     2569 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/nodes.py
+-rw-r--r--   0        0        0      739 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/page.py
+-rw-r--r--   0        0        0      686 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/paragraph.py
+-rw-r--r--   0        0        0     3476 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/source.py
+-rw-r--r--   0        0        0     1004 2024-04-28 20:04:41.973523 mau-4.0.0/mau/nodes/toc.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/mau/parsers/__init__.py
+-rw-r--r--   0        0        0     1287 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/arguments.py
+-rw-r--r--   0        0        0     3876 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/arguments_parser.py
+-rw-r--r--   0        0        0      855 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/attributes.py
+-rw-r--r--   0        0        0    12389 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/base_parser.py
+-rw-r--r--   0        0        0     3758 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/footnotes.py
+-rw-r--r--   0        0        0      998 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/internal_links.py
+-rw-r--r--   0        0        0    38156 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/main_parser.py
+-rw-r--r--   0        0        0     2254 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/preprocess_variables_parser.py
+-rw-r--r--   0        0        0    14892 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/text_parser.py
+-rw-r--r--   0        0        0     3516 2024-04-28 20:04:41.973523 mau-4.0.0/mau/parsers/toc.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/mau/text_buffer/__init__.py
+-rw-r--r--   0        0        0     1169 2024-04-23 21:38:42.846385 mau-4.0.0/mau/text_buffer/context.py
+-rw-r--r--   0        0        0     5331 2024-03-29 22:28:59.350920 mau-4.0.0/mau/text_buffer/text_buffer.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.346920 mau-4.0.0/mau/tokens/__init__.py
+-rw-r--r--   0        0        0     1230 2024-03-29 22:28:59.346920 mau-4.0.0/mau/tokens/tokens.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/mau/visitors/__init__.py
+-rw-r--r--   0        0        0    13054 2024-04-28 20:04:41.973523 mau-4.0.0/mau/visitors/base_visitor.py
+-rw-r--r--   0        0        0     8564 2024-04-28 20:04:41.977522 mau-4.0.0/mau/visitors/jinja_visitor.py
+-rw-r--r--   0        0        0      152 2023-08-14 07:33:57.844796 mau-4.0.0/noxfile.py
+-rw-r--r--   0        0        0     2040 2024-04-28 20:04:41.977522 mau-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-08-14 07:33:57.844796 mau-4.0.0/requirements.txt
+-rw-r--r--   0        0        0       15 2023-08-14 07:33:57.844796 mau-4.0.0/requirements/development.txt
+-rw-r--r--   0        0        0        2 2023-08-14 07:33:57.844796 mau-4.0.0/requirements/production.txt
+-rw-r--r--   0        0        0       11 2023-08-14 07:33:57.844796 mau-4.0.0/requirements/testing.txt
+-rw-r--r--   0        0        0        0 2024-04-17 20:37:15.825771 mau-4.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     6907 2024-04-28 20:04:41.977522 mau-4.0.0/tests/environment/test_environment.py
+-rw-r--r--   0        0        0     2209 2024-04-28 20:04:41.977522 mau-4.0.0/tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/lexers/__init__.py
+-rw-r--r--   0        0        0      483 2023-08-14 07:33:57.844796 mau-4.0.0/tests/lexers/data_file_lexer.txt
+-rw-r--r--   0        0        0     5165 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_arguments_lexer.py
+-rw-r--r--   0        0        0     6038 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_base_lexer.py
+-rw-r--r--   0        0        0    20055 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_main_lexer.py
+-rw-r--r--   0        0        0     4905 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_preprocess_variables_lexer.py
+-rw-r--r--   0        0        0     7048 2024-04-28 20:04:41.977522 mau-4.0.0/tests/lexers/test_text_lexer.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/nodes/__init__.py
+-rw-r--r--   0        0        0      566 2024-03-29 22:28:59.350920 mau-4.0.0/tests/nodes/test_arguments.py
+-rw-r--r--   0        0        0      357 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_block.py
+-rw-r--r--   0        0        0     1044 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_content.py
+-rw-r--r--   0        0        0     2207 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_footnotes.py
+-rw-r--r--   0        0        0      793 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_header.py
+-rw-r--r--   0        0        0     1075 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_inline.py
+-rw-r--r--   0        0        0     1281 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_lists.py
+-rw-r--r--   0        0        0     2224 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_macros.py
+-rw-r--r--   0        0        0      937 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_nodes.py
+-rw-r--r--   0        0        0     1142 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_page.py
+-rw-r--r--   0        0        0      741 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_paragraph.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_references.py
+-rw-r--r--   0        0        0     1511 2024-03-29 22:28:59.350920 mau-4.0.0/tests/nodes/test_source.py
+-rw-r--r--   0        0        0     1689 2024-04-28 20:04:41.977522 mau-4.0.0/tests/nodes/test_toc.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/parsers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/parsers/main_parser/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_arguments.py
+-rw-r--r--   0        0        0    11978 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_attributes.py
+-rw-r--r--   0        0        0     4537 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_basic.py
+-rw-r--r--   0        0        0     4448 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_engine_group.py
+-rw-r--r--   0        0        0     7240 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_engine_mau.py
+-rw-r--r--   0        0        0     1063 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_engine_raw.py
+-rw-r--r--   0        0        0     2107 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_other.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_block_source.py
+-rw-r--r--   0        0        0     2625 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_content.py
+-rw-r--r--   0        0        0     6304 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_control.py
+-rw-r--r--   0        0        0    11881 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_footnotes.py
+-rw-r--r--   0        0        0     7903 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_headers.py
+-rw-r--r--   0        0        0      795 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_horizontal_rule.py
+-rw-r--r--   0        0        0     4214 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_internal_links.py
+-rw-r--r--   0        0        0     8408 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_lists.py
+-rw-r--r--   0        0        0     3880 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_main_parser.py
+-rw-r--r--   0        0        0     2153 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_paragraph.py
+-rw-r--r--   0        0        0      778 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_parent.py
+-rw-r--r--   0        0        0     7926 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_source.py
+-rw-r--r--   0        0        0     2459 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_title.py
+-rw-r--r--   0        0        0     7622 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_toc.py
+-rw-r--r--   0        0        0     4100 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/main_parser/test_variables.py
+-rw-r--r--   0        0        0    11168 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_arguments_parser.py
+-rw-r--r--   0        0        0    12199 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_base_parser.py
+-rw-r--r--   0        0        0     4287 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_create_toc.py
+-rw-r--r--   0        0        0     3468 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/test_preprocess_variables_parser.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_arguments.py
+-rw-r--r--   0        0        0     1637 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_class.py
+-rw-r--r--   0        0        0     5553 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_control.py
+-rw-r--r--   0        0        0      575 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_footnote.py
+-rw-r--r--   0        0        0     1290 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_generic_macro.py
+-rw-r--r--   0        0        0      802 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_header.py
+-rw-r--r--   0        0        0      973 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_image.py
+-rw-r--r--   0        0        0     1929 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/macros/test_link.py
+-rw-r--r--   0        0        0     1223 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_basic_text.py
+-rw-r--r--   0        0        0     2443 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_escaped.py
+-rw-r--r--   0        0        0     2624 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_style.py
+-rw-r--r--   0        0        0     1246 2024-04-28 20:04:41.977522 mau-4.0.0/tests/parsers/text_parser/test_verbatim.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/text_buffer/__init__.py
+-rw-r--r--   0        0        0      386 2024-03-29 22:28:59.354920 mau-4.0.0/tests/text_buffer/test_context.py
+-rw-r--r--   0        0        0     4786 2024-03-29 22:28:59.354920 mau-4.0.0/tests/text_buffer/test_text_buffer.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/tokens/__init__.py
+-rw-r--r--   0        0        0     2192 2024-03-29 22:28:59.350920 mau-4.0.0/tests/tokens/test_tokens.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.354920 mau-4.0.0/tests/visitors/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:28:59.350920 mau-4.0.0/tests/visitors/base_visitor/__init__.py
+-rw-r--r--   0        0        0     8808 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_block.py
+-rw-r--r--   0        0        0     3074 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_content.py
+-rw-r--r--   0        0        0     3093 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_footnotes.py
+-rw-r--r--   0        0        0     1556 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_header.py
+-rw-r--r--   0        0        0    13787 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_inline.py
+-rw-r--r--   0        0        0     2547 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_lists.py
+-rw-r--r--   0        0        0     2370 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_page.py
+-rw-r--r--   0        0        0     1872 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_paragraph.py
+-rw-r--r--   0        0        0     4295 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_source.py
+-rw-r--r--   0        0        0     5265 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/base_visitor/test_toc.py
+-rw-r--r--   0        0        0     6392 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_block.py
+-rw-r--r--   0        0        0     2115 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_content.py
+-rw-r--r--   0        0        0     1406 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_footnotes.py
+-rw-r--r--   0        0        0     1151 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_header.py
+-rw-r--r--   0        0        0     7556 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_inline.py
+-rw-r--r--   0        0        0     1638 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_lists.py
+-rw-r--r--   0        0        0      857 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_page.py
+-rw-r--r--   0        0        0     2069 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_paragraph.py
+-rw-r--r--   0        0        0     1283 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_source.py
+-rw-r--r--   0        0        0     7366 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/test_templates.py
+-rw-r--r--   0        0        0     1354 2024-04-28 20:04:41.977522 mau-4.0.0/tests/visitors/jinja_visitor/toc.py
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 mau-4.0.0/PKG-INFO
```

### Comparing `mau-3.1.0/.gitignore` & `mau-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/CHANGELOG.rst` & `mau-4.0.0/CHANGELOG.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,44 @@
 =========
 Changelog
 =========
 
+Version 4.0.0
+=============
+
+Please be aware that this major release contains breaking changes from Mau 3. All changes marked `syntax` are breaking and thus require manual modification of the Mau source.
+
+- [enhancement] Block aliases can be defined through the environment.
+- [enhancement] Header anchor can be forced through the attribute `anchor`.
+- [enhancement] Headers support variables and rich text.
+- [enhancement] Variable values can contain other variables.
+- [enhancement] List start can be forced through the attribute `start` and automated to link to a previous list.
+- [enhancement] Macros can contain rich text.
+- [enhancement] New macro `[header](id)` that creates an internal link to a header with that `id`.
+- [enhancement] New macro `if` that renders text conditionally.
+- [enhancement] New macro `ifeval` that renders the content of variables conditionally (short-circuit evaluation). 
+- [enhancement] Paragraphs now store a title defined before them.
+- [enhancement] Parser output contains a separate ToC that can be rendered using different templates (e.g. using a prefix).
+- [enhancement] The list of template names that Mau considers for each node has been considerably increased. Now templates can include the parent type, subtype, the node position in the parent node, visitor prefixes, node subtype, and node tags.
+- [enhancement] The variable `mau.visitor.format` contains the output format.
+- [enhancement] Added `$` and `%` to escape text like verbatim without using `VerbatimNode`.
+- [internal] All nodes contain a link to the parent node and to the position they have in it.
+- [internal] Blocks use positions `primary` and `secondary` for children.
+- [internal] Titles and headers use `SentenceNode` and all nodes inside the sentence are given the position `title` or `header` respectively.
+- [internal] All nodes receive the same basic arguments to promote a uniform interface.
+- [syntax] Content nodes receive only the content type and the list of URIs, all other parameters are passed as attributes.
+- [syntax] New way to define and print boolean variables
+- [syntax] Node subtype is created using `*` in the attributes. All document nodes can now have a subtype.
+- [syntax] Removed reference engine, reference macro, and references command from syntax.
+- [syntax] The variable `mau.parser.content_wrapper` now accepts an instance and not a class any more, which allows to customise the wrapper through attributes like subtype and tags.
+- [syntax] New syntax for control statements that allow uniform conditional rendering of document and text nodes.
+- [syntax] Removed `condition` flag to render blocks (replaced with control statements).
+- [syntax] Admonitions don't use the argument `label` any more. They use the block title.
+- [syntax] Macro `class` now accepts multiple classes as arguments instead of using a comma-separated single argument.
+
 Version 3.1.0
 =============
 
 - [fix] Added RawNode node and make source blocks emit lists of RawNode instead of TextNode. This prevents escaping characters in formats like HTML. Raw blocks now use a list of RawNode as well.
 
 Version 3.0.3
 =============
```

### Comparing `mau-3.1.0/LICENSE` & `mau-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/mau/errors.py` & `mau-4.0.0/mau/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 class MauErrorException(ValueError):
     """
     This is a processing error that can occour
     during lexing, parsing, or visiting.
     """
 
     def __init__(self, error):
-        super().__init__()
+        super().__init__(error.message)
 
         self.error = error
 
 
 class MauError:
     """
     This is a processing error that can occour
```

### Comparing `mau-3.1.0/mau/lexers/arguments_lexer.py` & `mau-4.0.0/mau/lexers/arguments_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/mau/lexers/base_lexer.py` & `mau-4.0.0/mau/lexers/base_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,29 @@
     """
     The base class for lexers.
     The lexer decomposes the input text into a list of tokens
     and provides basic navigation functions in the
     output results.
     """
 
-    def __init__(self, text_buffer):
-        self._text_buffer = text_buffer
+    def __init__(self, environment):
+        self.text_buffer = None
 
         # These are the tokens identified so far
         self.tokens = []
 
         # The last visited context. Used to detect loops.
         self.last_visited_context = None
 
-    def process(self):
+        # The configuration environment
+        self.environment = environment
+
+    def process(self, text_buffer):
+        self.text_buffer = text_buffer
+
         # Process tokens until we reach the end of file
         self._process()
         while True:
             # Check if the last thing we processed is an EOF
             if len(self.tokens) > 0 and self.tokens[-1].type is TokenTypes.EOF:
                 break
 
@@ -52,41 +57,41 @@
 
         # if Token(TokenTypes.EOF) in self.tokens:
         #     self.tokens.remove(Token(TokenTypes.EOF))
 
     @property
     def _current_char(self):
         # Return the current character
-        return self._text_buffer.current_char
+        return self.text_buffer.current_char
 
     @property
     def _current_line(self):
         # Return the current line
-        return self._text_buffer.current_line
+        return self.text_buffer.current_line
 
     @property
     def _context(self):
         # Return the context
-        return self._text_buffer.context
+        return self.text_buffer.context
 
     @property
     def _tail(self):
         # A wrapper to return the rest of the line
-        return self._text_buffer.tail
+        return self.text_buffer.tail
 
     def _nextline(self):
         # Skip the whole line including the EOL
-        self._text_buffer.nextline()
+        self.text_buffer.nextline()
 
     def _skip(self, value):
         # Skip only the given amount of characters
         # This is very useful with regexp groups
         # that can be None.
         if value is not None:
-            self._text_buffer.skip(len(value))
+            self.text_buffer.skip(len(value))
 
     def _error(self, message=None):
         error = MauLexerError(
             message=message,
             details={
                 "context": self._context,
             },
@@ -175,15 +180,15 @@
         ]
 
         self._nextline()
 
         return tokens
 
     def _process_eof(self):
-        if self._text_buffer.eof:
+        if self.text_buffer.eof:
             return [self._create_token(TokenTypes.EOF)]
 
         return None
 
     def _process_eol(self):
         # This cannot use TextBuffer.eol as we want to eat any spaces
         # that are present in the line.
```

### Comparing `mau-3.1.0/mau/lexers/main_lexer.py` & `mau-4.0.0/mau/lexers/main_lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 
 
 class TokenTypes:
     ARGUMENTS = "ARGUMENTS"
     BLOCK = "BLOCK"
     COMMAND = "COMMAND"
     COMMENT = "COMMENT"
+    CONTENT = "CONTENT"
+    CONTROL = "CONTROL"
     HEADER = "HEADER"
     HORIZONTAL_RULE = "HORIZONTAL_RULE"
-    INCLUDE = "INCLUDE"
     LIST = "LIST"
     MULTILINE_COMMENT = "MULTILINE_COMMENT"
     TITLE = "TITLE"
     VARIABLE = "VARIABLE"
 
 
 class MainLexer(BaseLexer):
     def _process_functions(self):
         return [
             self._process_multiline_comment,
             self._process_comment,
             self._process_horizontal_rule,
             self._process_block,
             self._process_command_or_directive,
+            self._process_control,
             self._process_include,
             self._process_variable,
             self._process_arguments,
             self._process_title,
             self._process_list,
             self._process_header,
             # This is provided by BaseLexer
@@ -77,20 +79,21 @@
 
         return self._create_tokens_from_line(TokenTypes.BLOCK)
 
     def _run_directive(self, name, value):
         if name == "include":
             with open(value, encoding="utf-8") as included_file:
                 text = included_file.read()
-                text_buffer = self._text_buffer.__class__(text, Context(source=value))
+                text_buffer = self.text_buffer.__class__(text, Context(source=value))
 
-                lexer = MainLexer(text_buffer)
-                lexer.process()
+                lexer = MainLexer(self.environment)
+                lexer.process(text_buffer)
 
-                self.tokens.extend(lexer.tokens)
+                # Remove the last token as it is an EOF
+                self.tokens.extend(lexer.tokens[:-1])
 
     def _process_command_or_directive(self):
         match = rematch(r"::([a-z0-9_#]+):(.*)?", self._current_line)
 
         if not match:
             return None
 
@@ -117,24 +120,46 @@
 
         tokens.append(self._create_token(BLTokenTypes.EOL))
 
         self._nextline()
 
         return tokens
 
+    def _process_control(self):
+        match = rematch(r"@([^:]+):(.*)", self._current_line)
+
+        if not match:
+            return None
+
+        operator = match.group(1)
+        statement = match.group(2)
+
+        tokens = [
+            self._create_token_and_skip(TokenTypes.CONTROL, "@"),
+            self._create_token_and_skip(BLTokenTypes.TEXT, operator),
+            self._create_token_and_skip(BLTokenTypes.LITERAL, ":"),
+            self._create_token_and_skip(BLTokenTypes.TEXT, statement),
+        ]
+
+        tokens.append(self._create_token(BLTokenTypes.EOL))
+
+        self._nextline()
+
+        return tokens
+
     def _process_include(self):
-        match = rematch(r"^<<( *)([a-z0-9_#\\]+):(.*)?", self._current_line)
+        match = rematch(r"^<<( *)([a-z0-9_#\\\.]+):(.*)?", self._current_line)
 
         if not match:
             return None
 
         if not match.group(2):  # pragma: no cover
             return None
 
-        tokens = [self._create_token_and_skip(TokenTypes.INCLUDE, "<<")]
+        tokens = [self._create_token_and_skip(TokenTypes.CONTENT, "<<")]
 
         if match.group(1):
             tokens.append(
                 self._create_token_and_skip(BLTokenTypes.WHITESPACE, match.group(1))
             )
 
         tokens.extend(
@@ -155,15 +180,15 @@
 
         return tokens
 
     def _process_variable(self):
         if not self._current_line.startswith(":"):
             return None
 
-        match = rematch(r":([!a-zA-Z0-9\-_\.]+):(.*)?", self._current_line)
+        match = rematch(r":([a-zA-Z0-9_\.\+\-]+):(.*)?", self._current_line)
 
         if not match:  # pragma: no cover
             return None
 
         tokens = [
             self._create_token_and_skip(TokenTypes.VARIABLE, ":"),
             self._create_token_and_skip(BLTokenTypes.TEXT, match.group(1)),
```

### Comparing `mau-3.1.0/mau/lexers/preprocess_variables_lexer.py` & `mau-4.0.0/mau/lexers/preprocess_variables_lexer.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/mau/lexers/text_lexer.py` & `mau-4.0.0/mau/lexers/text_lexer.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
         if not match:
             return None
 
         return [self._create_token_and_skip(TokenTypes.TEXT, " ")]
 
     def _process_literal(self):
-        if self._current_char not in '~^_*`{}()[]\\"':
+        if self._current_char not in '~^_*`{}()[]\\"$%':
             return None
 
         return [self._create_token_and_skip(TokenTypes.LITERAL, self._current_char)]
 
     def _process_text(self):
-        match = rematch(r'[^~\^_*`{}()[\]"\\ ]+', self._tail)
+        match = rematch(r'[^~\^_*`{}()[\]"\\ \$%]+', self._tail)
 
         if not match:  # pragma: no cover
             return None
 
         return [self._create_token_and_skip(TokenTypes.TEXT, match.group())]
 
     def _process_functions(self):
```

### Comparing `mau-3.1.0/mau/main.py` & `mau-4.0.0/mau/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import argparse
 import logging
 import sys
 from importlib import metadata
 
 import yaml
 from mau import ConfigurationError, Mau, load_visitors
+from mau.environment.environment import Environment
 from mau.errors import MauErrorException, print_error
+from mau.nodes.page import DocumentNode
 from tabulate import tabulate
 
 __version__ = metadata.version("mau")
-_logger = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 visitor_classes = load_visitors()
 visitors = {i.format_code: i for i in visitor_classes}
 
 
 def parse_args():
     parser = argparse.ArgumentParser()
@@ -77,14 +79,21 @@
         "--parse-only",
         dest="parseonly",
         help="performs only parsing and prints nodes",
         action="store_true",
     )
 
     parser.add_argument(
+        "--profile",
+        dest="profile",
+        help="runs the profiler",
+        action="store_true",
+    )
+
+    parser.add_argument(
         "--version", action="version", version=f"Mau version {__version__}"
     )
 
     return parser.parse_args()
 
 
 def setup_logging(loglevel):
@@ -122,67 +131,83 @@
 
     # Load the YAML configuration file into a dictionary
     config = {}
     if args.config_file:
         with open(args.config_file, "r", encoding="utf-8") as config_file:
             config = yaml.load(config_file, Loader=yaml.FullLoader)
 
-    # The directory that contains custom templates.
-    templates_directory = config.get("templates_directory", None)
+    environment = Environment(config)
 
     # Select the visitor class according to the target
     # format specified on the command line
+    # This is always successful as the list of arguments
+    # is generated fromthe list of plugins
     visitor_class = visitors[args.format]
-
-    # This extracts the custom templates defined
-    # in the config file
-    custom_templates = config.get("custom_templates", None)
+    environment.setvar("mau.visitor.class", visitor_class)
+    environment.setvar("mau.visitor.format", args.format)
 
     # Find out the name of the output file
     output_file = args.output_file or args.input_file.replace(
         ".mau", visitor_class.extension
     )
 
+    # Wrap the content with a DocumentNode
+    # so that the output can be rendered as
+    # a stand-alone document
+    environment.setvar("mau.parser.content_wrapper", DocumentNode())
+
     # The Mau object configured with what we figured out above.
     mau = Mau(
         args.input_file,
-        visitor_class=visitor_class,
-        config=config,
-        custom_templates=custom_templates,
-        templates_directory=templates_directory,
-        full_document=True,
+        environment=environment,
     )
 
+    if args.profile:
+        import cProfile
+        import pstats
+
+        profiler = cProfile.Profile()
+        profiler.enable()
+
     # Run the lexer on the input data
     try:
-        lexer = mau.run_lexer(text)
+        logger.info(f"* Lexing {args.input_file}")
+        mau.run_lexer(text)
 
         if args.lexonly:
             write_output(
                 tabulate(
-                    [(t.type, t.value, t.context) for t in lexer.tokens],
+                    [(t.type, t.value, t.context) for t in mau.lexer.tokens],
                     maxcolwidths=[10, 60, 30],
                 ),
                 output_file,
             )
 
             sys.exit(1)
 
-        parser = mau.run_parser(lexer.tokens)
+        logger.info(f"* Parsing {args.input_file}")
+        mau.run_parser(mau.lexer.tokens)
 
         if args.parseonly:
-            write_output(parser.nodes, output_file)
+            output = "\n".join([str(node) for node in mau.parser.nodes])
+            write_output(output, output_file)
 
             sys.exit(1)
 
-        output = mau.process(parser.nodes, parser.environment)
+        logger.info(f"* Rendering {args.input_file}")
+        output = mau.run_visitor(mau.parser.output["content"])
 
     except ConfigurationError as exception:
         print(f"Configuration error: {exception}")
         sys.exit(1)
     except MauErrorException as exception:
         print_error(exception.error)
         sys.exit(1)
-    except Exception as exception:  # pylint: disable=broad-exception-caught
+    except Exception:  # pylint: disable=broad-exception-caught,try-except-raise
         raise
 
     write_output(output, output_file, transform=visitor_class.transform)
+
+    if args.profile:
+        profiler.disable()
+        stats = pstats.Stats(profiler).sort_stats("cumtime")
+        stats.print_stats(0.1)
```

### Comparing `mau-3.1.0/mau/nodes/source.py` & `mau-4.0.0/mau/nodes/source.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,83 @@
 from mau.nodes.nodes import Node
-from mau.nodes.page import PageNode
 
 
 class CalloutsEntryNode(Node):
     # This is an entry in the list of callouts after source code
 
     node_type = "callouts_entry"
 
-    def __init__(self, marker, value):
-        super().__init__()
+    def __init__(
+        self,
+        marker,
+        value,
+        parent=None,
+        parent_position=None,
+        children=None,
+        subtype=None,
+        args=None,
+        kwargs=None,
+        tags=None,
+    ):
+        super().__init__(
+            parent=parent,
+            parent_position=parent_position,
+            children=children,
+            subtype=subtype,
+            args=args,
+            kwargs=kwargs,
+            tags=tags,
+        )
         self.marker = marker
         self.value = value
 
-    @property
-    def _content(self):
+    def _custom_dict(self):
         return {
-            "type": self.node_type,
-            "marker": self.marker,
             "value": self.value,
+            "marker": self.marker,
         }
 
 
 class CalloutNode(Node):
     # This is a marker near a source code line
 
     node_type = "callout"
 
-    def __init__(self, line, marker):
-        super().__init__()
+    def __init__(
+        self,
+        line,
+        marker,
+        parent=None,
+        parent_position=None,
+        children=None,
+        subtype=None,
+        args=None,
+        kwargs=None,
+        tags=None,
+    ):
+        super().__init__(
+            parent=parent,
+            parent_position=parent_position,
+            children=children,
+            subtype=subtype,
+            args=args,
+            kwargs=kwargs,
+            tags=tags,
+        )
         self.line = line
         self.marker = marker
 
-    @property
-    def _content(self):
+    def _custom_dict(self):
         return {
-            "type": self.node_type,
             "line": self.line,
             "marker": self.marker,
         }
 
 
-class SourceNode(PageNode):
+class SourceNode(Node):
     """A block of verbatim text or source code.
 
     This node contains verbatim text or source code.
 
     Arguments:
         language: the language of the code contained in this block
         callouts: a list of callout CalloutEntryNode objects
@@ -56,51 +89,55 @@
         kwargs: named arguments
     """
 
     node_type = "source"
 
     def __init__(
         self,
-        blocktype="default",
         code=None,
         language="text",
         callouts=None,
         delimiter=":",
         markers=None,
         highlights=None,
         classes=None,
         title=None,
         preprocessor=None,
+        parent=None,
+        parent_position=None,
+        children=None,
+        subtype=None,
         args=None,
         kwargs=None,
         tags=None,
     ):
-        super().__init__(args, kwargs, tags)
-        self.blocktype = blocktype
+        super().__init__(
+            parent=parent,
+            parent_position=parent_position,
+            children=children,
+            subtype=subtype,
+            args=args,
+            kwargs=kwargs,
+            tags=tags,
+        )
         self.code = code or []
         self.language = language
         self.callouts = callouts or []
-        self.markers = markers or []
         self.delimiter = delimiter
+        self.markers = markers or []
         self.highlights = highlights or []
         self.classes = classes or []
         self.title = title
         self.preprocessor = preprocessor
 
-    @property
-    def _content(self):
+    def _custom_dict(self):
         return {
-            "type": self.node_type,
-            "blocktype": self.blocktype,
             "code": self.code,
             "language": self.language,
             "callouts": self.callouts,
-            "markers": self.markers,
             "delimiter": self.delimiter,
+            "markers": self.markers,
             "highlights": self.highlights,
             "classes": self.classes,
             "title": self.title,
             "preprocessor": self.preprocessor,
-            "args": self.args,
-            "kwargs": self.kwargs,
-            "tags": self.tags,
         }
```

### Comparing `mau-3.1.0/mau/nodes/toc.py` & `mau-4.0.0/mau/nodes/toc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-from mau.nodes.page import PageNode
+from mau.nodes.nodes import Node
 
 
-class TocNode(PageNode):
-    """A Table of Contents.
-
-    This node contains the entries of the Table of Contents.
-    """
-
-    node_type = "toc"
-
-    def __init__(self, entries, args=None, kwargs=None, tags=None):
-        super().__init__(args, kwargs, tags)
-        self.entries = entries
-
-    @property
-    def _content(self):
-        return {
-            "type": self.node_type,
-            "entries": self.entries,
-            "args": self.args,
-            "kwargs": self.kwargs,
-            "tags": self.tags,
-        }
-
-
-class TocEntryNode(PageNode):
+class TocEntryNode(Node):
     """An entry of the Table of Contents.
 
     This node contains an entry of the Table of Contents.
     """
 
     node_type = "toc_entry"
 
-    def __init__(self, value, anchor, children=None, args=None, kwargs=None, tags=None):
-        super().__init__(args, kwargs, tags)
+    def __init__(
+        self,
+        value=None,
+        anchor=None,
+        parent=None,
+        parent_position=None,
+        children=None,
+        subtype=None,
+        args=None,
+        kwargs=None,
+        tags=None,
+    ):
+        super().__init__(
+            parent=parent,
+            parent_position=parent_position,
+            children=children,
+            subtype=subtype,
+            args=args,
+            kwargs=kwargs,
+            tags=tags,
+        )
         self.value = value
         self.anchor = anchor
-        self.children = children or []
 
-    @property
-    def _content(self):
+    def _custom_dict(self):
         return {
-            "type": self.node_type,
             "value": self.value,
             "anchor": self.anchor,
-            "children": self.children,
-            "args": self.args,
-            "kwargs": self.kwargs,
-            "tags": self.tags,
         }
+
+
+class TocNode(Node):
+    """A Table of Contents command.
+
+    This node contains the headers that go into the ToC.
+    """
+
+    node_type = "toc"
```

### Comparing `mau-3.1.0/mau/parsers/arguments.py` & `mau-4.0.0/mau/parsers/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     """
 
     if default_values is not None:
         _default_values = default_values.copy()
     else:
         _default_values = {}
 
+    # If a named argument provides the value for a
+    # positional name we consider it set
+    positional_names = [i for i in positional_names if i not in kwargs]
+
     # If we pass more positional values than names,
     # some of them won't be converted and become flags
     remaining_args = args[len(positional_names) :]
 
     positional_arguments = dict(zip(positional_names, args))
 
     # Named arguments win over the defaults
```

### Comparing `mau-3.1.0/mau/parsers/arguments_parser.py` & `mau-4.0.0/mau/parsers/arguments_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from mau.parsers.base_parser import BaseParser
 from mau.tokens.tokens import Token
 
 
 class ArgumentsParser(BaseParser):
     lexer_class = ArgumentsLexer
 
-    def __init__(self, tokens):
-        super().__init__(tokens)
+    def __init__(self, environment):
+        super().__init__(environment)
 
         # This flag is turned on as soon as
         # a named argument is parsed
         self._named_arguments = False
 
     def _process_functions(self):
         return [
@@ -101,14 +101,25 @@
             for node in self.nodes
             if node.node_type == "named_argument"
         }
 
         # Isolate tags
         tags = [i for i in args if i.startswith("#")]
 
-        # Isolate non-tags
-        args = [i for i in args if i not in tags]
+        # Isolate subtypes
+        subtypes = [i for i in args if i.startswith("*")]
+
+        if len(subtypes) == 0:
+            subtype = None
+        if len(subtypes) == 1:
+            # Get the first subtype and remove the leading "*"
+            subtype = subtypes[0][1:]
+        if len(subtypes) > 1:
+            self._error("Multiple subtypes detected")
+
+        # Keep normal args
+        args = [i for i in args if i not in tags + subtypes]
 
         # Remove the "#" from tags
         tags = [i[1:] for i in tags]
 
-        return args, kwargs, tags
+        return args, kwargs, tags, subtype
```

### Comparing `mau-3.1.0/mau/parsers/base_parser.py` & `mau-4.0.0/mau/parsers/base_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,41 +29,55 @@
         print_context(context)
 
 
 class BaseParser:
     text_buffer_class = TextBuffer
     lexer_class = BaseLexer
 
-    def __init__(self, tokens):
+    def __init__(self, environment, parent_node=None, parent_position=None):
         # This is the position of the current token.
         self.index = -1
 
         # These are the tokens parsed by the parser.
-        self.tokens = tokens
+        self.tokens = None
 
         # A stack for the parser's state.
         # Currently the state is represented only
         # by the current index in the input tokens.
         self._stack = []
 
         # These are the nodes created by the parsing.
         self.nodes = []
 
         # The last processed token. Used to detect loops.
         self.last_processed_token = Token(TokenTypes.EOF)
 
+        # The configuration environment
+        self.environment = environment
+
+        # This is the parent node of all the nodes
+        # created by this parser
+        self.parent_node = parent_node
+
+        # This is the position of all the nodes
+        # in the parent
+        self.parent_position = parent_position
+
     @property
     def _current_token(self):
         """
         Returns the token being parsed.
         We often need to know which token we are currently
         parsing, but we might already have parsed all
         of them, so this convenience method wraps the
         possible index error.
         """
+        if not self.tokens:
+            return None
+
         if self.index < 0:
             return self.tokens[-1]
 
         try:
             return self.tokens[self.index]
         except IndexError:
             return self.tokens[-1]
@@ -121,14 +135,20 @@
         # At this point we know that there was
         # an exception but we can ignore it as
         # it is one of the expected ones
         return True
 
     def _save(self, node):
         # Store the node.
+        node.parent = self.parent_node
+
+        self.nodes.append(node)
+
+    def save(self, node):
+        # Store the node.
         self.nodes.append(node)
 
     def _check_token(
         self,
         token,
         ttype=None,
         tvalue=None,
@@ -159,18 +179,22 @@
         return token
 
     def _process_functions(self):
         # The parse functions available in this parser
         return []
 
     def _error(self, message=None):
+        context = None
+        if self._current_token:
+            context = self._current_token.context
+
         error = MauParserError(
             message=message,
             details={
-                "context": self._current_token.context,
+                "context": context,
             },
         )
 
         raise MauErrorException(error)
 
     def _put_token(self, token):
         self.tokens.insert(self.index + 1, token)
@@ -296,19 +320,21 @@
         try:
             return set_names_and_defaults(
                 args, kwargs, positional_names, default_values
             )
         except ValueError as exception:
             self._error(str(exception))
 
-    def parse(self):
+    def parse(self, tokens):
         """
         Run the parser on the lexed tokens.
         """
 
+        self.tokens = tokens
+
         # A loop on all lexed tokens until we reach EOF
         while not self._peek_token_is(TokenTypes.EOF):
             # This detects infinite loops created by incomplete
             # parsing functions. Those functions keep trying
             # to parse the same token, so if we spot that
             # we are doing it we should raise an error.
             next_token = self._peek_token()
@@ -341,17 +367,20 @@
             # If we get here and result is still False
             # we didn't find any function to parse the
             # current token.
             if result is False:
                 self._error("Cannot parse token")
 
     @classmethod
-    def analyse(cls, text, context, *args, **kwargs):
+    def analyse(cls, text, context, environment, *args, **kwargs):
         text_buffer = cls.text_buffer_class(text, context)
 
-        lex = cls.lexer_class(text_buffer)
-        lex.process()
+        lex = cls.lexer_class(environment)
+        lex.process(text_buffer)
 
-        par = cls(lex.tokens, *args, **kwargs)
-        par.parse()
+        par = cls(environment, *args, **kwargs)
+        par.parse(lex.tokens)
 
         return par
+
+    def finalise(self):
+        pass
```

### Comparing `mau-3.1.0/mau/parsers/main_parser.py` & `mau-4.0.0/mau/parsers/main_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,290 +1,199 @@
 # pylint: disable=too-many-lines
 
-import hashlib
-import re
-
+from mau.environment.environment import Environment
 from mau.lexers.base_lexer import TokenTypes as BLTokenTypes
 from mau.lexers.main_lexer import MainLexer
 from mau.lexers.main_lexer import TokenTypes as MLTokenTypes
-from mau.nodes.footnotes import CommandFootnotesNode, FootnotesEntryNode
-from mau.nodes.inline import ListItemNode, RawNode, TextNode
-from mau.nodes.page import (
-    BlockNode,
-    CommandTocNode,
-    ContentImageNode,
-    ContentNode,
-    HeaderNode,
-    HorizontalRuleNode,
-    ListNode,
-    ParagraphNode,
-)
-from mau.nodes.references import CommandReferencesNode, ReferencesEntryNode
+from mau.nodes.block import BlockGroupNode, BlockNode
+from mau.nodes.content import ContentImageNode, ContentNode
+from mau.nodes.header import HeaderNode
+from mau.nodes.inline import RawNode, SentenceNode
+from mau.nodes.lists import ListItemNode, ListNode
+from mau.nodes.page import ContainerNode, HorizontalRuleNode
+from mau.nodes.paragraph import ParagraphNode
 from mau.nodes.source import CalloutNode, CalloutsEntryNode, SourceNode
 from mau.parsers.arguments_parser import ArgumentsParser
+from mau.parsers.attributes import AttributesManager
 from mau.parsers.base_parser import BaseParser
-from mau.parsers.environment import Environment
+from mau.parsers.footnotes import FootnotesManager
+from mau.parsers.internal_links import InternalLinksManager
 from mau.parsers.preprocess_variables_parser import PreprocessVariablesParser
 from mau.parsers.text_parser import TextParser
+from mau.parsers.toc import TocManager, header_anchor
 from mau.tokens.tokens import Token
 
 
-def header_anchor(text, level):
-    """
-    Return a sanitised anchor for a header.
-    """
-
-    # Everything lowercase
-    sanitised_text = text.lower()
-
-    # Get only letters, numbers, dashes, spaces, and dots
-    sanitised_text = "".join(re.findall("[a-z0-9-\\. ]+", sanitised_text))
-
-    # Remove multiple spaces
-    sanitised_text = "-".join(sanitised_text.split())
-
-    hashed_value = hashlib.md5(f"{level} {text}".encode("utf-8")).hexdigest()[:4]
-
-    return f"{sanitised_text}-{hashed_value}"
-
-
-def footnote_anchor(content):
-    return hashlib.md5(str(content).encode("utf-8")).hexdigest()[:8]
-
-
-def reference_anchor(content):
-    return hashlib.md5(str(content).encode("utf-8")).hexdigest()[:8]
-
-
 # The MainParser is in charge of parsing
 # the whole input, calling other parsers
 # to manage single paragraphs or other
 # things like variables.
 class MainParser(BaseParser):
     lexer_class = MainLexer
 
-    def __init__(
-        self, tokens, environment=None, references=None, reference_entries=None
-    ):
-        super().__init__(tokens)
-
-        self.environment = environment or Environment()
-
-        self.headers = []
+    def __init__(self, environment, parent_node=None, parent_position=None):
+        super().__init__(environment, parent_node, parent_position)
 
-        # This dictionary containes the footnotes created
-        # in the text through a macro.
-        self.footnotes = {}
-
-        # This dictionary contains the content of each
-        # footnote created through blocks.
-        # This is a helper dictionary that will be merged
-        # with self.footnotes once the parsing is completed.
-        self.footnotes_data = {}
-
-        # This list contains all the footnote entries
-        # that will be shown by a footnotes command.
-        self.footnote_entries = []
-
-        # This dictionary containes the references created
-        # in the text through a macro.
-        self.reference_mentions = {}
-
-        # This dictionary contains the content of each
-        # reference created through blocks.
-        self.reference_data = {}
-
-        # This list contains all the references contained
-        # in this parser in the form
-        # {content_type:[references]}.
-        self.references = references if references is not None else {}
-
-        # This list contains all the reference entries
-        # that will be shown by a references command in the form
-        # {content_type:[references]}.
-        # This is a copy of self.references that however
-        # contains ReferencesEntryNode nodes.
-        self.reference_entries = (
-            reference_entries if reference_entries is not None else {}
-        )
-
-        # When we define a block we establish an alias
-        # {alias:actual_block_name}.
-        self.block_aliases = {}
-
-        # Each block we define can have default values
-        # {actual_block_name:kwargs}.
-        self.block_defaults = {}
-
-        # Each block we define can have names for unnamed arguments
-        # {actual_block_name:kwargs}.
-        self.block_names = {}
-
-        # This establishes a default block definition so that
-        # [source] = [source, engine=source]
-        # This definition can be overridden by custom block definitions.
-        self.block_aliases["source"] = "default"
-        self.block_defaults["source"] = {"engine": "source", "language": "text"}
-        self.block_names["source"] = ["language"]
-
-        self.block_aliases["footnote"] = "default"
-        self.block_defaults["footnote"] = {"engine": "footnote"}
-        self.block_names["footnote"] = ["name"]
-
-        self.block_aliases["reference"] = "default"
-        self.block_defaults["reference"] = {"engine": "reference"}
-        self.block_names["reference"] = ["type", "name"]
-
-        self.block_aliases["admonition"] = "admonition"
-        self.block_names["admonition"] = ["class", "icon", "label"]
+        self.internal_links_manager = InternalLinksManager(self)
+        self.footnotes_manager = FootnotesManager(self)
+        self.toc_manager = TocManager(self)
+        self.attributes_manager = AttributesManager(self)
+
+        # These are the default block aliases
+        # If subtype is not set it will be the alias itself.
+        self.block_aliases = {
+            "source": {
+                "subtype": None,
+                "mandatory_args": ["language"],
+                "defaults": {"engine": "source", "language": "text"},
+            },
+            "footnote": {
+                "subtype": None,
+                "mandatory_args": ["name"],
+                "defaults": {"engine": "footnote"},
+            },
+            "admonition": {
+                "mandatory_args": ["class", "icon"],
+            },
+        }
 
         # Iterate through block definitions passed as variables
-        # for alias, block_definition in (
-        #     self.variables["mau"].get("block_definitions", {}).items()
-        # ):
-        #     try:
-        #         blocktype = block_definition["blocktype"]
-        #         self.block_aliases[alias] = blocktype
-        #     except KeyError:
-        #         raise ConfigurationError(
-        #             f"Block definition '{alias}' is missing key 'blocktype'"
-        #         )
-
-        #     try:
-        #         self.block_defaults[blocktype] = block_definition["kwargs"]
-        #     except KeyError:
-        #         raise ConfigurationError(
-        #             f"Block definition '{alias}' is missing key 'kwargs'"
-        #         )
+        self.block_aliases.update(
+            self.environment.getvar(
+                "mau.parser.block_definitions", Environment()
+            ).asdict()
+        )
 
         # This is a buffer for a block title
-        self._title = None
+        self.title = (None, None)
+
+        # This is a buffer for a control
+        self.control = (None, None, None)
 
         # This is the function used to create the header
-        # anchors. It can be specified through
-        # mau.header_anchor_function to override
-        # the default one.
+        # anchors.
         self.header_anchor = self.environment.getvar(
-            "mau.header_anchor_function", header_anchor
+            "mau.parser.header_anchor_function", header_anchor
         )
 
-        # A temporary space to store parsed arguments
-        # The tuple represents (args, kwargs, tags)
-        self.arguments = ([], {}, [])
-
-    def create_footnotes(self):
-        for num, footnote in enumerate(self.footnotes.values(), start=1):
-            footnote.number = num
-
-        for key, footnote in self.footnotes.items():
-            data = self.footnotes_data[key]
-            footnote.content = data["content"]
-            anchor = footnote_anchor(footnote.content)
-
-            footnote.reference_anchor = f"fr-{anchor}-{footnote.number}"
-            footnote.content_anchor = f"fd-{anchor}-{footnote.number}"
-
-            self.footnote_entries.append(
-                FootnotesEntryNode(
-                    content=footnote.content,
-                    number=footnote.number,
-                    reference_anchor=footnote.reference_anchor,
-                    content_anchor=footnote.content_anchor,
-                )
-            )
-
-    def process_references(self):
-        # Example of stored content
-        # self.references = {
-        #  (type1, name1) = node1
-        #  (type1, name2) = node2
-        #  (type2, name3) = node3
-        # }
-        #
-        # self.reference_data = {
-        #  (type1, name1) = content
-        #  (type1, name2) = content
-        #  (type2, name3) = content
-        # }
-
-        content_types = {i[0] for i in self.reference_data}
-        content_types_num = {}
-
-        for content_type in content_types:
-            content_types_num[content_type] = 1
-
-        for key, value in self.reference_mentions.items():
-            data = self.reference_data[key]
-            content_type = value.content_type
-
-            value.content = data["content"]
-            value.title = data["title"]
-            anchor = reference_anchor(value.content)
-
-            value.number = content_types_num[content_type]
-            content_types_num[content_type] += 1
-
-            value.reference_anchor = f"ref-{content_type}-{value.number}-{anchor}"
-            value.content_anchor = f"cnt-{content_type}-{value.number}-{anchor}"
-
-            self.references[key] = value
-            self.reference_entries[key] = ReferencesEntryNode(
-                content_type=value.content_type,
-                name=value.name,
-                category=value.category,
-                content=value.content,
-                number=value.number,
-                title=value.title,
-                reference_anchor=value.reference_anchor,
-                content_anchor=value.content_anchor,
-            )
-
-    def _pop_arguments(self):
-        # This return the arguments and resets the
-        # cached ones.
-        args, kwargs, tags = self.arguments
-        self.arguments = ([], {}, [])
+        # The last index in the latest ordered list,
+        # used to calculate the beginning value of them
+        # next one when start=auto
+        self.latest_ordered_list_index = 0
+
+        # This is the dictionary of block groups
+        # defineed in the document
+        self.grouped_blocks = {}
 
-        return args, kwargs, tags
-
-    def _push_arguments(self, args, kwargs, tags):
-        self.arguments = (args, kwargs, tags)
+        # This is the final output of the parser
+        self.output = {}
 
     def _process_functions(self):
         # All the functions that this parser provides.
 
         return [
             self._process_eol,
             self._process_horizontal_rule,
             self._process_single_line_comment,
             self._process_multi_line_comment,
             self._parse_variable_definition,
             self._process_command,
             self._process_title,
+            self._process_control,
             self._process_arguments,
             self._process_header,
             self._process_block,
-            self._process_include_content,
+            self._process_content,
             self._process_list,
             self._process_paragraph,
         ]
 
-    def _pop_title(self):
+    def _push_title(self, text, context):
+        # When we parse a title we can store it here
+        # so that it is available to the next block
+        # that will use it.
+        self.title = (text, context)
+
+    def _pop_title(self, node):
         # This return the title and resets the
         # cached one, so no other block will
         # use it.
-        title = self._title
-        self._title = None
-        return title
+        text, context = self.title
+        self._reset_title()
 
-    def _push_title(self, title):
-        # When we parse a title we can store it here
-        # so that it is available to the next block
-        # that will use it.
-        self._title = title
+        if text is None:
+            return None
+
+        text_parser = TextParser.analyse(
+            text,
+            context,
+            self.environment,
+            parent_node=node,
+            parent_position="title",
+        )
+
+        return SentenceNode(
+            parent=node,
+            parent_position="title",
+            children=text_parser.nodes,
+        )
+
+    def _reset_title(self):
+        self.title = (None, None)
+
+    def _push_control(self, operator, statement, context):
+        self.control = (operator, statement, context)
+
+    def _pop_control(self):
+        # This return the title and resets the
+        # cached one, so no other block will
+        # use it.
+        operator, statement, context = self.control
+        self._reset_control()
+
+        if operator is None:
+            return True
+
+        if operator != "if":
+            self._error(f"Control operator '{operator}' is not supported")
+
+        try:
+            variable, test = statement.split(":", 1)
+        except ValueError:
+            self._error(f"Statement '{statement}' is not in the form variable:test")
+
+        variable_value = self.environment.getvar(variable, None)
+
+        if variable_value is None:
+            self._error(f"Variable '{variable}' has not been defined")
+
+        if test.startswith("="):
+            value = test[1:]
+            return variable_value == value
+
+        if test.startswith("!="):
+            value = test[2:]
+
+            return variable_value != value
+
+        if test.startswith("&"):
+            value = test[1:]
+
+            if value not in ["true", "false"]:
+                self._error(f"Boolean value '{value}' is invalid")
+
+            # pylint: disable=simplifiable-if-expression
+            value = True if value == "true" else False
+
+            return variable_value and value
+
+        self._error(f"Test '{test}' is not supported")
+
+    def _reset_control(self):
+        self.control = (None, None, None)
 
     def _collect_text_content(self):
         # Collects all adjacent text tokens
         # into a single string
 
         if not self._peek_token_is(BLTokenTypes.TEXT):  # pragma: no cover
             return None
@@ -294,15 +203,17 @@
         # Get all tokens
         while self._peek_token_is(BLTokenTypes.TEXT):
             values.append(self._get_token().value)
             self._get_token(BLTokenTypes.EOL)
 
         return " ".join(values)
 
-    def _parse_text_content(self, text, context=None):
+    def _parse_text_content(
+        self, text, parent_node=None, parent_position=None, context=None
+    ):
         # Parse a piece of text using the TextParser.
 
         current_context = context or self._current_token.context
 
         # Replace variables
         preprocess_parser = PreprocessVariablesParser.analyse(
             text,
@@ -311,43 +222,51 @@
         )
         text = preprocess_parser.nodes[0].value
 
         # Parse the text
         text_parser = TextParser.analyse(
             text,
             current_context,
+            self.environment,
+            parent_node=parent_node,
+            parent_position=parent_position,
         )
 
-        # A text parser returns a single sentence node
-        result = text_parser.nodes[0]
-
-        # Store the footnotes
-        self.footnotes.update(text_parser.footnotes)
+        # Extract the footnote mentions
+        # found in this piece of text
+        self.footnotes_manager.update_mentions(text_parser.footnotes)
+
+        # Extract the internal links
+        # found in this piece of text
+        self.internal_links_manager.update_links(text_parser.links)
 
-        # The format of the stored content dictionary is
-        # {(content_type,name): node}
-        self.reference_mentions.update(text_parser.references)
-
-        return result
+        return text_parser.nodes
 
     def _process_eol(self):
         # This simply parses the end of line.
 
         self._get_token(BLTokenTypes.EOL)
 
         return True
 
     def _process_horizontal_rule(self):
         # The horizontal rule ---
 
         self._get_token(MLTokenTypes.HORIZONTAL_RULE)
 
-        args, kwargs, tags = self._pop_arguments()
+        args, kwargs, tags, subtype = self.attributes_manager.pop()
 
-        self._save(HorizontalRuleNode(args, kwargs, tags))
+        self._save(
+            HorizontalRuleNode(
+                subtype=subtype,
+                args=args,
+                kwargs=kwargs,
+                tags=tags,
+            )
+        )
 
         return True
 
     def _process_single_line_comment(self):
         # // A comment on a single line
 
         self._get_token(MLTokenTypes.COMMENT)
@@ -375,172 +294,191 @@
         # and as False booleas as :!name:
         #
         # Variable names can use a namespace with
         # :namespace.name:value
 
         # Get the mandatory variable name
         self._get_token(MLTokenTypes.VARIABLE, ":")
-        variable_name = self._get_token(BLTokenTypes.TEXT).value
+        variable_token = self._get_token(BLTokenTypes.TEXT)
         self._get_token(BLTokenTypes.LITERAL, ":")
 
-        # Assume the variable is a flag
-        variable_value = True
-
-        # If the name starts with ! it's a false flag
-        if variable_name.startswith("!"):
-            variable_value = False
-            variable_name = variable_name[1:]
+        context = variable_token.context
+        variable_name = variable_token.value
 
         # Get the optional value
         value = self._collect_join([Token(BLTokenTypes.EOL)])
 
-        # The value is assigned only if the variable
-        # is not a negative flag. In that case it is ignored
-        if variable_value and len(value) > 0:
-            variable_value = value
+        # If the name starts with "+" it's a true flag
+        # If the name starts with "-" it's a false flag
+        if variable_name.startswith("+"):
+            variable_name = variable_name[1:]
+            value = True
+        elif variable_name.startswith("-"):
+            variable_name = variable_name[1:]
+            value = False
+        else:
+            preprocess_parser = PreprocessVariablesParser.analyse(
+                value,
+                context,
+                self.environment,
+            )
+            value = preprocess_parser.nodes[0].value
 
-        self.environment.setvar(variable_name, variable_value)
+        self.environment.setvar(variable_name, value)
 
         return True
 
     def _process_command(self):
         # Parse a command in the form ::command:arguments
 
         self._get_token(MLTokenTypes.COMMAND, "::")
         name = self._get_token(BLTokenTypes.TEXT).value
         self._get_token(BLTokenTypes.LITERAL, ":")
 
-        args = []
-        kwargs = {}
-        tags = []
+        args, kwargs, tags, subtype = self.attributes_manager.pop()
 
         # Commands can have arguments
-        arguments = ""
+        command_args = []
+        command_kwargs = {}
         with self:
-            arguments = self._get_token(BLTokenTypes.TEXT).value
-
-            current_context = self._current_token.context
+            arguments = self._get_token(BLTokenTypes.TEXT)
 
             arguments_parser = ArgumentsParser.analyse(
-                arguments,
-                current_context,
+                arguments.value, arguments.context, self.environment
             )
 
-            args, kwargs, tags = arguments_parser.process_arguments()
+            (
+                command_args,
+                command_kwargs,
+                _,
+                command_subtype,
+            ) = arguments_parser.process_arguments()
 
         if name == "defblock":
-            # Block definitions must have at least 2 arguments,
-            # the alias and the block type.
-            if len(args) < 2:
-                self._error(
-                    "Block definitions require at least two unnamed arguments: ALIAS and BLOCKTYPE"
-                )
+            if len(command_args) < 1:
+                self._error("Block definitions require at least the alias")
 
-            block_alias = args.pop(0)
-            block_type = args.pop(0)
+            alias = command_args.pop(0)
 
-            self.block_aliases[block_alias] = block_type
-            self.block_defaults[block_alias] = kwargs
-            self.block_names[block_alias] = args
+            self.block_aliases[alias] = {
+                "subtype": command_subtype,
+                "mandatory_args": command_args,
+                "defaults": command_kwargs,
+            }
 
         elif name == "toc":
-            self._save(
-                CommandTocNode(
-                    entries=self.headers, args=args, kwargs=kwargs, tags=tags
-                )
-            )
+            self.toc_manager.create_toc_node(subtype, args, kwargs, tags)
 
         elif name == "footnotes":
-            self._save(
-                CommandFootnotesNode(
-                    entries=self.footnote_entries, args=args, kwargs=kwargs, tags=tags
-                )
-            )
+            # Create a footnotes node
+            self.footnotes_manager.create_node(subtype, args, kwargs, tags)
 
-        elif name == "references":
-            # Assign names
-            args, kwargs = self._set_names_and_defaults(
-                args,
-                kwargs,
-                ["content_type", "category", "name"],
-                {"category": None, "name": None},
+        elif name == "blockgroup":
+            command_args, command_kwargs = self._set_names_and_defaults(
+                command_args,
+                command_kwargs,
+                ["group"],
             )
 
-            content_type = kwargs.pop("content_type")
-            category = kwargs.pop("category")
-            name = kwargs.pop("name")
-
-            self._save(
-                CommandReferencesNode(
-                    entries=self.reference_entries,
-                    content_type=content_type,
-                    name=name,
-                    category=category,
-                    args=args,
-                    kwargs=kwargs,
-                    tags=tags,
+            group_name = command_kwargs.pop("group")
+
+            try:
+                group = self.grouped_blocks.pop(group_name)
+            except KeyError:
+                self._error(
+                    (
+                        f"The group of blocks {group_name} doesn't exist. "
+                        "No blocks belong to that group."
+                    )
                 )
+
+            node = BlockGroupNode(
+                group_name=group_name,
+                group=group,
+                subtype=subtype,
+                args=args,
+                kwargs=kwargs,
+                tags=tags,
             )
 
+            for position, block in group.items():
+                block.parent = node
+                block.parent_position = position
+
+            self.save(node)
+
         return True
 
     def _process_title(self):
         # Parse a title in the form
         #
         # . This is a title
         # or
         # .This is a title
 
         # Parse the mandatory dot
-        self._get_token(MLTokenTypes.TITLE, ".")
+        dot = self._get_token(MLTokenTypes.TITLE, ".")
 
         # Parse the optional white spaces
         with self:
             self._get_token(BLTokenTypes.WHITESPACE)
 
         # Get the text of the title
         text = self._get_token(BLTokenTypes.TEXT).value
         self._get_token(BLTokenTypes.EOL)
 
-        current_context = self._current_token.context
+        self._push_title(text, dot.context)
 
-        # Titles can contain Mau code
-        text_parser = TextParser.analyse(text, current_context)
+        return True
+
+    def _process_control(self):
+        # Parse a control statement in the form
+        #
+        # @operator:control_statement
+
+        # Parse the mandatory @
+        at = self._get_token(MLTokenTypes.CONTROL, "@")
+
+        # Get the operator
+        operator = self._get_token(BLTokenTypes.TEXT).value
+
+        # Discard the :
+        self._get_token(BLTokenTypes.LITERAL, ":")
 
-        title = text_parser.nodes[0]
+        # Get the statement
+        statement = self._get_token(BLTokenTypes.TEXT).value
 
-        self._push_title(title)
+        self._get_token(BLTokenTypes.EOL)
+
+        self._push_control(operator, statement, at.context)
 
         return True
 
     def _process_arguments(self):
         # Parse arguments in the form
         # [unnamed1, unnamed2, ..., named1=value1, name2=value2, ...]
 
         self._get_token(MLTokenTypes.ARGUMENTS, "[")
-        text = self._get_token(BLTokenTypes.TEXT).value
+        text_token = self._get_token(BLTokenTypes.TEXT)
         self._get_token(BLTokenTypes.LITERAL, "]")
 
-        current_context = self._current_token.context
-
         preprocess_parser = PreprocessVariablesParser.analyse(
-            text,
-            current_context,
-            environment=self.environment,
+            text_token.value,
+            text_token.context,
+            self.environment,
         )
         text = preprocess_parser.nodes[0].value
 
         # Parse the text
         arguments_parser = ArgumentsParser.analyse(
-            text,
-            current_context,
+            text, text_token.context, self.environment
         )
 
-        args, kwargs, tags = arguments_parser.process_arguments()
-        self._push_arguments(args, kwargs, tags)
+        args, kwargs, tags, subtype = arguments_parser.process_arguments()
+        self.attributes_manager.push(args, kwargs, tags, subtype)
 
         return True
 
     def _process_header(self):
         # Parse a header in the form
         #
         # = Header
@@ -553,36 +491,63 @@
         # Get all the equal signs
         header = self._get_token(MLTokenTypes.HEADER).value
 
         # Get the mandatory white spaces
         self._get_token(BLTokenTypes.WHITESPACE)
 
         # Get the text of the header and calculate the level
-        text = self._get_token(BLTokenTypes.TEXT).value
+        text_token = self._get_token(BLTokenTypes.TEXT)
         level = len(header)
 
-        # Generate the anchor and append it to the TOC
-        anchor = self.header_anchor(text, level)
+        preprocess_parser = PreprocessVariablesParser.analyse(
+            text_token.value,
+            text_token.context,
+            self.environment,
+        )
+        text = preprocess_parser.nodes[0].value
 
-        # Consume the arguments
-        args, kwargs, tags = self._pop_arguments()
+        # Check the control
+        if self._pop_control() is False:
+            return True
+
+        # Consume the parser arguments
+        args, kwargs, tags, subtype = self.attributes_manager.pop()
+
+        # Create the anchor
+        anchor = kwargs.pop("anchor", self.header_anchor(text, level))
 
-        # Generate the header node
-        header_node = HeaderNode(
-            value=text,
+        node = HeaderNode(
             level=str(level),
             anchor=anchor,
+            subtype=subtype,
             args=args,
-            tags=tags,
             kwargs=kwargs,
+            tags=tags,
         )
 
-        self.headers.append(header_node)
+        # Titles can contain Mau code
+        text_parser = TextParser.analyse(
+            text,
+            text_token.context,
+            self.environment,
+            parent_node=node,
+        )
+        node.value = SentenceNode(
+            parent=node,
+            children=text_parser.nodes,
+        )
 
-        self._save(header_node)
+        # If there is an id store the header
+        # to be processed by internal links
+        if "id" in node.kwargs:
+            self.internal_links_manager.add_header(node.kwargs["id"], node)
+
+        self.toc_manager.add_header_node(node)
+
+        self._save(node)
 
         return True
 
     def _collect_lines(self, stop_tokens):
         # This collects several lines of text in a list
         # until it gets to a line that begins with one
         # of the tokens listed in stop_tokens.
@@ -639,214 +604,187 @@
 
             # Where ["Text", "----"] is considered the secondary content
             # of an empty block.
             self._error(
                 "Detected unclosed block (possibly before this line)"
             )  # pragma: no cover
 
-        # Consume the title
-        title = self._pop_title()
-
-        # Consume the arguments
-        args, kwargs, _ = self._pop_arguments()
-
-        # The first unnamed argument is the block type
-        try:
-            blocktype = args.pop(0)
-        except IndexError:
-            blocktype = "default"
+        # Create the block
+        block = BlockNode(children=content, secondary_children=secondary_content)
 
-        # If there is a block alias for blocktype replace it
-        # otherwise use the blocktype we already have
+        block.title = self._pop_title(block)
 
-        # Retrieve the block names and defaults for the
-        # specific type of block
+        # Consume the arguments
+        args, kwargs, tags, subtype = self.attributes_manager.pop()
 
-        block_names = self.block_names.get(blocktype, [])
-        block_defaults = self.block_defaults.get(blocktype, {})
+        # Check the control
+        if self._pop_control() is False:
+            return True
 
-        # Now replace the alias with the true block type
-        blocktype = self.block_aliases.get(blocktype, blocktype)
+        # If the subtype is an alias process it
+        alias = self.block_aliases.get(subtype, {})
+        block.subtype = alias.get("subtype", subtype)
+        block_names = alias.get("mandatory_args", [])
+        block_defaults = alias.get("defaults", {})
 
-        # Assign names
         args, kwargs = self._set_names_and_defaults(
             args,
             kwargs,
             block_names,
             block_defaults,
         )
 
         # Extract classes and convert them into a list
         classes = []
         if "classes" in kwargs:
             classes = kwargs.pop("classes")
 
             if classes:
                 classes = classes.split(",")
-
-        # Extract condition if present and process it
-        condition = kwargs.pop("condition", None)
-
-        # Run this only if there is a condition on this block
-        if condition is not None:
-            try:
-                # The condition should be either test:variable:value or test:variable:
-                test, variable, value = condition.split(":")
-            except ValueError:
-                self._error(
-                    (
-                        f"Condition {condition} is not in the form"
-                        '"test:variable:value" or "test:variable:'
-                    )
-                )
-
-            # If there is no value use True
-            if len(value) == 0:
-                value = True
-
-            # Check if the variable matches the value and apply the requested test
-            match = self.environment.getvar(variable) == value
-            result = test == "if"
-
-            # If the condition is not satisfied return
-            if match is not result:
-                return True
+        block.classes = classes
 
         # Extract the preprocessor
-        preprocessor = kwargs.pop("preprocessor", "none")
+        block.preprocessor = kwargs.pop("preprocessor", "none")
 
         # Extract the engine
-        engine = kwargs.pop("engine", "default")
-
-        if engine == "source":
-            # Engine "source" extracts the content (source code),
-            # the callouts, and the highlights.
-            # The default language is "text".
-
-            self._parse_source_engine(
-                blocktype, content, secondary_content, title, kwargs
-            )
-
-            return True
-
-        if engine == "footnote":
-            name = kwargs.pop("name")
+        block.engine = kwargs.pop("engine", None)
 
-            current_context = self._current_token.context
+        block.args = args
+        block.kwargs = kwargs
+        block.tags = tags
+
+        if block.engine is None:
+            self._parse_default_engine(block)
+        elif block.engine == "mau":
+            self._parse_mau_engine(block)
+        elif block.engine == "source":
+            self._parse_source_engine(block)
+        elif block.engine == "footnote":
+            self._parse_footnote_engine(block)
+        elif block.engine == "raw":
+            self._parse_raw_engine(block)
+        elif block.engine == "group":
+            self._parse_group_engine(block)
+        else:
+            self._error(f"Engine {block.engine} is not available")
 
-            environment = self.environment
+        return True
 
-            content_parser = MainParser.analyse(
-                "\n".join(content),
-                current_context,
-                environment=environment,
-                references=self.references,
-                reference_entries=self.reference_entries,
-            )
+    def _parse_block_content(self, block):
+        current_context = self._current_token.context
 
-            content = content_parser.nodes
+        content_parser = MainParser.analyse(
+            "\n".join(block.children),
+            current_context,
+            Environment(),
+            parent_node=block,
+            parent_position="primary",
+        )
+        content_parser.finalise()
 
-            self.footnotes_data[name] = {
-                "content": content,
-            }
+        secondary_content_parser = MainParser.analyse(
+            "\n".join(block.secondary_children),
+            current_context,
+            Environment(),
+            parent_node=block,
+            parent_position="secondary",
+        )
+        secondary_content_parser.finalise()
 
-            return True
+        block.children = content_parser.nodes
+        block.secondary_children = secondary_content_parser.nodes
 
-        if engine == "reference":
-            content_type = kwargs["type"]
-            name = kwargs["name"]
-
-            current_context = self._current_token.context
-
-            environment = self.environment
-
-            content_parser = MainParser.analyse(
-                "\n".join(content),
-                current_context,
-                environment=environment,
-                references=self.references,
-                reference_entries=self.reference_entries,
-            )
+    def _parse_block_content_update(self, block):
+        current_context = self._current_token.context
 
-            content = content_parser.nodes
+        content_parser = MainParser.analyse(
+            "\n".join(block.children),
+            current_context,
+            self.environment,
+            parent_node=block,
+            parent_position="primary",
+        )
 
-            self.reference_data[(content_type, name)] = {
-                "content": content,
-                "title": title,
-            }
+        secondary_content_parser = MainParser.analyse(
+            "\n".join(block.secondary_children),
+            current_context,
+            self.environment,
+            parent_node=block,
+            parent_position="secondary",
+        )
 
-            return True
+        block.children = content_parser.nodes
+        block.secondary_children = secondary_content_parser.nodes
 
-        # Create the node parameters according to the engine
-        if engine == "raw":
-            # Engine "raw" doesn't process the content,
-            # so we just pass it untouched in the form of
-            # a RawNode per line.
-            content = [RawNode(line) for line in content]
-            secondary_content = [RawNode(line) for line in secondary_content]
-        elif engine in ["default", "mau"]:
-            # Both engines parse content and secondary content
-            # using a new parser but the default one should merge
-            # headers and footnotes into the current one.
+        # The footnote mentions and definitions
+        # found in this block are part of the
+        # main document. Import them.
+        self.footnotes_manager.update(content_parser.footnotes_manager)
+
+        # The internal links and headers
+        # found in this block are part of the
+        # main document. Import them.
+        self.internal_links_manager.update(content_parser.internal_links_manager)
+
+        self.toc_manager.update(content_parser.toc_manager)
+
+    def _parse_mau_engine(self, block):
+        self._parse_block_content(block)
+        self._save(block)
+
+    def _parse_default_engine(self, block):
+        self._parse_block_content_update(block)
+        self._save(block)
+
+    def _parse_group_engine(self, block):
+        block.args, block.kwargs = self._set_names_and_defaults(
+            block.args,
+            block.kwargs,
+            ["group", "position"],
+        )
 
-            current_context = self._current_token.context
+        group_name = block.kwargs.pop("group")
+        position = block.kwargs.pop("position")
 
-            if engine == "default":
-                environment = self.environment
-            else:
-                environment = Environment()
+        group = self.grouped_blocks.setdefault(group_name, {})
 
-            content_parser = MainParser.analyse(
-                "\n".join(content),
-                current_context,
-                environment=environment,
-                references=self.references,
-                reference_entries=self.reference_entries,
+        if position in group:
+            self._error(
+                f"Block with position {position} already defined in group {group_name}"
             )
 
-            secondary_content_parser = MainParser.analyse(
-                "\n".join(secondary_content),
-                current_context,
-                environment=environment,
-            )
+        group[position] = block
 
-            content = content_parser.nodes
-            secondary_content = secondary_content_parser.nodes
+        self._parse_block_content_update(block)
 
-            if engine == "default":
-                self.footnotes.update(content_parser.footnotes)
-                self.footnotes_data.update(content_parser.footnotes_data)
-                self.headers.extend(content_parser.headers)
-                self.reference_mentions.update(content_parser.reference_mentions)
-                self.reference_data.update(content_parser.reference_data)
-            else:
-                content_parser.create_footnotes()
-                content_parser.process_references()
-        else:
-            self._error(f"Engine {engine} is not available")
-
-        self._save(
-            BlockNode(
-                blocktype=blocktype,
-                content=content,
-                secondary_content=secondary_content,
-                classes=classes,
-                title=title,
-                engine=engine,
-                preprocessor=preprocessor,
-                args=args,
-                kwargs=kwargs,
-            )
+    def _parse_footnote_engine(self, block):
+        # The current block contains footnote data.
+        # Extract the content and store it in
+        # the footnotes manager.
+        name = block.kwargs.pop("name")
+
+        content_parser = MainParser.analyse(
+            "\n".join(block.children),
+            self._current_token.context,
+            self.environment,
+            parent_node=block,
         )
 
-        return True
+        self.footnotes_manager.add_data(name, content_parser.nodes)
+
+    def _parse_raw_engine(self, block):
+        # Engine "raw" doesn't process the content,
+        # so we just pass it untouched in the form of
+        # a RawNode per line.
+        block.children = [RawNode(line) for line in block.children]
+        block.secondary_children = [RawNode(line) for line in block.secondary_children]
 
-    def _parse_source_engine(
-        self, blocktype, content, secondary_content, title, kwargs
-    ):  # pylint: disable=too-many-locals
+        self._save(block)
+
+    def _parse_source_engine(self, block):  # pylint: disable=too-many-locals
         # Parse a source block in the form
         #
         # [source, language, attributes...]
         # ----
         # content
         # ----
         #
@@ -871,37 +809,40 @@
         # [source, language, attributes...]
         # ----
         # content:name:
         # ----
         # <name>: <description>
         #
         # Since Mau uses Pygments, the attribute language
-        # is one of the langauges supported by that tool.
+        # is one of the languages supported by that tool.
 
         # Get the delimiter for callouts (":" by default)
-        delimiter = kwargs.pop("callouts", ":")
+        delimiter = block.kwargs.pop("callouts", ":")
 
         # A list that contains callout markers in
         # the form (linenum,name)
         callout_markers = []
 
         # Get the marker for highlighted lines ("@" by default)
-        highlight_marker = kwargs.pop("highlight", "@")
+        highlight_marker = block.kwargs.pop("highlight", "@")
 
         # A list of highlighted lines
         highlighted_lines = []
 
+        # Get the language
+        language = block.kwargs.pop("language")
+
         # Source blocks preserve anything is inside
 
         # This is a list of all lines that might contain
         # a callout. They will be further processed
         # later to be sure.
         lines_with_callouts = [
             (linenum, line)
-            for linenum, line in enumerate(content)
+            for linenum, line in enumerate(block.children)
             if line.endswith(delimiter)
         ]
 
         # Each line in the previous list is processed
         # and stored if it contains a callout
         for linenum, line in lines_with_callouts:
             # Remove the final delimiter
@@ -912,34 +853,34 @@
                 # It's a trap! There are no separators left
                 continue
 
             # Get the callout and the line
             callout_name = splits[-1]
             line = delimiter.join(splits[:-1])
 
-            content[linenum] = line
+            block.children[linenum] = line
 
             # Check if we want to just highlight the line
             if callout_name == highlight_marker:
                 highlighted_lines.append(linenum)
             else:
                 callout_markers.append(CalloutNode(linenum, callout_name))
 
         # A list of CalloutEntryNode objects that contain the
         # text for each marker
         callout_contents = []
 
         # If there was secondary content it should be formatted
         # with callout names followed by colon and the
         # callout text.
-        for line in secondary_content:
+        for line in block.secondary_children:
             if ":" not in line:
                 self._error(
                     (
-                        "Callout description should be written"
+                        "Callout description should be written "
                         f"as 'name: text'. Missing ':' in '{line}'"
                     )
                 )
 
             name, text = line.split(":")
 
             text = text.strip()
@@ -949,121 +890,125 @@
         # Source blocks must preserve the content literally.
         # However, we need to remove escape characters from directives.
         # Directives are processed by the lexer, so if we want to
         # prevent Mau from interpreting them we have to escape them.
         # Escape characters are preserved by source blocks as anything
         # else, but in this case the character should be removed.
         textlines = []
-        for line in content:
+        for line in block.children:
             if line.startswith(r"\::#"):
                 line = line[1:]
 
             textlines.append(RawNode(line))
 
-        self._save(
-            SourceNode(
-                blocktype=blocktype,
-                code=textlines,
-                language=kwargs["language"],
-                callouts=callout_contents,
-                highlights=highlighted_lines,
-                markers=callout_markers,
-                title=title,
-            )
+        node = SourceNode(
+            code=textlines,
+            language=language,
+            callouts=callout_contents,
+            highlights=highlighted_lines,
+            markers=callout_markers,
+            title=block.title,
+            subtype=block.subtype,
+            args=block.args,
+            kwargs=block.kwargs,
+            tags=block.tags,
         )
 
-    def _process_include_content(self):
-        # Parse include content in the form
+        self._save(node)
+
+    def _process_content(self):
+        # Parse content in the form
         #
-        # << content_type:arguments
+        # << content_type:URI
 
         # Get the mandatory "<<"
-        self._get_token(MLTokenTypes.INCLUDE)
+        self._get_token(MLTokenTypes.CONTENT)
 
         with self:
             self._get_token(BLTokenTypes.WHITESPACE)
 
         # Get the content type
         content_type = self._get_token(BLTokenTypes.TEXT).value
         self._get_token(BLTokenTypes.LITERAL, ":")
 
-        title = self._pop_title()
+        args, kwargs, tags, subtype = self.attributes_manager.pop()
 
-        args = []
-        kwargs = {}
-        tags = []
+        uris = self._get_token(BLTokenTypes.TEXT)
 
-        # Commands can have arguments
-        arguments = ""
         with self:
-            arguments = self._get_token(BLTokenTypes.TEXT).value
-
-            current_context = self._current_token.context
-
             arguments_parser = ArgumentsParser.analyse(
-                arguments,
-                current_context,
+                uris.value, uris.context, self.environment
             )
 
-            args, kwargs, tags = arguments_parser.process_arguments()
+            uris, _, _, _ = arguments_parser.process_arguments()
+
+        # Check the control
+        if self._pop_control() is False:
+            return True
 
         if content_type == "image":
-            return self._parse_content_image(title, args, kwargs, tags)
+            return self._parse_content_image(uris, subtype, args, kwargs, tags)
 
-        return self._parse_standard_content(content_type, title, args, kwargs, tags)
+        return self._parse_standard_content(
+            content_type, uris, subtype, args, kwargs, tags
+        )
 
-    def _parse_content_image(self, title, args, kwargs, tags):
+    def _parse_content_image(self, uris, subtype, args, kwargs, tags):
         # Parse a content image in the form
         #
         # << image:uri,alt_text,classes
         #
         # alt_text is the alternate text to use is the image is not reachable
         # and classes is a comma-separated list of classes
 
         # Consume the arguments
         args, kwargs = self._set_names_and_defaults(
             args,
             kwargs,
-            ["uri", "alt_text", "classes"],
+            ["alt_text", "classes"],
             {"alt_text": None, "classes": None},
         )
 
-        uri = kwargs.pop("uri")
+        uri = uris[0]
         alt_text = kwargs.pop("alt_text")
         classes = kwargs.pop("classes")
 
         if classes:
             classes = classes.split(",")
 
-        self._save(
-            ContentImageNode(
-                uri=uri,
-                alt_text=alt_text,
-                classes=classes,
-                title=title,
-                kwargs=kwargs,
-                tags=tags,
-            )
+        node = ContentImageNode(
+            uri=uri,
+            alt_text=alt_text,
+            classes=classes,
+            subtype=subtype,
+            args=args,
+            kwargs=kwargs,
+            tags=tags,
         )
 
+        node.title = self._pop_title(node)
+        self._save(node)
+
         return True
 
-    def _parse_standard_content(self, content_type, title, args, kwargs, tags):
+    def _parse_standard_content(self, content_type, uris, subtype, args, kwargs, tags):
         # This is the fallback for an unknown content type
 
-        self._save(
-            ContentNode(
-                content_type=content_type,
-                title=title,
-                args=args,
-                kwargs=kwargs,
-                tags=tags,
-            )
+        node = ContentNode(
+            content_type=content_type,
+            uris=uris,
+            subtype=subtype,
+            args=args,
+            kwargs=kwargs,
+            tags=tags,
         )
 
+        node.title = self._pop_title(node)
+        self._save(node)
+
         return True
 
     def _process_list(self):
         # Parse a list.
         # Lists can be ordered (using numbers)
         #
         # * One item
@@ -1095,24 +1040,38 @@
 
         # Ignore initial white spaces
         with self:
             self._get_token(BLTokenTypes.WHITESPACE)
 
         # Get the header and decide if it's a numbered or unnumbered list
         header = self._peek_token(MLTokenTypes.LIST)
-        numbered = header.value[0] == "#"
+        ordered = header.value[0] == "#"
 
-        args, kwargs, tags = self._pop_arguments()
+        args, kwargs, tags, subtype = self.attributes_manager.pop()
 
         # Parse all the following items
         nodes = self._process_list_nodes()
 
+        if (start := kwargs.pop("start", 1)) == "auto":
+            start = self.latest_ordered_list_index
+            self.latest_ordered_list_index += len(nodes)
+        else:
+            start = int(start)
+            self.latest_ordered_list_index = len(nodes) + start
+
         self._save(
             ListNode(
-                numbered, nodes, main_node=True, args=args, kwargs=kwargs, tags=tags
+                ordered=ordered,
+                main_node=True,
+                start=start,
+                children=nodes,
+                subtype=subtype,
+                args=args,
+                kwargs=kwargs,
+                tags=tags,
             )
         )
 
         return True
 
     def _process_list_nodes(self):
         # This parses all items of a list
@@ -1126,29 +1085,34 @@
         self._get_token(BLTokenTypes.WHITESPACE)
 
         # Get the context of the first text token
         context = self._peek_token().context
 
         # Collect and parse the text of the item
         text = self._collect_text_content()
-        content = self._parse_text_content(text, context)
+        content = self._parse_text_content(
+            text,
+            parent_node=self.parent_node,
+            parent_position=self.parent_position,
+            context=context,
+        )
 
         # Compute the level of the item
         level = len(header)
 
         nodes = []
-        nodes.append(ListItemNode(str(level), content))
+        nodes.append(ListItemNode(level=str(level), children=content))
 
         while self._peek_token() not in [
             Token(BLTokenTypes.EOF),
             Token(BLTokenTypes.EOL),
         ]:
-            # This is the SentenceNode inside the last node added to the list
-            # which is used to append potential nested nodes
-            last_node_sentence = nodes[-1].content
+            # This are the nodes inside the last element added to the list
+            # which is used to append potential nested elements
+            last_element_nodes = nodes[-1].children
 
             # Ignore the initial white spaces
             with self:
                 self._get_token(BLTokenTypes.WHITESPACE)
 
             if len(self._peek_token().value) == level:
                 # The new item is on the same level
@@ -1160,25 +1124,32 @@
                 self._get_token(BLTokenTypes.WHITESPACE)
 
                 # Get the context of the first text token
                 context = self._peek_token().context
 
                 # Collect and parse the text of the item
                 text = self._collect_text_content()
-                content = self._parse_text_content(text, context)
+                content = self._parse_text_content(
+                    text,
+                    parent_node=self.parent_node,
+                    parent_position=self.parent_position,
+                    context=context,
+                )
+
+                level = len(header)
 
-                nodes.append(ListItemNode(str(len(header)), content))
+                nodes.append(ListItemNode(level=str(level), children=content))
             elif len(self._peek_token().value) > level:
                 # The new item is on a deeper level
 
                 # Treat the new line as a new list
                 numbered = self._peek_token().value[0] == "#"
                 subnodes = self._process_list_nodes()
 
-                last_node_sentence.content.append(ListNode(numbered, subnodes))
+                last_element_nodes.append(ListNode(ordered=numbered, children=subnodes))
             else:
                 break
 
         return nodes
 
     def _process_paragraph(self):
         # This parses a paragraph.
@@ -1203,16 +1174,71 @@
                     [
                         Token(BLTokenTypes.EOL),
                     ]
                 )
             )
             self._get_token(BLTokenTypes.EOL)
 
+        # Check the control
+        if self._pop_control() is False:
+            return True
+
         text = " ".join(lines)
-        sentence = self._parse_text_content(text, context)
 
         # Consume the arguments
-        args, kwargs, tags = self._pop_arguments()
+        args, kwargs, tags, subtype = self.attributes_manager.pop()
+
+        node = ParagraphNode(
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+            subtype=subtype,
+            args=args,
+            kwargs=kwargs,
+            tags=tags,
+        )
 
-        self._save(ParagraphNode(sentence, args=args, kwargs=kwargs, tags=tags))
+        node.title = self._pop_title(node)
+
+        node.children = self._parse_text_content(
+            text, parent_node=node, context=context
+        )
+
+        self._save(node)
 
         return True
+
+    def finalise(self):
+        super().finalise()
+
+        # This processes all footnotes stored in
+        # the manager merging mentions and data
+        # and updating the nodes that contain
+        # a list of footnotes
+        self.footnotes_manager.process_footnotes()
+
+        # This processes all links stored in
+        # the manager linking them to the
+        # correct headers
+        self.internal_links_manager.process_links()
+
+        # Process ToC
+        toc = self.toc_manager.process_toc()
+
+        # The content wrappers are cloned to avoid
+        # storing the whole parsed document in the
+        # environment.
+        content_wrapper = self.environment.getvar(
+            "mau.parser.content_wrapper", ContainerNode()
+        ).clone()
+        content_wrapper.children = self.nodes
+
+        toc_wrapper = self.environment.getvar(
+            "mau.parser.toc_wrapper", ContainerNode()
+        ).clone()
+        toc_wrapper.add_children([toc])
+
+        self.output.update(
+            {
+                "content": content_wrapper,
+                "toc": toc_wrapper,
+            }
+        )
```

### Comparing `mau-3.1.0/mau/parsers/preprocess_variables_parser.py` & `mau-4.0.0/mau/parsers/preprocess_variables_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from mau.lexers.base_lexer import TokenTypes
 from mau.lexers.preprocess_variables_lexer import PreprocessVariablesLexer
 from mau.nodes.inline import TextNode
 from mau.parsers.base_parser import BaseParser
-from mau.parsers.environment import Environment
 from mau.tokens.tokens import Token
 
 
 class PreprocessVariablesParser(BaseParser):
     lexer_class = PreprocessVariablesLexer
 
-    def __init__(self, tokens, environment=None):
-        super().__init__(tokens)
-
-        self.environment = environment or Environment()
+    def __init__(self, environment):
+        super().__init__(environment)
 
     def _process_verbatim(self):
         self._get_token(TokenTypes.LITERAL, "`")
         text = self._collect_join(
             [Token(TokenTypes.LITERAL, "`")],
             preserve_escaped_stop_tokens=True,
         )
@@ -42,15 +39,20 @@
 
     def _process_curly(self):
         self._get_token(TokenTypes.LITERAL, "{")
         variable_name = self._collect_join(stop_tokens=[Token(TokenTypes.LITERAL, "}")])
         self._get_token(TokenTypes.LITERAL, "}")
 
         try:
-            variable_value = self.environment.getvar(variable_name)
+            variable_value = self.environment.getvar_nodefault(variable_name)
+
+            # Boolean variables are used in
+            # conditions but shouldn't be printed
+            if variable_value in [True, False]:
+                variable_value = ""
 
             self._save(TextNode(variable_value))
         except KeyError:
             self._error(f'Attribute "{variable_name}" has not been defined')
 
         return True
 
@@ -63,14 +65,14 @@
         return [
             self._process_escaped_char,
             self._process_verbatim,
             self._process_curly,
             self._process_pass,
         ]
 
-    def parse(self):
-        super().parse()
+    def parse(self, tokens):
+        super().parse(tokens)
 
         # After having parsed the text and replaced the
         # variables, this should return a piece of text again
         text = "".join([str(i.value) for i in self.nodes])
         self.nodes = [TextNode(text)]
```

### Comparing `mau-3.1.0/mau/parsers/text_parser.py` & `mau-4.0.0/mau/parsers/text_parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import itertools
 
 from mau.lexers.base_lexer import Token, TokenTypes
 from mau.lexers.text_lexer import TextLexer
 from mau.nodes.footnotes import FootnoteNode
-from mau.nodes.inline import (
-    ClassNode,
-    ImageNode,
-    LinkNode,
+from mau.nodes.inline import SentenceNode, StyleNode, TextNode, VerbatimNode, WordNode
+from mau.nodes.macros import (
+    MacroClassNode,
+    MacroHeaderNode,
+    MacroImageNode,
+    MacroLinkNode,
     MacroNode,
-    SentenceNode,
-    StyleNode,
-    TextNode,
-    VerbatimNode,
-    WordNode,
 )
-from mau.nodes.references import ReferenceNode
 from mau.parsers.arguments import set_names_and_defaults
 from mau.parsers.arguments_parser import ArgumentsParser
 from mau.parsers.base_parser import BaseParser
 
 # This is a simple map to keep track of the official
 # name of styles introduced by special characters
 MAP_STYLES = {"_": "underscore", "*": "star", "^": "caret", "~": "tilde"}
@@ -26,45 +22,50 @@
 
 # The TextParser is a nested parser.
 # The parsing always starts with parse_sentence
 # and from there all components of the text are explored
 class TextParser(BaseParser):
     lexer_class = TextLexer
 
-    def __init__(self, tokens):
-        super().__init__(tokens)
+    def __init__(self, environment, parent_node=None, parent_position=None):
+        super().__init__(environment, parent_node, parent_position)
 
         # These are the footnotes found in this text
+        # The format of this dictionary is
+        # {"name": node}
         self.footnotes = {}
 
-        # These are the references found in this text
-        # The format of this dictionary is
-        # {("content_type", "name"): node}
-        self.references = {}
+        # These are the internal links found in this text
+        self.links = []
 
     def _process_functions(self):
         return [self._process_eol, self._process_sentence]
 
     def _process_eol(self):
         # This simply parses the end of line.
 
         self._get_token(TokenTypes.EOL)
 
         return True
 
     def _process_sentence(self):
-        self._save(self._parse_sentence())
+        for node in self._parse_sentence():
+            self._save(node)
 
         return True
 
     def _parse_word(self):
         """
         Parse a single word.
         """
-        return WordNode(self._get_token().value)
+        return WordNode(
+            value=self._get_token().value,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
 
     def _parse_style(self):
         """
         Parse a sentence surrounded by style markers.
         """
 
         # Get the style marker
@@ -74,25 +75,34 @@
 
         # Get everything until the next marker
         content = self._parse_sentence(stop_tokens={Token(TokenTypes.LITERAL, style)})
 
         # Get the closing marker
         self._get_token(TokenTypes.LITERAL, style)
 
-        return StyleNode(MAP_STYLES[style], content)
+        return StyleNode(
+            value=MAP_STYLES[style],
+            children=content,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
 
     def _parse_escape(self):
         """
         Parse an escaped element.
         """
 
         # Drop the backslash
         self._get_token(TokenTypes.LITERAL, "\\")
 
-        return WordNode(self._get_token().value)
+        return WordNode(
+            value=self._get_token().value,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
 
     def _parse_styled_text(self, stop_tokens=None):
         """
         Parse multiple possible elements: escapes, classes,
         macros, verbatim, styles, links, words.
         This is a helper for the function _parse_sentence
         that takes into account all possible elements of
@@ -109,14 +119,17 @@
         with self:
             return self._parse_macro()
 
         with self:
             return self._parse_verbatim()
 
         with self:
+            return self._parse_escaped()
+
+        with self:
             return self._parse_style()
 
         return self._parse_word()
 
     def _parse_sentence(self, stop_tokens=None):
         """
         Parse a sentence, which is made of multiple
@@ -135,19 +148,25 @@
             result = self._parse_styled_text(stop_tokens)
 
         # Group consecutive WordNode nodes into a single TextNode
         grouped_nodes = []
         for key, group in itertools.groupby(content, lambda x: x.__class__ == WordNode):
             if key:
                 text = "".join([n.value for n in group])
-                grouped_nodes.append(TextNode(text))
+                grouped_nodes.append(
+                    TextNode(
+                        value=text,
+                        parent=self.parent_node,
+                        parent_position=self.parent_position,
+                    )
+                )
             else:
                 grouped_nodes.extend(list(group))
 
-        return SentenceNode(content=grouped_nodes)
+        return grouped_nodes
 
     def _parse_verbatim(self):
         """
         Parse text in `verbatim`.
         """
 
         # Get the verbatim marker
@@ -158,15 +177,38 @@
         content = self._collect_join(
             [Token(TokenTypes.LITERAL, "`"), Token(TokenTypes.EOL)],
         )
 
         # Remove the closing marker
         self._get_token(TokenTypes.LITERAL, "`")
 
-        return VerbatimNode(content)
+        return VerbatimNode(
+            content, parent=self.parent_node, parent_position=self.parent_position
+        )
+
+    def _parse_escaped(self):
+        """
+        Parse $escaped$ or %escaped% text.
+        """
+
+        # Get the escaped marker
+        marker = self._get_token(TokenTypes.LITERAL, check=lambda x: x in "$%").value
+
+        # Get the content tokens until the
+        # next verbatim marker or EOL
+        content = self._collect_join(
+            [Token(TokenTypes.LITERAL, marker), Token(TokenTypes.EOL)],
+        )
+
+        # Remove the closing marker
+        self._get_token(TokenTypes.LITERAL, marker)
+
+        return TextNode(
+            content, parent=self.parent_node, parent_position=self.parent_position
+        )
 
     def _parse_macro_link(self, args, kwargs):
         """
         Parse a link macro in the form [link](target, text).
         """
 
         args, kwargs = set_names_and_defaults(
@@ -175,15 +217,49 @@
 
         target = kwargs.get("target")
 
         text = kwargs["text"]
         if text is None:
             text = target
 
-        return LinkNode(target=target, text=text)
+        current_context = self._current_token.context
+        par = self.analyse(text, current_context, self.environment)
+
+        return MacroLinkNode(
+            target=target,
+            children=par.nodes,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
+
+    def _parse_macro_header(self, args, kwargs):
+        """
+        Parse a link macro in the form [header](header_id, text).
+        """
+
+        args, kwargs = set_names_and_defaults(
+            args, kwargs, ["target", "text"], {"text": ""}
+        )
+
+        target = kwargs.get("target")
+        text = kwargs["text"]
+
+        current_context = self._current_token.context
+        par = self.analyse(text, current_context, self.environment)
+
+        node = MacroHeaderNode(
+            header_id=target,
+            children=par.nodes,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
+
+        self.links.append(node)
+
+        return node
 
     def _parse_macro_mailto(self, args, kwargs):
         """
         Parse a mailto macro in the form [mailto](email).
         """
 
         args, kwargs = set_names_and_defaults(
@@ -193,38 +269,120 @@
         email = kwargs.get("email")
         text = kwargs.get("text")
 
         target = f"mailto:{email}"
         if text is None:
             text = email
 
-        return LinkNode(target, text)
+        current_context = self._current_token.context
+        par = self.analyse(text, current_context, self.environment)
+
+        return MacroLinkNode(
+            target=target,
+            children=par.nodes,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
 
     def _parse_macro_class(self, args, kwargs):
         """
-        Parse a class macro in the form [class](text, "class1,class2,...").
+        Parse a class macro in the form [class](text, class1, class2, ...).
         """
 
+        args, kwargs = set_names_and_defaults(args, kwargs, ["text"])
+
+        current_context = self._current_token.context
+
+        text = kwargs.get("text")
+
+        par = self.analyse(text, current_context, self.environment)
+
+        return MacroClassNode(
+            classes=args,
+            children=par.nodes,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
+
+    def _parse_macro_control(self, macro_name, args, kwargs):
+        """
+        Parse a class macro in the form [@if:variable:test](true, false).
+        """
+
+        # Skip the initial @
+        macro_name = macro_name[1:]
+
+        try:
+            operator, variable, test = macro_name.split(":", 2)
+        except ValueError:
+            self._error(
+                f"Macro '{macro_name}' is not in the form @operator:variable:test"
+            )
+
+        if operator not in ["if", "ifeval"]:
+            self._error(f"Control operator '{operator}' is not supported")
+
         args, kwargs = set_names_and_defaults(
-            args, kwargs, ["text", "classes"], {"classes": ""}
+            args,
+            kwargs,
+            ["true", "false"],
+            {"false": ""},
         )
 
         current_context = self._current_token.context
 
-        text = kwargs.get("text")
+        variable_value = self.environment.getvar(variable, None)
+
+        if variable_value is None:
+            self._error(f"Variable '{variable}' has not been defined")
+
+        test_result = False
+
+        if test.startswith("="):
+            value = test[1:]
+            test_result = variable_value == value
+        elif test.startswith("!="):
+            value = test[2:]
+            test_result = variable_value != value
+        elif test.startswith("&"):
+            value = test[1:]
+
+            if value not in ["true", "false"]:
+                self._error(f"Boolean value '{value}' is invalid")
+
+            # pylint: disable=simplifiable-if-expression
+            value = True if value == "true" else False
+
+            test_result = variable_value and value
+        else:
+            self._error(f"Test '{test}' is not supported")
+
+        if operator == "if":
+            if test_result is True:
+                text = kwargs.get("true")
+            else:
+                text = kwargs.get("false")
+        else:
+            if test_result is True:
+                text_variable = kwargs.get("true")
+            else:
+                text_variable = kwargs.get("false")
 
-        par = self.analyse(text, current_context)
+            text = self.environment.getvar(text_variable)
 
-        # Text should return a single sentence node
-        result = par.nodes[0]
+            if text is None:
+                self._error(f"Variable '{text_variable}' has not been defined")
 
-        # Multiple classes are separated by commas
-        classes = kwargs["classes"].split(",")
+        par = self.analyse(text, current_context, self.environment)
 
-        return ClassNode(classes, result)
+        return SentenceNode(
+            children=par.nodes,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
 
     def _parse_macro_image(self, args, kwargs):
         """
         Parse an inline image macro in the form
         [image](uri, alt_text, width, height).
         """
 
@@ -232,57 +390,38 @@
         args, kwargs = set_names_and_defaults(
             args,
             kwargs,
             ["uri", "alt_text", "width", "height"],
             {"alt_text": None, "width": None, "height": None},
         )
 
-        return ImageNode(
+        return MacroImageNode(
             uri=kwargs.get("uri"),
             alt_text=kwargs.get("alt_text"),
             width=kwargs.get("width"),
             height=kwargs.get("height"),
+            parent=self.parent_node,
+            parent_position=self.parent_position,
         )
 
     def _parse_macro_footnote(self, args, kwargs):
         """
         Parse a footnote macro in the form
         [footnote](name).
         """
 
         args, kwargs = set_names_and_defaults(args, kwargs, ["name"])
 
         name = kwargs["name"]
 
-        node = FootnoteNode()
-
-        self.footnotes[name] = node
-
-        return node
-
-    def _parse_macro_reference(self, args, kwargs):
-        """
-        Parse a reference macro in the form
-        [reference](type, name, category).
-        """
-
-        args, kwargs = set_names_and_defaults(
-            args,
-            kwargs,
-            ["type", "name", "category"],
-            {"category": None},
+        node = FootnoteNode(
+            parent=self.parent_node, parent_position=self.parent_position
         )
 
-        content_type = kwargs["type"]
-        name = kwargs["name"]
-        category = kwargs["category"]
-
-        node = ReferenceNode(content_type, name, category=category)
-
-        self.references[(content_type, name)] = node
+        self.footnotes[name] = node
 
         return node
 
     def _collect_macro_args(self):
         self._get_token(TokenTypes.LITERAL, "(")
 
         all_args = []
@@ -324,30 +463,45 @@
         macro_name = self._get_token(TokenTypes.TEXT).value
         self._get_token(TokenTypes.LITERAL, "]")
 
         arguments = self._collect_macro_args()
 
         current_context = self._peek_token().context
 
-        par = ArgumentsParser.analyse(arguments, current_context)
+        par = ArgumentsParser.analyse(arguments, current_context, self.environment)
+
+        args, kwargs, _, _ = par.process_arguments()
 
-        args, kwargs, _ = par.process_arguments()
+        if macro_name.startswith("@"):
+            return self._parse_macro_control(macro_name, args, kwargs)
 
         if macro_name == "link":
             return self._parse_macro_link(args, kwargs)
 
+        if macro_name == "header":
+            return self._parse_macro_header(args, kwargs)
+
         if macro_name == "mailto":
             return self._parse_macro_mailto(args, kwargs)
 
         if macro_name == "image":
             return self._parse_macro_image(args, kwargs)
 
         if macro_name == "footnote":
             return self._parse_macro_footnote(args, kwargs)
 
-        if macro_name == "reference":
-            return self._parse_macro_reference(args, kwargs)
-
         if macro_name == "class":
             return self._parse_macro_class(args, kwargs)
 
-        return MacroNode(macro_name, args=args, kwargs=kwargs)
+        # if macro_name == "if":
+        #     return self._parse_macro_if(args, kwargs)
+
+        # if macro_name == "ifeval":
+        #     return self._parse_macro_ifeval(args, kwargs)
+
+        return MacroNode(
+            macro_name,
+            args=args,
+            kwargs=kwargs,
+            parent=self.parent_node,
+            parent_position=self.parent_position,
+        )
```

### Comparing `mau-3.1.0/mau/text_buffer/context.py` & `mau-4.0.0/mau/text_buffer/context.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/mau/text_buffer/text_buffer.py` & `mau-4.0.0/mau/text_buffer/text_buffer.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/mau/tokens/tokens.py` & `mau-4.0.0/mau/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/pyproject.toml` & `mau-4.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mau"
-version = "3.1.0"
+version = "4.0.0"
 description = "A lightweight template-driven markup language"
 authors = [{name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
 "Development Status :: 5 - Production/Stable",
 "License :: OSI Approved :: MIT License",
 "Intended Audience :: Developers",
```

### Comparing `mau-3.1.0/tests/lexers/test_arguments_lexer.py` & `mau-4.0.0/tests/lexers/test_arguments_lexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,60 @@
+from mau.environment.environment import Environment
 from mau.lexers.arguments_lexer import ArgumentsLexer
 from mau.lexers.base_lexer import TokenTypes
 from mau.text_buffer.context import Context
 from mau.text_buffer.text_buffer import TextBuffer
 from mau.tokens.tokens import Token
 
 
 def test_single_unnamed_argument():
     text_buffer = TextBuffer("value1")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_single_named_argument():
     text_buffer = TextBuffer("argument1=value1")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "argument1"),
         Token(TokenTypes.LITERAL, "="),
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_multiple_unnamed_arguments():
     text_buffer = TextBuffer("value1, value2")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.LITERAL, ","),
         Token(TokenTypes.WHITESPACE, " "),
         Token(TokenTypes.TEXT, "value2"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_multiple_named_arguments():
     text_buffer = TextBuffer("argument1=value1, argument2=value2")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "argument1"),
         Token(TokenTypes.LITERAL, "="),
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.LITERAL, ","),
         Token(TokenTypes.WHITESPACE, " "),
@@ -63,16 +64,16 @@
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_mixed_arguments():
     text_buffer = TextBuffer("value1, value2,argument1=value1, argument2=value2")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.LITERAL, ","),
         Token(TokenTypes.WHITESPACE, " "),
         Token(TokenTypes.TEXT, "value2"),
         Token(TokenTypes.LITERAL, ","),
@@ -87,16 +88,16 @@
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_quotes():
     text_buffer = TextBuffer('argument1="value1,value2"')
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "argument1"),
         Token(TokenTypes.LITERAL, "="),
         Token(TokenTypes.LITERAL, '"'),
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.LITERAL, ","),
@@ -105,32 +106,32 @@
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_spaces():
     text_buffer = TextBuffer("argument1=value1 value2")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "argument1"),
         Token(TokenTypes.LITERAL, "="),
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.WHITESPACE, " "),
         Token(TokenTypes.TEXT, "value2"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_escaped_quotes():
     text_buffer = TextBuffer(r"Argument \"with\" quotes")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "Argument"),
         Token(TokenTypes.WHITESPACE, " "),
         Token(TokenTypes.LITERAL, "\\"),
         Token(TokenTypes.LITERAL, '"'),
         Token(TokenTypes.TEXT, "with"),
@@ -141,16 +142,16 @@
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_context():
     text_buffer = TextBuffer("argument1=value1")
-    lex = ArgumentsLexer(text_buffer)
-    lex.process()
+    lex = ArgumentsLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "argument1"),
         Token(TokenTypes.LITERAL, "="),
         Token(TokenTypes.TEXT, "value1"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
```

### Comparing `mau-3.1.0/tests/lexers/test_base_lexer.py` & `mau-4.0.0/tests/lexers/test_base_lexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from unittest.mock import Mock, patch
 
 import pytest
+from mau.environment.environment import Environment
 from mau.errors import MauErrorException
 from mau.lexers.base_lexer import BaseLexer, TokenTypes
 from mau.text_buffer.context import Context
 from mau.text_buffer.text_buffer import TextBuffer
 from mau.tokens.tokens import Token
 
 from tests.helpers import dedent
 
 
 def test_text_buffer_properties():
     mock_text_buffer = Mock()
-    lex = BaseLexer(text_buffer=mock_text_buffer)
+    lex = BaseLexer(Environment())
+    lex.text_buffer = mock_text_buffer
 
     assert lex._current_char == mock_text_buffer.current_char
 
     assert lex._current_line == mock_text_buffer.current_line
 
     assert lex._tail == mock_text_buffer.tail
 
@@ -25,92 +27,95 @@
 
     lex._skip("four")
     mock_text_buffer.skip.assert_called_with(4)
 
 
 def test_create_token():
     mock_text_buffer = Mock()
-    lex = BaseLexer(mock_text_buffer)
+    lex = BaseLexer(Environment())
+    lex.text_buffer = mock_text_buffer
 
     token = lex._create_token("sometype", "somevalue")
     assert token == Token("sometype", "somevalue")
-    assert token.context == lex._text_buffer.context
+    assert token.context == lex.text_buffer.context
 
 
 @patch("mau.lexers.base_lexer.BaseLexer._nextline")
 def test_create_tokens_from_line(mock_nextline):
     text_buffer = TextBuffer("Content")
-    lex = BaseLexer(text_buffer)
+    lex = BaseLexer(Environment())
+    lex.text_buffer = text_buffer
 
     tokens = lex._create_tokens_from_line(TokenTypes.TEXT)
 
     assert tokens == [
         Token(TokenTypes.TEXT, "Content"),
         Token(TokenTypes.EOL),
     ]
     mock_nextline.assert_called()
 
 
 def test_create_token_and_skip():
     mock_text_buffer = Mock()
-    lex = BaseLexer(mock_text_buffer)
+    lex = BaseLexer(Environment())
+    lex.text_buffer = mock_text_buffer
     lex._skip = Mock()
 
     token = lex._create_token_and_skip("sometype", "somevalue")
     assert token == Token("sometype", "somevalue")
     lex._skip.assert_called_with("somevalue")
 
 
 def test_error():
     mock_text_buffer = Mock()
-    lex = BaseLexer(mock_text_buffer)
+    lex = BaseLexer(Environment())
+    lex.text_buffer = mock_text_buffer
 
     with pytest.raises(MauErrorException):
         lex._process_error()
 
 
 def test_empty_text():
-    mock_text_buffer = Mock()
-    lex = BaseLexer(mock_text_buffer)
-    lex.process()
+    lex = BaseLexer(Environment())
+    lex.process(Mock())
 
     assert lex.tokens == [
         Token(TokenTypes.EOF),
     ]
 
 
 def test_just_empty_lines():
     text_buffer = TextBuffer("\n")
-    lex = BaseLexer(text_buffer)
-    lex.process()
+    lex = BaseLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_lines_with_only_spaces():
     text_buffer = TextBuffer("    \n    ")
-    lex = BaseLexer(text_buffer)
-    lex.process()
+    lex = BaseLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_text():
     text = "Just simple text"
     text_buffer = TextBuffer(text)
-    lex = BaseLexer(text_buffer)
-    lex.process()
+    lex = BaseLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, text),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
@@ -121,16 +126,16 @@
         This is text
         split into multiple lines
 
         with an empty line
         """
     )
     text_buffer = TextBuffer(text)
-    lex = BaseLexer(text_buffer)
-    lex.process()
+    lex = BaseLexer(Environment())
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "This is text"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.TEXT, "split into multiple lines"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOL),
@@ -147,16 +152,16 @@
 
         ---
 
         This is another line of text
         """
     )
     text_buffer = TextBuffer(text)
-    lex = BaseLexer(text_buffer)
-    lex.process()
+    lex = BaseLexer(Environment())
+    lex.process(text_buffer)
 
     assert [i.context.asdict() for i in lex.tokens] == [
         {"column": 0, "line": 0, "source": None, "text": "This is a line of text"},
         {"column": 22, "line": 0, "source": None, "text": "This is a line of text"},
         {"column": 0, "line": 1, "source": None, "text": ""},
         {"column": 0, "line": 2, "source": None, "text": "---"},
         {"column": 3, "line": 2, "source": None, "text": "---"},
@@ -189,16 +194,16 @@
 
         ---
 
         This is another line of text
         """
     )
     text_buffer = TextBuffer(text, Context(line=42, column=123, source="main"))
-    lex = BaseLexer(text_buffer)
-    lex.process()
+    lex = BaseLexer(Environment())
+    lex.process(text_buffer)
 
     assert [i.context.asdict() for i in lex.tokens] == [
         {"column": 123, "line": 42, "source": "main", "text": "This is a line of text"},
         {"column": 145, "line": 42, "source": "main", "text": "This is a line of text"},
         {"column": 123, "line": 43, "source": "main", "text": ""},
         {"column": 123, "line": 44, "source": "main", "text": "---"},
         {"column": 126, "line": 44, "source": "main", "text": "---"},
```

### Comparing `mau-3.1.0/tests/lexers/test_main_lexer.py` & `mau-4.0.0/tests/lexers/test_main_lexer.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,117 +2,103 @@
 
 from mau.lexers.base_lexer import TokenTypes as BLTokenTypes
 from mau.lexers.main_lexer import MainLexer, TokenTypes
 from mau.text_buffer.context import Context
 from mau.text_buffer.text_buffer import TextBuffer
 from mau.tokens.tokens import Token
 
-from tests.helpers import dedent
+from tests.helpers import dedent, init_lexer_factory, lexer_runner_factory
+
+init_lexer = init_lexer_factory(MainLexer)
+
+runner = lexer_runner_factory(MainLexer)
 
 
 def test_empty_text():
-    text_buffer = TextBuffer("")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("")
 
     assert lex.tokens == [
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_empty_lines():
-    text_buffer = TextBuffer("\n")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("\n")
 
     assert lex.tokens == [
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_lines_with_only_spaces():
-    text_buffer = TextBuffer("      \n      ")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("      \n      ")
 
     assert lex.tokens == [
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_horizontal_rule():
-    text_buffer = TextBuffer("---")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("---")
 
     assert lex.tokens == [
         Token(TokenTypes.HORIZONTAL_RULE, "---"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_escape_line():
-    text_buffer = TextBuffer(r"\[name]")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner(r"\[name]")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, r"\[name]"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_escape_line_beginning_with_backslash():
-    text_buffer = TextBuffer(r"\\[name]")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner(r"\\[name]")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, r"\\[name]"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_arguments():
-    text_buffer = TextBuffer("[name]")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("[name]")
 
     assert lex.tokens == [
         Token(TokenTypes.ARGUMENTS, "["),
         Token(BLTokenTypes.TEXT, "name"),
         Token(BLTokenTypes.LITERAL, "]"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_attributes_no_closing_bracket():
-    text_buffer = TextBuffer("[name")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("[name")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "[name"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_attributes_marker_in_text():
-    text_buffer = TextBuffer("Not [attributes]")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("Not [attributes]")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "Not [attributes]"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
@@ -120,17 +106,15 @@
         Context(0, 0, None, "Not [attributes]"),
         Context(0, 16, None, "Not [attributes]"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_variable_definition():
-    text_buffer = TextBuffer(":variable:value123")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner(":variable:value123")
 
     assert lex.tokens == [
         Token(TokenTypes.VARIABLE, ":"),
         Token(BLTokenTypes.TEXT, "variable"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.TEXT, "value123"),
         Token(BLTokenTypes.EOL),
@@ -143,68 +127,72 @@
         Context(0, 9, None, ":variable:value123"),
         Context(0, 10, None, ":variable:value123"),
         Context(0, 18, None, ":variable:value123"),
         Context(1, 0, None, ""),
     ]
 
 
-def test_variable_negation():
-    text_buffer = TextBuffer(":!variable:")
-    lex = MainLexer(text_buffer)
-    lex.process()
+def test_variable_flag_true():
+    lex = runner(":+variable:")
+
+    assert lex.tokens == [
+        Token(TokenTypes.VARIABLE, ":"),
+        Token(BLTokenTypes.TEXT, "+variable"),
+        Token(BLTokenTypes.LITERAL, ":"),
+        Token(BLTokenTypes.EOL),
+        Token(BLTokenTypes.EOF),
+    ]
+
+
+def test_variable_flag_false():
+    lex = runner(":-variable:")
 
     assert lex.tokens == [
         Token(TokenTypes.VARIABLE, ":"),
-        Token(BLTokenTypes.TEXT, "!variable"),
+        Token(BLTokenTypes.TEXT, "-variable"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_variable_marker_in_text():
-    text_buffer = TextBuffer("Not a :variable:")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("Not a :variable:")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "Not a :variable:"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_variable_definition_accepted_characters():
-    text_buffer = TextBuffer(":abcAB.C0123-_:value123")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner(":abcAB.C0123-_:value123")
 
     assert lex.tokens == [
         Token(TokenTypes.VARIABLE, ":"),
         Token(BLTokenTypes.TEXT, "abcAB.C0123-_"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.TEXT, "value123"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_multiple_lines():
-    text_buffer = TextBuffer(
+    lex = runner(
         dedent(
             """
             This is text
             split into multiple lines
 
             with an empty line
             """
         )
     )
-    lex = MainLexer(text_buffer)
-    lex.process()
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "This is text"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.TEXT, "split into multiple lines"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOL),
@@ -222,17 +210,15 @@
         Context(3, 0, None, "with an empty line"),
         Context(3, 18, None, "with an empty line"),
         Context(4, 0, None, ""),
     ]
 
 
 def test_title():
-    text_buffer = TextBuffer(".A title")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner(".A title")
 
     assert lex.tokens == [
         Token(TokenTypes.TITLE, "."),
         Token(BLTokenTypes.TEXT, "A title"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
@@ -242,17 +228,15 @@
         Context(0, 1, None, ".A title"),
         Context(0, 8, None, ".A title"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_title_with_space():
-    text_buffer = TextBuffer(".      A title")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner(".      A title")
 
     assert lex.tokens == [
         Token(TokenTypes.TITLE, "."),
         Token(BLTokenTypes.WHITESPACE, "      "),
         Token(BLTokenTypes.TEXT, "A title"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
@@ -264,17 +248,15 @@
         Context(0, 7, None, ".      A title"),
         Context(0, 14, None, ".      A title"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_command():
-    text_buffer = TextBuffer("::command:arg0,arg1")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("::command:arg0,arg1")
 
     assert lex.tokens == [
         Token(TokenTypes.COMMAND, "::"),
         Token(BLTokenTypes.TEXT, "command"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.TEXT, "arg0,arg1"),
         Token(BLTokenTypes.EOL),
@@ -288,53 +270,47 @@
         Context(0, 10, None, "::command:arg0,arg1"),
         Context(0, 19, None, "::command:arg0,arg1"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_command_without_arguments():
-    text_buffer = TextBuffer("::command:")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("::command:")
 
     assert lex.tokens == [
         Token(TokenTypes.COMMAND, "::"),
         Token(BLTokenTypes.TEXT, "command"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_comment():
-    text_buffer = TextBuffer("// Some comment")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("// Some comment")
 
     assert lex.tokens == [
         Token(TokenTypes.COMMENT, "// Some comment"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_multiline_comment():
-    text_buffer = TextBuffer(
+    lex = runner(
         dedent(
             """
             ////
             Some comment
 
                another line
             ////
             """
         )
     )
-    lex = MainLexer(text_buffer)
-    lex.process()
 
     assert lex.tokens == [
         Token(TokenTypes.MULTILINE_COMMENT, "////"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.TEXT, "Some comment"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOL),
@@ -356,20 +332,18 @@
         Context(4, 0, None, "////"),
         Context(4, 4, None, "////"),
         Context(5, 0, None, ""),
     ]
 
 
 def test_include_content():
-    text_buffer = TextBuffer("<<type:/path/to/it.jpg")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("<<type:/path/to/it.jpg")
 
     assert lex.tokens == [
-        Token(TokenTypes.INCLUDE, "<<"),
+        Token(TokenTypes.CONTENT, "<<"),
         Token(BLTokenTypes.TEXT, "type"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.TEXT, "/path/to/it.jpg"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
@@ -380,20 +354,18 @@
         Context(0, 7, None, "<<type:/path/to/it.jpg"),
         Context(0, 22, None, "<<type:/path/to/it.jpg"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_include_content_with_space():
-    text_buffer = TextBuffer("<<      type:/path/to/it.jpg")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("<<      type:/path/to/it.jpg")
 
     assert lex.tokens == [
-        Token(TokenTypes.INCLUDE, "<<"),
+        Token(TokenTypes.CONTENT, "<<"),
         Token(BLTokenTypes.WHITESPACE, "      "),
         Token(BLTokenTypes.TEXT, "type"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.TEXT, "/path/to/it.jpg"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
@@ -406,20 +378,18 @@
         Context(0, 13, None, "<<      type:/path/to/it.jpg"),
         Context(0, 28, None, "<<      type:/path/to/it.jpg"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_include_content_without_arguments():
-    text_buffer = TextBuffer("<<type:")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("<<type:")
 
     assert lex.tokens == [
-        Token(TokenTypes.INCLUDE, "<<"),
+        Token(TokenTypes.CONTENT, "<<"),
         Token(BLTokenTypes.TEXT, "type"),
         Token(BLTokenTypes.LITERAL, ":"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
     assert [i.context for i in lex.tokens] == [
@@ -428,17 +398,15 @@
         Context(0, 6, None, "<<type:"),
         Context(0, 7, None, "<<type:"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_unordered_list():
-    text_buffer = TextBuffer("* Item")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("* Item")
 
     assert lex.tokens == [
         Token(TokenTypes.LIST, "*"),
         Token(BLTokenTypes.WHITESPACE, " "),
         Token(BLTokenTypes.TEXT, "Item"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
@@ -451,87 +419,77 @@
         Context(0, 6, None, "* Item"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_unordered_list_leading_space():
     text_buffer = TextBuffer("    * Item")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = init_lexer()
+    lex.process(text_buffer)
 
     assert lex.tokens == [
         Token(BLTokenTypes.WHITESPACE, "    "),
         Token(TokenTypes.LIST, "*"),
         Token(BLTokenTypes.WHITESPACE, " "),
         Token(BLTokenTypes.TEXT, "Item"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_unordered_list_trailing_space():
-    text_buffer = TextBuffer("*       Item")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("*       Item")
 
     assert lex.tokens == [
         Token(TokenTypes.LIST, "*"),
         Token(BLTokenTypes.WHITESPACE, "       "),
         Token(BLTokenTypes.TEXT, "Item"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_unordered_list_multiple_stars():
-    text_buffer = TextBuffer("*** Item")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("*** Item")
 
     assert lex.tokens == [
         Token(TokenTypes.LIST, "***"),
         Token(BLTokenTypes.WHITESPACE, " "),
         Token(BLTokenTypes.TEXT, "Item"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_ordered_list():
-    text_buffer = TextBuffer("# Item")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("# Item")
 
     assert lex.tokens == [
         Token(TokenTypes.LIST, "#"),
         Token(BLTokenTypes.WHITESPACE, " "),
         Token(BLTokenTypes.TEXT, "Item"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_ordered_list_multiple_stars():
-    text_buffer = TextBuffer("### Item")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("### Item")
 
     assert lex.tokens == [
         Token(TokenTypes.LIST, "###"),
         Token(BLTokenTypes.WHITESPACE, " "),
         Token(BLTokenTypes.TEXT, "Item"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_header():
-    text_buffer = TextBuffer("=Header")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("=Header")
 
     assert lex.tokens == [
         Token(TokenTypes.HEADER, "="),
         Token(BLTokenTypes.TEXT, "Header"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
@@ -541,121 +499,105 @@
         Context(0, 1, None, "=Header"),
         Context(0, 7, None, "=Header"),
         Context(1, 0, None, ""),
     ]
 
 
 def test_header_with_space():
-    text_buffer = TextBuffer("=    Header")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("=    Header")
 
     assert lex.tokens == [
         Token(TokenTypes.HEADER, "="),
         Token(BLTokenTypes.WHITESPACE, "    "),
         Token(BLTokenTypes.TEXT, "Header"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_empty_header():
-    text_buffer = TextBuffer("=")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("=")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "="),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_multiple_header_markers():
-    text_buffer = TextBuffer("=== Header")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("=== Header")
 
     assert lex.tokens == [
         Token(TokenTypes.HEADER, "==="),
         Token(BLTokenTypes.WHITESPACE, " "),
         Token(BLTokenTypes.TEXT, "Header"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_header_marker_in_header_text():
-    text_buffer = TextBuffer("= a=b")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("= a=b")
 
     assert lex.tokens == [
         Token(TokenTypes.HEADER, "="),
         Token(BLTokenTypes.WHITESPACE, " "),
         Token(BLTokenTypes.TEXT, "a=b"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 def test_header_markers_in_text():
-    text_buffer = TextBuffer("Definitely not a === header")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("Definitely not a === header")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "Definitely not a === header"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
 
 @patch("mau.lexers.main_lexer.MainLexer._run_directive")
 def test_directive(mock_run_directive):
-    text_buffer = TextBuffer("::#name:/path/to/file")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    runner("::#name:/path/to/file")
 
     assert mock_run_directive.called_with("name", "/path/to/file")
 
 
 @patch("builtins.open", new_callable=mock_open, read_data="just some data")
 def test_import_directive(mock_file):  # pylint: disable=unused-argument
-    text_buffer = TextBuffer("::#include:/path/to/file")
-    lex = MainLexer(text_buffer)
-    lex.process()
+    lex = runner("::#include:/path/to/file")
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "just some data"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
 
     assert [i.context for i in lex.tokens] == [
         Context(0, 0, "/path/to/file", "just some data"),
         Context(0, 14, "/path/to/file", "just some data"),
-        Context(1, 0, "/path/to/file", ""),
+        Context(1, 0, None),
     ]
 
 
 def test_block():
-    text_buffer = TextBuffer(
+    lex = runner(
         dedent(
             """
             ----
             Some comment
 
                another line
             ----
             """
         )
     )
-    lex = MainLexer(text_buffer)
-    lex.process()
 
     assert lex.tokens == [
         Token(TokenTypes.BLOCK, "----"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.TEXT, "Some comment"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOL),
@@ -677,27 +619,25 @@
         Context(4, 0, None, "----"),
         Context(4, 4, None, "----"),
         Context(5, 0, None, ""),
     ]
 
 
 def test_block_four_characters():
-    text_buffer = TextBuffer(
+    lex = runner(
         dedent(
             """
             ####
             Some comment
 
                another line
             ####
             """
         )
     )
-    lex = MainLexer(text_buffer)
-    lex.process()
 
     assert lex.tokens == [
         Token(TokenTypes.BLOCK, "####"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.TEXT, "Some comment"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOL),
@@ -719,25 +659,23 @@
         Context(4, 0, None, "####"),
         Context(4, 4, None, "####"),
         Context(5, 0, None, ""),
     ]
 
 
 def test_block_with_comment():
-    text_buffer = TextBuffer(
+    lex = runner(
         dedent(
             """
             ----
             // Comment
             ----
             """
         )
     )
-    lex = MainLexer(text_buffer)
-    lex.process()
 
     assert lex.tokens == [
         Token(TokenTypes.BLOCK, "----"),
         Token(BLTokenTypes.EOL),
         Token(TokenTypes.COMMENT, "// Comment"),
         Token(BLTokenTypes.EOL),
         Token(TokenTypes.BLOCK, "----"),
@@ -753,22 +691,64 @@
         Context(2, 0, None, "----"),
         Context(2, 4, None, "----"),
         Context(3, 0, None, ""),
     ]
 
 
 def test_block_has_to_begin_with_four_identical_characters():
-    text_buffer = TextBuffer(
+    lex = runner(
         dedent(
             """
             abcd
             """
         )
     )
-    lex = MainLexer(text_buffer)
-    lex.process()
 
     assert lex.tokens == [
         Token(BLTokenTypes.TEXT, "abcd"),
         Token(BLTokenTypes.EOL),
         Token(BLTokenTypes.EOF),
     ]
+
+
+def test_conditional():
+    lex = runner("@if:somevar:=value")
+
+    assert lex.tokens == [
+        Token(TokenTypes.CONTROL, "@"),
+        Token(BLTokenTypes.TEXT, "if"),
+        Token(BLTokenTypes.LITERAL, ":"),
+        Token(BLTokenTypes.TEXT, "somevar:=value"),
+        Token(BLTokenTypes.EOL),
+        Token(BLTokenTypes.EOF),
+    ]
+
+    assert [i.context for i in lex.tokens] == [
+        Context(0, 0, None, "@if:somevar:=value"),
+        Context(0, 1, None, "@if:somevar:=value"),
+        Context(0, 3, None, "@if:somevar:=value"),
+        Context(0, 4, None, "@if:somevar:=value"),
+        Context(0, 18, None, "@if:somevar:=value"),
+        Context(1, 0, None, ""),
+    ]
+
+
+def test_conditional_no_value():
+    lex = runner("@if:somevar:")
+
+    assert lex.tokens == [
+        Token(TokenTypes.CONTROL, "@"),
+        Token(BLTokenTypes.TEXT, "if"),
+        Token(BLTokenTypes.LITERAL, ":"),
+        Token(BLTokenTypes.TEXT, "somevar:"),
+        Token(BLTokenTypes.EOL),
+        Token(BLTokenTypes.EOF),
+    ]
+
+    assert [i.context for i in lex.tokens] == [
+        Context(0, 0, None, "@if:somevar:"),
+        Context(0, 1, None, "@if:somevar:"),
+        Context(0, 3, None, "@if:somevar:"),
+        Context(0, 4, None, "@if:somevar:"),
+        Context(0, 12, None, "@if:somevar:"),
+        Context(1, 0, None, ""),
+    ]
```

### Comparing `mau-3.1.0/tests/lexers/test_preprocess_variables_lexer.py` & `mau-4.0.0/tests/lexers/test_preprocess_variables_lexer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from mau.lexers.base_lexer import TokenTypes
 from mau.lexers.preprocess_variables_lexer import PreprocessVariablesLexer
-from mau.text_buffer.text_buffer import TextBuffer
 from mau.tokens.tokens import Token
 
+from tests.helpers import init_lexer_factory, lexer_runner_factory
+
+init_lexer = init_lexer_factory(PreprocessVariablesLexer)
+
+runner = lexer_runner_factory(PreprocessVariablesLexer)
+
 
 def test_normal_text():
-    text_buffer = TextBuffer("Some text")
-    lex = PreprocessVariablesLexer(text_buffer)
-    lex.process()
+    lex = runner("Some text")
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "S"),
         Token(TokenTypes.TEXT, "o"),
         Token(TokenTypes.TEXT, "m"),
         Token(TokenTypes.TEXT, "e"),
         Token(TokenTypes.TEXT, " "),
@@ -21,17 +24,15 @@
         Token(TokenTypes.TEXT, "t"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_match_only_backticks_and_curly_braces():
-    text_buffer = TextBuffer("Normal text `{curly}` _other_ *text*")
-    lex = PreprocessVariablesLexer(text_buffer)
-    lex.process()
+    lex = runner("Normal text `{curly}` _other_ *text*")
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "N"),
         Token(TokenTypes.TEXT, "o"),
         Token(TokenTypes.TEXT, "r"),
         Token(TokenTypes.TEXT, "m"),
         Token(TokenTypes.TEXT, "a"),
@@ -68,17 +69,15 @@
         Token(TokenTypes.TEXT, "*"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_escape_curly_braces():
-    text_buffer = TextBuffer(r"Normal text \{curly\} _other_ *text*")
-    lex = PreprocessVariablesLexer(text_buffer)
-    lex.process()
+    lex = runner(r"Normal text \{curly\} _other_ *text*")
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "N"),
         Token(TokenTypes.TEXT, "o"),
         Token(TokenTypes.TEXT, "r"),
         Token(TokenTypes.TEXT, "m"),
         Token(TokenTypes.TEXT, "a"),
@@ -115,17 +114,15 @@
         Token(TokenTypes.TEXT, "*"),
         Token(TokenTypes.EOL),
         Token(TokenTypes.EOF),
     ]
 
 
 def test_preserve_escapes():
-    text_buffer = TextBuffer(r"Normal \text \_other\_")
-    lex = PreprocessVariablesLexer(text_buffer)
-    lex.process()
+    lex = runner(r"Normal \text \_other\_")
 
     assert lex.tokens == [
         Token(TokenTypes.TEXT, "N"),
         Token(TokenTypes.TEXT, "o"),
         Token(TokenTypes.TEXT, "r"),
         Token(TokenTypes.TEXT, "m"),
         Token(TokenTypes.TEXT, "a"),
```

### Comparing `mau-3.1.0/tests/nodes/test_arguments.py` & `mau-4.0.0/tests/nodes/test_arguments.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/tests/nodes/test_footnotes.py` & `mau-4.0.0/tests/nodes/test_footnotes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,65 @@
-from mau.nodes.footnotes import CommandFootnotesNode, FootnoteNode, FootnotesEntryNode
+from mau.nodes.footnotes import FootnoteNode, FootnotesNode
 from mau.nodes.inline import TextNode, VerbatimNode
 
 
 def test_footnote_node():
-    node = FootnoteNode([VerbatimNode("somevalue"), TextNode("othervalue")])
+    node = FootnoteNode(children=[VerbatimNode("somevalue"), TextNode("othervalue")])
 
-    assert node.content == [VerbatimNode("somevalue"), TextNode("othervalue")]
+    assert node.children == [VerbatimNode("somevalue"), TextNode("othervalue")]
     assert node.number is None
     assert node.reference_anchor is None
     assert node.content_anchor is None
     assert node.node_type == "footnote"
-    assert node == FootnoteNode([VerbatimNode("somevalue"), TextNode("othervalue")])
+    assert node == FootnoteNode(
+        children=[VerbatimNode("somevalue"), TextNode("othervalue")]
+    )
 
 
 def test_footnote_node_with_number_and_anchor():
     node = FootnoteNode(
-        [VerbatimNode("somevalue"), TextNode("othervalue")],
+        children=[VerbatimNode("somevalue"), TextNode("othervalue")],
         number="3",
         reference_anchor="someanchor",
         content_anchor="someanchor-def",
     )
 
-    assert node.content == [VerbatimNode("somevalue"), TextNode("othervalue")]
+    assert node.children == [VerbatimNode("somevalue"), TextNode("othervalue")]
     assert node.number == "3"
     assert node.reference_anchor == "someanchor"
     assert node.content_anchor == "someanchor-def"
     assert node.node_type == "footnote"
     assert node == FootnoteNode(
-        [VerbatimNode("somevalue"), TextNode("othervalue")],
+        children=[VerbatimNode("somevalue"), TextNode("othervalue")],
         number="3",
         reference_anchor="someanchor",
         content_anchor="someanchor-def",
     )
 
 
 def test_footnotes_entry_node():
-    node = FootnotesEntryNode(
-        content=TextNode("Some text"),
-        number="1",
-        reference_anchor="someanchor",
-        content_anchor="someanchor-def",
-    )
+    node = FootnoteNode(
+        children=[VerbatimNode("somevalue"), TextNode("othervalue")]
+    ).to_entry()
 
-    assert node.content == TextNode("Some text")
-    assert node.number == "1"
-    assert node.reference_anchor == "someanchor"
-    assert node.content_anchor == "someanchor-def"
     assert node.node_type == "footnotes_entry"
-    assert node == FootnotesEntryNode(
-        content=TextNode("Some text"),
-        number="1",
-        reference_anchor="someanchor",
-        content_anchor="someanchor-def",
-    )
 
 
-def test_command_footnotes_node():
-    node = CommandFootnotesNode(
-        entries=[TextNode("somevalue1"), TextNode("somevalue2")],
+def test_footnotes_node():
+    node = FootnotesNode(
+        children=[TextNode("somevalue1"), TextNode("somevalue2")],
         args=["value1", "value2"],
         tags=["tag1", "tag2"],
         kwargs={"key1": "text1", "key2": "text2"},
     )
 
-    assert node.entries == [TextNode("somevalue1"), TextNode("somevalue2")]
+    assert node.children == [TextNode("somevalue1"), TextNode("somevalue2")]
     assert node.args == ["value1", "value2"]
     assert node.tags == ["tag1", "tag2"]
     assert node.kwargs == {"key1": "text1", "key2": "text2"}
-    assert node.node_type == "command_footnotes"
-    assert node == CommandFootnotesNode(
-        entries=[TextNode("somevalue1"), TextNode("somevalue2")],
+    assert node.node_type == "footnotes"
+    assert node == FootnotesNode(
+        children=[TextNode("somevalue1"), TextNode("somevalue2")],
         args=["value1", "value2"],
         tags=["tag1", "tag2"],
         kwargs={"key1": "text1", "key2": "text2"},
     )
```

### Comparing `mau-3.1.0/tests/nodes/test_nodes.py` & `mau-4.0.0/tests/nodes/test_nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from mau.nodes.nodes import Node, ValueNode
 
 
 def test_node():
     node = Node()
 
     assert node.node_type == "node"
-    assert node._content == {"type": "node"}
+    assert node.asdict() == {
+        "type": "node",
+        "subtype": None,
+        "children": [],
+        "args": [],
+        "kwargs": {},
+        "tags": [],
+    }
 
 
 def test_value_node():
     node = ValueNode("somevalue")
 
     assert node.value == "somevalue"
     assert node.node_type == "value_node"
     assert node == ValueNode("somevalue")
 
 
-def test_node_value_is_none_by_default():
-    node = ValueNode()
-
-    assert node.value is None
-    assert node == ValueNode()
-
-
 def test_node_accept():
     visitor = Mock()
     node = Node()
     node.node_type = "mynode"
 
     assert node.accept(visitor) == visitor._visit_mynode()
```

### Comparing `mau-3.1.0/tests/nodes/test_source.py` & `mau-4.0.0/tests/nodes/test_source.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/tests/nodes/test_toc.py` & `mau-4.0.0/tests/nodes/test_toc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from mau.nodes.header import HeaderNode
 from mau.nodes.toc import TocEntryNode, TocNode
 
 
 def test_toc_entry_node():
     node = TocEntryNode(value="Header 1", anchor="header-1", children=[])
 
     assert node.value == "Header 1"
@@ -9,24 +10,48 @@
     assert node.children == []
     assert node.node_type == "toc_entry"
     assert node == TocEntryNode(value="Header 1", anchor="header-1", children=[])
 
 
 def test_toc_node():
     node = TocNode(
-        entries=[],
+        children=[
+            HeaderNode(
+                "somevalue",
+                "somelevel",
+                "someanchor",
+                args=["hvalue1", "hvalue2"],
+                kwargs={"hkey1": "htext1", "hkey2": "htext2"},
+            )
+        ],
         args=["value1", "value2"],
         tags=["tag1", "tag2"],
         kwargs={"key1": "text1", "key2": "text2"},
     )
 
-    assert node.entries == []
+    assert node.children == [
+        HeaderNode(
+            "somevalue",
+            "somelevel",
+            "someanchor",
+            args=["hvalue1", "hvalue2"],
+            kwargs={"hkey1": "htext1", "hkey2": "htext2"},
+        )
+    ]
     assert node.args == ["value1", "value2"]
     assert node.tags == ["tag1", "tag2"]
     assert node.kwargs == {"key1": "text1", "key2": "text2"}
     assert node.node_type == "toc"
     assert node == TocNode(
-        entries=[],
+        children=[
+            HeaderNode(
+                "somevalue",
+                "somelevel",
+                "someanchor",
+                args=["hvalue1", "hvalue2"],
+                kwargs={"hkey1": "htext1", "hkey2": "htext2"},
+            )
+        ],
         args=["value1", "value2"],
         tags=["tag1", "tag2"],
         kwargs={"key1": "text1", "key2": "text2"},
     )
```

### Comparing `mau-3.1.0/tests/parsers/main_parser/test_block_attributes.py` & `mau-4.0.0/tests/parsers/main_parser/test_block_attributes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,686 +1,526 @@
-from unittest.mock import patch
-
 import pytest
+from mau.environment.environment import Environment
 from mau.errors import MauErrorException
 from mau.lexers.main_lexer import MainLexer
-from mau.nodes.inline import SentenceNode, TextNode, RawNode
-from mau.nodes.page import BlockNode, HeaderNode, ParagraphNode
+from mau.nodes.block import BlockNode
+from mau.nodes.header import HeaderNode
+from mau.nodes.inline import SentenceNode, TextNode
 from mau.parsers.main_parser import MainParser
 
 from tests.helpers import init_parser_factory, parser_runner_factory
 
 init_parser = init_parser_factory(MainLexer, MainParser)
 
 runner = parser_runner_factory(MainLexer, MainParser)
 
 
-def test_attributes_block():
+def test_block_attributes_args_and_kwargs():
     source = """
-    [blocktype,myattr1=value1]
+    [*subtype,arg1,key1=value1]
     ----
-    This is a simple line of text
-    followed by another line of text
-
-    And this is another paragraph
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[
-                ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode(
-                                "This is a simple line of text followed by another line of text"
-                            ),
-                        ]
-                    )
-                ),
-                ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode("And this is another paragraph"),
-                        ]
-                    )
-                ),
-            ],
-            secondary_content=[],
+            subtype="subtype",
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
-            args=[],
-            kwargs={"myattr1": "value1"},
+            args=["arg1"],
+            kwargs={"key1": "value1"},
         )
     ]
 
 
-def test_attributes_can_contain_variables():
+def test_block_attributes_can_contain_variables():
     source = """
-    :value:42
+    :value1:42
 
-    [blocktype,myattr1={value}]
+    [*subtype,key1={value1}]
     ----
-    This is a simple line of text
-    followed by another line of text
-
-    And this is another paragraph
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[
-                ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode(
-                                "This is a simple line of text followed by another line of text"
-                            ),
-                        ]
-                    )
-                ),
-                ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode("And this is another paragraph"),
-                        ]
-                    )
-                ),
-            ],
-            secondary_content=[],
+            subtype="subtype",
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
-            kwargs={"myattr1": "42"},
+            kwargs={"key1": "42"},
         )
     ]
 
 
 def test_parse_block_title_and_attributes():
     source = """
     .Just a title
-    [blocktype, name1=value1, name2=value2]
+    [*subtype, name1=value1, name2=value2]
     ----
     ----
     """
 
-    assert runner(source).nodes == [
+    parser = runner(source)
+
+    assert parser.nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
             classes=[],
             title=SentenceNode(
-                [
+                children=[
                     TextNode("Just a title"),
                 ]
             ),
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={"name1": "value1", "name2": "value2"},
         )
     ]
 
+    block_node = parser.nodes[0]
+    text_node = block_node.title.children[0]
+
+    assert text_node.parent == block_node
+    assert text_node.parent_position == "title"
+
 
 def test_parse_block_title_and_attributes_are_reset():
     source = """
     .Just a title
-    [blocktype1, name1=value1, name2=value2]
+    [*subtype1, name1=value1, name2=value2]
     ----
     ----
 
-    [blocktype2]
+    [*subtype2]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype1",
-            content=[],
-            secondary_content=[],
+            subtype="subtype1",
             classes=[],
             title=SentenceNode(
-                [
+                children=[
                     TextNode("Just a title"),
                 ]
             ),
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={"name1": "value1", "name2": "value2"},
         ),
         BlockNode(
-            blocktype="blocktype2",
-            content=[],
-            secondary_content=[],
+            subtype="subtype2",
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={},
         ),
     ]
 
 
 def test_block_classes_single_class():
     source = """
-    [blocktype,classes=cls1]
+    [*subtype,classes=cls1]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
             classes=["cls1"],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={},
         ),
     ]
 
 
 def test_block_classes_multiple_classes():
     source = """
-    [blocktype,classes="cls1,cls2"]
+    [*subtype,classes="cls1,cls2"]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
             classes=["cls1", "cls2"],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={},
         ),
     ]
 
 
 def test_block_engine():
     source = """
-    [blocktype,engine=someengine]
+    [*subtype,engine=someengine]
     ----
     ----
     """
 
     with pytest.raises(MauErrorException):
         runner(source)
 
 
-def test_block_mau_has_no_external_variables():
-    source = """
-    :answer:42
-    [block, engine=mau]
-    ----
-    The answer is {answer}.
-    ----
-    """
-
-    with pytest.raises(MauErrorException):
-        assert runner(source)
-
-
-def test_block_raw_engine():
-    source = """
-    [block, engine=raw]
-    ----
-    Raw content
-    on multiple lines
-    ----
-    Secondary content
-    on multiple lines as well
-    """
-
-    assert runner(source).nodes == [
-        BlockNode(
-            blocktype="block",
-            content=[
-                RawNode("Raw content"),
-                RawNode("on multiple lines"),
-            ],
-            secondary_content=[
-                RawNode("Secondary content"),
-                RawNode("on multiple lines as well"),
-            ],
-            classes=[],
-            title=None,
-            engine="raw",
-            preprocessor="none",
-            args=[],
-            kwargs={},
-        )
-    ]
-
-
 @patch("mau.parsers.main_parser.header_anchor")
 def test_block_default_engine_adds_headers_to_global_toc(mock_header_anchor):
     mock_header_anchor.return_value = "XXYY"
 
     source = """
     = Global header
 
-    [someblock]
+    [*someblock]
     ----
     = Block header
     ----
     """
 
     par = runner(source)
 
     assert par.nodes == [
-        HeaderNode("Global header", "1", "XXYY"),
-        BlockNode(
-            blocktype="someblock",
-            content=[
-                HeaderNode("Block header", "1", "XXYY"),
-            ],
-            secondary_content=[],
-            classes=[],
-            title=None,
-            engine="default",
-            preprocessor="none",
-            args=[],
-            kwargs={},
+        HeaderNode(
+            value=SentenceNode(children=[TextNode("Global header")]),
+            level="1",
+            anchor="XXYY",
         ),
-    ]
-
-    assert par.headers == [
-        HeaderNode("Global header", "1", "XXYY"),
-        HeaderNode("Block header", "1", "XXYY"),
-    ]
-
-
-def test_block_positive_condition_matches():
-    source = """
-    :render:yes
-
-    [block, condition="if:render:yes"]
-    ----
-    This is a paragraph.
-    ----
-    """
-
-    assert runner(source).nodes == [
         BlockNode(
-            blocktype="block",
-            content=[
-                ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode("This is a paragraph."),
-                        ]
-                    )
+            subtype="someblock",
+            children=[
+                HeaderNode(
+                    value=SentenceNode(children=[TextNode("Block header")]),
+                    level="1",
+                    anchor="XXYY",
                 ),
             ],
-            secondary_content=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={},
-        )
+        ),
     ]
 
-
-def test_block_positive_condition_doesnt_match():
-    source = """
-    :render:no
-
-    [block, condition="if:render:yes"]
-    ----
-    This is a paragraph.
-    ----
-    """
-
-    assert runner(source).nodes == []
-
-
-def test_block_negative_condition_matches():
-    source = """
-    :render:yes
-
-    [block, condition="ifnot:render:no"]
-    ----
-    This is a paragraph.
-    ----
-    """
-
-    assert runner(source).nodes == [
-        BlockNode(
-            blocktype="block",
-            content=[
-                ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode("This is a paragraph."),
-                        ]
-                    )
-                ),
-            ],
-            secondary_content=[],
-            classes=[],
-            title=None,
-            engine="default",
-            preprocessor="none",
-            args=[],
-            kwargs={},
-        )
+    assert par.toc_manager.headers == [
+        HeaderNode(
+            value=SentenceNode(children=[TextNode("Global header")]),
+            level="1",
+            anchor="XXYY",
+        ),
+        HeaderNode(
+            value=SentenceNode(children=[TextNode("Block header")]),
+            level="1",
+            anchor="XXYY",
+        ),
     ]
 
 
-def test_block_negative_condition_doesnt_match():
+def test_command_defblock():
     source = """
-    :render:no
-
-    [block, condition="ifnot:render:no"]
-    ----
-    This is a paragraph.
-    ----
+    ::defblock:alias, *myblock, language=python, engine=source
     """
 
-    assert runner(source).nodes == []
-
-
-def test_block_condition_accepts_booleans():
-    source = """
-    :render:
-
-    [block, condition="ifnot:render:"]
-    ----
-    This is a paragraph.
-    ----
-    """
+    par = runner(source)
 
-    assert runner(source).nodes == []
+    assert par.block_aliases["alias"] == {
+        "subtype": "myblock",
+        "mandatory_args": [],
+        "defaults": {"language": "python", "engine": "source"},
+    }
 
 
-def test_block_condition_raises_exception():
+def test_define_block_in_environment():
     source = """
-    [block, condition="if:render"]
-    ----
-    This is a paragraph.
-    ----
     """
 
-    with pytest.raises(MauErrorException):
-        runner(source)
+    environment = Environment()
+    environment.setvar(
+        "mau.parser.block_definitions",
+        {
+            "alias": {
+                "subtype": "type",
+                "mandatory_args": ["arg1", "arg2"],
+                "defaults": {"key1": "value1"},
+            },
+        },
+    )
 
+    par = runner(source, environment=environment)
 
-def test_block_condition_can_use_variable_namespace():
-    source = """
-    :flags.render:yes
+    assert par.block_aliases["alias"] == {
+        "subtype": "type",
+        "mandatory_args": ["arg1", "arg2"],
+        "defaults": {"key1": "value1"},
+    }
 
-    [block, condition="if:flags.render:yes"]
-    ----
-    This is a paragraph.
-    ----
-    """
 
-    assert runner(source).nodes == [
-        BlockNode(
-            blocktype="block",
-            content=[
-                ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode("This is a paragraph."),
-                        ]
-                    )
-                ),
-            ],
-            secondary_content=[],
-            classes=[],
-            title=None,
-            engine="default",
-            preprocessor="none",
-            args=[],
-            kwargs={},
-        )
-    ]
-
-
-def test_command_defblock():
+def test_command_defblock_no_subtype():
     source = """
-    ::defblock:alias, myblock, language=python, engine=source
+    ::defblock:alias, language=python, engine=source
     """
 
     par = runner(source)
 
-    assert par.block_aliases["alias"] == "myblock"
-    assert par.block_defaults["alias"] == {"language": "python", "engine": "source"}
+    assert par.block_aliases["alias"] == {
+        "subtype": None,
+        "mandatory_args": [],
+        "defaults": {"language": "python", "engine": "source"},
+    }
 
 
 def test_command_defblock_source():
     source = """
     """
 
     par = runner(source)
 
-    assert par.block_aliases["source"] == "default"
-    assert par.block_defaults["source"] == {"language": "text", "engine": "source"}
+    assert par.block_aliases["source"] == {
+        "subtype": None,
+        "mandatory_args": ["language"],
+        "defaults": {"language": "text", "engine": "source"},
+    }
 
 
 def test_command_defblock_source_can_be_overridden():
     source = """
-    ::defblock:source, source, language=python, engine=source
+    ::defblock:source, *source, language=python, engine=source
     """
 
     par = runner(source)
 
-    assert par.block_aliases["source"] == "source"
-    assert par.block_defaults["source"] == {"language": "python", "engine": "source"}
+    assert par.block_aliases["source"] == {
+        "subtype": "source",
+        "mandatory_args": [],
+        "defaults": {"language": "python", "engine": "source"},
+    }
 
 
 def test_command_defblock_no_args():
     source = """
     ::defblock:
     """
 
     with pytest.raises(MauErrorException):
         runner(source)
 
 
-def test_command_defblock_single_arg():
-    source = """
-    ::defblock:source
-    """
-
-    with pytest.raises(MauErrorException):
-        runner(source)
-
-
 def test_block_definitions_are_used():
     source = """
-    ::defblock:alias, blocktype, name1=value1, name2=value2
+    ::defblock:alias, *subtype, name1=value1, name2=value2
 
-    [alias]
+    [*alias]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
+            children=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={"name1": "value1", "name2": "value2"},
         ),
     ]
 
 
 def test_block_definitions_local_kwargs_overwrite_defined_ones():
     source = """
-    ::defblock:alias, blocktype, name1=value1, name2=value2
+    ::defblock:alias, *subtype, name1=value1, name2=value2
 
-    [alias, name1=value99]
+    [*alias, name1=value99]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
+            children=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={"name1": "value99", "name2": "value2"},
         ),
     ]
 
 
 def test_block_definitions_local_args_are_used():
     # This is testing that local args are used even when
     # an alias is used. However, the test should fail as
     # blocks cannot have unnamed arguments.
 
     source = """
-    ::defblock:alias, blocktype, name1=value1, name2=value2
+    ::defblock:alias, *subtype, name1=value1, name2=value2
 
-    [alias, attr1, name1=value99]
+    [*alias, attr1, name1=value99]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
+            children=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=["attr1"],
             kwargs={"name1": "value99", "name2": "value2"},
         ),
     ]
 
 
 def test_block_definitions_unnamed_args_are_used_as_names():
     # This is testing that the unnamed args specified
     # in the block definition are used as names for the
     # unnamed arguments passed to the block.
 
     source = """
-    ::defblock:alias, blocktype, attr1, attr2
+    ::defblock:alias, *subtype, attr1, attr2
 
-    [alias, value1, value2]
+    [*alias, value1, value2]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
+            children=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={"attr1": "value1", "attr2": "value2"},
         ),
     ]
 
 
 def test_block_definitions_unnamed_and_named_args():
     # This is testing that any named are specifid in
     # the block definition is included in the block
     # kwargs if not redefined.
 
     source = """
-    ::defblock:alias, blocktype, attr1, attr2, attr3=value3
+    ::defblock:alias, *subtype, attr1, attr2, attr3=value3
 
-    [alias, value1, value2]
+    [*alias, value1, value2]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
+            children=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={"attr1": "value1", "attr2": "value2", "attr3": "value3"},
         ),
     ]
 
 
 def test_block_definitions_no_values_for_unnamed_args():
     # This is testing that is there are unnamed args in
     # the block definiton they should be given values
     # when the block is created.
 
     source = """
-    ::defblock:alias, blocktype, attr1, attr2, attr3=value3
+    ::defblock:alias, *subtype, attr1, attr2, attr3=value3
 
-    [alias]
+    [*alias]
     ----
     ----
     """
 
     with pytest.raises(ValueError):
         runner(source)
 
 
 def test_block_definitions_values_without_unnamed_args():
     # This is testing that values passed to the
     # block at creation time should match the parameters
     # specified in the block definition.
 
     source = """
-    ::defblock:alias, blocktype, attr3=value3
+    ::defblock:alias, *subtype, attr3=value3
 
-    [alias, value1, value2]
+    [*alias, value1, value2]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="blocktype",
-            content=[],
-            secondary_content=[],
+            subtype="subtype",
+            children=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=["value1", "value2"],
             kwargs={"attr3": "value3"},
         ),
     ]
+
+
+def test_block_definitions_named_override_unnamed():
+    # This is testing that values passed to the
+    # block at creation time should match the parameters
+    # specified in the block definition.
+
+    source = """
+    ::defblock:alias, *subtype, arg1, key1=value1
+
+    [*alias, value2, arg1=value1]
+    ----
+    ----
+    """
+
+    assert runner(source).nodes == [
+        BlockNode(
+            subtype="subtype",
+            children=[],
+            secondary_children=[],
+            classes=[],
+            title=None,
+            engine=None,
+            preprocessor="none",
+            args=["value2"],
+            kwargs={"arg1": "value1", "key1": "value1"},
+        ),
+    ]
```

### Comparing `mau-3.1.0/tests/parsers/main_parser/test_block_engine.py` & `mau-4.0.0/tests/parsers/test_create_toc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,180 +1,143 @@
-from unittest.mock import patch
-
-from mau.lexers.main_lexer import MainLexer
-from mau.nodes.page import BlockNode, CommandTocNode, HeaderNode
-from mau.parsers.main_parser import MainParser
-
-from tests.helpers import init_parser_factory, parser_runner_factory
-
-init_parser = init_parser_factory(MainLexer, MainParser)
-
-runner = parser_runner_factory(MainLexer, MainParser)
-
-
-@patch("mau.parsers.main_parser.header_anchor")
-def test_engine_mau(mock_header_anchor):
-    mock_header_anchor.return_value = "XXYY"
-
-    source = """
-    = Header 1
-
-    = Header 2
-
-    [sometype, engine=mau]
-    ----
-    = Header 3
-
-    = Header 4
-    ----
-    """
-
-    par = runner(source)
-
-    assert par.nodes == [
-        HeaderNode("Header 1", "1", "XXYY"),
-        HeaderNode("Header 2", "1", "XXYY"),
-        BlockNode(
-            blocktype="sometype",
-            content=[
-                HeaderNode("Header 3", "1", "XXYY"),
-                HeaderNode("Header 4", "1", "XXYY"),
+from mau.nodes.header import HeaderNode
+from mau.nodes.toc import TocEntryNode
+from mau.parsers.toc import create_toc
+
+
+def test_create_toc():
+    headers_list = [
+        HeaderNode("Header 1", "1", "header-1"),
+        HeaderNode("Header 1.1", "2", "header-1-1"),
+        HeaderNode("Header 1.2", "2", "header-1-2"),
+        HeaderNode("Header 2", "1", "header-2"),
+        HeaderNode("Header 2.1", "2", "header-2-1"),
+        HeaderNode("Header 2.1.1", "3", "header-2-1-1"),
+    ]
+
+    assert create_toc(headers_list) == [
+        TocEntryNode(
+            value="Header 1",
+            anchor="header-1",
+            children=[
+                TocEntryNode(
+                    value="Header 1.1",
+                    anchor="header-1-1",
+                    children=[],
+                ),
+                TocEntryNode(
+                    value="Header 1.2",
+                    anchor="header-1-2",
+                    children=[],
+                ),
+            ],
+        ),
+        TocEntryNode(
+            value="Header 2",
+            anchor="header-2",
+            children=[
+                TocEntryNode(
+                    value="Header 2.1",
+                    anchor="header-2-1",
+                    children=[
+                        TocEntryNode(
+                            value="Header 2.1.1",
+                            anchor="header-2-1-1",
+                            children=[],
+                        ),
+                    ],
+                ),
             ],
-            secondary_content=[],
-            classes=[],
-            title=None,
-            engine="mau",
-            preprocessor="none",
-            args=[],
-            kwargs={},
         ),
     ]
 
-    assert par.headers == [
-        HeaderNode("Header 1", "1", "XXYY"),
-        HeaderNode("Header 2", "1", "XXYY"),
-    ]
-
-
-@patch("mau.parsers.main_parser.header_anchor")
-def test_engine_mau_multiple_blocks_are_independent(mock_header_anchor):
-    mock_header_anchor.return_value = "XXYY"
-
-    source = """
-    = Header 1
-
-    = Header 2
-
-    [sometype, engine=mau]
-    ----
-    = Header 3
 
-    = Header 4
-    ----
-
-    [sometype, engine=mau]
-    ----
-    = Header 5
-
-    = Header 6
-    ----
-    """
-
-    par = runner(source)
-
-    assert par.nodes == [
-        HeaderNode("Header 1", "1", "XXYY"),
-        HeaderNode("Header 2", "1", "XXYY"),
-        BlockNode(
-            blocktype="sometype",
-            content=[
-                HeaderNode("Header 3", "1", "XXYY"),
-                HeaderNode("Header 4", "1", "XXYY"),
-            ],
-            secondary_content=[],
-            classes=[],
-            title=None,
-            engine="mau",
-            preprocessor="none",
-            args=[],
-            kwargs={},
-        ),
-        BlockNode(
-            blocktype="sometype",
-            content=[
-                HeaderNode("Header 5", "1", "XXYY"),
-                HeaderNode("Header 6", "1", "XXYY"),
+def test_create_toc_exclude_top_level():
+    headers_list = [
+        HeaderNode("Header 1", "1", "header-1", tags=["notoc"]),
+        HeaderNode("Header 1.1", "2", "header-1-1"),
+        HeaderNode("Header 1.2", "2", "header-1-2"),
+        HeaderNode("Header 2", "1", "header-2"),
+        HeaderNode("Header 2.1", "2", "header-2-1"),
+        HeaderNode("Header 2.1.1", "3", "header-2-1-1"),
+    ]
+
+    assert create_toc(headers_list, exclude_tag="notoc") == [
+        TocEntryNode(
+            value="Header 2",
+            anchor="header-2",
+            children=[
+                TocEntryNode(
+                    value="Header 2.1",
+                    anchor="header-2-1",
+                    children=[
+                        TocEntryNode(
+                            value="Header 2.1.1",
+                            anchor="header-2-1-1",
+                            children=[],
+                        ),
+                    ],
+                ),
             ],
-            secondary_content=[],
-            classes=[],
-            title=None,
-            engine="mau",
-            preprocessor="none",
-            args=[],
-            kwargs={},
         ),
     ]
 
-    assert par.headers == [
-        HeaderNode("Header 1", "1", "XXYY"),
-        HeaderNode("Header 2", "1", "XXYY"),
-    ]
-
-
-@patch("mau.parsers.main_parser.header_anchor")
-def test_engine_mau_toc(mock_header_anchor):
-    mock_header_anchor.return_value = "XXYY"
-
-    source = """
-    = Header 1
-
-    = Header 2
-
-    [sometype, engine=mau]
-    ----
-    = Header 3
 
-    = Header 4
-
-    ::toc:
-    ----
-
-    ::toc:
-    """
-
-    par = runner(source)
-
-    assert par.nodes == [
-        HeaderNode("Header 1", "1", "XXYY"),
-        HeaderNode("Header 2", "1", "XXYY"),
-        BlockNode(
-            blocktype="sometype",
-            content=[
-                HeaderNode("Header 3", "1", "XXYY"),
-                HeaderNode("Header 4", "1", "XXYY"),
-                CommandTocNode(
-                    [
-                        HeaderNode("Header 3", "1", "XXYY"),
-                        HeaderNode("Header 4", "1", "XXYY"),
-                    ]
+def test_create_toc_exclude_lower_level():
+    headers_list = [
+        HeaderNode("Header 1", "1", "header-1"),
+        HeaderNode("Header 1.1", "2", "header-1-1"),
+        HeaderNode("Header 1.2", "2", "header-1-2"),
+        HeaderNode("Header 2", "1", "header-2"),
+        HeaderNode("Header 2.1", "2", "header-2-1", tags=["notoc"]),
+        HeaderNode("Header 2.1.1", "3", "header-2-1-1"),
+    ]
+
+    assert create_toc(headers_list, exclude_tag="notoc") == [
+        TocEntryNode(
+            value="Header 1",
+            anchor="header-1",
+            children=[
+                TocEntryNode(
+                    value="Header 1.1",
+                    anchor="header-1-1",
+                    children=[],
+                ),
+                TocEntryNode(
+                    value="Header 1.2",
+                    anchor="header-1-2",
+                    children=[],
                 ),
             ],
-            secondary_content=[],
-            classes=[],
-            title=None,
-            engine="mau",
-            preprocessor="none",
-            args=[],
-            kwargs={},
-        ),
-        CommandTocNode(
-            [
-                HeaderNode("Header 1", "1", "XXYY"),
-                HeaderNode("Header 2", "1", "XXYY"),
-            ]
+        ),
+        TocEntryNode(
+            value="Header 2",
+            anchor="header-2",
+            children=[],
         ),
     ]
 
-    assert par.headers == [
-        HeaderNode("Header 1", "1", "XXYY"),
-        HeaderNode("Header 2", "1", "XXYY"),
+
+def test_create_toc_orphan_nodes():
+    headers_list = [
+        HeaderNode("Header 1", "1", "header-1"),
+        HeaderNode("Header 1.1.1", "3", "header-1-1-1"),
+        HeaderNode("Header 1.2", "2", "header-1-2"),
+    ]
+
+    assert create_toc(headers_list) == [
+        TocEntryNode(
+            value="Header 1",
+            anchor="header-1",
+            children=[
+                TocEntryNode(
+                    value="Header 1.1.1",
+                    anchor="header-1-1-1",
+                    children=[],
+                ),
+                TocEntryNode(
+                    value="Header 1.2",
+                    anchor="header-1-2",
+                    children=[],
+                ),
+            ],
+        ),
     ]
```

### Comparing `mau-3.1.0/tests/parsers/main_parser/test_block_other.py` & `mau-4.0.0/tests/parsers/main_parser/test_block_other.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,82 @@
 from mau.lexers.main_lexer import MainLexer
-from mau.nodes.inline import SentenceNode, StyleNode, TextNode
-from mau.nodes.page import BlockNode, ParagraphNode
+from mau.nodes.block import BlockNode
+from mau.nodes.inline import StyleNode, TextNode
+from mau.nodes.paragraph import ParagraphNode
 from mau.parsers.main_parser import MainParser
 
 from tests.helpers import init_parser_factory, parser_runner_factory
 
 init_parser = init_parser_factory(MainLexer, MainParser)
 
 runner = parser_runner_factory(MainLexer, MainParser)
 
 
 def test_admonition():
     source = """
-    [admonition,someclass,someicon,somelabel]
+    [*admonition,someclass,someicon]
     ----
     Content
     ----
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="admonition",
-            content=[
+            subtype="admonition",
+            children=[
                 ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode("Content"),
-                        ]
-                    )
+                    children=[
+                        TextNode("Content"),
+                    ]
                 ),
             ],
-            secondary_content=[],
+            secondary_children=[],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
-            kwargs={"class": "someclass", "icon": "someicon", "label": "somelabel"},
+            kwargs={"class": "someclass", "icon": "someicon"},
         )
     ]
 
 
 def test_parse_block_quote_attribution_in_secondary_content():
     source = """
-    [quote]
+    [*quote]
     ----
     Learn about the Force, Luke.
     ----
     _Star Wars_, 1977
     """
 
     assert runner(source).nodes == [
         BlockNode(
-            blocktype="quote",
-            content=[
+            subtype="quote",
+            children=[
                 ParagraphNode(
-                    SentenceNode(
-                        [
-                            TextNode("Learn about the Force, Luke."),
-                        ]
-                    )
+                    children=[
+                        TextNode("Learn about the Force, Luke."),
+                    ]
                 ),
             ],
-            secondary_content=[
+            secondary_children=[
                 ParagraphNode(
-                    SentenceNode(
-                        [
-                            StyleNode(
-                                "underscore",
-                                SentenceNode(
-                                    [
-                                        TextNode("Star Wars"),
-                                    ]
-                                ),
-                            ),
-                            TextNode(", 1977"),
-                        ]
-                    )
+                    children=[
+                        StyleNode(
+                            value="underscore",
+                            children=[
+                                TextNode("Star Wars"),
+                            ],
+                        ),
+                        TextNode(", 1977"),
+                    ]
                 ),
             ],
             classes=[],
             title=None,
-            engine="default",
+            engine=None,
             preprocessor="none",
             args=[],
             kwargs={},
         )
     ]
```

### Comparing `mau-3.1.0/tests/parsers/main_parser/test_block_source.py` & `mau-4.0.0/tests/parsers/main_parser/test_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import pytest
 from mau.errors import MauErrorException
 from mau.lexers.main_lexer import MainLexer
-from mau.nodes.inline import SentenceNode, TextNode, RawNode
+from mau.nodes.inline import RawNode, SentenceNode, TextNode
 from mau.nodes.source import CalloutNode, CalloutsEntryNode, SourceNode
 from mau.parsers.main_parser import MainParser
 
 from tests.helpers import init_parser_factory, parser_runner_factory
 
 init_parser = init_parser_factory(MainLexer, MainParser)
 
 runner = parser_runner_factory(MainLexer, MainParser)
 
 
 def test_source_empty_block():
     source = """
-    [source]
+    [*source]
     ----
     ----
     """
 
     assert runner(source).nodes == [
-        SourceNode(blocktype="default", code=[]),
+        SourceNode(subtype=None, code=[]),
     ]
 
 
 def test_source_language():
     source = """
-    [source, python]
+    [*source, python]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         SourceNode(code=[], language="python"),
     ]
 
 
 def test_source_contains_mau():
     source = """
-    [source, callouts="|"]
+    [*source, callouts="|"]
     ----
     // A comment
     ::toc:
     ----
     """
 
     assert runner(source).nodes == [
@@ -53,15 +53,15 @@
             ],
         ),
     ]
 
 
 def test_source_removes_escape_from_directive_like_text():
     source = r"""
-    [source]
+    [*source]
     ----
     \::#looks like a directive
     ----
     """
 
     assert runner(source).nodes == [
         SourceNode(
@@ -70,15 +70,15 @@
             ],
         ),
     ]
 
 
 def test_source_with_code():
     source = """
-    [source]
+    [*source]
     ----
     import os
 
     print(os.environ["HOME"])
     ----
     """
 
@@ -91,39 +91,39 @@
             ],
         ),
     ]
 
 
 def test_source_explicit_engine():
     source = """
-    [myblock, engine=source, language=somelang]
+    [*myblock, engine=source, language=somelang]
     ----
     import os
 
     print(os.environ["HOME"])
     ----
     """
 
     assert runner(source).nodes == [
         SourceNode(
-            blocktype="myblock",
+            subtype="myblock",
             language="somelang",
             code=[
                 RawNode("import os"),
                 RawNode(""),
                 RawNode('print(os.environ["HOME"])'),
             ],
         ),
     ]
 
 
 def test_source_with_title():
     source = """
     . Title
-    [source, somelang]
+    [*source, somelang]
     ----
     import os
 
     print(os.environ["HOME"])
     ----
     """
 
@@ -131,22 +131,22 @@
         SourceNode(
             language="somelang",
             code=[
                 RawNode("import os"),
                 RawNode(""),
                 RawNode('print(os.environ["HOME"])'),
             ],
-            title=SentenceNode([TextNode("Title")]),
+            title=SentenceNode(children=[TextNode("Title")]),
         ),
     ]
 
 
 def test_source_ignores_mau_syntax():
     source = """
-    [source]
+    [*source]
     ----
     :answer:42
     The answer is {answer}
     ----
     """
 
     assert runner(source).nodes == [
@@ -157,15 +157,15 @@
             ],
         ),
     ]
 
 
 def test_source_respects_spaces_and_indentation():
     source = """
-    [source]
+    [*source]
     ----
       //    This is a comment
     ----
     """
 
     assert runner(source).nodes == [
         SourceNode(
@@ -174,15 +174,15 @@
             ],
         ),
     ]
 
 
 def test_source_callouts():
     source = """
-    [source, somelang, callouts=":"]
+    [*source, somelang, callouts=":"]
     ----
     import sys
     import os:imp:
 
     print(os.environ["HOME"]):env:
     ----
     imp: This is an import
@@ -205,15 +205,15 @@
             ],
         ),
     ]
 
 
 def test_source_callouts_possible_clash():
     source = """
-    [source, somelang, callouts=":"]
+    [*source, somelang, callouts=":"]
     ----
     import sys
     import: os:imp:
 
     print(os.environ["HOME"]):env:
     ----
     imp: This is an import
@@ -236,15 +236,15 @@
             ],
         ),
     ]
 
 
 def test_source_callouts_one_single_marker_is_skipped():
     source = """
-    [source, somelang, callouts=":"]
+    [*source, somelang, callouts=":"]
     ----
     def something:
         print("AAA")
     ----
     """
 
     assert runner(source).nodes == [
@@ -258,15 +258,15 @@
             callouts=[],
         ),
     ]
 
 
 def test_source_callouts_custom_delimiter():
     source = """
-    [source, language=somelang, callouts="|"]
+    [*source, language=somelang, callouts="|"]
     ----
     import sys
     import os|imp|
 
     print(os.environ["HOME"])|env|
     ----
     """
@@ -303,15 +303,15 @@
 
     with pytest.raises(MauErrorException):
         runner(source)
 
 
 def test_source_highlights():
     source = """
-    [source, language=somelang]
+    [*source, language=somelang]
     ----
     import sys
     import os:@:
 
     print(os.environ["HOME"]):@:
     ----
     """
@@ -328,15 +328,15 @@
             highlights=[1, 3],
         ),
     ]
 
 
 def test_source_highlights_custom_marker():
     source = """
-    [source, language=somelang, highlight="#"]
+    [*source, language=somelang, highlight="#"]
     ----
     import sys
     import os:#:
 
     print(os.environ["HOME"]):#:
     ----
     """
@@ -353,19 +353,19 @@
             highlights=[1, 3],
         ),
     ]
 
 
 def test_engine_source_language_is_reset():
     source = """
-    [source, python]
+    [*source, python]
     ----
     ----
 
-    [source]
+    [*source]
     ----
     ----
     """
 
     assert runner(source).nodes == [
         SourceNode(
             language="python",
```

### Comparing `mau-3.1.0/tests/parsers/main_parser/test_include_content.py` & `mau-4.0.0/tests/parsers/main_parser/test_content.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,112 +1,113 @@
 from mau.lexers.main_lexer import MainLexer
+from mau.nodes.content import ContentImageNode, ContentNode
 from mau.nodes.inline import SentenceNode, TextNode
-from mau.nodes.page import ContentImageNode, ContentNode
 from mau.parsers.main_parser import MainParser
 
 from tests.helpers import init_parser_factory, parser_runner_factory
 
 init_parser = init_parser_factory(MainLexer, MainParser)
 
 runner = parser_runner_factory(MainLexer, MainParser)
 
 
-def test_include_standard_content():
+def test_include_content():
     source = """
-    << somecontent:attr1,attr2,#atag,attr3=value3
+    ["text", #tag1, key1=value1, key2=value2]
+    << ctype1:/path/to/it,/another/path
     """
 
     assert runner(source).nodes == [
         ContentNode(
-            "somecontent",
-            args=["attr1", "attr2"],
-            tags=["atag"],
-            kwargs={"attr3": "value3"},
+            uris=["/path/to/it", "/another/path"],
+            content_type="ctype1",
+            args=["text"],
+            tags=["tag1"],
+            kwargs={"key1": "value1", "key2": "value2"},
         )
     ]
 
 
-def test_include_image_with_only_path():
-    source = """
-    << image:/path/to/it.jpg
-    """
-
-    assert runner(source).nodes == [ContentImageNode("/path/to/it.jpg")]
-
-
-def test_include_image_with_http():
+def test_include_content_with_subtype():
     source = """
-    << image:https:///some.domain/path/to/it.jpg
+    [*subtype1]
+    << ctype1:/path/to/it
     """
 
     assert runner(source).nodes == [
-        ContentImageNode("https:///some.domain/path/to/it.jpg")
+        ContentNode(
+            uris=["/path/to/it"],
+            content_type="ctype1",
+            subtype="subtype1",
+            args=[],
+            tags=[],
+            kwargs={},
+        )
     ]
 
 
-def test_include_image_with_alt_text():
+def test_include_image_with_only_path():
     source = """
-    << image:/path/to/it.jpg,alt_text="This is a beautiful image"
+    << image:/path/to/it.jpg
     """
 
-    assert runner(source).nodes == [
-        ContentImageNode("/path/to/it.jpg", alt_text="This is a beautiful image")
-    ]
+    assert runner(source).nodes == [ContentImageNode("/path/to/it.jpg")]
 
 
-def test_include_image_with_classes():
+def test_include_image_with_http():
     source = """
-    << image:/path/to/it.jpg,classes="class1,class2"
+    << image:https:///some.domain/path/to/it.jpg
     """
 
     assert runner(source).nodes == [
-        ContentImageNode("/path/to/it.jpg", classes=["class1", "class2"])
+        ContentImageNode("https:///some.domain/path/to/it.jpg")
     ]
 
 
 def test_include_image_with_arguments():
     source = """
-   << image:/path/to/it.jpg,"alternate text", argument1=value1,argument2=value2
-   """
+    ["alt text", #tag1, key1=value1, key2=value2, classes="class1,class2"]
+    << image:/path/to/it.jpg,
+    """
 
     assert runner(source).nodes == [
         ContentImageNode(
             "/path/to/it.jpg",
             args=[],
-            kwargs={"argument1": "value1", "argument2": "value2"},
-            alt_text="alternate text",
+            tags=["tag1"],
+            kwargs={"key1": "value1", "key2": "value2"},
+            alt_text="alt text",
+            classes=["class1", "class2"],
         )
     ]
 
 
-def test_include_image_with_tags():
+def test_include_image_with_title():
     source = """
-   << image:/path/to/it.jpg,"alternate text", #tag1, #tag2, argument1=value1,argument2=value2
-   """
+    . A nice caption
+    << image:/path/to/it.jpg
+    """
 
     assert runner(source).nodes == [
         ContentImageNode(
             "/path/to/it.jpg",
-            args=[],
-            tags=["tag1", "tag2"],
-            kwargs={"argument1": "value1", "argument2": "value2"},
-            alt_text="alternate text",
+            title=SentenceNode(
+                children=[
+                    TextNode("A nice caption"),
+                ]
+            ),
         )
     ]
 
 
-def test_include_image_with_title():
+def test_include_image_with_subtype():
     source = """
-    . A nice caption
+    [*subtype1]
     << image:/path/to/it.jpg
     """
 
     assert runner(source).nodes == [
         ContentImageNode(
             "/path/to/it.jpg",
-            title=SentenceNode(
-                [
-                    TextNode("A nice caption"),
-                ]
-            ),
-        )
+            subtype="subtype1",
+        ),
     ]
```

### Comparing `mau-3.1.0/tests/parsers/main_parser/test_variables.py` & `mau-4.0.0/tests/parsers/main_parser/test_variables.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,53 @@
 from mau.lexers.main_lexer import MainLexer
-from mau.nodes.inline import SentenceNode, StyleNode, TextNode
-from mau.nodes.page import ParagraphNode
+from mau.nodes.inline import StyleNode, TextNode
+from mau.nodes.paragraph import ParagraphNode
 from mau.parsers.main_parser import MainParser
 
 from tests.helpers import init_parser_factory, parser_runner_factory
 
 init_parser = init_parser_factory(MainLexer, MainParser)
 
 runner = parser_runner_factory(MainLexer, MainParser)
 
 
-def test_parse_variable_definition_without_value_is_loaded_as_boolean():
+def test_parse_variable_definition_without_value_is_empty():
     source = ":attr:"
     parser = runner(source)
 
     assert parser.nodes == []
+    assert parser.environment.asdict() == {"attr": ""}
+
+
+def test_parse_variable_definition_with_plus_is_true():
+    source = ":+attr:"
+    parser = runner(source)
+
+    assert parser.nodes == []
     assert parser.environment.asdict() == {"attr": True}
 
 
-def test_parse_variable_definition_without_value_can_be_negated():
-    source = ":!attr:"
+def test_parse_variable_definition_with_minus_is_false():
+    source = ":-attr:"
     parser = runner(source)
 
     assert parser.nodes == []
     assert parser.environment.asdict() == {"attr": False}
 
 
-def test_parse_variable_definition_negative_flag_ignores_value():
-    source = ":!attr:42"
+def test_parse_variable_definition_flag_plus_ignores_value():
+    source = ":+attr:42"
+    parser = runner(source)
+
+    assert parser.nodes == []
+    assert parser.environment.asdict() == {"attr": True}
+
+
+def test_parse_variable_definition_flag_minus_ignores_value():
+    source = ":-attr:42"
     parser = runner(source)
 
     assert parser.nodes == []
     assert parser.environment.asdict() == {"attr": False}
 
 
 def test_parse_variable_definition_with_value_is_loaded():
@@ -75,17 +91,15 @@
     The answer is {answer}
     """
 
     parser = runner(source)
 
     assert parser.nodes == [
         ParagraphNode(
-            SentenceNode(
-                [TextNode("The answer is 42")],
-            )
+            children=[TextNode("The answer is 42")],
         )
     ]
 
 
 def test_variable_replacement_with_namespace():
     source = """
     :mau.answer:42
@@ -93,33 +107,29 @@
     The answer is {mau.answer}
     """
 
     parser = runner(source)
 
     assert parser.nodes == [
         ParagraphNode(
-            SentenceNode(
-                [TextNode("The answer is 42")],
-            )
+            children=[TextNode("The answer is 42")],
         )
     ]
 
 
 def test_variable_definition_escape():
     source = r"""
     \:answer:42
     """
 
     parser = runner(source)
 
     assert parser.nodes == [
         ParagraphNode(
-            SentenceNode(
-                [TextNode(":answer:42")],
-            )
+            children=[TextNode(":answer:42")],
         )
     ]
 
 
 def test_skip_variable_replacement():
     source = r"""
     :answer:42
@@ -127,17 +137,15 @@
     The answer is \{answer\}
     """
 
     parser = runner(source)
 
     assert parser.nodes == [
         ParagraphNode(
-            SentenceNode(
-                [TextNode("The answer is {answer}")],
-            )
+            children=[TextNode("The answer is {answer}")],
         )
     ]
 
 
 def test_variables_are_preprocessed():
     source = r"""
     :important:*IMPORTANT*
@@ -145,22 +153,35 @@
     This is {important}
     """
 
     parser = runner(source)
 
     assert parser.nodes == [
         ParagraphNode(
-            SentenceNode(
-                [
-                    TextNode("This is "),
-                    StyleNode(
-                        "star",
-                        SentenceNode(
-                            [
-                                TextNode("IMPORTANT"),
-                            ]
-                        ),
-                    ),
-                ],
-            )
+            children=[
+                TextNode("This is "),
+                StyleNode(
+                    value="star",
+                    children=[
+                        TextNode("IMPORTANT"),
+                    ],
+                ),
+            ],
+        )
+    ]
+
+
+def test_variable_replacement_in_variable():
+    source = """
+    :answer:42
+    :sentence:The answer is {answer}
+
+    {sentence}
+    """
+
+    parser = runner(source)
+
+    assert parser.nodes == [
+        ParagraphNode(
+            children=[TextNode("The answer is 42")],
         )
     ]
```

### Comparing `mau-3.1.0/tests/parsers/test_arguments_parser.py` & `mau-4.0.0/tests/parsers/test_arguments_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+from mau.environment.environment import Environment
 from mau.errors import MauErrorException
 from mau.lexers.arguments_lexer import ArgumentsLexer
 from mau.nodes.arguments import NamedArgumentNode, UnnamedArgumentNode
 from mau.parsers.arguments import set_names_and_defaults
 from mau.parsers.arguments_parser import ArgumentsParser
 
 from tests.helpers import parser_runner_factory
@@ -233,147 +234,183 @@
     )
 
     assert args == []
     assert kwargs == {"attr1": "value1", "attr2": "value2", "attr3": "value3"}
 
 
 def test_apply_prototype_unnamed_and_named_arguments():
-    parser = ArgumentsParser(tokens=[])
+    parser = ArgumentsParser(Environment())
 
     parser.nodes = [
         UnnamedArgumentNode("value1"),
         UnnamedArgumentNode("value2"),
         NamedArgumentNode("attr5", "value5"),
     ]
 
-    args, kwargs, tags = parser.process_arguments()
+    args, kwargs, tags, subtype = parser.process_arguments()
 
     args, kwargs = set_names_and_defaults(
         args, kwargs, ["attr1", "attr2"], {"attr3": "value3"}
     )
 
     assert args == []
     assert kwargs == {
         "attr1": "value1",
         "attr2": "value2",
         "attr3": "value3",
         "attr5": "value5",
     }
     assert tags == []
+    assert subtype is None
 
 
 def test_apply_prototype_clash_between_default_value_and_named_value():
-    parser = ArgumentsParser(tokens=[])
+    parser = ArgumentsParser(Environment())
 
     parser.nodes = [
         UnnamedArgumentNode("value1"),
         UnnamedArgumentNode("value2"),
         NamedArgumentNode("attr3", "value5"),
     ]
 
-    args, kwargs, tags = parser.process_arguments()
+    args, kwargs, tags, subtype = parser.process_arguments()
 
     args, kwargs = set_names_and_defaults(
         args, kwargs, ["attr1", "attr2"], {"attr3": "value3"}
     )
 
     assert args == []
     assert kwargs == {
         "attr1": "value1",
         "attr2": "value2",
         "attr3": "value5",
     }
     assert tags == []
+    assert subtype is None
 
 
 def test_apply_prototype_clash_between_positional_value_and_named_value():
-    parser = ArgumentsParser(tokens=[])
+    parser = ArgumentsParser(Environment())
 
     parser.nodes = [
         UnnamedArgumentNode("value1"),
         UnnamedArgumentNode("value2"),
         NamedArgumentNode("attr1", "value5"),
     ]
 
-    args, kwargs, tags = parser.process_arguments()
+    args, kwargs, tags, subtype = parser.process_arguments()
 
     args, kwargs = set_names_and_defaults(
         args, kwargs, ["attr1", "attr2"], {"attr3": "value3"}
     )
 
-    assert args == []
+    assert args == ["value2"]
     assert kwargs == {
-        "attr1": "value1",
-        "attr2": "value2",
+        "attr1": "value5",
+        "attr2": "value1",
         "attr3": "value3",
     }
     assert tags == []
+    assert subtype is None
 
 
 def test_apply_prototype_clash_in_prototype():
-    parser = ArgumentsParser(tokens=[])
+    parser = ArgumentsParser(Environment())
 
     parser.nodes = [
         UnnamedArgumentNode("value1"),
         UnnamedArgumentNode("value2"),
         NamedArgumentNode("attr3", "value3"),
     ]
 
-    args, kwargs, tags = parser.process_arguments()
+    args, kwargs, tags, subtype = parser.process_arguments()
 
     args, kwargs = set_names_and_defaults(
         args, kwargs, ["attr1", "attr2"], {"attr1": "value7"}
     )
 
     assert args == []
     assert kwargs == {
         "attr1": "value1",
         "attr2": "value2",
         "attr3": "value3",
     }
     assert tags == []
+    assert subtype is None
 
 
 def test_apply_prototype_positional_values_not_provided():
-    parser = ArgumentsParser(tokens=[])
+    parser = ArgumentsParser(Environment())
 
     parser.nodes = [UnnamedArgumentNode("value1")]
 
-    args, kwargs, _ = parser.process_arguments()
+    args, kwargs, _, _ = parser.process_arguments()
 
     with pytest.raises(ValueError):
         set_names_and_defaults(args, kwargs, ["attr1", "attr2"], {"attr3": "value3"})
 
 
 def test_apply_prototype_positional_values_without_name():
-    parser = ArgumentsParser(tokens=[])
+    parser = ArgumentsParser(Environment())
 
     parser.nodes = [UnnamedArgumentNode("value1"), UnnamedArgumentNode("value2")]
 
-    args, kwargs, tags = parser.process_arguments()
+    args, kwargs, tags, subtype = parser.process_arguments()
 
     args, kwargs = set_names_and_defaults(args, kwargs, ["attr1"], {"attr3": "value3"})
 
     assert args == ["value2"]
     assert kwargs == {
         "attr1": "value1",
         "attr3": "value3",
     }
     assert tags == []
+    assert subtype is None
 
 
 def test_apply_prototype_missing_positional_with_default():
-    parser = ArgumentsParser(tokens=[])
+    parser = ArgumentsParser(Environment())
 
     parser.nodes = [
         NamedArgumentNode("attr1", "value5"),
     ]
 
-    args, kwargs, tags = parser.process_arguments()
+    args, kwargs, tags, subtype = parser.process_arguments()
 
     args, kwargs = set_names_and_defaults(args, kwargs, ["attr1"])
 
     assert args == []
     assert kwargs == {
         "attr1": "value5",
     }
     assert tags == []
+    assert subtype is None
+
+
+def test_tags_and_subtype():
+    parser = ArgumentsParser(Environment())
+
+    parser.nodes = [
+        UnnamedArgumentNode("value1"),
+        UnnamedArgumentNode("#value2"),
+        UnnamedArgumentNode("*value3"),
+    ]
+
+    args, kwargs, tags, subtype = parser.process_arguments()
+
+    assert args == ["value1"]
+    assert kwargs == {}
+    assert tags == ["value2"]
+    assert subtype == "value3"
+
+
+def test_multiple_subtypes():
+    parser = ArgumentsParser(Environment())
+
+    parser.nodes = [
+        UnnamedArgumentNode("value1"),
+        UnnamedArgumentNode("*value2"),
+        UnnamedArgumentNode("*value3"),
+    ]
+
+    with pytest.raises(MauErrorException):
+        parser.process_arguments()
```

### Comparing `mau-3.1.0/tests/parsers/test_base_parser.py` & `mau-4.0.0/tests/parsers/test_base_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from unittest.mock import Mock
 
 import pytest
+from mau.environment.environment import Environment
 from mau.errors import MauErrorException
 from mau.lexers.base_lexer import BaseLexer, TokenTypes
 from mau.parsers.base_parser import BaseParser, TokenError
 from mau.tokens.tokens import Token
 
 from tests.helpers import init_parser_factory
 
 init_parser = init_parser_factory(BaseLexer, BaseParser)
 
 
 def test_save():
-    parser = BaseParser(tokens=[Token(TokenTypes.EOF)])
+    parser = BaseParser(Environment())
     node = Mock()
     parser._save(node)
 
     assert parser.nodes == [node]
 
 
 def test_initial_state():
-    parser = BaseParser(tokens=[Token(TokenTypes.EOF)])
+    parser = BaseParser(Environment())
+    parser.tokens = [Token(TokenTypes.EOF)]
 
     assert parser.index == -1
     assert parser._current_token == Token(TokenTypes.EOF)
 
 
 def test_load():
     parser = init_parser("\n")
 
     assert parser.index == -1
     assert parser._current_token == Token(TokenTypes.EOF)
 
 
 def test_get_token_without_load():
-    parser = BaseParser(tokens=[Token(TokenTypes.EOF)])
+    parser = BaseParser(Environment())
+    parser.tokens = [Token(TokenTypes.EOF)]
 
     assert parser._get_token() == Token(TokenTypes.EOF)
 
 
 def test_get_token():
     parser = init_parser("")
 
@@ -114,43 +117,47 @@
 
     with pytest.raises(TokenError):
         parser._get_token(TokenTypes.TEXT, check=lambda x: x == "foobar")
 
 
 def test_check_current_token():
     parser = init_parser("Some text\nSome other text")
+
     parser._get_token()
 
     assert parser._check_current_token(TokenTypes.TEXT) == Token(
         TokenTypes.TEXT, "Some text"
     )
 
     # check_current_token doesn't advance the index
     assert parser._get_token() == Token(TokenTypes.EOL)
 
 
 def test_check_current_token_raises_exception():
     parser = init_parser("Some text\nSome other text")
+
     parser._get_token()
 
     with pytest.raises(TokenError):
         parser._check_current_token(TokenTypes.EOF)
 
 
 def test_check_current_token_value():
     parser = init_parser("Some text\nSome other text")
+
     parser._get_token()
 
     assert parser._check_current_token(TokenTypes.TEXT, "Some text") == Token(
         TokenTypes.TEXT, "Some text"
     )
 
 
 def test_check_current_token_with_function():
     parser = init_parser("Some text\nSome other text")
+
     parser._get_token()
 
     assert parser._check_current_token(
         TokenTypes.TEXT, check=lambda x: x == "Some text"
     ) == Token(TokenTypes.TEXT, "Some text")
 
 
@@ -392,33 +399,34 @@
         Token(TokenTypes.LITERAL, "\\"),
         Token(TokenTypes.LITERAL, "["),
     ]
 
 
 def test_error():
     parser = init_parser("Some text")
+
     parser._get_token()
     parser._get_token()
 
     with pytest.raises(MauErrorException) as exception:
         parser._error()
 
 
 def test_error_with_message():
     parser = init_parser("Some text")
+
     parser._get_token()
     parser._get_token()
 
     with pytest.raises(MauErrorException) as exception:
         parser._error("Some message")
 
     assert exception.value.error.message == "Some message"
 
 
 def test_unknown_token():
-    unknown = Token("UNKNOWN")
-    parser = BaseParser(tokens=[unknown])
+    parser = BaseParser(Environment())
 
     with pytest.raises(MauErrorException) as exception:
-        parser.parse()
+        parser.parse([Token("UNKNOWN")])
 
     assert exception.value.error.message == "Cannot parse token"
```

### Comparing `mau-3.1.0/tests/parsers/test_preprocess_variables_parser.py` & `mau-4.0.0/tests/parsers/test_preprocess_variables_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
+from mau.environment.environment import Environment
 from mau.errors import MauErrorException
 from mau.lexers.preprocess_variables_lexer import PreprocessVariablesLexer
 from mau.nodes.inline import TextNode
-from mau.parsers.environment import Environment
 from mau.parsers.preprocess_variables_parser import PreprocessVariablesParser
 
 from tests.helpers import init_parser_factory, parser_runner_factory
 
 init_parser = init_parser_factory(PreprocessVariablesLexer, PreprocessVariablesParser)
 runner = parser_runner_factory(PreprocessVariablesLexer, PreprocessVariablesParser)
 
@@ -35,27 +35,27 @@
     source = "This is {attr"
     result = runner(source, environment=Environment({"attr": "5"}))
 
     assert result.nodes == [TextNode("This is {attr")]
 
 
 def test_replace_variable_with_namespace():
-    source = "This is number {config.attr}"
+    source = "This is number {app.attr}"
     result = runner(
         source,
-        environment=Environment({"config": {"attr": "5"}}),
+        environment=Environment({"app": {"attr": "5"}}),
     )
 
     assert result.nodes == [TextNode("This is number 5")]
 
 
 def test_replace_boolean():
     result = runner("This flag is {flag}", environment=Environment({"flag": True}))
 
-    assert result.nodes == [TextNode("This flag is True")]
+    assert result.nodes == [TextNode("This flag is ")]
 
 
 def test_escape_curly_braces():
     source = r"This is \{attr\}"
     result = runner(source, environment=Environment({"attr": "5"}))
 
     assert result.nodes == [TextNode("This is {attr}")]
```

### Comparing `mau-3.1.0/tests/text_buffer/test_text_buffer.py` & `mau-4.0.0/tests/text_buffer/test_text_buffer.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/tests/tokens/test_tokens.py` & `mau-4.0.0/tests/tokens/test_tokens.py`

 * *Files identical despite different names*

### Comparing `mau-3.1.0/tests/visitors/base_visitor/test_inline_nodes.py` & `mau-4.0.0/tests/visitors/base_visitor/test_block.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,390 +1,257 @@
-import pytest
-from mau.errors import MauErrorException
-from mau.nodes.footnotes import FootnoteNode
-from mau.nodes.inline import (
-    ClassNode,
-    ImageNode,
-    LinkNode,
-    ListItemNode,
-    MacroNode,
-    SentenceNode,
-    StyleNode,
-    RawNode,
-    TextNode,
-    VerbatimNode,
-)
-from mau.nodes.references import ReferenceNode
+from mau.environment.environment import Environment
+from mau.nodes.block import BlockGroupNode, BlockNode
+from mau.nodes.inline import SentenceNode, TextNode
+from mau.nodes.paragraph import ParagraphNode
 from mau.visitors.base_visitor import BaseVisitor
 
 
-def test_no_node():
-    visitor = BaseVisitor()
+def test_block_node_standard_block_template():
+    visitor = BaseVisitor(Environment())
 
-    result = visitor.visit(None)
-
-    assert result == {}
-
-
-def test_unknown_node():
-    visitor = BaseVisitor()
-
-    node = TextNode("Just some text.")
-    node.node_type = "unknown"
-
-    with pytest.raises(MauErrorException):
-        visitor.visit(node)
-
-
-def test_raw_node():
-    visitor = BaseVisitor()
-
-    node = RawNode("Just some text.")
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "raw",
-            "value": "Just some text.",
-        }
-    }
-
-
-def test_text_node():
-    visitor = BaseVisitor()
-
-    node = TextNode("Just some text.")
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "text",
-            "value": "Just some text.",
-        }
-    }
-
-
-def test_verbatim_node():
-    visitor = BaseVisitor()
-
-    node = VerbatimNode("Just some text.")
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "verbatim",
-            "value": "Just some text.",
-        }
-    }
-
-
-def test_sentence_node():
-    visitor = BaseVisitor()
-
-    node = SentenceNode(
-        [
-            TextNode("Just some text. "),
-            TextNode("More text."),
-        ]
+    node = BlockNode(
+        subtype="someblock",
+        children=[
+            ParagraphNode(
+                children=[
+                    TextNode("my content"),
+                ]
+            ),
+        ],
+        secondary_children=[
+            ParagraphNode(
+                children=[
+                    TextNode("my secondary content"),
+                ]
+            ),
+        ],
+        classes=["class1", "class2"],
+        title=SentenceNode(children=[TextNode("sometitle")]),
+        engine="someengine",
+        preprocessor="somepreprocessor",
+        args=["arg1", "arg2"],
+        kwargs={"key1": "value1"},
+        tags=["tag1", "tag2"],
     )
 
     result = visitor.visit(node)
 
     assert result == {
         "data": {
-            "type": "sentence",
+            "type": "block",
+            "subtype": "someblock",
             "content": [
                 {
                     "data": {
-                        "type": "text",
-                        "value": "Just some text. ",
+                        "type": "paragraph",
+                        "content": [
+                            {
+                                "data": {
+                                    "type": "text",
+                                    "value": "my content",
+                                    "args": [],
+                                    "kwargs": {},
+                                    "subtype": None,
+                                    "tags": [],
+                                }
+                            }
+                        ],
+                        "title": {},
+                        "args": [],
+                        "kwargs": {},
+                        "subtype": None,
+                        "tags": [],
                     }
-                },
+                }
+            ],
+            "secondary_content": [
                 {
                     "data": {
-                        "type": "text",
-                        "value": "More text.",
-                    }
-                },
-            ],
-        }
-    }
-
-
-def test_style_node_star():
-    visitor = BaseVisitor()
-
-    node = StyleNode("star", SentenceNode([TextNode("Just some text.")]))
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "style",
-            "content": {
-                "data": {
-                    "type": "sentence",
-                    "content": [
-                        {
-                            "data": {
-                                "type": "text",
-                                "value": "Just some text.",
+                        "type": "paragraph",
+                        "content": [
+                            {
+                                "data": {
+                                    "type": "text",
+                                    "value": "my secondary content",
+                                    "args": [],
+                                    "kwargs": {},
+                                    "subtype": None,
+                                    "tags": [],
+                                }
                             }
-                        },
-                    ],
+                        ],
+                        "title": {},
+                        "args": [],
+                        "kwargs": {},
+                        "subtype": None,
+                        "tags": [],
+                    }
                 }
-            },
-            "value": "star",
-        }
-    }
-
-
-def test_style_node_underscore():
-    visitor = BaseVisitor()
-
-    node = StyleNode("underscore", SentenceNode([TextNode("Just some text.")]))
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "style",
-            "content": {
+            ],
+            "classes": ["class1", "class2"],
+            "title": {
                 "data": {
-                    "type": "sentence",
                     "content": [
                         {
                             "data": {
                                 "type": "text",
-                                "value": "Just some text.",
+                                "value": "sometitle",
+                                "args": [],
+                                "kwargs": {},
+                                "subtype": None,
+                                "tags": [],
                             }
                         },
                     ],
-                }
-            },
-            "value": "underscore",
-        }
-    }
-
-
-def test_style_node_tilde():
-    visitor = BaseVisitor()
-
-    node = StyleNode("tilde", SentenceNode([TextNode("Just some text.")]))
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "style",
-            "content": {
-                "data": {
                     "type": "sentence",
-                    "content": [
-                        {
-                            "data": {
-                                "type": "text",
-                                "value": "Just some text.",
-                            }
-                        },
-                    ],
-                }
-            },
-            "value": "tilde",
-        }
-    }
-
-
-def test_style_node_caret():
-    visitor = BaseVisitor()
-
-    node = StyleNode("caret", SentenceNode([TextNode("Just some text.")]))
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "style",
-            "content": {
-                "data": {
-                    "type": "sentence",
-                    "content": [
-                        {
-                            "data": {
-                                "type": "text",
-                                "value": "Just some text.",
-                            }
-                        },
-                    ],
-                }
+                    "args": [],
+                    "kwargs": {},
+                    "subtype": None,
+                    "tags": [],
+                },
             },
-            "value": "caret",
-        }
-    }
-
-
-def test_macro_node():
-    visitor = BaseVisitor()
-
-    node = MacroNode("somename", ["arg1", "arg2"], {"key1": "value1"})
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "macro",
-            "name": "somename",
+            "engine": "someengine",
+            "preprocessor": "somepreprocessor",
             "args": ["arg1", "arg2"],
             "kwargs": {"key1": "value1"},
+            "tags": ["tag1", "tag2"],
         }
     }
 
 
-def test_footnote_node():
-    visitor = BaseVisitor()
+def test_block_group():
+    visitor = BaseVisitor(Environment())
 
-    node = FootnoteNode(
-        content=[TextNode("Just some text.")],
-        number="5",
-        reference_anchor="someanchor",
-        content_anchor="someanchor-def",
+    node = BlockGroupNode(
+        group_name="somegroup",
+        group={
+            "left": BlockNode(
+                subtype="sometype1",
+                children=[
+                    ParagraphNode(
+                        children=[
+                            TextNode("Block 1"),
+                        ]
+                    ),
+                ],
+                secondary_children=[],
+                classes=[],
+                title=None,
+                engine="group",
+                preprocessor="none",
+                args=[],
+                kwargs={},
+            ),
+            "right": BlockNode(
+                subtype="sometype2",
+                children=[
+                    ParagraphNode(
+                        children=[
+                            TextNode("Block 2"),
+                        ]
+                    ),
+                ],
+                secondary_children=[],
+                classes=[],
+                title=None,
+                engine="group",
+                preprocessor="none",
+                args=[],
+                kwargs={},
+            ),
+        },
+        args=[],
+        kwargs={},
+        tags=[],
     )
 
     result = visitor.visit(node)
 
     assert result == {
         "data": {
-            "type": "footnote",
-            "number": "5",
-            "reference_anchor": "someanchor",
-            "content_anchor": "someanchor-def",
-            "content": [
-                {"data": {"type": "text", "value": "Just some text."}},
-            ],
-        }
-    }
-
-
-def test_reference_node():
-    visitor = BaseVisitor()
-
-    node = ReferenceNode(
-        content_type="somecontent",
-        name="somename",
-        category="somecategory",
-        content=[TextNode("Just some text.")],
-        number="5",
-        title=SentenceNode([TextNode("Some title")]),
-        reference_anchor="someanchor",
-        content_anchor="someanchor-def",
-    )
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "reference",
-            "category": "somecategory",
-            "content_type": "somecontent",
-            "name": "somename",
-            "number": "5",
-            "reference_anchor": "someanchor",
-            "content_anchor": "someanchor-def",
-            "content": [
-                {
-                    "data": {"type": "text", "value": "Just some text."},
-                }
-            ],
-            "title": {
-                "data": {
-                    "type": "sentence",
-                    "content": [
-                        {
-                            "data": {
-                                "type": "text",
-                                "value": "Some title",
-                            },
-                        }
-                    ],
-                }
-            },
-        }
-    }
-
-
-def test_class_node():
-    visitor = BaseVisitor()
-
-    node = ClassNode(["class1", "class2"], TextNode("Just some text."))
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "class",
-            "content": {
-                "data": {
-                    "type": "text",
-                    "value": "Just some text.",
-                }
-            },
-            "classes": ["class1", "class2"],
-        }
-    }
-
-
-def test_link_node():
-    visitor = BaseVisitor()
-
-    node = LinkNode(target="sometarget", text="sometext")
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "link",
-            "text": "sometext",
-            "target": "sometarget",
-        }
-    }
-
-
-def test_image_node():
-    visitor = BaseVisitor()
-
-    node = ImageNode(uri="someuri", alt_text="sometext", width="100", height="400")
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "image",
-            "uri": "someuri",
-            "alt_text": "sometext",
-            "width": "100",
-            "height": "400",
-        }
-    }
-
-
-def test_list_item_node():
-    visitor = BaseVisitor()
-
-    node = ListItemNode("4", TextNode("Just some text."))
-
-    result = visitor.visit(node)
-
-    assert result == {
-        "data": {
-            "type": "list_item",
-            "level": 4,
-            "content": {
-                "data": {
-                    "type": "text",
-                    "value": "Just some text.",
-                }
+            "type": "block_group",
+            "group_name": "somegroup",
+            "group": {
+                "left": {
+                    "data": {
+                        "type": "block",
+                        "subtype": "sometype1",
+                        "content": [
+                            {
+                                "data": {
+                                    "type": "paragraph",
+                                    "content": [
+                                        {
+                                            "data": {
+                                                "type": "text",
+                                                "value": "Block 1",
+                                                "args": [],
+                                                "kwargs": {},
+                                                "subtype": None,
+                                                "tags": [],
+                                            }
+                                        }
+                                    ],
+                                    "title": {},
+                                    "args": [],
+                                    "kwargs": {},
+                                    "subtype": None,
+                                    "tags": [],
+                                }
+                            }
+                        ],
+                        "secondary_content": [],
+                        "classes": [],
+                        "title": {},
+                        "engine": "group",
+                        "preprocessor": "none",
+                        "args": [],
+                        "kwargs": {},
+                        "tags": [],
+                    },
+                },
+                "right": {
+                    "data": {
+                        "type": "block",
+                        "subtype": "sometype2",
+                        "content": [
+                            {
+                                "data": {
+                                    "type": "paragraph",
+                                    "content": [
+                                        {
+                                            "data": {
+                                                "type": "text",
+                                                "value": "Block 2",
+                                                "args": [],
+                                                "kwargs": {},
+                                                "subtype": None,
+                                                "tags": [],
+                                            }
+                                        }
+                                    ],
+                                    "title": {},
+                                    "args": [],
+                                    "kwargs": {},
+                                    "subtype": None,
+                                    "tags": [],
+                                }
+                            }
+                        ],
+                        "secondary_content": [],
+                        "classes": [],
+                        "title": {},
+                        "engine": "group",
+                        "preprocessor": "none",
+                        "args": [],
+                        "kwargs": {},
+                        "tags": [],
+                    },
+                },
             },
+            "title": {},
+            "args": [],
+            "kwargs": {},
+            "tags": [],
+            "subtype": None,
         }
     }
```

### Comparing `mau-3.1.0/PKG-INFO` & `mau-4.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mau
-Version: 3.1.0
+Version: 4.0.0
 Summary: A lightweight template-driven markup language
 Author-email: Leonardo Giordani <giordani.leonardo@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 Requires-Dist: pytest ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Requires-Dist: pytest-icdiff ; extra == "testing"
 Project-URL: Home, https://github.com/Project-Mau/mau
 Provides-Extra: development
 Provides-Extra: testing
 
-# Mau v3
+# Mau v4
 
 Mau is a lightweight markup language heavily inspired by [AsciiDoc](https://asciidoctor.org/docs/what-is-asciidoc), [Asciidoctor](https://asciidoctor.org/) and [Markdown](https://daringfireball.net/projects/markdown/).
 
 As I wasn't satisfied by the results I got with those tools I decided to try to write my own language and the tool to render it.
 
 I am currently using Mau to render posts on my blog [The Digital Cat](https://www.thedigitalcatonline.com) and the online version of my book ["Clean Architectures in Python"](https://www.thedigitalcatbooks.com). I also used it to transpile the code of the book to Markua, to be able to publish the book on Leanpub using their toolchain.
 
@@ -61,43 +61,18 @@
 
 To convert Mau sources into HTML just run
 
 ``` sh
 mau -i source.mau -o destination.html -f html
 ```
 
-To use Mau in your tool you can run it programmatically
-
-``` python
-from mau import Mau, load_visitors
-
-visitor_classes = load_visitors()
-
-visitors = {i.format_code: i for i in visitor_classes}
-visitor_class = visitors["html"]
-
-mau = Mau(
-    "path/of/the/source",
-    visitor_class=visitor_class,
-)
-
-lexer = self._mau.run_lexer(text)
-parser = self._mau.run_parser(lexer.tokens)
-content = self._mau.process(parser.nodes, parser.environment)
-
-if visitor_class.transform:
-    content = visitor_class.transform(content)
-```
-
-Check out Mau [documentation](https://mau.readthedocs.io/en/latest/) for further information.
+Check out Mau [documentation](https://project-mau.github.io/) for further information.
 
 ## Pelican plugin
 
 There is a Pelican plugin that enables you to use Mau in your blog. Check it at https://github.com/pelican-plugins/mau-reader.
 
-You can see the plugin in action at https://www.thedigitalcatonline.com/blog/2021/02/22/mau-a-lightweight-markup-language/ and on other pages in my blog.
-
 ## Support
 
 You may report bugs or missing features use the [issues page](https://github.com/Project-Mau/mau/issues).
 If you want to ask for help or discuss ideas use the [discussions page](https://github.com/Project-Mau/mau/discussions)
```

