# Comparing `tmp/openparse-0.5.4.tar.gz` & `tmp/openparse-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.5.4.tar", last modified: Wed Apr 24 15:01:10 2024, max compression
+gzip compressed data, was "openparse-0.5.5.tar", last modified: Sun Apr 28 17:39:34 2024, max compression
```

## Comparing `openparse-0.5.4.tar` & `openparse-0.5.5.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.596647 openparse-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 15:01:06.000000 openparse-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-24 15:01:10.596647 openparse-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-24 15:01:06.000000 openparse-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 15:01:06.000000 openparse-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:01:10.596647 openparse-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.580647 openparse-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.584647 openparse-0.5.4/src/evals/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:01:06.000000 openparse-0.5.4/src/evals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 15:01:06.000000 openparse-0.5.4/src/evals/run_evals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.584647 openparse-0.5.4/src/openparse/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/doc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.584647 openparse-0.5.4/src/openparse/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/processing/basic_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/processing/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/processing/semantic_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.588647 openparse-0.5.4/src/openparse/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.588647 openparse-0.5.4/src/openparse/tables/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.588647 openparse-0.5.4/src/openparse/tables/table_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.588647 openparse-0.5.4/src/openparse/tables/unitable/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/tabular_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/unitable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/unitable/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/tables/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.588647 openparse-0.5.4/src/openparse/text/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/text/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.588647 openparse-0.5.4/src/openparse/text/pdfminer/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.588647 openparse-0.5.4/src/openparse/text/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 15:01:06.000000 openparse-0.5.4/src/openparse/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/openparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-24 15:01:10.000000 openparse-0.5.4/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-24 15:01:10.000000 openparse-0.5.4/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:01:10.000000 openparse-0.5.4/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 15:01:10.000000 openparse-0.5.4/src/openparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 15:01:10.000000 openparse-0.5.4/src/openparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 15:01:10.000000 openparse-0.5.4/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/processing/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/processing/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/tests/tables/pymupdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/tests/tables/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/transformers/test_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/tests/tables/unitable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/unitable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   190851 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/unitable/sample_pred_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/tables/unitable/test_pred_to_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/test_doc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/test_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.580647 openparse-0.5.4/src/tests/text/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:01:10.592647 openparse-0.5.4/src/tests/text/pdf_miner/
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-24 15:01:06.000000 openparse-0.5.4/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-28 17:39:30.000000 openparse-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-28 17:39:34.749753 openparse-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-28 17:39:30.000000 openparse-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-28 17:39:30.000000 openparse-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:39:34.749753 openparse-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.737753 openparse-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.737753 openparse-0.5.5/src/evals/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:30.000000 openparse-0.5.5/src/evals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-28 17:39:30.000000 openparse-0.5.5/src/evals/run_evals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/basic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/processing/semantic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.741752 openparse-0.5.5/src/openparse/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/tables/table_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/tabular_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/unitable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/unitable/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/tables/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/text/pdfminer/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/openparse/text/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-28 17:39:30.000000 openparse-0.5.5/src/openparse/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/openparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-28 17:39:34.000000 openparse-0.5.5/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.745752 openparse-0.5.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/processing/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/transformers/test_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190851 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/unitable/sample_pred_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/tables/unitable/test_pred_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/test_doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.737753 openparse-0.5.5/src/tests/text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:39:34.749753 openparse-0.5.5/src/tests/text/pdf_miner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-28 17:39:30.000000 openparse-0.5.5/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.5.4/LICENSE` & `openparse-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/PKG-INFO` & `openparse-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.5.4
+Version: 0.5.5
 Summary: Streamlines the process of preparing documents for LLM's.
 Author-email: Sergey Filimonov <hello@sergey.fyi>
 Project-URL: homepage, https://github.com/Filimoa/open-parse
 Project-URL: repository, https://github.com/Filimoa/open-parse
 Project-URL: documentation, https://filimoa.github.io/open-parse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openparse-0.5.4/README.md` & `openparse-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/pyproject.toml` & `openparse-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openparse"
 description = "Streamlines the process of preparing documents for LLM's."
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.5.4"
+version = "0.5.5"
 authors = [{name = "Sergey Filimonov", email = "hello@sergey.fyi"}]
 dependencies = [
     "PyMuPDF >= 1.23.2",
     "pillow >= 8.3",
     "pydantic >= 2.0",
     "pypdf >= 4.0.0",
     "pdfminer.six >= 20200401",
```

### Comparing `openparse-0.5.4/src/evals/run_evals.py` & `openparse-0.5.5/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/__init__.py` & `openparse-0.5.5/src/openparse/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/cli.py` & `openparse-0.5.5/src/openparse/cli.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/config.py` & `openparse-0.5.5/src/openparse/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/doc_parser.py` & `openparse-0.5.5/src/openparse/doc_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import List, Literal, Optional, TypedDict, Union, TypeVar
 
 from openparse import tables, text, consts
 from openparse.pdf import Pdf
-from openparse.types import NOT_GIVEN, NotGiven
+from openparse._types import NOT_GIVEN, NotGiven
 from openparse.processing import (
     IngestionPipeline,
     BasicIngestionPipeline,
     NoOpIngestionPipeline,
 )
 from openparse.schemas import Node, TableElement, TextElement, ParsedDocument
 
@@ -30,15 +30,15 @@
 
 class PyMuPDFArgsDict(TypedDict, total=False):
     parsing_algorithm: Literal["pymupdf"]
     table_output_format: Literal["markdown", "html"]
 
 
 def _table_args_dict_to_model(
-    args_dict: Union[TableTransformersArgsDict, PyMuPDFArgsDict]
+    args_dict: Union[TableTransformersArgsDict, PyMuPDFArgsDict],
 ) -> Union[tables.TableTransformersArgs, tables.PyMuPDFArgs]:
     if args_dict["parsing_algorithm"] == "table-transformers":
         return tables.TableTransformersArgs(**args_dict)
     elif args_dict["parsing_algorithm"] == "pymupdf":
         return tables.PyMuPDFArgs(**args_dict)
     elif args_dict["parsing_algorithm"] == "unitable":
         return tables.UnitableArgs(**args_dict)
```

### Comparing `openparse-0.5.4/src/openparse/pdf.py` & `openparse-0.5.5/src/openparse/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
-import tempfile
+import io
 from pathlib import Path
 from typing import Iterator, List, Literal, Optional, Union, Tuple, Any
-from pydantic import BaseModel
 
+from pydantic import BaseModel
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LTPage
 from pypdf import PdfReader, PdfWriter
 
 from openparse.schemas import Bbox, Node
 from openparse import consts
 
@@ -111,17 +111,17 @@
             raise ImportError(
                 "PyMuPDF (fitz) is not installed. This method requires PyMuPDF."
             )
 
         if not self.writer.pages:
             return fitz.open(self.file_path)
 
-        with tempfile.NamedTemporaryFile(delete=False, suffix=".pdf") as tmpfile:
-            self.writer.write(tmpfile.name)
-            return fitz.open(tmpfile.name)
+        byte_stream = io.BytesIO()
+        self.writer.write(byte_stream)
+        return fitz.open(None, byte_stream)
 
     def _draw_bboxes(
         self,
         bboxes_with_color: List[_BboxWithColor],
         coordinates: Literal["top-left", "bottom-left"],
     ):
         try:
```

### Comparing `openparse-0.5.4/src/openparse/processing/__init__.py` & `openparse-0.5.5/src/openparse/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/processing/basic_transforms.py` & `openparse-0.5.5/src/openparse/processing/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/processing/ingest.py` & `openparse-0.5.5/src/openparse/processing/ingest.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/processing/semantic_transforms.py` & `openparse-0.5.5/src/openparse/processing/semantic_transforms.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/schemas.py` & `openparse-0.5.5/src/openparse/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/parse.py` & `openparse-0.5.5/src/openparse/tables/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/pymupdf/parse.py` & `openparse-0.5.5/src/openparse/tables/pymupdf/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/table_transformers/geometry.py` & `openparse-0.5.5/src/openparse/tables/table_transformers/geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/table_transformers/ml.py` & `openparse-0.5.5/src/openparse/tables/table_transformers/ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/table_transformers/schemas.py` & `openparse-0.5.5/src/openparse/tables/table_transformers/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/unitable/config.py` & `openparse-0.5.5/src/openparse/tables/unitable/config.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/unitable/core.py` & `openparse-0.5.5/src/openparse/tables/unitable/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/unitable/schemas.py` & `openparse-0.5.5/src/openparse/tables/unitable/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/unitable/tabular_transformer.py` & `openparse-0.5.5/src/openparse/tables/unitable/tabular_transformer.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/unitable/tokens.py` & `openparse-0.5.5/src/openparse/tables/unitable/tokens.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/unitable/unitable_model.py` & `openparse-0.5.5/src/openparse/tables/unitable/unitable_model.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/unitable/utils.py` & `openparse-0.5.5/src/openparse/tables/unitable/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/tables/utils.py` & `openparse-0.5.5/src/openparse/tables/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/text/parse.py` & `openparse-0.5.5/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/text/pdfminer/core.py` & `openparse-0.5.5/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/text/pymupdf/core.py` & `openparse-0.5.5/src/openparse/text/pymupdf/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/types.py` & `openparse-0.5.5/src/openparse/_types.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/openparse/version.py` & `openparse-0.5.5/src/openparse/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-OPEN_PARSE_VERSION = "0.5.4"
+OPEN_PARSE_VERSION = "0.5.5"
 
 
 def version_info() -> str:
     """Return complete version information for OpenParse and its dependencies."""
     import importlib.metadata as importlib_metadata
     import platform
     import sys
```

### Comparing `openparse-0.5.4/src/openparse.egg-info/PKG-INFO` & `openparse-0.5.5/src/openparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openparse
-Version: 0.5.4
+Version: 0.5.5
 Summary: Streamlines the process of preparing documents for LLM's.
 Author-email: Sergey Filimonov <hello@sergey.fyi>
 Project-URL: homepage, https://github.com/Filimoa/open-parse
 Project-URL: repository, https://github.com/Filimoa/open-parse
 Project-URL: documentation, https://filimoa.github.io/open-parse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `openparse-0.5.4/src/openparse.egg-info/SOURCES.txt` & `openparse-0.5.5/src/openparse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 src/evals/__init__.py
 src/evals/run_evals.py
 src/openparse/__init__.py
+src/openparse/_types.py
 src/openparse/cli.py
 src/openparse/config.py
 src/openparse/consts.py
 src/openparse/doc_parser.py
 src/openparse/pdf.py
 src/openparse/schemas.py
-src/openparse/types.py
 src/openparse/utils.py
 src/openparse/version.py
 src/openparse.egg-info/PKG-INFO
 src/openparse.egg-info/SOURCES.txt
 src/openparse.egg-info/dependency_links.txt
 src/openparse.egg-info/entry_points.txt
 src/openparse.egg-info/requires.txt
```

### Comparing `openparse-0.5.4/src/tests/processing/test_pipeline.py` & `openparse-0.5.5/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/processing/test_steps.py` & `openparse-0.5.5/src/tests/processing/test_steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.5.5/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/tables/transformers/test_geometry.py` & `openparse-0.5.5/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/tables/transformers/test_ml.py` & `openparse-0.5.5/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/tables/unitable/sample_pred_outputs.py` & `openparse-0.5.5/src/tests/tables/unitable/sample_pred_outputs.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/tables/unitable/test_pred_to_schema.py` & `openparse-0.5.5/src/tests/tables/unitable/test_pred_to_schema.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/test_doc_parser.py` & `openparse-0.5.5/src/tests/test_doc_parser.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/test_schemas.py` & `openparse-0.5.5/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.4/src/tests/text/pdf_miner/test_core.py` & `openparse-0.5.5/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*

